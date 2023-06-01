---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 806e465b7c1df6cd26d68103c45b175371d73485
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 63%

---

# Erweiterte Workflow-Einstellungen konfigurieren {#workflow-settings}

Bei der Orchestrierung von Workflow-Aktivitäten auf der Arbeitsfläche können Sie auf erweiterte Einstellungen im Zusammenhang mit dem Workflow zugreifen. Sie können beispielsweise eine bestimmte Zeitzone für den Workflow festlegen, verwalten, wie sich der Workflow im Fehlerfall verhält, oder die Verzögerung verwalten, nach der der Workflow-Verlauf bereinigt werden soll.

Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Workflow-Einstellungen]** in der linken oberen Ecke der Arbeitsfläche neben der Workflow-Beschriftung.

![](assets/workflow-settings.png)

## Workflow-Eigenschaften  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow-Eigenschaften"
>abstract="Noch nicht definiert"

Der Abschnitt mit den Workflow-Eigenschaften enthält allgemeine Eigenschaften, auf die auch beim Erstellen des Workflows zugegriffen werden kann.

* **[!UICONTROL Titel]**: Der Titel des Workflows, der in der Liste angezeigt wird.
* **[!UICONTROL Interner Name]**: Interner Name des Workflows.
* **[!UICONTROL Ordner]**: Der Ordner, in dem der Workflow gespeichert werden soll.
* **[!UICONTROL Verknüpfte Kampagne]**: Dieses Feld wird angezeigt, wenn der Workflow innerhalb einer Kampagne erstellt wurde. Damit können Sie die zugehörige Kampagne öffnen.
* **[!UICONTROL Zeitzone]**: Definieren Sie eine bestimmte Zeitzone, die standardmäßig in allen Workflow-Aktivitäten verwendet werden soll. Standardmäßig ist die Zeitzone des Workflows die für den aktuellen Campaign-Benutzer bzw. die aktuelle Campaign-Benutzerin definierte Zeitzone.
* **[!UICONTROL Supervisor]**: Wenn ein Workflow fehlerhaft ist, werden die zur Workflow-Überwachungsgruppe gehörenden Benutzer per E-Mail benachrichtigt, sofern ihre E-Mail-Adresse in ihrem Profil angegeben ist.
* **[!UICONTROL Beschreibung]**: Verwenden Sie dieses Feld, um eine Beschreibung Ihres Workflows anzugeben.

## Segmentierungseinstellungen

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentierungseinstellungen"
>abstract="Noch nicht definiert"

* **[!UICONTROL Zielgruppendimension]**: Wählen Sie die Zielgruppendimension aus, die für die Zielgruppenbestimmung von Profilen verwendet werden soll: Empfänger, Empfänger, Betreiber, Abonnenten usw.
* **[!UICONTROL Zwischen zwei Ausführungen die ermittelte Population festhalten]**: Standardmäßig werden nur die Arbeitstabellen der letzten Ausführung des Workflows beibehalten. Arbeitstabellen früherer Ausführungen werden durch einen technischen Workflow bereinigt, der täglich ausgeführt wird.

   Wenn diese Option aktiviert ist, werden Arbeitstabellen auch nach Ausführung des Workflows beibehalten. Sie können sie zu Testzwecken verwenden und dürfen daher nur in Entwicklungs- oder Staging-Umgebungen verwendet werden. Sie darf nie in einem Produktions-Workflow überprüft werden.

## Workflow-Ausführungsparameter

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Ausführungseinstellungen"
>abstract="Noch nicht definiert"

* Verlauf in Tagen: Die Arbeitstabellen der Datenbank speichern den Verlauf der Ausführungen (Aufgaben, Ereignisse, Protokoll). Hier können Sie die Anzahl der Tage definieren, die für diesen Workflow archiviert werden sollen: Der Bereinigungsprozess löscht die ältesten Archive einmal täglich. Wenn der Wert in diesem Feld null ist, wird das Archiv nie gelöscht.

   Gibt die Anzahl der Tage an, nach denen der Verlauf bereinigt werden muss. Der Verlauf enthält Elemente, die mit dem Workflow verbunden sind: Protokolle, Aufgaben, Ereignisse (technische Objekte, die mit dem Workflow-Ablauf verknüpft sind) sowie Dateien, die von der Aktivität **[!UICONTROL Dateiübertragung]** heruntergeladen wurden. Der Standardwert bei nativen Workflow-Vorlagen beträgt 30 Tage.

   Die Bereinigung des Verlaufs erfolgt durch den technischen Workflow für die Datenbankbereinigung, der standardmäßig täglich ausgeführt wird.

   >[!IMPORTANT]
   >
   >Wenn das Feld **[!UICONTROL Verlauf in Tagen]** leer gelassen wird, wird sein Wert als „1“ betrachtet; der Verlauf wird also nach einem Tag bereinigt.

* Standard-Affinität: Hier können Sie für die Ausführung eines Workflows oder einer Workflow-Aktivität die Verwendung eines bestimmten Rechners vorschreiben.   Verwenden Sie dieses Feld, wenn Ihre Installation mehrere Workflow-Server aufweist, um festzulegen, auf welchem Server der Workflow laufen soll. Sollte der in diesem Feld angegebene Wert auf keinem Server existieren, bleibt der Workflow ausstehend.

* SQL-Abfragen im Protokoll speichern: Hier können Sie die SQL-Abfragen aus dem Workflow in den Protokollen speichern. (Wo kann ich auf SQL-Protokolle zugreifen?)

   Diese Funktion richtet sich an erfahrene Benutzer. Sie betrifft Workflows mit Zielgruppenbestimmungs-Aktivitäten (Abfrage, Vereinigung, Schnittmenge usw.). Wenn diese Option aktiviert wurde, werden die bei Ausführung des Workflows an die Datenbank gesendeten SQL-Abfragen in Adobe Campaign gespeichert. Auf diese Weise haben Sie die Möglichkeit, die Abfragen zu analysieren und eventuelle Probleme zu erkennen.

   Die Abfragen werden in diesem Fall im Tab **[!UICONTROL SQL-Logs]** angezeigt, der dem Workflow (außer bei Kampagnen-Workflows) und dem Fenster der Workflow-**[!UICONTROL Eigenschaften]** hinzugefügt wird. Die SQL-Abfragen werden darüber hinaus im **[!UICONTROL Verfolgung]**-Tab angezeigt.

## Einstellungen für den Umgang mit Fehlern

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Einstellungen für den Umgang mit Fehlern"
>abstract="Noch nicht definiert"

* In diesem Feld können Sie angeben, welche Aktion ausgeführt werden soll, wenn eine Workflow-Aufgabe einen Fehler ausgibt. Zwei Optionen stehen zur Verfügung:

   Prozess anhalten: der Workflow wird automatisch ausgesetzt. Der Workflow-Status wechselt zu „Fehlgeschlagen“. Nach Behebung des Problems können Sie den Workflow mithilfe der entsprechenden Schaltflächen starten oder neu starten.

   Ignorieren: die den Fehler verursachende Aufgabe wechselt in den Status „Fehlgeschlagen“, der Workflow behält jedoch den Status „Gestartet“. Diese Konfiguration empfiehlt sich bei wiederkehrenden Aufgaben: Wenn der Workflow-Zweig eine Planungsaktivität enthält, wird diese bei der nächsten Ausführung des Workflows normal gestartet.

* Aufeinanderfolgende Fehler: Dieses Feld wird verfügbar, wenn im Feld „Bei Fehler“ der Wert „Ignorieren“ ausgewählt ist. Sie können die Anzahl der Fehler angeben, die ignoriert werden können, bevor der Prozess angehalten wird. Sobald diese Zahl erreicht ist, wechselt der Workflow-Status zu „Fehlgeschlagen“. Wenn der Wert dieses Felds 0 beträgt, wird der Workflow unabhängig von der Fehleranzahl nie angehalten.
