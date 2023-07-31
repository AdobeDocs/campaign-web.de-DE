---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Alpha"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 100%

---


# Grundlegende Prinzipien der Workflow-Erstellung {#gs-workflow-creation}

Mit Campaign v8 Web können Sie Workflows in einer visuellen Arbeitsfläche erstellen, um kanalübergreifende Prozesse wie Segmentierung, Kampagnenausführung und Dateiverarbeitung zu entwerfen.

Workflows können entweder als eigenständige Workflows, im Menü „Workflows“ oder direkt in einer Kampagne erstellt werden. In diesem Fall wird der Workflow mit der Kampagne verknüpft und zusammen mit allen anderen Kampagnen-Workflows ausgeführt.

## Was befindet sich in einem Workflow?

Das Workflow-Diagramm zeigt, was passieren soll. Es beschreibt die verschiedenen Aufgaben, die ausgeführt und miteinander verknüpft werden sollen.

![](assets/workflow-example.png)

Jeder Workflow besteht aus:

* **Activities**: Eine Aktivität ist eine Aufgabe, die ausgeführt werden soll. Die verschiedenen verfügbaren Aktivitäten werden im Diagramm durch Symbole dargestellt. Jede Aktivität verfügt über bestimmte Eigenschaften sowie andere Eigenschaften, die für alle Aktivitäten gelten.

  In einem Workflow-Diagramm kann eine einzelne Aktivität verschiedene Aufgaben auslösen. Dies ist insbesondere der Fall bei Schleifen oder wiederkehrenden Aktionen.

* **Transitionen**: Transitionen verknüpfen eine Quellaktivität mit einer Zielaktivität und definieren deren Sequenz.

* **Arbeitstabellen**: Die Arbeitstabelle enthält alle von der Transition übermittelten Informationen. Jeder Workflow verwendet mehrere Arbeitstabellen. Die in diesen Tabellen übermittelten Daten können während des gesamten Lebenszyklus des Workflows verwendet werden.

## Die wichtigsten Schritte zum Erstellen eines Workflows

Die wichtigsten Schritte zum Erstellen von Workflows sehen wie folgt aus:

![](assets/workflow-creation-process.png)
