---
audience: end-user
title: Konfigurieren von Workflow-Einstellungen
description: Erfahren Sie, wie Sie Workflow-Einstellungen mit Adobe Campaign Web festlegen
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: 73dfc1e14e04493a76e1ca91fab0306cd1e88b26
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 100%

---

# Konfigurieren von Workflow-Einstellungen {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow-Eigenschaften"
>abstract="Wählen Sie in diesem Bildschirm die Vorlage aus, die zum Erstellen des Workflows verwendet werden soll, und geben Sie einen Titel an. Erweitern Sie den Abschnitt **Weitere Optionen**, um weitere Einstellungen wie den internen Namen des Workflows, seine Ordner, die Zeitzone und die Gruppe der Verantwortlichen zu konfigurieren. Es wird dringend empfohlen, eine Gruppe von Verantwortlichen auszuwählen, damit Benutzende benachrichtigt werden, wenn Fehler auftreten."

Greifen Sie bei der Erstellung eines Workflows oder Orchestrierung von Workflow-Aktivitäten auf der Arbeitsfläche auf erweiterte Einstellungen im Zusammenhang mit dem Workflow zu. Legen Sie beispielsweise eine bestimmte Zeitzone für den Workflow fest, verwalten Sie, wie sich der Workflow im Fehlerfall verhält, oder verwalten Sie die Verzögerung, nach der der Workflow-Verlauf bereinigt wird.

Diese Einstellungen sind in der bei der Workflow-Erstellung ausgewählten Vorlage vorkonfiguriert, können aber bei Bedarf für diesen spezifischen Workflow bearbeitet werden.

![Benutzeroberfläche mit der Schaltfläche „Workflow-Einstellungen“](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Workflow-Eigenschaften  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow-Eigenschaften "
>abstract="Dieser Abschnitt enthält allgemeine Workflow-Eigenschaften, auf die auch beim Erstellen des Workflows zugegriffen werden kann. Sie können die Vorlage auswählen, die zum Erstellen des Workflows verwendet werden soll, und einen Titel angeben. Erweitern Sie den Abschnitt „Weitere Optionen“, um bestimmte Einstellungen zu konfigurieren, z. B. den Ordner, in dem der Workflow gespeichert wird, oder die Zeitzone."

Der Abschnitt **[!UICONTROL Eigenschaften]** bietet allgemeine Einstellungen, die beim Erstellen eines Workflows konfiguriert werden können. Um auf die Eigenschaften eines bestehenden Workflows zuzugreifen, klicken Sie auf die Schaltfläche **[!UICONTROL Einstellungen]**, die in der Aktionsleiste über der Workflow-Arbeitsfläche verfügbar ist.

![Benutzeroberfläche mit der Schaltfläche „Workflow-Einstellungen“](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

Zu diesen Eigenschaften zählen:

* Der **[!UICONTROL Titel]** des Workflows, der in der Liste angezeigt wird.
* Der **[!UICONTROL interne Name]** des Workflows.
* Der **[!UICONTROL Ordner]**, in dem der Workflow gespeichert werden soll.
* Die Standard-**[!UICONTROL Zeitzone]**, die in allen Workflow-Aktivitäten zu verwenden ist. Standardmäßig ist die Zeitzone des Workflows die für die bzw. den aktuellen Campaign-Benutzerin oder -Benutzer definierte Zeitzone.
Mögliche Werte:
   * **Server-Zeitzone**, um die Zeitzone des Anwendungs-Servers von Adobe Campaign zu verwenden
   * **Benutzer-Zeitzone**, um die Zeitzone der Benutzerin bzw. des Benutzers von Adobe Campaign zu verwenden, die bzw. der den Workflow entsprechend der Definition im Benutzerprofil in der Client-Konsole ausführt.
   * **Zeitzone der Datenbank**, um die Zeitzone des Datenbank-Servers zu verwenden.
   * Eine bestimmte Zeitzone.
* Wenn ein Workflow fehlschlägt, werden die Benutzenden der im Feld **[!UICONTROL Verantwortliche(r)]** ausgewählten Benutzergruppe per E-Mail benachrichtigt.
* Geben Sie eine **[!UICONTROL Beschreibung]** Ihres Workflows ein.

Wenn der Workflow [mit einer Kampagne verknüpft](create-workflow.md) ist, wird dies im Feld **[!UICONTROL Zugehörige Kampagne]** angezeigt. Öffnen Sie die zugehörige Kampagne über dieses Feld.

## Segmentierungseinstellungen {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentierungseinstellungen"
>abstract="In diesem Bereich können Sie die Zielgruppendimension auswählen, um Profile im Workflow auszuwählen, und entscheiden, ob die Workflow-Ergebnisse zwischen zwei Ausführungen beibehalten werden sollen. Diese Option sollte nur zu Testzwecken verwendet werden und darf in einem Produktions-Workflow nie aktiviert werden."

* **[!UICONTROL Zielgruppendimension]**: Wählen Sie die Zielgruppendimension aus, die für die Zielgruppenbestimmung von Profilen wie z. B. Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnierende und andere verwendet werden soll. [Erfahren Sie mehr über Zielgruppendimensionen](../audience/targeting-dimensions.md)

* **[!UICONTROL Zwischen zwei Ausführungen die ermittelte Population festhalten]**: Standardmäßig werden nur die Arbeitstabellen der letzten Ausführung des Workflows beibehalten. Arbeitstabellen früherer Ausführungen werden durch einen technischen Workflow bereinigt, der täglich ausgeführt wird.

  Wenn diese Option aktiviert ist, werden Arbeitstabellen auch nach Ausführung des Workflows beibehalten. Verwenden Sie sie zu Testzwecken und stellen Sie sicher, dass sie **nur** in Entwicklungs- oder Staging-Umgebungen genutzt werden. Sie darf niemals in einem Produktions-Workflow aktiviert sein.

## Ausführungsparameter {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Ausführungsparameter"
>abstract="In diesem Abschnitt können Sie Einstellungen für die Ausführung des Workflows konfigurieren, z. B. für wie viele Tage der Workflow-Verlauf gespeichert wird."

* **[!UICONTROL Verlauf in Tagen]**: Gibt die Anzahl der Tage an, nach denen der Verlauf bereinigt werden muss. Der Verlauf enthält Elemente im Zusammenhang mit dem Workflow: Protokolle, Aufgaben und Ereignisse (technische Objekte, die mit dem Workflow-Vorgang verknüpft sind). Der Standardwert bei vordefinierten Workflow-Vorlagen beträgt 30 Tage. Die Bereinigung des Verlaufs erfolgt durch den technischen Workflow für die Datenbankbereinigung, der täglich ausgeführt wird.

  >[!IMPORTANT]
  >
  >Wenn das Feld **[!UICONTROL Verlaufsumfang in Tagen]** leer gelassen wird, wird sein Wert als „1“ betrachtet; der Verlauf wird also nach einem Tag bereinigt.

* **[!UICONTROL Standard-Affinität]**: Wenn Ihre Installation mehrere Workflow-Server umfasst, geben Sie über dieses Feld den Server an, auf dem der Workflow ausgeführt werden soll. Dies erzwingt die Ausführung dieses Workflows auf einem bestimmten Server. Wählen Sie einen beliebigen vorhandenen Affinitätsnamen aus. Stellen Sie jedoch sicher, dass Sie keine Leerzeichen oder Satzzeichen verwenden. Wenn Sie verschiedene Server verwenden, geben Sie unterschiedliche Namen an, die durch Kommas getrennt sind.

  >[!IMPORTANT]
  >
  >Wenn der in diesem Feld definierte Wert auf keinem Server vorhanden ist, bleibt der Workflow ausstehend.

* **[!UICONTROL SQL-Abfragen im Protokoll speichern]**: Mit dieser Option können Sie die SQL-Abfragen aus dem Workflow in den Protokollen speichern. Diese Funktion ist erfahrenen Benutzerinnen und Benutzern vorbehalten. Sie gilt für Workflows, die Zielgruppenbestimmungsaktivitäten enthalten, wie **[!UICONTROL Zielgruppe erstellen]**. Wenn diese Option aktiviert ist, werden die während der Workflow-Ausführung an die Datenbank gesendeten SQL-Abfragen in den Protokollen des Workflows angezeigt, sodass Sie sie analysieren können, um Abfragen zu optimieren oder Probleme zu diagnostizieren.

## Einstellungen für den Umgang mit Fehlern {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Einstellungen für den Umgang mit Fehlern"
>abstract="In diesem Abschnitt können Sie definieren, wie der Workflow mit Fehlern während seiner Ausführung umgehen soll. Sie können festlegen, dass der Prozess angehalten werden soll, dass eine bestimmte Anzahl von Fehlern ignoriert werden soll oder dass die Ausführung des Workflows gestoppt werden soll."

* **[!UICONTROL Umgang mit Fehlern]**: In diesem Feld können Sie festlegen, welche Aktionen ausgeführt werden sollen, wenn eine Workflow-Aufgabe Fehler aufweist. Es gibt drei mögliche Optionen:

   * **[!UICONTROL Prozess aussetzen]**: Der Workflow wird automatisch ausgesetzt und der Status wechselt zu **[!UICONTROL Fehlgeschlagen]**. Sobald das Problem behoben ist, setzen Sie den Workflow mit der Schaltfläche **[!UICONTROL Fortsetzen]** fort.
   * **[!UICONTROL Ignorieren]**: Der Status der Aufgabe, die den Fehler ausgelöst hat, ändert sich in **[!UICONTROL Fehlgeschlagen]**, der Workflow behält jedoch den Status **[!UICONTROL Gestartet]**. <!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Vorgang abbrechen]**: Der Workflow wird automatisch angehalten und der Status ändert sich zu **[!UICONTROL Fehlgeschlagen]**. Sobald das Problem behoben ist, starten Sie den Workflow mit der Schaltfläche **[!UICONTROL Starten]** neu.

* **[!UICONTROL Aufeinanderfolgende Fehler]**: Dieses Feld wird verfügbar, wenn im Feld **[!UICONTROL Im Fehlerfall]** der Wert **[!UICONTROL Ignorieren]** ausgewählt wurde. Geben Sie die Anzahl der Fehler an, die ignoriert werden können, bevor der Prozess angehalten wird. Sobald diese Zahl erreicht ist, wechselt der Workflow-Status zu **[!UICONTROL Fehlgeschlagen]**. Wenn der Wert dieses Felds 0 beträgt, wird der Workflow unabhängig von der Fehleranzahl nie angehalten.

## Initialisierungsskript {#initialization-script}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initialization"
>title="Initialisierungsskript"
>abstract="In diesem Abschnitt können Sie JavaScript-Code definieren, der zu Beginn des Workflows ausgeführt wird. Er kann verwendet werden, um Variablen zu initialisieren, Parameter festzulegen oder Daten vorzubereiten, bevor Workflow-Aktivitäten ausgeführt werden."

Mit dem **Initialisierungsskript** können Sie Variablen initialisieren oder Aktivitätseigenschaften ändern. Klicken Sie auf die Schaltfläche **Code bearbeiten** und geben Sie das auszuführende Code-Snippet ein. Das Skript wird aufgerufen, wenn der Workflow ausgeführt wird. Weitere Informationen finden Sie im Abschnitt zu den [Ereignisvariablen](../workflows/event-variables.md).