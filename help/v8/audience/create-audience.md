---
audience: end-user
title: Audiences erstellen
description: Erfahren Sie, wie Sie Zielgruppen im Adobe Campaign Web erstellen
badge: label="Beta"
source-git-commit: ba449ee0b5a4b41db8efbbabeb37ce7cd7cc3720
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 4%

---


# Audiences erstellen {#create-audiences}

Zielgruppenmenü

Sie können sie in eigenständigen Sendungen oder Kampagnen erstellen und gezielt ausrichten.

## Erstellen der ersten Zielgruppe {#create}

1. Zielgruppe > Menü
1. Zielgruppe erstellen
1. Eigenschaften : Titel und zusätzliche Optionen
1. Arbeitsfläche mit der Aktivität &quot;Zielgruppe erstellen&quot;
1. Aktivität bearbeiten, Workflow je nach Bedarf bearbeiten
1. Starten Sie den Workflow (kann nur Zielgruppenbestimmungsaktivitäten hinzugefügt werden? Keine Kanalaktivitäten?) = Erstellt die Audience und den Workflow.

## Zielgruppen überwachen und verwalten {#monitor}

Dashboard in der erstellten Audience mit zwei Registerkarten:
* Übersicht: Eigenschaften + Workflow-Status und Anzahl der Empfänger dieser Audience durch Klick auf die Schaltfläche calculate + Workflow von hier aus aufrufen und bearbeiten kann
* data: zum Anzeigen von Datenprofilen in der Audience. Kann bei Bedarf neue Spalten hinzufügen. Anzeigen angereicherter Daten

Zielgruppenliste: Duplizieren, löschen

**Fragen:**

Workflow im &quot;Zielgruppenmodus&quot;=> Senden von Kanalaktivitäten nicht verfügbar

* in der Staging-Instanz: Wir können die letzte Abfrage-Aktivität entfernen und stattdessen eine Kanalaktivität hinzufügen.
* Wie erkennen wir einen Workflow im &#39;Audience&#39;-Modus?
