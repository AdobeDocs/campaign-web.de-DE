---
audience: end-user
title: Erstellen von Zielgruppen
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Campaign Web erstellen.
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 52%

---

# Erstellen von Zielgruppen {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Zielgruppen"
>abstract="Auf diesem Bildschirm kann die Liste aller Zielgruppen aufgerufen werden, die in Workflows oder eigenständigen Sendungen ausgewählt werden können. Klicken Sie auf **Erstellen**, um eine neue Zielgruppe in einer visuellen Arbeitsfläche zu erstellen.<br/><br/>Sie können nicht nur von Grund auf eine neue einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppe genauer zu bestimmen. Sie können beispielsweise mehrere Zielgruppen in einer Zielgruppe kombinieren, Ihre Zielgruppe mit externen Attributen anreichern oder sie auf der Grundlage von Regeln Ihrer Wahl in mehrere Zielgruppen unterteilen."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Mit Campaign Web können Sie in einer visuellen Workflow-Arbeitsfläche neue Audiences erstellen. Sie können nicht nur von Grund auf eine einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppe zu präzisieren. Sie können beispielsweise mehrere Zielgruppen in einer Zielgruppe kombinieren, Ihre Zielgruppe mit externen Attributen anreichern oder sie auf der Grundlage von Regeln Ihrer Wahl in mehrere Zielgruppen unterteilen.

Nach der Erstellung des Workflows werden die resultierenden Audiences automatisch in der Campaign-Datenbank zusammen mit den bestehenden Audiences gespeichert. Diese Zielgruppen können dann in Workflows oder in eigenständigen Sendungen ausgewählt werden.

Die Spalte **[!UICONTROL Herkunft]** gibt den Ursprung der Zielgruppen an: **[!UICONTROL Adobe Campaign]**-Zielgruppen werden in der Adobe Campaign v8-Konsole oder in der Web-Benutzeroberfläche erstellt, während **[!UICONTROL Adobe Experience Platform:]**-Zielgruppen in Adobe Experience Platform erstellt und mithilfe der Adobe-Quell- und Zielintegration in Campaign integriert werden.

➡️ [Entdecken Sie diese Funktion im Video](#video)

## Erstellen Ihrer ersten Zielgruppe {#create}

Gehen Sie wie folgt vor, um eine Zielgruppe zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Zielgruppen]**-Menü und klicken Sie oben rechts auf **[!UICONTROL Schaltfläche]** Zielgruppe erstellen .

1. Es wird automatisch ein neuer Workflow erstellt, der es Ihnen ermöglicht, Aktivitäten zu kombinieren, um Ihre Zielgruppe zu generieren. Standardmäßig enthält die Arbeitsfläche zwei Hauptaktivitäten:

   * Die Aktivität „Abfrage **[!UICONTROL Zielgruppe aufbauen]** ist der Ausgangspunkt Ihres Workflows. Damit können Sie eine Zielgruppe erstellen und als Grundlage für Ihren Workflow verwenden.

   * Die Aktivität „Neue Zielgruppe **[!UICONTROL Zielgruppe speichern]** stellt den letzten Schritt in Ihrem Workflow dar. Dadurch können Sie die Ergebnisse als neue Zielgruppe speichern.

   ![Eine leere Arbeitsfläche für die Erstellung von Zielgruppen mit zwei Standardaktivitäten: Zielgruppe aufbauen und Zielgruppe speichern.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >Zielgruppen-Workflows werden im Menü **Workflows** neben Ihren anderen Kampagnen-Workflows gespeichert. Sie sind speziell für den Aufbau einer Zielgruppe konzipiert und können an ihrer vertikalen Arbeitsfläche identifiziert werden.

1. Ändern Sie zugunsten einer besseren Lesbarkeit den Namen des Workflows in den Workflow-Einstellungen im Feld **Titel**. [Erfahren Sie, wie Sie Workflow-Einstellungen konfigurieren](../workflows/workflow-settings.md)

1. Öffnen Sie die Aktivität **[!UICONTROL Zielgruppe aufbauen]** und verwenden Sie den Abfrage-Modellierer, um die Population zu definieren, die in Ihre Zielgruppe aufgenommen werden soll, indem Sie die in der Datenbank enthaltenen Daten filtern. [Erfahren Sie, wie Sie die Aktivität „Zielgruppe erstellen“ konfigurieren können](../workflows/activities/build-audience.md)

1. Wenn Sie zusätzliche Vorgänge auf die im Workflow ausgewählte Population anwenden möchten, fügen Sie beliebig viele Aktivitäten hinzu und verbinden Sie sie miteinander. Weitere Informationen zur Konfiguration von Workflow-Aktivitäten finden Sie in der [ zu Workflows ](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktivitäten stehen nicht zur Verwendung in Zielgruppen-Workflows zur Verfügung.

   ![Eine Arbeitsfläche zur Zielgruppenerstellung mit mehreren verbundenen Aktivitäten zur Verfeinerung der Zielgruppe.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Konfigurieren Sie die Aktivität **[!UICONTROL Zielgruppe speichern]**, um anzugeben, wie die zuvor im Workflow berechnete Population gespeichert werden soll. [Erfahren Sie, wie Sie eine Aktivität „Zielgruppe speichern“ konfigurieren können](../workflows/activities/save-audience.md)

1. Wenn Ihr Workflow bereit ist, klicken Sie auf **[!UICONTROL Starten]**, um ihn auszuführen.

Der Workflow wird in der Liste **[!UICONTROL Workflows]** gespeichert, während die resultierende(n) Zielgruppe(n) in der Liste **[!UICONTROL Zielgruppen]** unter dem in der Aktivität **Zielgruppe speichern** definierten Titel zugänglich sind. Erfahren Sie [in diesem Abschnitt](manage-audience.md), wie Sie Zielgruppen überwachen und verwalten.

Jetzt können Sie diese Zielgruppe als Hauptzielgruppe eines Versands verwenden. [Weitere Informationen](add-audience.md)

## Beispiel für einen Zielgruppen-Workflow {#example}

Das folgende Beispiel zeigt einen Zielgruppen-Workflow, der so konfiguriert ist, dass Kundinnen, die in New York leben, ausgewählt werden und je nach ihrem letzten Kauf (Joga- oder Laufkleidung) zwei neue Zielgruppen erstellt werden.

![Ein Beispiel für einen Zielgruppen-Workflow, der sich an weibliche Kunden in New York richtet und sie nach ihrem letzten Kauf aufteilt.](assets/audiences-example.png){zoomable="yes"}

1. Die Aktivität **[!UICONTROL Zielgruppe erstellen]** richtet sich an alle in New York lebenden weiblichen Profile.
1. Die Aktivität **[!UICONTROL Anreicherung]** erweitert die Zielgruppe um Informationen aus der Tabelle „Käufe“, um zu ermitteln, welcher Produkttyp von den Kundinnen gekauft wurde.
1. Die Aktivität **[!UICONTROL Aufspaltung]** unterteilt den Workflow in zwei Pfade, die auf dem aktuellen Kauf der Kundinnen basieren.
1. Die **[!UICONTROL Zielgruppe speichern]**-Aktivitäten am Ende jedes Pfads erstellen zwei neue Zielgruppen in der Datenbank, einschließlich der in jedem Pfad berechneten Population.

## Bearbeiten einer Zielgruppe {#edit}

Sie können eine aus einem Workflow generierte Zielgruppe bei Bedarf ändern, indem Sie den entsprechenden Workflow erneut ausführen. Auf diese Weise können Sie Zielgruppendaten aktualisieren oder die Zielgruppe einschränken, indem Sie die Abfrage an Ihre Anforderungen anpassen.

1. Navigieren Sie zum **Zielgruppen**-Menü und öffnen Sie die Zielgruppe, die Sie bearbeiten möchten.
1. Auf der Registerkarte **Übersicht** enthält der Abschnitt **Letzter Workflow** einen Link zu dem Workflow, der zur Erstellung der Zielgruppe verwendet wurde. Klicken Sie darauf, um auf den Workflow zuzugreifen.
1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie auf die Schaltfläche **Starten**, um den Workflow erneut auszuführen. Nach Abschluss des Workflows wird die aus dem Workflow resultierende Audience automatisch mit den neuesten Workflow-Ergebnissen aktualisiert.

Standardmäßig wird bei der erneuten Ausführung eines Zielgruppen-Workflows der gesamte Inhalt der Zielgruppe durch neue Daten ersetzt, was zum Verlust der vorherigen Daten führt.

Wenn Sie die vorherigen Zielgruppenergebnisse nicht ersetzen möchten, konfigurieren Sie die Aktivitäten **Zielgruppe speichern** entsprechend dementsprechend. Sie können beispielsweise das Feld **Zielgruppentitel** ändern, um die neuen Ergebnisse in einer neuen Zielgruppe zu speichern, oder die neuen Ergebnisse zum vorhandenen Zielgruppeninhalt hinzufügen, ohne vorherige Daten zu löschen. [Erfahren Sie, wie Sie eine Aktivität „Zielgruppe speichern“ konfigurieren können](../workflows/activities/save-audience.md)

![Der Konfigurationsbildschirm für die Aktivität „Zielgruppe speichern“ mit Optionen zum Anpassen des Speicherverhaltens für Zielgruppen.](assets/edit-audience-save.png){zoomable="yes"}

## Anleitungsvideo {#video}

Erfahren Sie, wie Sie Zielgruppen erstellen und verwalten, wie Sie Zielgruppen für einen Versand auswählen und Kontrollgruppen definieren.

>[!VIDEO](https://video.tv.adobe.com/v/3453211?quality=12&captions=ger)