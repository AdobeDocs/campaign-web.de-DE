---
audience: end-user
title: Verwenden der Workflow-Aktivität „Planung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Planung“ verwenden.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 023777b88fa5c80e110fcf334517f7cef1c7f1ee
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 100%

---

# Planung {#scheduler}


>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Planungsaktivität"
>abstract="Mit der Aktivität **Planung** können Sie planen, wann der Workflow gestartet werden soll. Diese Aktivität sollte als geplanter Start betrachtet werden. Sie kann nur als erste Aktivität des Workflows verwendet werden."


Die Aktivität **Planung** ist eine Aktivität zur **Flusssteuerung**. Damit können Sie planen, wann der Workflow gestartet werden soll. Diese Aktivität sollte als geplanter Start betrachtet werden. Sie kann nur als erste Aktivität des Workflows verwendet werden.

## Best Practices{#scheduler-best-practices}

* Es wird empfohlen, Workflows nicht öfter als alle 15 Minuten auszuführen, da die Gesamt-Performance des Systems beeinträchtigt werden kann und Blöcke in der Datenbank entstehen können.
* Wenn Sie in Ihrem Workflow einen einmaligen Versand senden möchten, können Sie eine Planungsaktivität hinzufügen und für sie festlegen, dass sie **einmal** ausgeführt wird. Sie können außerdem den **Zeitplan** in den Versandeinstellungen festlegen.
* Wenn Sie einen wiederkehrenden Versand in Ihrem Workflow durchführen möchten, müssen Sie eine **Planungsaktivität** verwenden und die Ausführungshäufigkeit festlegen. Die Aktivität „Wiederkehrender Versand“ ermöglicht keine Festlegung eines Zeitplans.

## Konfigurieren der Aktivität „Planung“ {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Gültigkeit der Planung"
>abstract="Sie können einen Gültigkeitszeitraum für die Planung definieren. Er kann dauerhaft sein (Standard) oder bis zu einem bestimmten Datum gültig sein."


>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Planungsoptionen"
>abstract="Definieren Sie die Häufigkeit der Planung. Er kann zu einem bestimmten Zeitpunkt, einmal oder mehrmals pro Tag, Woche oder Monat, ausgeführt werden."

Gehen Sie folgendermaßen vor, um die Aktivität **Planung** zu konfigurieren:

![](../assets/workflow-scheduler.png)

1. Fügen Sie eine **Planungsaktivität** zu Ihrem Workflow hinzu.

1. Konfigurieren Sie die **Ausführungshäufigkeit**:

   * **Einmal** – der Workflow wird nur einmal ausgeführt.

   * **Täglich** – der Workflow wird jeden Tag einmal zu einem bestimmten Zeitpunkt ausgeführt.

   * **Mehrmals pro Tag** – der Workflow wird wiederholt zu bestimmten Zeiten am Tag ausgeführt. Sie können Ausführungen zu bestimmten Zeiten oder in regelmäßigen Abständen einrichten.

   * **Wöchentlich** - der Workflow wird wiederholt zu bestimmten Zeiten in der Woche ausgeführt.

   * **Monatlich** - der Workflow wird wiederholt zu bestimmten Zeiten im Monat ausgeführt. Sie können die Monate auswählen, in denen der Workflow ausgeführt werden soll. Sie können für die Ausführung von Workflows auch bestimmte Wochentage des Monats auswählen, z. B. am zweiten Dienstag des Monats.

1. Definieren Sie die Ausführungsdetails. Je nach gewählter Frequenz sind verschiedene Parameter (Uhrzeit, Ausführungsintervall, bestimmte Tage etc.) zu konfigurieren.

1. Klicken Sie auf **Vorschau der Startzeiten anzeigen**, um den Zeitplan der nächsten zehn Ausführungen Ihres Workflows zu überprüfen.

1. Definieren Sie den Gültigkeitszeitraum der Planung:

   * **Permanent (läuft nie ab)** – der Workflow auf Dauer in den angegebenen Intervallen ausgeführt, ohne Begrenzungen, was den Zeitrahmen oder die Anzahl von Iterationen betrifft.

   * **Gültigkeitszeitraum** – Der Workflow wird in der angegebenen Häufigkeit bis zu einem bestimmten Datum ausgeführt. Sie müssen Start- und Enddaten angeben.

>[!NOTE]
>
>Wenn Sie den Workflow sofort starten möchten, können Sie auf die Schaltfläche **Ausstehende Aufgabe ausführen** in der oberen Symbolleiste der Planung klicken. Diese Schaltfläche ist nur verfügbar, wenn Sie den Workflow gestartet haben.

## Beispiel{#scheduler-example}

Im folgenden Beispiel wird die Aktivität so konfiguriert, dass der Workflow mehrmals am Tag um 9 Uhr und 12 Uhr ausgeführt wird, und zwar jeden Wochentag vom 1. Oktober 2023 bis zum 1. Januar 2024.

![](../assets/workflow-scheduler2.png)
