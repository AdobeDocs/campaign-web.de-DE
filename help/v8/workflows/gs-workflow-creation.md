---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: ht
source-wordcount: '286'
ht-degree: 100%

---


# Grundlegende Prinzipien der Workflow-Erstellung {#gs-workflow-creation}

Mit Campaign v8 Web können Sie Workflows in einer visuellen Arbeitsfläche erstellen, um kanalübergreifende Prozesse wie Segmentierung, Kampagnenausführung und Dateiverarbeitung zu entwerfen.

Workflows können entweder als eigenständige Workflows über das Menü „Workflows“ oder innerhalb einer Kampagne über das Menü „Kampagnen“ erstellt werden.

TBD: Besonderheiten eigenständiger und Kampagnen-Workflows detaillieren.

## Was befindet sich in einem Workflow?

Das Workflow-Diagramm zeigt, was passieren soll. Es beschreibt die verschiedenen Aufgaben, die ausgeführt und miteinander verknüpft werden sollen.

Jeder Workflow besteht aus:

* **Activities**: Eine Aktivität ist eine Aufgabe, die ausgeführt werden soll. Die verschiedenen verfügbaren Aktivitäten werden im Diagramm durch Symbole dargestellt. Jede Aktivität verfügt über bestimmte Eigenschaften sowie andere Eigenschaften, die für alle Aktivitäten gelten.

   In einem Workflow-Diagramm kann eine einzelne Aktivität verschiedene Aufgaben auslösen. Dies ist insbesondere der Fall bei Schleifen oder wiederkehrenden Aktionen.

* **Transitionen**: Transitionen verknüpfen eine Quellaktivität mit einer Zielaktivität und definieren deren Sequenz.

* **Arbeitstabellen**: Die Arbeitstabelle enthält alle von der Transition übermittelten Informationen. Jeder Workflow verwendet mehrere Arbeitstabellen. Die in diesen Tabellen übermittelten Daten können beschleunigt und während des gesamten Lebenszyklus des Workflows verwendet werden, sofern sie nicht bereinigt werden. Tatsächlich werden nicht benötigte Tabellen jedes Mal bereinigt, wenn der Workflow passiviert wird, und möglicherweise während der Ausführung der größten Workflows, um eine Überlastung des Servers zu vermeiden.

## Die wichtigsten Schritte zum Erstellen eines Workflows

Die wichtigsten Schritte zum Erstellen von Workflows sehen wie folgt aus:

TBD: Grafik, die den gesamten Prozess mit Erläuterung und Verweis auf Dokumentseiten zeigt

Eigenschaften erstellen und definieren > Aktivitäten auf der Arbeitsfläche koordinieren > Einstellungen bei Bedarf konfigurieren > Ausführung starten und überwachen