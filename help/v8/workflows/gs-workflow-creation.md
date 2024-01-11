---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: 24521be2c796b5714712849355c3d033537847bc
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 96%

---

# Grundlegende Prinzipien der Workflow-Erstellung {#gs-workflow-creation}

Mit Campaign v8 Web können Sie Workflows in einer visuellen Arbeitsfläche erstellen, um kanalübergreifende Prozesse wie Segmentierung, Kampagnenausführung und Dateiverarbeitung zu entwerfen.


## Was befindet sich in einem Workflow? {#gs-workflow-inside}

Das Workflow-Diagramm zeigt, was passieren soll. Es beschreibt die verschiedenen Aufgaben, die ausgeführt und miteinander verknüpft werden sollen.

![](assets/workflow-example.png) {zoomable=&quot;yes&quot;}

Jeder Workflow besteht aus:

* **Tätigkeiten**: Eine Aktivität ist eine Aufgabe, die ausgeführt werden muss. Die verschiedenen verfügbaren Aktivitäten werden im Diagramm durch Symbole dargestellt. Jede Aktivität verfügt über bestimmte Eigenschaften sowie andere Eigenschaften, die für alle Aktivitäten gelten.

  In einem Workflow-Diagramm kann eine einzelne Aktivität verschiedene Aufgaben auslösen. Dies ist insbesondere der Fall bei Schleifen oder wiederkehrenden Aktionen.

* **Transitionen**: Transitionen verknüpfen eine Quellaktivität mit einer Zielaktivität und definieren deren Sequenz.

* **Arbeitstabellen**: Die Arbeitstabelle enthält alle von der Transition übermittelten Informationen. Jeder Workflow verwendet mehrere Arbeitstabellen. Die in diesen Tabellen übermittelten Daten können während des gesamten Lebenszyklus des Workflows verwendet werden.

## Wichtige Schritte zum Erstellen eines Workflows {#gs-workflow-steps}


Campaign bietet zwei Möglichkeiten, einen Workflow zu erstellen:

1. Workflows können als eigenständige Workflows über das Menü **Workflows** erstellt werden.

   ![](assets/create-a-standalone-wf.png)

1. Workflows können direkt in einer Kampagne erstellt werden, und zwar über die Registerkarte **Workflow** der Kampagne. Wenn der Workflow in einer Kampagne enthalten ist, wird er mit allen anderen Kampagnen-Workflows ausgeführt, und die Berichtsmetriken werden alle auf Kampagnenebene gruppiert.

   ![](assets/create-a-wf-from-a-campaign.png)


Die wichtigsten Schritte zum Erstellen von Workflows sehen wie folgt aus:

![](assets/workflow-creation-process.png)

Ausführliche Schritte dazu finden Sie im folgenden Abschnitt:

1. [Erstellen eines Workflows und Definieren seiner Eigenschaften](create-workflow.md)
1. [Koordinieren und Konfigurieren von Aktivitäten](orchestrate-activities.md)
1. [Konfigurieren von erweiterten Workflow-Einstellungen](workflow-settings.md)
1. [Starten des Workflows und Überwachen der Ausführung](start-monitor-workflows.md)
