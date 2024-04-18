---
audience: end-user
title: Workflow-Ereignisvariablen
description: Erfahren Sie, wie Sie Ereignisvariablen in Ihren Workflows nutzen können.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: c3f04d3828f22207bd5e9a0e8c334e8f7a57b2c1
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Workflow-Ereignisvariablen {#event-variables}

Einige Workflow-Aktivitäten ermöglichen es Ihnen, Skripte im Ausdruckseditor zu bearbeiten, um bestimmte Aktionen durchzuführen, z. B. das Abrufen von Daten aus früheren Aktivitäten, das Erstellen von Bedingungen oder das Berechnen von Dateinamen basierend auf Ereignisvariablen.

## Was sind Ereignisvariablen {#scripting}

Im Rahmen eines Workflows ausgeführte Skripte greifen auf eine Reihe zusätzlicher globaler **Objekte** z. B. der selbst ausgeführte Workflow (`ìnstance`), die verschiedenen Aufgaben (`task`) oder die Ereignisse, die eine bestimmte Aufgabe (`event`).

Für jeden Typ von **Objekt** ist mit einer Kategorie von **variables** die im Ausdruckseditor beim Bearbeiten von Skripten in Aktivitäten wie **[!UICONTROL JavaScript-Code]** oder **[!UICONTROL Test]**.

* **Instanzvariablen** (`instance.vars.xxx`) sind mit globalen Variablen vergleichbar. Sie werden für alle Aktivitäten freigegeben.
* **Aufgabenvariablen** (`task.vars.xxx`) sind mit lokalen Variablen vergleichbar. Sie werden nur von der aktuellen Aufgabe verwendet. Diese Variablen werden von persistenten Aktivitäten verwendet, um Daten beizubehalten, und manchmal zum Austausch von Daten zwischen den verschiedenen Skripten einer Aktivität verwendet.
* **Ereignisvariablen** (`vars.xxx`) ermöglichen den Austausch von Daten zwischen elementaren Aufgaben eines Workflow-Prozesses. Diese Variablen werden von der Aufgabe übergeben, die die laufende Aufgabe aktiviert hat. Sie werden dann an die folgenden Aktivitäten übergeben. **Ereignisvariablen** sind die am häufigsten verwendeten Variablen, und sie sollten Instanzvariablen vorgezogen werden.

>[!NOTE]
>
>Weitere Informationen zur Skripterstellung sowie zu den angezeigten Objekten und Variablen in Adobe Campaign finden Sie in der Dokumentation zu Campaign v8 (Clientkonsole) in [diesem Abschnitt](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Beachten Sie, dass diese Ressource zwar wertvolle Einblicke bietet, jedoch möglicherweise Diskrepanzen vorliegen, da sie speziell für die Clientkonsole und nicht für die Campaign-Webbenutzeroberfläche gilt.

## Ereignisvariablen im Ausdruckseditor nutzen {#expression-editor}

Vordefinierte Ereignisvariablen sind im linken Bereich des Ausdruckseditors verfügbar. Sie können auch neue erstellen, indem Sie eine neue Variable in Ihrem Code initialisieren.

![](assets/event-variables.png)

Zusätzlich zu diesen Ereignisvariablen können Sie auch die **[!UICONTROL Bedingungen]** im linken Bereich, um Bedingungen zu erstellen, und die **[!UICONTROL Aktuelles Datum hinzufügen]** Menü zur Verwendung von Funktionen zur Datumsformatierung.
