---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 9a4ca68d475cfbbcccb7a5b0d84f841589824288
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 34%

---


# Grundlegende Prinzipien der Workflow-Erstellung {#gs-workflow-creation}

In einem Workflow wird der Ablauf eines Prozesses definiert, der in einem Workflow-Diagramm dargestellt wird. Ein Workflow ist auch eine Instanz dieses Prozesses, da in der Workflow-Instanz der tatsächliche Verlauf darstellt wird.

Die Workflow-Vorlage beschreibt die verschiedenen auszuführenden Aufgaben und ihre Abfolge. Aufgabenvorlagen werden als Aktivitäten bezeichnet und durch Symbole dargestellt. Sie sind durch Transitionen miteinander verbunden.

Screenshot TBD

## Was befindet sich in einem Workflow?

Jeder Workflow besteht aus:

* **Activities**: Eine Aktivität beschreibt eine Aufgabenvorlage. Die verschiedenen verfügbaren Aktivitäten werden im Diagramm durch Symbole dargestellt. Jeder Typ verfügt über gemeinsame Eigenschaften und spezifische Eigenschaften.

   In einem Workflow-Diagramm kann eine bestimmte Aktivität mehrere Aufgaben auslösen, insbesondere bei Schleifen oder wiederkehrenden Aktionen.

* **Transitionen**: Mit Transitionen können Sie Aktivitäten verknüpfen und ihre Reihenfolge definieren. Eine Transition verknüpft eine Quellaktivität mit einer Zielaktivität.

* **Arbeitstabellen**: Die Arbeitstabelle enthält alle von der Transition übermittelten Informationen. Jeder Workflow verwendet mehrere Arbeitstabellen. Die in diesen Tabellen übermittelten Daten können beschleunigt und während des gesamten Lebenszyklus des Workflows verwendet werden, sofern sie nicht bereinigt werden. Tatsächlich werden nicht benötigte Tabellen jedes Mal bereinigt, wenn der Workflow passiviert wird, und möglicherweise während der Ausführung der größten Workflows, um eine Überlastung des Servers zu vermeiden.

## Eigenständige und Kampagnen-Workflows

Workflows können entweder als eigenständige Workflows oder aus einer Kampagne heraus erstellt werden.

TBD: Details zwischen eigenständigen und Kampagnen-Workflows.

## Die wichtigsten Schritte zum Erstellen eines Workflows

Die wichtigsten Schritte zum Erstellen von Workflows sind:

TBD: Grafik, die den gesamten Prozess mit Erläuterung und Referenz zu Dokumentenseiten anzeigt