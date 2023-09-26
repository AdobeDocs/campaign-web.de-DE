---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Beta"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 140c12fbfb40ec2df2c25aacc762f344f78d9a5a
workflow-type: ht
source-wordcount: '903'
ht-degree: 100%

---

# Konfigurieren von Workflow-Einstellungen {#workflow-settings}

Bei der Orchestrierung von Workflow-Aktivitäten auf der Arbeitsfläche können Sie auf erweiterte Einstellungen im Zusammenhang mit dem Workflow zugreifen. Sie können beispielsweise eine bestimmte Zeitzone für den Workflow festlegen, verwalten, wie sich der Workflow im Fehlerfall verhält, oder die Verzögerung verwalten, nach der der Workflow-Verlauf bereinigt werden soll.

Diese Einstellungen sind in der bei der Workflow-Erstellung ausgewählten Vorlage vorkonfiguriert, können aber bei Bedarf für diesen spezifischen Workflow bearbeitet werden.

Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Einstellungen]** in der Aktionsleiste über der Workflow-Arbeitsfläche.

![](assets/workflow-settings.png)

## Workflow-Eigenschaften  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow-Eigenschaften "
>abstract="Dieser Abschnitt enthält allgemeine Workflow-Eigenschaften, auf die auch beim Erstellen des Workflows zugegriffen werden kann. Sie können die Vorlage auswählen, die zum Erstellen des Workflows verwendet werden soll, und einen Titel angeben. Erweitern Sie den Abschnitt „zusätzliche Optionen“, um bestimmte Einstellungen zu konfigurieren, z. B. den Ordner, in dem der Workflow gespeichert wird, oder die Zeitzone."

Der Abschnitt **[!UICONTROL Eigenschaften]** enthält allgemeine Einstellungen, auf die auch bei der Erstellung des Workflows zugegriffen werden kann.

* **[!UICONTROL Titel]**: Der Titel des Workflows, der in der Liste angezeigt wird.
* **[!UICONTROL Name]**: Interner Name des Workflows.
* **[!UICONTROL Ordner]**: Der Ordner, in dem der Workflow gespeichert werden soll.
* **[!UICONTROL Verknüpfte Kampagne]**: Dieses Feld wird angezeigt, wenn der Workflow innerhalb einer Kampagne erstellt wurde. Damit können Sie die zugehörige Kampagne öffnen.
* **[!UICONTROL Zeitzone]**: Definieren Sie eine bestimmte Zeitzone, die standardmäßig für alle Aktivitäten des Workflows verwendet werden soll. Standardmäßig ist die Zeitzone des Workflows die für die aktuelle Campaign-Benutzerin bzw. den aktuellen Campaign-Benutzer definierte Zeitzone.
Andere mögliche Werte sind:
   * **Server-Zeitzone**, um die Zeitzone des Anwendungs-Servers von Adobe Campaign zu verwenden
   * **Benutzer-Zeitzone**, um die Zeitzone der Benutzerin bzw. des Benutzers von Adobe Campaign zu verwenden, die bzw. der den Workflow entsprechend der Definition im Benutzerprofil in der Client-Konsole ausführt.
   * **Zeitzone der Datenbank**, um die Zeitzone des Datenbank-Servers zu verwenden.
   * Eine bestimmte Zeitzone

* **[!UICONTROL Supervisor(en)]**: Wenn ein Workflow fehlschlägt, werden die Benutzenden der in diesem Feld ausgewählten Benutzergruppe per E-Mail benachrichtigt.
* **[!UICONTROL Beschreibung]**: Verwenden Sie dieses Feld, um eine Beschreibung Ihres Workflows anzugeben.

## Segmentierungseinstellungen

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentierungseinstellungen"
>abstract="In diesem Bereich können Sie die Zielgruppendimension auswählen, um Profile im Workflow auszuwählen, und entscheiden, ob die Workflow-Ergebnisse zwischen zwei Ausführungen beibehalten werden sollen. Diese Option sollte nur zu Testzwecken verwendet werden und darf in einem Produktions-Workflow nie aktiviert werden."

* **[!UICONTROL Zielgruppendimension]**: Wählen Sie die Zielgruppendimension aus, die für die Zielgruppenbestimmung von Profilen verwendet werden soll: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw.
* **[!UICONTROL Zwischen zwei Ausführungen die ermittelte Population festhalten]**: Standardmäßig werden nur die Arbeitstabellen der letzten Ausführung des Workflows beibehalten. Arbeitstabellen früherer Ausführungen werden durch einen technischen Workflow bereinigt, der täglich ausgeführt wird.

  Wenn diese Option aktiviert ist, werden Arbeitstabellen auch nach Ausführung des Workflows beibehalten. Sie können sie zu Testzwecken verwenden, weswegen sie nur in Entwicklungs- oder Staging-Umgebungen verwendet werden darf. Sie darf niemals in einem Produktions-Workflow aktiviert sein.

## Ausführungsparameter

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Ausführungsparameter"
>abstract="In diesem Abschnitt können Sie Einstellungen für die Ausführung des Workflows konfigurieren, z. B. für wie viele Tage der Workflow-Verlauf gespeichert wird."

* **[!UICONTROL Verlauf in Tagen]**: Gibt die Anzahl der Tage an, nach denen der Verlauf bereinigt werden muss. Der Verlauf enthält Elemente im Zusammenhang mit dem Workflow: Protokolle, Aufgaben, Ereignisse (technische Objekte, die mit dem Workflow-Vorgang verknüpft sind). Der Standardwert bei vordefinierten Workflow-Vorlagen beträgt 30 Tage. Die Bereinigung des Verlaufs erfolgt durch den technischen Workflow für die Datenbankbereinigung, der standardmäßig täglich ausgeführt wird.

  >[!IMPORTANT]
  >
  >Wenn das Feld **[!UICONTROL Verlauf in Tagen]** leer gelassen wird, wird sein Wert als „1“ betrachtet; der Verlauf wird also nach einem Tag bereinigt.

* **[!UICONTROL Standardaffinität]**: Wenn Ihre Installation mehrere Workflow-Server umfasst, wählen Sie in diesem Feld den Computer aus, auf dem der Workflow ausgeführt werden soll. Wenn der in diesem Feld definierte Wert auf keinem Server vorhanden ist, bleibt der Workflow ausstehend.

* **[!UICONTROL SQL-Abfragen im Protokoll speichern]**: Hiermit können Sie die SQL-Abfragen aus dem Workflow in den Protokollen speichern. Diese Funktion ist erfahrenen Benutzerinnen und Benutzern vorbehalten. Sie gilt für Workflows, die Zielgruppenbestimmungsaktivitäten enthalten, wie **[!UICONTROL Zielgruppe aufbauen]**. Wenn diese Option aktiviert ist, werden die während der Workflow-Ausführung an die Datenbank gesendeten SQL-Abfragen in den Protokollen des Workflows angezeigt, sodass Sie sie analysieren können, um Abfragen zu optimieren oder Probleme zu diagnostizieren.

## Einstellungen für den Umgang mit Fehlern

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Einstellungen für den Umgang mit Fehlern"
>abstract="In diesem Abschnitt erfahren Sie, wie sich der Workflow verhalten soll, wenn während seiner Ausführung ein Fehler auftritt (Ausführung aussetzen/anhalten oder Fehler ignorieren)."

* **[!UICONTROL Umgang mit Fehlern]**: In diesem Feld können Sie festlegen, welche Aktionen ausgeführt werden sollen, wenn eine Workflow-Aufgabe Fehler aufweist. Es gibt zwei mögliche Optionen:

   * **[!UICONTROL Prozess aussetzen]**: Der Workflow wird automatisch ausgesetzt und der Status wechselt zu **[!UICONTROL Fehlgeschlagen]**. Sobald das Problem behoben ist, setzen Sie den Workflow mit der Schaltfläche **[!UICONTROL Fortsetzen]** fort.
   * **[!UICONTROL Ignorieren]**: Der Status der Aufgabe, die den Fehler ausgelöst hat, ändert sich in **[!UICONTROL Fehlgeschlagen]**, der Workflow behält jedoch den Status **[!UICONTROL Gestartet]**. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Vorgang abbrechen]**: Der Workflow wird automatisch angehalten und der Status ändert sich in **[!UICONTROL Fehlgeschlagen]**. Sobald das Problem behoben ist, starten Sie den Workflow mit der Schaltfläche **[!UICONTROL Starten]** erneut.

* **[!UICONTROL Aufeinanderfolgende Fehler]**: Dieses Feld wird verfügbar, wenn im Feld **[!UICONTROL Im Fehlerfall]** der Wert **[!UICONTROL Ignorieren]** ausgewählt wurde. Sie können die Anzahl der Fehler angeben, die ignoriert werden können, bevor der Prozess angehalten wird. Sobald diese Zahl erreicht ist, wechselt der Workflow-Status zu **[!UICONTROL Fehlgeschlagen]**. Wenn der Wert dieses Felds 0 beträgt, wird der Workflow unabhängig von der Fehleranzahl nie angehalten.
