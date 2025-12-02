---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 100%

---

# Starten und Überwachen Ihres Workflows {#start-monitor}

Sobald Sie Ihren Workflow erstellt und die Aufgaben in der Arbeitsfläche entworfen haben, können Sie ihn starten und seine Ausführung überwachen.

## Starten des Workflows {#start}

Um den Workflow zu starten, navigieren Sie zum Menü **[!UICONTROL Workflows]** oder zur zugehörigen Kampagne und klicken Sie auf die Schaltfläche **[!UICONTROL Starten]** in der rechten oberen Ecke der Arbeitsfläche.

Nach Ausführung des Workflows wird jede Aktivität auf der Arbeitsfläche sequenziell ausgeführt, bis das Ende des Workflows erreicht ist.

Anhand eines visuellen Flusses können Sie den Fortschritt von Zielgruppenprofilen in Echtzeit verfolgen. Auf diese Weise können Sie den Status jeder Aktivität und die Anzahl der Profile, die zwischen ihnen wechseln, schnell identifizieren.

![Visuelle Darstellung der laufenden Workflow-Ausführung.](assets/workflow-execution.png){zoomable="yes"}

## Workflow-Transitionen {#transitions}

In einem Workflow werden die von einer Aktivität zu einer anderen übertragenen Daten in temporären Arbeitstabellen gespeichert. Diese Daten können für jede Transition angezeigt werden. Wählen Sie zum Anzeigen der Daten eine Transition aus, um ihre Eigenschaften auf der rechten Seite des Bildschirms zu öffnen.

* Klicken Sie auf **[!UICONTROL Vorschau für Schema]**, um das Schema der Arbeitstabelle anzuzeigen.
* Klicken Sie auf **[!UICONTROL Vorschau der Ergebnisse]**, um die in der ausgewählten Transition übertragenen Daten anzuzeigen.

![Beispiel für Transitionseigenschaften und Datenvorschau.](assets/transition.png){zoomable="yes"}

## Überwachen der Aktivitätsausführung {#activities}

Visuelle Indikatoren in der rechten oberen Ecke eines jeden Aktivitätsfeldes ermöglichen es, den Ausführungsstatus zu überprüfen:

| Visueller Indikator | Beschreibung |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | Die Aktivität wird derzeit ausgeführt. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | Die Aktivität erfordert Ihre Aufmerksamkeit. Dies kann die Bestätigung eines Versands oder die Ergreifung einer notwendigen Maßnahme beinhalten. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | Bei der Aktivität ist ein Fehler aufgetreten. Um das Problem zu beheben, öffnen Sie die Workflow-Protokolle, um weitere Informationen zu erhalten. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | Die Aktivität wurde erfolgreich ausgeführt. |

## Überwachen der Protokolle und Aufgaben {#logs-tasks}

Die Überwachung von Workflow-Protokollen und -Aufgaben ist ein wichtiger Schritt, um Ihre Workflows zu analysieren und sicherzustellen, dass sie ordnungsgemäß ausgeführt werden. Protokolle und Aufgaben können über das Symbol **[!UICONTROL Logs]** in der Aktionssymbolleiste und im Eigenschaftenbereich jeder Aktivität aufgerufen werden.

Das Menü **[!UICONTROL Logs und Aufgaben]** enthält einen Verlauf der Workflow-Ausführung, in dem alle Benutzeraktionen und aufgetretenen Fehler aufgezeichnet werden. Dieser Verlauf wird für die in den [Ausführungsoptionen](workflow-settings.md) des Workflows angegebene Dauer gespeichert. Innerhalb dieser Dauer werden alle Nachrichten gespeichert, auch wenn der Workflow neu gestartet wurde. Wenn Sie die Nachrichten einer früheren Ausführung nicht speichern möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Verlauf bereinigen]**.

![Beispiel für die Benutzeroberfläche für Workflow-Protokolle und -Aufgaben.](assets/workflow-logs.png){zoomable="yes"}

Es stehen zwei Arten von Informationen zur Verfügung:

* Die Registerkarte **[!UICONTROL Log]** enthält den Ausführungsverlauf aller Workflow-Aktivitäten. Er zeigt in chronologischer Abfolge alle Vorgänge und Ausführungsfehler.
* Die Registerkarte **[!UICONTROL Aufgaben]** liefert Details zur Ausführungsabfolge der Aktivitäten.

In beiden Registerkarten können Sie die angezeigten Spalten und ihre Reihenfolge auswählen, Filter anwenden und das Suchfeld verwenden, um die gewünschten Informationen schnell zu finden.

## Workflow-Ausführungsbefehle {#execution-commands}

Die Symbolleiste oben rechts enthält Befehle, mit denen Sie die Ausführung des Workflows verwalten können. Sie haben folgende Möglichkeiten:

* **[!UICONTROL Starten]**/**[!UICONTROL Wieder aufnehmen]** der Ausführung des Workflows. Wenn der Workflow angehalten wurde, wird er fortgesetzt. Andernfalls wird gestartet und die anfänglichen Aktivitäten werden aktiviert.
* **[!UICONTROL Aussetzen]** der Ausführung des Workflows. Der Workflow nimmt dann den Status „Ausgesetzt“ an. Bis zur Wiederaufnahme werden keine neuen Aktivitäten aktiviert, laufende Vorgänge werden jedoch fortgeführt.
* **[!UICONTROL Anhalten]** eines Workflows, der ausgeführt wird. Der Workflow nimmt dann den Status „Abgeschlossen“ an. Laufende Vorgänge werden nach Möglichkeit unterbrochen. Sie können den Workflow nicht an dem Punkt wieder aufnehmen, an dem er gestoppt wurde.