---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 34%

---

# Starten und Überwachen Ihres Workflows {#start-monitor}

Nachdem Sie Ihren Workflow erstellt und die Aufgaben entworfen haben, die auf der Arbeitsfläche ausgeführt werden sollen, können Sie ihn starten und seine Ausführung überwachen.

## Starten des Workflows {#start}

Um den Workflow zu starten, navigieren Sie zum **[!UICONTROL Workflows]**-Menü oder zur zugehörigen Kampagne und klicken Sie auf die **[!UICONTROL Starten]**-Schaltfläche in der oberen rechten Ecke der Arbeitsfläche.

Nach Ausführung des Workflows wird jede Aktivität auf der Arbeitsfläche sequenziell ausgeführt, bis das Ende des Workflows erreicht ist.

Sie können den Fortschritt von Zielgruppenprofilen in Echtzeit über einen visuellen Fluss verfolgen. Auf diese Weise können Sie den Status jeder Aktivität und die Anzahl der Profile, die zwischen ihnen wechseln, schnell identifizieren.

![Visuelle Darstellung der laufenden Workflow-Ausführung.](assets/workflow-execution.png){zoomable="yes"}

## Workflow-Transitionen {#transitions}

In einem Workflow werden die von einer Aktivität zu einer anderen übertragenen Daten in temporären Arbeitstabellen gespeichert. Diese Daten können für jede Transition angezeigt werden. Um die Daten anzuzeigen, wählen Sie eine Transition aus, um ihre Eigenschaften auf der rechten Seite des Bildschirms zu öffnen.

* Klicken Sie auf **[!UICONTROL Vorschau für Schema]**, um das Schema der Arbeitstabelle anzuzeigen.
* Klicken Sie auf **[!UICONTROL Vorschau der Ergebnisse]**, um die in der ausgewählten Transition übertragenen Daten anzuzeigen.

![Beispiel für Übergangseigenschaften und Datenvorschau.](assets/transition.png){zoomable="yes"}

## Überwachen der Aktivitätsausführung {#activities}

Visuelle Indikatoren in der rechten oberen Ecke jedes Aktivitätsfeldes ermöglichen es, den Ausführungsstatus zu überprüfen:

| Visueller Indikator | Beschreibung |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | Die Aktivität wird derzeit ausgeführt. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | Die Aktivität erfordert Ihre Aufmerksamkeit. Dies kann die Bestätigung eines Versands oder die Ergreifung einer notwendigen Maßnahme beinhalten. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | Bei der Aktivität ist ein Fehler aufgetreten. Um das Problem zu beheben, öffnen Sie die Workflow-Protokolle, um weitere Informationen zu erhalten. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | Die Aktivität wurde erfolgreich ausgeführt. |

## Überwachen der Protokolle und Aufgaben {#logs-tasks}

Die Überwachung von Workflow-Protokollen und -Aufgaben ist ein wichtiger Schritt, um Ihre Workflows zu analysieren und sicherzustellen, dass sie ordnungsgemäß ausgeführt werden. Protokolle und Aufgaben sind über das Symbol **[!UICONTROL Protokolle]** zugänglich, das in der Aktionssymbolleiste und im Eigenschaftenbereich jeder Aktivität verfügbar ist.

Das Menü **[!UICONTROL Protokolle und Aufgaben]** enthält einen Verlauf der Workflow-Ausführung, in dem alle Benutzeraktionen und aufgetretenen Fehler aufgezeichnet werden. Dieser Verlauf wird für die in den [Ausführungsoptionen](workflow-settings.md) des Workflows angegebene Dauer gespeichert. Während dieser Dauer werden alle Nachrichten gespeichert, auch nach einem Neustart des Workflows. Wenn Sie keine Nachrichten aus einer früheren Ausführung speichern möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Verlauf bereinigen]**.

![Beispiel für die Benutzeroberfläche für Workflow-Protokolle und Aufgaben.](assets/workflow-logs.png){zoomable="yes"}

Es stehen zwei Arten von Informationen zur Verfügung:

* Die **[!UICONTROL Log]**-Registerkarte enthält den Ausführungsverlauf aller Workflow-Aktivitäten. Dabei werden die durchgeführten Vorgänge und Ausführungsfehler in chronologischer Reihenfolge indiziert.
* Die Registerkarte **[!UICONTROL Aufgaben]** liefert Details zur Ausführungsabfolge der Aktivitäten.

In beiden Registerkarten können Sie die angezeigten Spalten und ihre Reihenfolge auswählen, Filter anwenden und das Suchfeld verwenden, um die gewünschten Informationen schnell zu finden.

## Workflow-Ausführungsbefehle {#execution-commands}

Die Aktionsleiste in der rechten oberen Ecke enthält Befehle zur Verwaltung der Workflow-Ausführung. Sie haben folgende Möglichkeiten:

* **[!UICONTROL Starten]**/**[!UICONTROL Fortsetzen]** der Ausführung des Workflows. Wenn der Workflow angehalten wurde, wird er fortgesetzt. Andernfalls wird gestartet und die anfänglichen Aktivitäten werden aktiviert.
* **[!UICONTROL Pause]** die Ausführung des Workflows. Der Workflow übernimmt dann den Status „Angehalten“. Neue Aktivitäten werden erst aktiviert, wenn sie fortgesetzt werden, die laufenden Vorgänge werden jedoch nicht ausgesetzt.
* **[!UICONTROL Anhalten]** Ein Workflow, der ausgeführt wird. Der Workflow nimmt dann den Status Beendet an. Laufende Vorgänge werden nach Möglichkeit unterbrochen. Sie können den Workflow nicht an der Stelle fortsetzen, an der er gestoppt wurde.