---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Alpha"
exl-id: 8aa76369-c9f3-4c5b-9a51-101b239727e6
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 18%

---

# Workflow starten und überwachen {#start-monitor}

Nachdem Sie Ihren Workflow erstellt und die auf der Arbeitsfläche auszuführenden Aufgaben entworfen haben, können Sie ihn starten und dessen Ausführung überwachen.

## Starten des Workflows {#start}

Um den Workflow zu starten, navigieren Sie zum **[!UICONTROL Workflows]** oder der zugehörigen Kampagne und klicken Sie auf **[!UICONTROL Starten]** in der oberen rechten Ecke der Arbeitsfläche.

Nach Ausführung des Workflows wird jede Aktivität auf der Arbeitsfläche in sequenzieller Reihenfolge ausgeführt, bis das Ende des Workflows erreicht ist.

Mit einem visuellen Verlauf können Sie den Fortschritt von Zielgruppenprofilen in Echtzeit verfolgen. Auf diese Weise können Sie den Status jeder Aktivität und die Anzahl der Profile, die zwischen ihnen wechseln, schnell identifizieren.

![](assets/workflow-execution.png)

>[!NOTE]
>
>Sie können den visuellen Fluss mithilfe der **[!UICONTROL Progression ausblenden]** in der oberen Aktionsleiste der Arbeitsfläche.

## Überwachung der Aktivitätsausführung {#activities}

Visuelle Indikatoren in der oberen rechten Ecke eines jeden Aktivitätsfeldes ermöglichen es, die Ausführung zu überprüfen:

| Visueller Indikator | Beschreibung |
|-----|------------|
| ![](assets/activity-status-pending.png) | Die Aktivität wird derzeit ausgeführt. |
| ![](assets/activity-status-orange.png) | Die Aktivität erfordert Ihre Aufmerksamkeit. Dies kann die Bestätigung des Versands oder die Ergreifung der notwendigen Maßnahmen umfassen. |
| ![](assets/activity-status-red.png) | Bei der Aktivität ist ein Fehler aufgetreten. Um das Problem zu beheben, öffnen Sie die Workflow-Protokolle , um weitere Informationen zu erhalten. |
| ![](assets/activity-status-green.png) | Die Aktivität wurde erfolgreich ausgeführt. |

## Protokolle und Aufgaben überwachen {#logs-tasks}

Die Überwachung der Workflow-Protokolle und -Aufgaben ist ein wichtiger Schritt, um Ihre Workflows zu analysieren und sicherzustellen, dass sie ordnungsgemäß ausgeführt werden. Sie können über die **[!UICONTROL Protokolle]** -Symbol, das in der Symbolleiste &quot;Aktion&quot;und im Eigenschaftenbereich jeder Aktivität verfügbar ist.

Die **[!UICONTROL Protokolle und Aufgaben]** enthält einen Verlauf der Workflow-Ausführung, in dem alle Benutzeraktionen und aufgetretenen Fehler aufgezeichnet werden. Dieser Verlauf wird für die im Workflow angegebene Dauer gespeichert. [Ausführungsoptionen](workflow-settings.md). Während dieser Dauer werden alle Nachrichten gespeichert, auch nach einem Neustart des Workflows. Wenn Sie die Nachrichten einer früheren Ausführung nicht speichern möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Verlauf bereinigen]** Schaltfläche.

![](assets/workflow-logs.png)

Es stehen zwei Arten von Informationen zur Verfügung:

* Die **[!UICONTROL Protokoll]** enthält den Ausführungsverlauf aller Workflow-Aktivitäten. Er zeigt in chronologischer Abfolge alle Vorgänge und Ausführungsfehler.
* Der **[!UICONTROL Aufgaben]**-Tab liefert Details zur Ausführungsabfolge der Aktivitäten.

In beiden Registerkarten können Sie die angezeigten Spalten und ihre Reihenfolge auswählen, Filter anwenden und das Suchfeld verwenden, um die gewünschten Informationen schnell zu finden.

## Workflow-Ausführungsbefehle {#execution-commands}

Die Symbolleiste oben rechts enthält Befehle, mit denen Sie die Ausführung des Workflows verwalten können. Sie haben folgende Möglichkeiten:

* **[!UICONTROL Starten]** / **[!UICONTROL Fortsetzen]** die Ausführung des Workflows, der daraufhin den Status Gestartet annimmt. Wenn der Workflow zuvor ausgesetzt war, handelt es sich um eine Wiederaufnahme, ansonsten werden die ersten Aktivitäten aktiviert.

* **[!UICONTROL Anhalten]** die Ausführung des Workflows, der dann den Status Ausgesetzt annimmt. Bis zur Wiederaufnahme werden keine neuen Aktivitäten aktiviert, laufende Vorgänge werden jedoch fortgeführt.

* **[!UICONTROL Anhalten]** einen Workflow, der ausgeführt wird und den Status Abgeschlossen annimmt. Die laufenden Vorgänge werden nach Möglichkeit unterbrochen. Eine Wiederaufnahme an der Stelle der Unterbrechung ist nicht möglich.
