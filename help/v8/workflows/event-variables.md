---
audience: end-user
title: Workflow-Ereignisvariablen
description: Erfahren Sie, wie Sie Ereignisvariablen in Ihren Workflows nutzen können.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 43%

---

# Workflow-Ereignisvariablen {#event-variables}

Einige Workflow-Aktivitäten ermöglichen es Ihnen, Skripte im Ausdruckseditor zu bearbeiten, um bestimmte Aktionen auszuführen, z. B. das Abrufen von Daten aus vorherigen Aktivitäten, Erstellen von Bedingungen oder Berechnen von Dateinamen basierend auf Ereignisvariablen.

## Was sind Ereignisvariablen? {#scripting}

Skripte, die im Kontext eines Workflows ausgeführt werden, greifen auf eine Reihe zusätzlicher globaler **Objekte** zu, z. B. den Workflow selbst, der ausgeführt wird (`instance`), seine verschiedenen Aufgaben (`task`) oder die Ereignisse, die eine bestimmte Aufgabe aktiviert haben (`event`).

Jeder Typ von **Objekt** ist mit einer Kategorie von **Variablen** verknüpft, die im Ausdruckseditor beim Bearbeiten von Skripten in Aktivitäten wie **[!UICONTROL JavaScript-Code]** oder **[!UICONTROL Test]** verwendet werden können.

* **Instanzvariablen** (`instance.vars.xxx`) sind mit globalen Variablen vergleichbar. Sie werden von allen Aktivitäten geteilt.
* **Task-Variablen** (`task.vars.xxx`) sind vergleichbar mit lokalen Variablen. Sie werden nur von der aktuellen Aufgabe verwendet. Diese Variablen werden von persistenten Aktivitäten verwendet, um Daten beizubehalten, und manchmal zum Austausch von Daten zwischen verschiedenen Skripten derselben Aktivität.
* **Ereignisvariablen** (`vars.xxx`) ermöglichen den Austausch von Daten zwischen den elementaren Aufgaben eines Workflow-Prozesses. Diese Variablen werden von der Aufgabe übergeben, die die in Bearbeitung befindliche Aufgabe aktiviert hat. Sie werden dann an die folgenden Aktivitäten weitergeleitet. **Ereignisvariablen** sind die am häufigsten verwendeten Variablen und sollten vorzugsweise anstelle von Instanzvariablen verwendet werden.

>[!NOTE]
>
>Weitere Informationen zur Skripterstellung und zu den Skript-Objekten und -Variablen in Adobe Campaign finden Sie in der Dokumentation zu Campaign v8 (Client-Konsole) [in diesem Abschnitt](https://experienceleague.adobe.com/de/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Bitte beachten Sie, dass diese Ressource zwar wertvolle Erkenntnisse bietet, es jedoch zu Unstimmigkeiten kommen kann, da sie sich speziell auf die Client-Konsole und nicht auf die Campaign Web-Benutzeroberfläche bezieht.

## Nutzung von Ereignisvariablen im Ausdruckseditor {#expression-editor}

Vordefinierte Ereignisvariablen sind für die Verwendung im linken Bereich des Ausdruckseditors verfügbar. Sie können auch neue erstellen, indem Sie eine neue Variable in Ihrem Code initialisieren.

![Screenshot mit vordefinierten Ereignisvariablen im linken Bereich des Ausdruckseditors](assets/event-variables.png)

Zusätzlich zu diesen Ereignisvariablen können Sie auch das Menü **[!UICONTROL Bedingungen]** im linken Bereich zum Erstellen von Bedingungen und das Menü **[!UICONTROL Aktuelles Datum hinzufügen]** zum Anwenden von Funktionen im Zusammenhang mit der Datumsformatierung verwenden.