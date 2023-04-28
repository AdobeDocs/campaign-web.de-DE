---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
source-git-commit: 60cd0ed8dcbe3e6003c1cde674fe3441d6d88869
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 61%

---

# Workflow-Einstellungen konfigurieren {#workflow-settings}

Inhalt TBD

Definieren der über die Schaltfläche in der Workflow-Arbeitsfläche verfügbaren Einstellungen
<!--à reformuler-->

## Workflow-Eigenschaften  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workflow-Eigenschaften"
>abstract="Noch nicht definiert"

(= identisch mit der Erstellung des Workflows ? zu überprüfen)

* Titel
* Zusätzliche Optionen
* Interner Name
* Ordner
* Verknüpfte Kampagnen > kann sie ändern. Wenn ja, wird der Workflow aus der aktuellen Kampagne entfernt und in der neuen verknüpften Kampagne angezeigt
* Zeitzone: eine bestimmte Zeitzone definieren, die standardmäßig in allen Aktivitäten des Workflows verwendet werden soll. Standardmäßig ist die Zeitzone des Workflows die für den aktuellen Campaign-Benutzer definierte Zeitzone.
* Supervisor: Wenn ein Workflow fehlerhaft ist, werden die zur Workflow-Überwachungsgruppe gehörenden Benutzer per E-Mail benachrichtigt, sofern ihre E-Mail-Adresse in ihrem Profil angegeben ist. Diese Gruppe wird im **[!UICONTROL Supervisor(en)]** -Feld der Workflow-Eigenschaften.
* description

## Segmentierungseinstellungen

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmentierungseinstellungen"
>abstract="Noch nicht definiert"

* Zielgruppendimension:

   Bei Vorgängen zur Datensegmentierung wird einer Zielgruppendimension in der Regel eine Filterdimension zugeordnet. Die Zielgruppendimension definiert die Population, die von einer Kampagne angesprochen werden soll: Empfänger, Kunden, Abonnenten, Benutzer etc. Die Filterdimension ermöglicht die Einschränkung der gewählten Population nach bestimmten Kriterien: Kauf eines bestimmten Produkts, Abonnement eines bestimmten Newsletters etc.

* Ergebnisse beibehalten: Die **Zwischen zwei Ausführungen die ermittelte Population festhalten** speichert temporäre Tabellen zwischen zwei Ausführungen eines Workflows.  Diese Option ist auf der Registerkarte **[!UICONTROL Allgemein]** der Workflow-Eigenschaften verfügbar und kann für Entwicklungs- und Testzwecke verwendet werden, um Daten zu überwachen und Ergebnisse zu überprüfen. Sie können diese Option in Entwicklungsumgebungen verwenden, sollten sie aber nie in Produktionsumgebungen verwenden. Die Beibehaltung temporärer Tabellen könnte dazu führen, dass die Größe der Datenbank erheblich zunimmt und letztendlich die Größenbeschränkung erreicht wird. Außerdem wird dadurch das Backup verlangsamt.

   Nur die Arbeitstabellen der letzten Ausführung des Workflows werden aufbewahrt. Arbeitstabellen früherer Ausführungen werden durch den täglich durchgeführten **[!UICONTROL Bereinigungs]**-Workflow bereinigt.

   >[!CAUTION]
   >
   >Diese Option darf **nie** in einem **Produktions**-Workflow aktiviert werden. Diese Option wird zur Analyse der Ergebnisse verwendet und ist nur für Testzwecke konzipiert. Sie darf daher nur in Entwicklungs- oder Staging-Umgebungen verwendet werden.

## Workflow-Ausführungsparameter

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Ausführungseinstellungen"
>abstract="Noch nicht definiert"

* Verlauf in Tagen: Die Arbeitstabellen der Datenbank speichern den Verlauf der Ausführungen (Aufgaben, Ereignisse, Protokoll). Hier können Sie die Anzahl der Tage definieren, die für diesen Workflow archiviert werden sollen: Der Bereinigungsprozess löscht die ältesten Archive einmal täglich. Wenn der Wert in diesem Feld null ist, wird das Archiv nie gelöscht.

   gibt die Anzahl der Tage an, nach denen der Verlauf bereinigt werden muss. Der Verlauf enthält Elemente, die mit dem Workflow verbunden sind: Protokolle, Aufgaben, Ereignisse (technische Objekte, die mit dem Workflow-Ablauf verknüpft sind) sowie Dateien, die von der Aktivität **[!UICONTROL Dateiübertragung]** heruntergeladen wurden. Der Standardwert bei nativen Workflow-Vorlagen beträgt 30 Tage.

   Die Bereinigung des Verlaufs wird durch den technischen Workflow Datenbankbereinigung durchgeführt, der standardmäßig täglich ausgeführt wird.

   >[!IMPORTANT]
   >
   >Wenn das Feld **[!UICONTROL Verlauf in Tagen]** leer gelassen wird, wird sein Wert als „1“ betrachtet; der Verlauf wird also nach einem Tag bereinigt.

* Standardaffinität: In diesem Feld können Sie die Ausführung eines Workflows oder einer Workflow-Aktivität auf einem bestimmten Computer erzwingen.   Verwenden Sie dieses Feld, wenn Ihre Installation mehrere Workflow-Server aufweist, um festzulegen, auf welchem Server der Workflow laufen soll. Sollte der in diesem Feld angegebene Wert auf keinem Server existieren, bleibt der Workflow im Stand-by.

* sql queriesi in log speichern: dient der Speicherung der SQL-Abfragen aus dem Workflow in den Logs. (Wo kann ich auf SQL-Protokolle zugreifen?)

   Diese Funktion richtet sich an erfahrene Benutzer. Sie betrifft Workflows mit Zielgruppenbestimmungs-Aktivitäten (Abfrage, Vereinigung, Schnittmenge usw.). Wenn diese Option aktiviert wurde, werden die bei Ausführung des Workflows an die Datenbank gesendeten SQL-Abfragen in Adobe Campaign gespeichert. Auf diese Weise haben Sie die Möglichkeit, die Abfragen zu analysieren und eventuelle Probleme zu erkennen.

   Die Abfragen werden in diesem Fall im Tab **[!UICONTROL SQL-Logs]** angezeigt, der dem Workflow (außer bei Kampagnen-Workflows) und dem Fenster der Workflow-**[!UICONTROL Eigenschaften]** hinzugefügt wird. Die SQL-Abfragen werden darüber hinaus im **[!UICONTROL Verfolgung]**-Tab angezeigt.

## Einstellungen für den Umgang mit Fehlern

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Einstellungen für den Umgang mit Fehlern"
>abstract="Noch nicht definiert"

* In diesem Feld können Sie angeben, welche Aktion ausgeführt werden soll, wenn eine Workflow-Aufgabe einen Fehler ausgibt. Zwei Optionen stehen zur Verfügung:

   Prozess aussetzen - der Workflow wird automatisch ausgesetzt. Der Workflow-Status wechselt zu Fehlgeschlagen. Nach Behebung des Problems können Sie den Workflow Starten oder Neu starten.

   Ignorieren - die den Fehler verursachende Aufgabe wechselt in den Status Fehlgeschlagen, der Workflow behält jedoch den Status Gestartet. Diese Konfiguration empfiehlt sich bei wiederkehrenden Aufgaben. Wenn der Workflow-Zweig eine Planungsaktivität enthält, löst diese automatisch zum nächsten geplanten Zeitpunkt die nächste Ausführung aus.

* Folgefehler: Dieses Feld wird verfügbar, wenn im Feld Bei Fehler die Option Ignorieren ausgewählt ist. Sie können die Anzahl der Fehler angeben, die ignoriert werden können, bevor der Prozess angehalten wird. Sobald diese Zahl erreicht ist, wechselt der Workflow-Status zu Fehlgeschlagen. Wenn der Wert dieses Felds 0 beträgt, wird der Workflow unabhängig von der Fehleranzahl nie angehalten.
