---
audience: end-user
title: Verwenden der Workflow-Aktivität „Datei laden“
description: So verwenden Sie die Workflow-Aktivität „Datei laden“
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 4518f7a2f280eca70f799b941c5d28bdc39c1def
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 23%

---

# Datei laden  {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Aktivität „Datei laden“"
>abstract="Die Aktivität **Datei laden** ist eine **Daten-Management**-Aktivität. Verwenden Sie diese Aktivität, um mit Daten zu arbeiten, die in einer externen Datei gespeichert sind. Profile und Daten werden nicht zur Datenbank hinzugefügt, aber alle Felder in der Eingabedatei stehen zur Personalisierung, zur Aktualisierung von Profilen oder anderen Tabellen zur Verfügung. "

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Ausgehende Transition von der Zurückweisungsverwaltung"
>abstract="Ausgehende Transition von der Zurückweisungsverwaltung"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Ausgehende Transition für Zurückweisungen der Zurückweisungsverwaltung"
>abstract="Ausgehende Transition für Zurückweisungen der Zurückweisungsverwaltung"


Die Aktivität **Datei laden** ist eine **Daten-Management**-Aktivität. Mit dieser Aktivität können Sie mit Profilen und Daten arbeiten, die in einer externen Datei gespeichert sind. Profile und Daten werden nicht zur Datenbank hinzugefügt, aber alle Felder in der Eingabedatei sind verfügbar zur [Personalisierung](../../personalization/gs-personalization.md) oder um Profile oder andere Tabellen zu aktualisieren.

>[!NOTE]
>Unterstützte Dateiformate sind: Text (TXT) und kommagetrennte Werte (CSV). Sie können Dateien mit einer maximalen Größe von 50 MB laden.

Diese Aktivität kann mit einer [Abstimmungs](reconciliation.md)-Aktivität verwendet werden, um nicht identifizierte Daten mit vorhandenen Ressourcen zu verknüpfen. Zum Beispiel kann die Aktivität **Datei laden** vor dem Import nicht standardmäßiger Daten in die Datenbank vor einer **Abstimmungs**-Aktivität platziert werden.

## Konfigurieren der Aktivität „Datei laden“ {#load-configuration}

Die **Datei laden** Die Aktivitätskonfiguration umfasst zwei Schritte. Definieren Sie zunächst die Struktur, die die Importdatei aufweisen soll, indem Sie eine Beispieldatei hochladen. Danach können Sie den Ursprung der Datei angeben, deren Daten importiert werden sollen. Gehen Sie wie folgt vor, um die Aktivität zu konfigurieren.

![](../assets/workflow-load-file.png)

### Beispieldatei konfigurieren {#sample}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Beispieldatei"
>abstract="Wählen Sie die erwartete Dateistruktur aus, indem Sie eine Beispieldatei hochladen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formatierung der Aktivität „Datei laden“"
>abstract="Im **Formatierung** angeben, wie die Datei formatiert wird, um sicherzustellen, dass die Daten korrekt importiert werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Erneute Wertzuweisung für die Aktivität „Datei laden“"
>abstract="Verwenden Sie diese Option, um bestimmte Werte aus den geladenen Dateien neuen Werten zuzuordnen. Wenn die Spalte beispielsweise Werte vom Typ &quot;True&quot;/&quot;False&quot; enthält, können Sie eine Zuordnung hinzufügen, um diese Werte automatisch durch &quot;0&quot;/&quot;1&quot; zu ersetzen."

Führen Sie die folgenden Schritte aus, um die Beispieldatei zu konfigurieren, mit der die erwartete Dateistruktur definiert wird:

1. Hinzufügen einer **Datei laden** in Ihren Workflow ein.

1. Wählen Sie die zu verwendende Beispieldatei aus, um die erwartete Dateistruktur zu definieren. Klicken Sie dazu auf die Schaltfläche **Datei auswählen** im **[!UICONTROL Beispieldatei]** und wählen Sie die zu verwendende lokale Datei.

   >[!NOTE]
   >
   >Die Daten der Beispieldatei werden für die Konfiguration der Aktivität verwendet aber nicht importiert. Es wird empfohlen, eine Beispieldatei mit wenig Daten zu verwenden. Das Dateiformat muss mit diesem [Beispieldatei](../../audience/file-audience.md#sample-file).

1. Es wird eine Vorschau der Beispieldatei mit maximal 30 Zeilen angezeigt.

1. Im **[!UICONTROL Dateityp]** Dropdown-Liste angeben, ob die Datei getrennte Spalten oder Spalten mit fester Breite verwendet.

   ![](../assets/workflow-load-file-sample.png)

1. Für die Dateitypen mit getrennten Spalten verwenden Sie die **Spalten** um die Eigenschaften der einzelnen Spalten zu konfigurieren.

   +++Verfügbare Optionen für Dateispalten

   * **[!UICONTROL Titel]**: Beschriftung für die Spalte.
   * **[!UICONTROL Datentyp]**: Datentyp, der in der Spalte enthalten ist.
   * **[!UICONTROL Breite]** (Datentyp Zeichenfolge): Maximale Anzahl an Zeichen, die in der Spalte angezeigt werden sollen.
   * **[!UICONTROL Datenumwandlung]** (Datentyp Zeichenfolge): Wenden Sie die Umwandlung auf die in der Spalte enthaltenen Werte an.
   * **[!UICONTROL Verwaltung von Leerraum]** (Datentyp Zeichenfolge): Geben Sie an, wie die in der Spalte enthaltenen Leerzeichen verwaltet werden.
   * **[!UICONTROL Trennzeichen]** (Datentypen für Datum, Uhrzeit, Ganzzahl und Zahl)*: Geben Sie die als Trennzeichen zu verwendenden Zeichen an.
   * **[!UICONTROL NULL zulassen]**: Geben Sie an, wie leere Werte in der Spalte verwaltet werden. Bei der Option &quot;Adobe Campaign default&quot;wird ein Fehler ausgegeben, wenn ein leerer Wert vorhanden ist.
   * **[!UICONTROL Fehlerverarbeitung]** (Datentyp Zeichenfolge): Geben Sie das Verhalten bei Fehlern in einer der Zeilen an.
   * **[!UICONTROL Neukodifizierung von Werten]**: Mit dieser Option können Sie bestimmte Werte neuen zuordnen. Wenn die Spalte beispielsweise Werte vom Typ &quot;True&quot;/&quot;False&quot; enthält, können Sie eine Zuordnung hinzufügen, um diese Werte automatisch durch &quot;0&quot;/&quot;1&quot; zu ersetzen.

+++

1. Im **Formatierung** angeben, wie die Datei formatiert wird, um sicherzustellen, dass die Daten korrekt importiert werden.

### Definieren der hochzuladenden Zieldatei {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Zieldatei für die Aktivität „Datei laden“"
>abstract="Im **[!UICONTROL Zieldatei]** geben Sie an, wie die auf den Server hochzuladende Datei abgerufen werden soll."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Name der Datei"
>abstract="Geben Sie den Namen des Felds an, das auf den Server hochgeladen werden soll. Klicken Sie auf **[!UICONTROL Personalisierungsdialogfeld öffnen]** -Symbol, um den Ausdruckseditor, einschließlich Ereignisvariablen, zur Berechnung des Dateinamens zu nutzen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Zieldatenbank"
>abstract="Wenn Sie auf eine **[!UICONTROL Datei laden]** -Aktivität, die bereits in der Client-Konsole eingerichtet wurde, eine zusätzliche **[!UICONTROL Zieldatenbank]** verfügbar, wenn Sie die Aktivität zum Hochladen der Datei in eine externe Datenbank konfiguriert haben."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Befehl „Datei laden“"
>abstract="Das Zulassen beliebiger Befehle für die Vorverarbeitung ist ein Sicherheitsproblem. Deaktivieren Sie die Sicherheitsoption „XtkSecurity_Disable_Preproc“, um die Verwendung einer vordefinierten Liste von Befehlen zu erzwingen."

>[!CAUTION]
>
>Bevor Sie die Zieldatei laden, stellen Sie sicher, dass sie die Formatierung der Beispieldatei einhält. Abweichungen vom Dateiformat, der Spaltenstruktur oder der Spaltenanzahl können bei der Ausführung des Workflows zu Fehlern führen.

Gehen Sie wie folgt vor, um die hochzuladende Zieldatei zu definieren:

1. Im **[!UICONTROL Zieldatei]** angeben, welche Aktion beim Abrufen der auf den Server hochzuladenden Datei ausgeführt werden soll.

   * **[!UICONTROL Datei von einem lokalen Computer hochladen]**: Wählen Sie die von Ihrem Computer hochzuladende Datei aus.

   * **[!UICONTROL Wird durch die Transition angegeben]**: Laden Sie die in der eingehenden Transition angegebene Datei hoch, die von einer vorherigen Aktivität wie **[!UICONTROL Dateiübertragung]**.

   * **[!UICONTROL Vorab-Bearbeitung der Datei]**: Laden Sie die in der vorherigen Transition angegebene Datei hoch und wenden Sie einen Vorab-Bearbeitungsbefehl an, z. B. **[!UICONTROL Dekomprimierung]** oder **[!UICONTROL Entschlüsseln]**.

   * **[!UICONTROL Berechnet]**: Laden Sie die Datei hoch, deren Name im Feld **[!UICONTROL Dateiname]** -Feld. Klicken Sie auf **[!UICONTROL Personalisierungsdialogfeld öffnen]** -Symbol, um den Ausdruckseditor, einschließlich Ereignisvariablen, zur Berechnung des Dateinamens zu nutzen.

   ![](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >Wenn Sie auf eine **[!UICONTROL Datei laden]** -Aktivität, die bereits in der Client-Konsole eingerichtet wurde, eine zusätzliche **[!UICONTROL Zieldatenbank]** angezeigt, wenn Sie die Aktivität zum Hochladen der Datei in eine externe Datenbank konfiguriert haben. Sie können damit angeben, ob die Datei auf den Campaign-Server oder die externe Datenbank hochgeladen werden soll.

### Zusätzliche Optionen {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Zurückweisungsverwaltung für die Aktivität „Datei laden“"
>abstract="Im **Verwaltung von Ablehnungen** geben Sie an, wie sich die Aktivität im Falle von Fehlern verhalten soll. Sie können die maximal zulässige Anzahl von Fehlern festlegen und die **[!UICONTROL Zurückweisungen in einer Datei beibehalten]** -Option, um eine Datei mit den während des Imports aufgetretenen Fehlern auf den Server herunterzuladen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Löschen von Dateien nach dem Importieren"
>abstract="Schalten Sie die Option **Datei nach dem Import löschen** ein, um die Originaldatei nach dem Import vom Server zu löschen."


1. Im **Verwaltung von Ablehnungen** geben Sie an, wie sich die Aktivität im Falle von Fehlern verhalten soll:

   * Im **[!UICONTROL Löschen]** -Feld geben Sie die maximale Anzahl von Fehlern an, die bei der Verarbeitung der zu ladenden Datei zulässig sind. Wenn der Wert beispielsweise auf &quot;20&quot;gesetzt ist, schlägt die Ausführung des Workflows fehl, wenn beim Laden der Datei mehr als 20 Fehler auftreten.

   * Um die beim Laden der Datei aufgetretenen Fehler beizubehalten, können Sie die **[!UICONTROL Zurückweisungen in einer Datei beibehalten]** -Option ein und geben Sie den gewünschten Namen für die Datei im **[!UICONTROL Zurückweisungsdatei]** -Feld.

     Nach der Aktivierung dieser Option wird eine zusätzliche ausgehende Transition mit dem Namen &quot;Komplement&quot;nach der Aktivität hinzugefügt. Fehler, die während des Imports auftreten, werden in der angegebenen Datei auf dem Server gespeichert.

1. Um die hochgeladene Datei nach der Ausführung des Workflows vom Server zu löschen, müssen Sie die **[!UICONTROL Datei nach Import löschen]** -Option.

   ![](../assets/workflow-load-file-options.png)

1. Klicken Sie auf **Bestätigen**, wenn die Einstellungen korrekt sind.

## Beispiel {#load-example}

Ein Beispiel für das Laden einer externen Datei mithilfe der Aktivität **Abstimmung**, ist in [diesem Abschnitt](reconciliation.md#reconciliation-example) verfügbar.
