---
audience: end-user
title: Konfigurieren von Workflow-Einstellungen
description: Erfahren Sie, wie Sie Workflow-Einstellungen mit Adobe Campaign Web festlegen
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 50%

---

# Konfigurieren von Workflow-Einstellungen {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow-Eigenschaften"
>abstract="Wählen Sie in diesem Bildschirm die Vorlage aus, die zum Erstellen des Workflows verwendet werden soll, und geben Sie einen Titel an. Erweitern Sie den Abschnitt **Zusätzliche Optionen**, um weitere Einstellungen wie den internen Namen des Workflows, seinen Ordner, seine Zeitzone und die Gruppe der Verantwortlichen zu konfigurieren. Es wird dringend empfohlen, eine Gruppe von Verantwortlichen auszuwählen, damit Benutzende benachrichtigt werden, wenn Fehler auftreten."

Greifen Sie beim Erstellen eines Workflows oder bei der Orchestrierung von Workflow-Aktivitäten auf der Arbeitsfläche auf die erweiterten Einstellungen zu, die sich auf den Workflow beziehen. Legen Sie beispielsweise eine bestimmte Zeitzone für den Workflow fest, verwalten Sie, wie sich der Workflow im Fehlerfall verhalten soll, oder verwalten Sie die Verzögerung, nach der der Workflow-Verlauf bereinigt wird.

Diese Einstellungen sind in der bei der Workflow-Erstellung ausgewählten Vorlage vorkonfiguriert, können aber bei Bedarf für diesen spezifischen Workflow bearbeitet werden.

![Benutzeroberfläche der Schaltfläche „Workflow-Einstellungen“](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Workflow-Eigenschaften  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow-Eigenschaften "
>abstract="Dieser Abschnitt enthält allgemeine Workflow-Eigenschaften, auf die auch beim Erstellen des Workflows zugegriffen werden kann. Sie können die Vorlage auswählen, die zum Erstellen des Workflows verwendet werden soll, und einen Titel angeben. Erweitern Sie den Abschnitt Zusätzliche Optionen , um bestimmte Einstellungen zu konfigurieren, z. B. den Ordner zum Speichern von Workflows oder die Zeitzone."

Der Abschnitt **[!UICONTROL Eigenschaften]** enthält allgemeine Einstellungen, die beim Erstellen eines Workflows konfiguriert werden können. Um auf die Eigenschaften eines bestehenden Workflows zuzugreifen, klicken Sie auf die Schaltfläche **[!UICONTROL Einstellungen]**, die in der Aktionsleiste über der Workflow-Arbeitsfläche verfügbar ist.

![Benutzeroberfläche für Workflow-Einstellungen](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

Zu diesen Eigenschaften gehören:

* Der **[!UICONTROL Titel]** des Workflows, der in der Liste angezeigt wird.
* Der **[!UICONTROL interne Name]** des Workflows.
* Der **[!UICONTROL Ordner]**, in dem der Workflow gespeichert werden soll.
* Die Standard-**[!UICONTROL Zeitzone]**, die in allen Workflow-Aktivitäten zu verwenden ist. Standardmäßig ist die Zeitzone des Workflows die für den aktuellen Campaign-Benutzer definierte Zeitzone.
Mögliche Werte:
   * **Server-Zeitzone**, um die Zeitzone des Adobe Campaign-Anwendungsservers zu verwenden.
   * **Zeitzone des Benutzers** um die Zeitzone des Adobe Campaign-Benutzers zu verwenden, der den Workflow ausführt, wie im Benutzerprofil in der Client-Konsole definiert.
   * **Zeitzone der Datenbank**, um die Zeitzone des Datenbank-Servers zu verwenden.
   * Eine bestimmte Zeitzone.
* Wenn ein Workflow fehlschlägt, werden die Benutzer, die zur Benutzergruppe gehören, die im Feld **[!UICONTROL Verantwortliche(r)) ausgewählt]**, per E-Mail benachrichtigt.
* Geben Sie **[!UICONTROL Beschreibung]** Ihres Workflows ein.

Wenn der Workflow [mit einer Kampagne verknüpft](create-workflow.md) wird er im Feld **[!UICONTROL Verknüpfte Kampagne]** angezeigt. Öffnen Sie die zugehörige Kampagne in diesem Feld.

## Segmentierungseinstellungen {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentierungseinstellungen"
>abstract="In diesem Abschnitt können Sie die Zielgruppendimension auswählen, um Profile im Workflow auszuwählen, und festlegen, dass die Workflow-Ergebnisse zwischen zwei Ausführungen beibehalten werden. Diese Option sollte nur zu Testzwecken verwendet werden und darf in einem Produktions-Workflow nie aktiviert werden."

* **[!UICONTROL Zielgruppendimension]**: Wählen Sie die Zielgruppendimension aus, die für die Zielgruppenbestimmung von Profilen verwendet werden soll, z. B. Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten und andere. [Erfahren Sie mehr über Zielgruppendimensionen](../audience/targeting-dimensions.md)

* **[!UICONTROL Zwischen zwei Ausführungen die ermittelte Population festhalten]**: Standardmäßig werden nur die Arbeitstabellen der letzten Ausführung des Workflows beibehalten. Arbeitstabellen früherer Ausführungen werden durch einen täglich ausgeführten technischen Workflow bereinigt.

  Wenn diese Option aktiviert ist, werden Arbeitstabellen auch nach Ausführung des Workflows beibehalten. Verwenden Sie sie zu Testzwecken und stellen Sie sicher, dass sie **nur** in Entwicklungs- oder Staging-Umgebungen verwendet wird. Sie darf niemals in einem Produktions-Workflow aktiviert sein.

## Ausführungsparameter {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Ausführungsparameter"
>abstract="In diesem Abschnitt können Sie Einstellungen für die Ausführung des Workflows konfigurieren, z. B. die Anzahl der Tage, die der Workflow-Verlauf gespeichert wird."

* **[!UICONTROL Verlauf in Tagen]**: Gibt die Anzahl der Tage an, nach denen der Verlauf bereinigt werden muss. Der Verlauf enthält Elemente, die mit dem Workflow verbunden sind, wie Protokolle, Aufgaben und Ereignisse (technische Objekte, die mit dem Workflow-Vorgang verknüpft sind). Der Standardwert bei nativen Workflow-Vorlagen beträgt 30 Tage. Die Bereinigung des Verlaufs erfolgt durch den technischen Workflow Datenbankbereinigung , der täglich ausgeführt wird.

  >[!IMPORTANT]
  >
  >Wenn das Feld **[!UICONTROL Verlauf in Tagen]** leer gelassen wird, wird sein Wert als „1“ betrachtet; der Verlauf wird also nach einem Tag bereinigt.

* **[!UICONTROL Standardaffinität]**: Wenn Ihre Installation mehrere Workflow-Server umfasst, geben Sie in diesem Feld den Server an, auf dem der Workflow ausgeführt werden soll. Dies erzwingt die Ausführung dieses Workflows auf einem bestimmten Server. Wählen Sie einen vorhandenen Affinitätsnamen aus, stellen Sie jedoch sicher, dass Sie keine Leerzeichen oder Satzzeichen verwenden. Wenn Sie verschiedene Server verwenden, geben Sie unterschiedliche Namen an, die durch Kommas getrennt sind.

  >[!IMPORTANT]
  >
  >Wenn der in diesem Feld definierte Wert auf keinem Server vorhanden ist, bleibt der Workflow ausstehend.

* **[!UICONTROL SQL-Abfragen im Protokoll speichern]**: Aktivieren Sie diese Option, um die SQL-Abfragen aus dem Workflow in den Protokollen zu speichern. Diese Funktion ist erfahrenen Benutzerinnen und Benutzern vorbehalten. Sie gilt für Workflows, die Zielgruppenbestimmungsaktivitäten enthalten, wie **[!UICONTROL Zielgruppe aufbauen]**. Wenn diese Option aktiviert ist, werden die während der Workflow-Ausführung an die Datenbank gesendeten SQL-Abfragen in den Protokollen des Workflows angezeigt, sodass Sie sie analysieren können, um Abfragen zu optimieren oder Probleme zu diagnostizieren.

## Einstellungen für den Umgang mit Fehlern {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Einstellungen für den Umgang mit Fehlern"
>abstract="In diesem Abschnitt können Sie definieren, wie der Workflow mit Fehlern während seiner Ausführung umgehen soll. Sie können festlegen, dass der Prozess angehalten werden soll, dass eine bestimmte Anzahl von Fehlern ignoriert werden soll oder dass die Ausführung des Workflows gestoppt werden soll."

* **[!UICONTROL Umgang mit Fehlern]**: In diesem Feld können Sie festlegen, welche Aktionen ausgeführt werden sollen, wenn eine Workflow-Aufgabe Fehler aufweist. Es gibt drei mögliche Optionen:

   * **[!UICONTROL Prozess aussetzen]**: Der Workflow wird automatisch ausgesetzt und der Status ändert sich in **[!UICONTROL Fehlgeschlagen]**. Sobald das Problem behoben ist, setzen Sie den Workflow mit der Schaltfläche **[!UICONTROL Fortsetzen]** fort.
   * **[!UICONTROL Ignorieren]**: Der Status der Aufgabe, die den Fehler ausgelöst hat, ändert sich in **[!UICONTROL Fehlgeschlagen]**, der Workflow behält jedoch den Status **[!UICONTROL Gestartet]**. <!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Vorgang abbrechen]**: Der Workflow wird automatisch angehalten und der Status ändert sich in **[!UICONTROL Fehlgeschlagen]**. Sobald das Problem behoben ist, starten Sie den Workflow mit der Schaltfläche **[!UICONTROL Starten]** erneut.

* **[!UICONTROL Aufeinanderfolgende Fehler]**: Dieses Feld wird verfügbar, wenn im Feld **[!UICONTROL Im Fehlerfall]** der Wert **[!UICONTROL Ignorieren]** ausgewählt wurde. Geben Sie die Anzahl der Fehler an, die ignoriert werden können, bevor der Prozess angehalten wird. Sobald diese Zahl erreicht ist, wechselt der Workflow-Status zu **[!UICONTROL Fehlgeschlagen]**. Wenn der Wert dieses Felds 0 beträgt, wird der Workflow unabhängig von der Fehleranzahl nie angehalten.

## Initialisierungsskript {#initialization-script}

Mit dem **Initialisierungsskript** können Sie Variablen initialisieren oder Aktivitätseigenschaften ändern. Klicken Sie auf die Schaltfläche **Code bearbeiten** und geben Sie das auszuführende Code-Snippet ein. Das Skript wird aufgerufen, wenn der Workflow ausgeführt wird. Weitere Informationen finden Sie im Abschnitt zu den [Ereignisvariablen](../workflows/event-variables.md).