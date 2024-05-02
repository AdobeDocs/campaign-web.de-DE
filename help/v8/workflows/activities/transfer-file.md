---
audience: end-user
title: Verwenden der Aktivität Dateiübertragung
description: Erfahren Sie, wie Sie die Workflow-Aktivität Dateiübertragung verwenden
source-git-commit: 6fe8be5510e13cdb9e9e1bce44aadb80619275e4
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 13%

---

# Dateiübertragung {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="Dateiübertragung"
>abstract="Die **Dateiübertragung** -Aktivität können Sie Dateien empfangen oder senden, auf Existenz von Dateien testen oder Dateien auf einem Server auflisten. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Dateiübertragungsoptionen"
>abstract="Dateiübertragungsoptionen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Dateiübertragungsaktivität"
>abstract="Dateiübertragungsaktivität"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Remote-Server für die Dateiübertragung"
>abstract="Remote-Server für die Dateiübertragung"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Dateiübertragungsquelle"
>abstract="Dateiübertragungsquelle"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Quelldateien nach der Übertragung löschen"
>abstract="Quelldateien nach der Übertragung löschen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Sitzungsprotokolle anzeigen"
>abstract="Sitzungsprotokolle anzeigen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Alle Dateien auflisten"
>abstract="Alle Dateien auflisten"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Dateiverlaufserstellung"
>abstract="Dateiverlaufserstellung"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Fehlen von Dateien verarbeiten"
>abstract="Fehlen von Dateien verarbeiten"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Fehler verarbeiten"
>abstract="Fehler verarbeiten"

Die **Dateiübertragung** -Aktivität **Data Management** -Aktivität. Damit können Sie Dateien empfangen oder senden, auf Existenz von Dateien testen oder Dateien auf einem Server auflisten. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein.

>[!NOTE]
>
>Mit der Campaign-Webbenutzeroberfläche haben wir zwei Aktivitäten zu einer zusammengefasst, indem wir beide zusammenführen **Dateiversand** und **HTTP-Übertragung** Funktionen. Diese Konsolidierung wirkt sich in keiner Weise auf die Funktionalität der Aktivität aus.

Gehen Sie wie folgt vor, um die **Dateiübertragung** -Aktivität.

## Übertragungsprotokoll und Vorgang auswählen {#protocol}

1. Hinzufügen einer **Dateiübertragung** -Aktivität in Ihren Workflow ein und geben Sie dann den Typ der Übertragung an, die je nach dem zu verwendenden Protokoll durchgeführt werden soll:

   * Wählen Sie für das HTTP-Protokoll **[!UICONTROL Web-Download]**. Auf diese Weise können Sie eine GET oder POST ausführen, die eine Datei auf eine explizite URL, ein externes Konto oder eine Adobe Campaign-Instanz herunterlädt.
   * Für andere Server-zu-Server-Protokolle und zugehörige Aktionen wählen Sie **[!UICONTROL Dateiversand]**.

1. Wählen Sie die mit der Aktivität auszuführende Aktion aus. Die verfügbaren Aktionen hängen vom gewählten Transfertyp ab. Erweitern Sie die folgenden Abschnitte, um weitere Informationen zu erhalten.

   +++ Aktionen verfügbar mit **Dateiversand** Typaktivitäten

   * **[!UICONTROL Dateidownload]**: Laden Sie eine Datei vom Server herunter.
   * **[!UICONTROL Datei-Upload]**: Laden Sie eine Datei auf den Server hoch.
   * **[!UICONTROL Existenztest einer Datei]**: Überprüfen Sie, ob eine bestimmte Datei auf dem Server vorhanden ist. Erzeugt im Anschluss an die Aktivität zwei ausgehende Transitionen: &quot;Datei vorhanden&quot;und &quot;Datei nicht vorhanden&quot;.
   * **[!UICONTROL Dateiauflistung]**: Liste aller auf dem Server verfügbaren Dateien.

+++

   +++ Aktionen verfügbar mit **HTTP-Übertragung** Typaktivitäten

   * **[!UICONTROL Einfache Übertragung (GET)]**: Rufen Sie eine Datei ab.
   * **[!UICONTROL Übertragen mithilfe eines Formulars (POST)]**: Laden Sie eine Datei und zusätzliche Parameter hoch.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. Standardmäßig verwendet die Aktivität bei Aktionen zum Hochladen von Dateien die in der vorherigen Aktivität angegebene Datei. Um eine andere Datei zu verwenden, können Sie die **[!UICONTROL Datei aus vorheriger Aktivität verwenden]** und klicken Sie auf **[!UICONTROL Datei hinzufügen]** Schaltfläche.

   Im **[!UICONTROL Quelle]** Geben Sie den gewünschten Dateinamen ein oder verwenden Sie den Ausdruckseditor, um den Dateinamen mithilfe von Ereignisvariablen zu berechnen. [Erfahren Sie, wie Sie mit Ereignisvariablen und dem Ausdruckseditor arbeiten.](../event-variables.md). Wiederholen Sie den Vorgang, um beliebig viele Dateien hinzuzufügen.

## Übertragungsziel definieren {#destination}

1. Im **[!UICONTROL Remote-Server]** Geben Sie mithilfe einer der folgenden Methoden den Server an, mit dem eine Verbindung hergestellt werden soll:

   * **[!UICONTROL In einem externen Konto definierte Verbindungsparameter verwenden]**: Stellen Sie mithilfe der Verbindungsparameter eines externen Kontos eine Verbindung zu einem Server her. Im **[!UICONTROL Server-Ordner]** Geben Sie den Pfad zur Datei (oder zum Ordner für die Dateiauflistungsaktionen) an.
   * **[!UICONTROL Schnellkonfiguration]**: Geben Sie die URL der Datei (oder des Ordners für die Dateiauflistungsaktionen) ein.
   * **[!UICONTROL Adobe Campaign-Instanz]** (HTTP-Übertragung): Laden Sie eine Datei von einem Adobe Campaign-Instanzserver herunter.

   ![](../assets/workflow-transfer-file-server.png)

1. Bei Aktionen zur POST von Webdownloads können Sie zusätzliche Parameter mit dem Vorgang übergeben. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Parameter hinzufügen]** und geben Sie dann den Namen und den Wert der Parameter an. Sie können beliebig viele Parameter hinzufügen.

1. Standardmäßig werden die auf einen Server hochgeladenen Dateien beim Datei-Upload automatisch gespeichert. Wenn Sie diesen Verlauf nicht beibehalten möchten, können Sie die **[!UICONTROL Verlauf der gesendeten Dateien speichern]** deaktiviert.

## Verlaufsparameter           {#historization}

Jedes Mal, wenn die Aktivität **[!UICONTROL Dateiübertragung]** ausgeführt wird, werden die hoch- oder heruntergeladenen Dateien in einem bestimmten Ordner gespeichert. Für jede Aktivität Dateiübertragung eines Workflows wird ein Ordner erstellt. Standardmäßig werden die Dateien im Standardspeicherverzeichnis des Adobe Campaign-Installationsordners gespeichert (`/vars`), bevor sie verarbeitet werden. Um einen bestimmten Ordner zu verwenden, können Sie die **[!UICONTROL Standardspeicherverzeichnis verwenden]** und geben Sie den Pfad des Ordners ein.

![](../assets/workflow-transfer-file-historization.png)

Es ist wichtig, die Größe dieses Ordners zu begrenzen, um physischen Speicherplatz auf dem Server zu erhalten. Dazu können Sie eine maximale Anzahl von Dateien oder die Gesamtgröße für den Ordner der Aktivität definieren. Standardmäßig sind 100 Dateien und 50 MB zugelassen.

Jedes Mal, wenn die Aktivität ausgeführt wird, wird der Ordner folgendermaßen überprüft:

* Nur Dateien, die mehr als 24 Stunden vor der Durchführung der Aktivität erstellt wurden, werden berücksichtigt.
* Wenn die Anzahl der berücksichtigten Dateien größer ist als der Wert der **[!UICONTROL Anzahl Dateien]** -Feld, werden die ältesten Dateien gelöscht, bis die maximal zulässige Anzahl von Dateien erreicht ist.
* Wenn die Gesamtgröße der berücksichtigten Dateien größer ist als der Wert der **[!UICONTROL Maximale Größe (in MB)]** werden die ältesten Dateien gelöscht, bis die zulässige Maximale Größe (in MB) erreicht ist.

>[!CAUTION]
>
>Wenn die Aktivität nicht ausgeführt wird, wird der Ordner weder überprüft noch geleert. Seien Sie deshalb achtsam beim Transfer großer Dateien.

## Erweiterte Optionen zur Fehlerverwaltung {#advanced}

1. Im **[!UICONTROL Erweiterte Optionen]**, stehen je nach Typ der Aktivität, die Sie konfigurieren, zusätzliche Optionen zur Verfügung. Erweitern Sie die folgenden Abschnitte, um weitere Informationen zu erhalten.

   ++ + Zusätzliche Optionen für **[!UICONTROL Dateiversand]** Typaktivitäten

   * **[!UICONTROL Quelldateien nach der Übertragung löschen]**: Löschen Sie die Quelldateien nach einer erfolgreichen Übertragung.
   * **[!UICONTROL Sitzungsprotokolle anzeigen]**: Wenn diese Option aktiviert ist, werden Informationen zum Übertragungsvorgang in den Workflow-Logs angezeigt, nachdem der Workflow ausgeführt wurde.
   * **[!UICONTROL Alle Dateien auflisten]** (Dateilistungsaktionen): Diese Option indiziert alle Dateien, die auf dem Server im `vars.filenames` Ereignisvariable, in der die Dateinamen durch die `n` Zeichen. [Erfahren Sie, wie Sie mit Ereignisvariablen arbeiten](../event-variables.md)

+++

   ++ + Zusätzliche Optionen für **[!UICONTROL HTTP-Übertragung]** Typaktivitäten

   * **[!UICONTROL Folgen Sie den Anweisungen]**: Mithilfe der Dateiumleitung können Sie Überschreibungen verwenden, um die Dateneingabe oder -ausgabe an ein Gerät eines anderen Typs zu leiten.
   * **[!UICONTROL Hinzufügen der HTTP-Header zur Datei]**: In einigen Fällen können Sie einer Datei zusätzliche HTTP-Header hinzufügen. In den meisten Fällen werden diese Header verwendet, um zusätzliche Informationen zur Fehlerbehebung bereitzustellen, um [Cross-Origin Resource Sharing (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS), oder um bestimmte Caching-Anweisungen festzulegen.
   * **[!UICONTROL Den HTTP-Rückgabecode ignorieren]**: HTTP-Rückgabe-Codes, auch HTTP-Status-Codes genannt, geben das Ergebnis einer HTTP-Anfrage an.

1. Die **[!UICONTROL Fehler verarbeiten]** ermöglicht die Aktivierung einer ausgehenden Transition vom Typ &quot;Fehler&quot; nach der Aktivität, falls bei der Übertragung ein Fehler auftritt.

   Zusätzlich gilt für **Dateiversand** Typaktivitäten, die **[!UICONTROL Fehlende Datei verarbeiten]** ermöglicht die Aktivierung einer ausgehenden Transition vom Typ &quot;Keine Datei&quot; im Anschluss an die Aktivität, wenn die Datei nicht im angegebenen Pfad verfügbar ist.
