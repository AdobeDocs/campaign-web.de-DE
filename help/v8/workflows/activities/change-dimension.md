---
audience: end-user
title: Verwenden der Workflow-Aktivität „Dimensionsänderung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Dimensionsänderung“ verwenden
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 100%

---

# Ändern der Dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Erzeugen eines Komplements"
>abstract="Sie können eine zusätzliche ausgehende Transition mit der verbleibenden Population generieren, die als Duplikat ausgeschlossen wurde. Schalten Sie dazu die Option **Komplement erzeugen** ein."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Aktivität „Dimensionsänderung“"
>abstract="Mithilfe dieser Aktivität können Sie die Zielgruppendimension beim Erstellen einer Zielgruppe ändern. Diese Aktivität verschiebt die Achse je nach Datenvorlage und der Eingabedimension. Beispielsweise können Sie von der Dimension „Verträge“ zur Dimension „Kundinnen und Kunden“ wechseln."

Die Aktivität **Dimensionsänderung** ist eine Aktivität zur **Zielgruppenbestimmung**. Mithilfe dieser Aktivität können Sie die Zielgruppendimension beim Erstellen des Workflows ändern. Diese Aktivität verschiebt die Achse je nach Datenvorlage und der Eingabedimension. [Erfahren Sie mehr über Zielgruppendimensionen](../../audience/about-recipients.md#targeting-dimensions)

Sie können beispielsweise die Zielgruppendimension eines Workflows von „Empfängerinnen und Empfänger“ in „Abonnentenanwendung“ ändern, um Push-Benachrichtigungen an die Zielgruppenempfängerinnen und -empfänger zu senden.

>[!IMPORTANT]
>
>Beachten Sie, dass die Aktivitäten **[!UICONTROL Dimension ändern]** und **[!UICONTROL Datenquelle ändern]** nicht in einer Zeile hinzugefügt werden sollten. Wenn Sie beide Aktivitäten nacheinander verwenden müssen, fügen Sie dazwischen die Aktivität **[!UICONTROL Anreicherung]** ein. Dadurch wird eine ordnungsgemäße Ausführung sichergestellt und potenzielle Konflikte oder Fehler werden vermieden.

## Konfigurieren der Aktivität „Dimensionsänderung“ {#configure}

Gehen Sie folgendermaßen vor, um die Aktivität **Dimensionsänderung** zu konfigurieren:

1. Fügen Sie die Aktivität **Dimensionsänderung** zu Ihrem Workflow hinzu.

   ![Screenshot der einem Workflow hinzugefügten Aktivität „Dimensionsänderung“](../assets/workflow-change-dimension.png)

1. Definieren Sie die **neue Zielgruppendimension**. Bei einer Dimensionsänderung werden alle Einträge beibehalten. Andere Optionen sind noch nicht verfügbar.

1. Führen Sie den Workflow aus, um das Ergebnis anzuzeigen. Vergleichen Sie die Daten in den Tabellen vor und nach der Aktivität „Dimensionsänderung“ sowie die Struktur der Workflow-Tabellen.

## Beispiel {#example}

In diesem Beispiel wird ein SMS-Versand an alle Profile durchgeführt, die einen Kauf getätigt haben. Dazu verwenden Sie zunächst die Aktivität **[!UICONTROL Zielgruppe erstellen]**, die mit einer benutzerdefinierten Zielgruppendimension „Kauf“ verknüpft ist, um alle erfolgten Käufe auszuwählen.

Verwenden Sie dann die Aktivität **[!UICONTROL Dimensionsänderung]**, um die Zielgruppendimension des Workflows in „Empfängerinnen und Empfänger“ zu ändern. Auf diese Weise können Sie die Empfängerinnen und Empfänger ansprechen, die der Abfrage entsprechen.

![Screenshot mit einem Beispiel für die in einem Workflow verwendete Aktivität „Dimensionsänderung“](../assets/workflow-change-dimension-example.png)