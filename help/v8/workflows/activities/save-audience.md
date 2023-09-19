---
audience: end-user
title: Verwenden der Workflow-Aktivität Audience-Speicherung
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Verzweigung“ verwenden.
badge: label="Beta"
source-git-commit: 2894766336d5ac52625175981c6969a0ac5882d8
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 21%

---


# Audience-Speicherung {#save-audience}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="Save an audience"
>abstract="Use this activity to save the workflow audience."
-->

Die **Audience-Speicherung** -Aktivität **Targeting** -Aktivität. Diese Aktivität ermöglicht die Aktualisierung einer existierenden Audience oder die Erstellung einer neuen Audience aus der zuvor durch einen Workflow berechneten Population. Die erstellten Audiences werden der Liste der Anwendungszielgruppen hinzugefügt und über die **Zielgruppen** Menü.

Diese Aktivität dient im Wesentlichen dazu, innerhalb desselben Workflows berechnete Populationen in wiederverwendbare Audiences umzuwandeln. Verbinden Sie ihn mit anderen Targeting-Aktivitäten, z. B. einer **Audience erstellen** oder **Kombinieren** -Aktivität.

## Konfigurieren Sie die Aktivität Audience-Speicherung .{#save-audience-configuration}

Führen Sie die folgenden Schritte aus, um die **Audience-Speicherung** Aktivität:

![](../assets/workflow-save-audience.png)

1. Hinzufügen einer **Audience-Speicherung** -Aktivität zu Ihrem Workflow hinzu.

1. Im **Modus** in der Dropdown-Liste die gewünschte Aktion auswählen:

   * **Erstellen oder Aktualisieren einer vorhandenen Zielgruppe**: Definieren Sie eine **Zielgruppenbezeichnung**. Wenn die Audience bereits existiert, wird sie aktualisiert. Andernfalls wird eine neue Audience erstellt.

   * **Vorhandene Audience aktualisieren**: Wählen Sie die **Zielgruppe** Sie möchten die Liste der existierenden Zielgruppen aktualisieren.

1. Wählen Sie die **Aktualisierungsmodus** wird für bestehende Zielgruppen gelten:

   * **Audience-Inhalt durch neue Daten ersetzen**: Der gesamte Inhalt der Audience wird ersetzt. die zuvor enthaltenen Daten gehen verloren. Nur die in der eingehenden Transition an die Audience-Speicherung-Aktivität übermittelten Daten werden beibehalten. Mit dieser Option werden der Audience-Typ und die Zielgruppendimension der aktualisierten Audience gelöscht.

   * **Vollständige Audience mit neuen Daten**: Der alte Inhalt der Audience wird beibehalten und die Daten aus der eingehenden Transition der Aktivität Audience speichern werden hinzugefügt.

1. Überprüfen Sie die **Ausgehende Transition erzeugen** , wenn Sie eine Transition nach der **Audience-Speicherung** -Aktivität.

Der Inhalt der gespeicherten Audience ist anschließend in der Detailansicht der Audience verfügbar, auf die Sie im Menü **Audiences** zugreifen können. Die in dieser Ansicht verfügbaren Spalten entsprechen den Spalten der in den Workflow eingehenden Transition. **Audience-Speicherung** -Aktivität.


## Beispiel{#save-audience-example}

Im folgenden Beispiel wird eine einfache Zielgruppenaktualisierung anhand der Zielgruppenbestimmung veranschaulicht. Eine Planung wird hinzugefügt, um den Workflow einmal monatlich auszuführen. Eine Abfrage ruft alle Profile ab, die für die verschiedenen verfügbaren Anwendungsdienste angemeldet sind. Die **Audience-Speicherung** aktualisiert in diesem Fall die angegebene Audience, indem die Profile, die seit der letzten Ausführung des Workflows den Informationsdienst abbestellt haben, gelöscht und die neuen Abonnenten hinzugefügt werden.


