---
audience: end-user
title: Verwenden der Workflow-Aktivität „Planung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Planung“ verwenden.
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 29%

---

# Planung {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Scheduler activity"
>abstract="The **Scheduler** activity allows you to schedule when the workflow gets started. This activity should be considered as a scheduled start. It can only be used as the first activity of the workflow."

## Best Practices {#scheduler-best-practices}

* Planen Sie die Ausführung eines Workflows nicht öfter als alle 15 Minuten, da die Gesamtleistung des Systems beeinträchtigt werden kann und Blockierungen in der Datenbank entstehen können.
* Um einen einmaligen Versand in Ihrem Workflow durchzuführen, fügen Sie eine Planungsaktivität hinzu und legen Sie sie auf &quot;**&quot;**. Definieren Sie **Zeitplan** in den Versandeinstellungen.
* Verwenden Sie zum Versand eines wiederkehrenden Versands in Ihrem Workflow eine **Planung**-Aktivität und legen Sie die Ausführungsfrequenz fest. Die Aktivität „Wiederkehrender Versand“ ermöglicht keine Festlegung eines Zeitplans.

## Konfigurieren der Aktivität „Planung“ {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Scheduler validity"
>abstract="You can define a validity period for the scheduler. It can be permanent (default), or can be valid until a specific date."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler options"
>abstract="Define the frequency of the scheduler. It can be executed at a specific moment, once or several times a day, week or month."

Gehen Sie folgendermaßen vor, um die Aktivität **Planung** zu konfigurieren:

![Benutzeroberfläche für die Konfiguration der Planungsaktivität](../assets/workflow-scheduler.png)

1. Fügen Sie eine **Planungsaktivität** zu Ihrem Workflow hinzu.

1. Konfigurieren Sie die **Ausführungshäufigkeit**:

   * **Einmal**: Der Workflow wird ein einziges Mal ausgeführt.
   * **Täglich**: Der Workflow wird zu einem bestimmten Zeitpunkt einmal täglich ausgeführt.
   * **Mehrmals am Tag**: Der Workflow wird regelmäßig mehrmals am Tag ausgeführt. Richten Sie Ausführungen zu bestimmten Zeiten oder regelmäßig ein.
   * **Wöchentlich**: Der Workflow wird zu einem bestimmten Zeitpunkt einmal oder mehrmals pro Woche ausgeführt.
   * **Monatlich**: Der Workflow wird zu einem bestimmten Zeitpunkt einmal oder mehrmals im Monat ausgeführt. Wählen Sie die Monate aus, in denen der Workflow ausgeführt werden muss. Sie können Ausführungen auch an bestimmten Wochentagen des Monats einrichten, z. B. am zweiten Dienstag des Monats.

1. Definieren Sie die Ausführungsdetails. Die Detailfelder können je nach verwendeter Häufigkeit variieren (Zeit, Wiederholungshäufigkeit, angegebene Tage und ähnliche Optionen).

1. Klicken Sie auf **Vorschau der Startzeiten anzeigen**, um den Zeitplan der nächsten zehn Ausführungen Ihres Workflows zu überprüfen.

1. Definieren Sie den Gültigkeitszeitraum der Planung:

   * **Permanent (läuft nie ab)**: Der Workflow wird mit der angegebenen Häufigkeit ausgeführt, ohne Begrenzung des Zeitrahmens oder der Anzahl der Iterationen.
   * **Gültigkeitszeitraum**: Der Workflow wird entsprechend der angegebenen Häufigkeit bis zu einem bestimmten Datum ausgeführt. Geben Sie das Start- und Enddatum an.

>[!NOTE]\
Wenn Sie den Workflow sofort starten möchten, klicken Sie in der oberen Aktionsleiste **Planung auf** Aufgabe ausführen. Diese Schaltfläche ist nur verfügbar, wenn der Workflow gestartet wurde.

## Beispiel {#scheduler-example}

Im folgenden Beispiel wird die Aktivität so konfiguriert, dass der Workflow mehrmals täglich um 9 und 12 Uhr ausgeführt wird, und zwar an jedem Wochentag vom 1. Oktober 2023 bis zum 1. Januar 2024.

![Beispielkonfiguration für Planungsaktivität](../assets/workflow-scheduler2.png)