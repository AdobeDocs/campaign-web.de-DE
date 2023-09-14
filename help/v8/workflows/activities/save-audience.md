---
audience: end-user
title: Verwenden der Workflow-Aktivität Audience-Speicherung
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Verzweigung“ verwenden.
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 18%

---


# Audience-Speicherung {#save-audience}

>[!CONTEXTUALHELP]
>id="???"
>title="Audience-Speicherung Aktivität"
>abstract="Die Audience-Speicherung ermöglicht..."

Bezeichnung der Modus-Zielgruppe Adobe Campaign wird diese Bezeichnung mit bestehenden Zielgruppen abgleichen. Wenn eine Übereinstimmung gefunden wird, wird diese Zielgruppe aktualisiert, andernfalls wird eine neue Zielgruppe erstellt.
Update-Methode

Zielgruppe durch neue Daten ersetzen

Vollständige Audience mit neuen Datenordnerlisten (/Profile und Zielgruppen/Listen/)

Ausgehende Transition erzeugen


Die **Audience-Speicherung** -Aktivität **Targeting** -Aktivität. Diese Aktivität ermöglicht die Aktualisierung einer existierenden Audience oder die Erstellung einer neuen Audience aus der zuvor durch einen Workflow berechneten Population. Die erstellten Audiences werden der Liste der Anwendungszielgruppen hinzugefügt und über die **Zielgruppen** Menü.

Diese Aktivität dient im Wesentlichen dazu, innerhalb desselben Workflows berechnete Populationen in wiederverwendbare Audiences umzuwandeln. Verbinden Sie ihn mit anderen Targeting-Aktivitäten, z. B. einer **Audience erstellen** oder **Kombinieren** -Aktivität.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Audience-Speicherung** Aktivität:

1. Hinzufügen einer **Audience-Speicherung** -Aktivität zu Ihrem Workflow hinzu.

   <!--![](../assets/workflow-save-audience.png)-->

1. Im **Modus** in der Dropdown-Liste die gewünschte Aktion auswählen:

   * **Erstellen oder Aktualisieren einer vorhandenen Zielgruppe**: Definieren Sie eine **Zielgruppenbezeichnung**. Wenn die Audience bereits existiert, wird sie aktualisiert. Andernfalls wird eine neue Audience erstellt.

   * **Vorhandene Audience aktualisieren**: Wählen Sie die **Zielgruppe** Sie möchten die Liste der existierenden Zielgruppen aktualisieren.

1. Wählen Sie die **Aktualisierungsmodus** wird für bestehende Zielgruppen gelten:

   * **Audience-Inhalt durch neue Daten ersetzen**: Der gesamte Inhalt der Audience wird ersetzt. die zuvor enthaltenen Daten gehen verloren. Nur die in der eingehenden Transition an die Audience-Speicherung-Aktivität übermittelten Daten werden beibehalten. Mit dieser Option werden der Audience-Typ und die Zielgruppendimension der aktualisierten Audience gelöscht.

   * **Vollständige Audience mit neuen Daten**: Der alte Inhalt der Audience wird beibehalten und die Daten aus der eingehenden Transition der Aktivität Audience speichern werden hinzugefügt.

1. Überprüfen Sie die **Komplement erzeugen** , wenn Sie die verbleibende Population ausnutzen möchten. Der Aktivität wird daraufhin eine zusätzliche Transition hinzugefügt.

Der Inhalt der gespeicherten Audience ist anschließend in der Detailansicht der Audience verfügbar, auf die Sie im Menü **Audiences** zugreifen können. Die in dieser Ansicht verfügbaren Spalten entsprechen den Spalten der in den Workflow eingehenden Transition. **SAve-Zielgruppe** -Aktivität.


## Beispiel



