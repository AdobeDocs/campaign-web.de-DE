---
audience: end-user
title: Verwenden der Workflow-Aktivität „Datenquelle ändern“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Datenquelle ändern“ verwenden.
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 80%

---

# Datenquelle ändern {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Datenquelle ändern"
>abstract="Die Aktivität **Datenquelle ändern** ermöglicht die Auswahl einer anderen Datenquelle für die Arbeitstabelle Ihres Workflows."

Die Aktivität **Datenquelle ändern** ist eine Aktivität zur **Zielgruppenbestimmung**. Mit dieser Aktivität können Sie die Datenquelle ändern, die von der Arbeitstabelle Ihres Workflows verwendet wird. Dies bietet mehr Flexibilität, da Sie Daten in allen Ihren verschiedenen Datenbanken verwalten und die Leistung verbessern können.

In einem Workflow werden die von einer Aktivität zu einer anderen übertragenen Daten in temporären **Arbeitstabellen** gespeichert. Standardmäßig werden die Arbeitstabellen auf derselben Datenbank erstellt wie die Quelle der verarbeiteten Daten. Wenn Sie beispielsweise die Tabelle „Profile“ in der Cloud-Datenbank abfragen, wird eine Arbeitstabelle in derselben Cloud-Datenbank erstellt.

In einigen Fällen sind entweder keine Daten in der aktuellen Datenbank verfügbar oder sie sind nicht effizient genug, um einzelne Vorgänge durchzuführen. Möglicherweise müssen Sie den Workflow zwingen, eine andere Datenbank zu verwenden, um solche Vorgänge durchzuführen, indem Sie die Aktivität **[!UICONTROL Datenquelle ändern]** hinzufügen.

Ausführliche Informationen zur Campaign-Architektur finden Sie in der [ zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html?lang=de).

>[!IMPORTANT]
>
>Beachten Sie, dass die Aktivitäten **[!UICONTROL Dimension ändern]** und **[!UICONTROL Datenquelle ändern]** nicht in einer Zeile hinzugefügt werden sollten. Wenn Sie beide Aktivitäten nacheinander verwenden müssen, schließen Sie eine Aktivität **[!UICONTROL Anreicherung]** zwischen sie ein. Dadurch wird eine ordnungsgemäße Ausführung sichergestellt und potenzielle Konflikte oder Fehler werden vermieden.

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Konfigurieren der Aktivität „Datenquelle ändern“ {#configure}

Führen Sie die folgenden Schritte aus, um die Aktivität **Datenquelle ändern** zu konfigurieren:

![Screenshot, der zeigt, wie die Aktivität „Datenquelle ändern“ zu einem Workflow hinzugefügt wird.](../assets/workflow-change-data-source-add.png)

1. Fügen Sie die Aktivität **Datenquelle ändern** zu Ihrem Workflow hinzu.

1. Definieren Sie die Datenquelle, in die Sie die Arbeitstabelle verschieben möchten:

   * **[!UICONTROL Standard-Campaign-Datenbank (PostgreSQL)]**: Es wird die standardmäßige lokale Campaign-Datenbank verwendet.
   * **[!UICONTROL Externes FDA-Konto]**: Es werden externe Cloud-Datenbanken verwendet, die über die Federated Data Access-Funktion mit Adobe Campaign verbunden sind.

     >[!AVAILABILITY]
     >
     >Die Konfiguration und Verbindung von Campaign mit externen Systemen ist erfahrenen Benutzenden vorbehalten und nur über die Client-Konsole verfügbar. [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=de){target="_blank"}

1. Konfigurieren Sie Ihren Workflow so, dass die gewünschten Vorgänge mit der neuen Datenquelle ausgeführt werden.

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->