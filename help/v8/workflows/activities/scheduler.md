---
audience: end-user
title: Verwenden der Workflow-Aktivität Planung
description: Erfahren Sie, wie Sie die Workflow-Aktivität Planung verwenden.
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 37%

---


# Planung {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Planungsaktivität"
>abstract="Die Aktivität Planung ..."

Die **Planung** -Aktivität **Flusssteuerung** -Aktivität. Damit können Sie den Beginn des Workflows planen. Diese Aktivität sollte als geplanter Start betrachtet werden. Sie kann nur als erste Aktivität des Workflows verwendet werden.

## Best Practices

Es wird empfohlen, Workflows nicht öfter als alle 15 Minuten auszuführen, da die Gesamtleistung des Systems beeinträchtigt werden kann und Blöcke in der Datenbank entstehen können.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Planung** Aktivität:

1. Hinzufügen einer **Planung** -Aktivität zu Ihrem Workflow hinzu.

   <!--![](../assets/workflow-scheduler.png)-->

1. Konfigurieren Sie die **Ausführungsfrequenz**:

   * **Einmal** - der Workflow wird nur einmal ausgeführt.

   * **Täglich** - der Workflow wird jeden Tag einmal zu einem bestimmten Zeitpunkt ausgeführt.

   * **Mehrmals am Tag:** Der Workflow wird wiederholt mehrmals täglich ausgeführt. Sie können Ausführungen zu bestimmten Zeiten oder in regelmäßigen Abständen einrichten.

   * **Wöchentlich** - der Workflow wird wiederholt zu bestimmten Zeiten in der Woche ausgeführt.

   * **Monatlich** - der Workflow wird wiederholt zu bestimmten Zeiten im Monat ausgeführt. Sie können die Monate auswählen, in denen der Workflow ausgeführt werden soll. Sie können auch Ausführungen an bestimmten Wochentagen des Monats einrichten, z. B. am zweiten Dienstag des Monats.

1. Definieren Sie die Ausführungsdetails. Je nach gewählter Frequenz sind verschiedene Parameter (Uhrzeit, Ausführungsintervall, bestimmte Tage etc.) zu konfigurieren.

1. Klicks **Vorschau der Startzeiten anzeigen** um den Zeitplan der nächsten zehn Ausführungen Ihres Workflows zu überprüfen.

1. Definieren Sie den Gültigkeitszeitraum der Planung:

   * **Dauerhaft (nie abläuft)**: Der Workflow wird in der angegebenen Häufigkeit ausgeführt, wobei der Zeitraum und die Anzahl der Ausführungen unbegrenzt sind.

   * **Gültigkeitszeitraum**: Der Workflow wird in der angegebenen Häufigkeit bis zu einem bestimmten Datum ausgeführt. Sie müssen Start- und Enddaten angeben.

## Beispiel

Im folgenden Beispiel wird die Aktivität so konfiguriert, dass der Workflow mehrmals täglich um 9 und 12 Uhr, jeden Wochentag vom 1. Oktober 2023 bis zum 1. Januar 2024 gestartet wird.

<!--![](../assets/workflow-scheduler2.png)-->



