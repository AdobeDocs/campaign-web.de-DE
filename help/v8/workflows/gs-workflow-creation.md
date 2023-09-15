---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 53148300ecb5d52d89875519c44ae979d29a4d76
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 57%

---


# Grundlegende Prinzipien der Workflow-Erstellung {#gs-workflow-creation}

Mit Campaign v8 Web können Sie Workflows in einer visuellen Arbeitsfläche erstellen, um kanalübergreifende Prozesse wie Segmentierung, Kampagnenausführung und Dateiverarbeitung zu entwerfen.


## Was befindet sich in einem Workflow? {#gs-workflow-inside}

Das Workflow-Diagramm zeigt, was passieren soll. Es beschreibt die verschiedenen Aufgaben, die ausgeführt und miteinander verknüpft werden sollen.

![](assets/workflow-example.png)

Jeder Workflow besteht aus:

* **Activities**: Eine Aktivität ist eine Aufgabe, die ausgeführt werden soll. Die verschiedenen verfügbaren Aktivitäten werden im Diagramm durch Symbole dargestellt. Jede Aktivität verfügt über bestimmte Eigenschaften sowie andere Eigenschaften, die für alle Aktivitäten gelten.

  In einem Workflow-Diagramm kann eine einzelne Aktivität verschiedene Aufgaben auslösen. Dies ist insbesondere der Fall bei Schleifen oder wiederkehrenden Aktionen.

* **Transitionen**: Transitionen verknüpfen eine Quellaktivität mit einer Zielaktivität und definieren deren Sequenz.

* **Arbeitstabellen**: Die Arbeitstabelle enthält alle von der Transition übermittelten Informationen. Jeder Workflow verwendet mehrere Arbeitstabellen. Die in diesen Tabellen übermittelten Daten können während des gesamten Lebenszyklus des Workflows verwendet werden.

## Wichtige Schritte zum Erstellen eines Workflows {#gs-workflow-steps}


Campaign bietet zwei Möglichkeiten, einen Workflow zu erstellen:

1. Workflows können als eigenständige Workflows aus dem **Workflows** Menü.

   ![](assets/create-a-standalone-wf.png)

1. Workflows können direkt in einer Kampagne erstellt werden, indem Sie über die **Workflow** der Kampagne. Wenn der Workflow in einer Kampagne enthalten ist, wird er mit allen anderen Kampagnen-Workflows ausgeführt, und die Berichtsmetriken werden alle auf Kampagnenebene gruppiert.

   ![](assets/create-a-wf-from-a-campaign.png)


Die wichtigsten Schritte zum Erstellen von Workflows sind:

![](assets/workflow-creation-process.png)

Diese Schritte werden im folgenden Abschnitt beschrieben:

1. [Workflow erstellen und Eigenschaften definieren](create-workflow.md)
1. [Aktivitäten koordinieren und konfigurieren](orchestrate-activities.md)
1. [Erweiterte Workflow-Einstellungen konfigurieren](workflow-settings.md)
1. [Workflow starten und die Ausführung überwachen](start-monitor-workflows.md)

