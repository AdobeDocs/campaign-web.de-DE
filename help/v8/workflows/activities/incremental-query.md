---
audience: end-user
title: Verwenden der Workflow-Aktivität „Inkrementelle Abfrage“
description: Informationen dazu, wie Sie die Workflow-Aktivität „Inkrementelle Abfrage“ verwenden
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Inkrementelle Abfrage {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Inkrementelle Abfrage"
>abstract="Die Aktivität **Inkrementelle Abfrage** ist eine Aktivität zur **Zielgruppenbestimmung**, die die Abfrage der Datenbank mithilfe des Abfrage-Modelers ermöglicht. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch lassen sich ausschließlich neue Elemente abrufen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Inkrementeller Abfrageverlauf"
>abstract="Inkrementeller Abfrageverlauf"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Inkrementelle Abfrage – Verarbeitete Daten"
>abstract="Inkrementelle Abfrage – Verarbeitete Daten"

Die Aktivität **Inkrementelle Abfrage** ist eine Aktivität zur **Zielgruppenbestimmung**, mit der Sie die Datenbank nach einem Plan abfragen können. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch lassen sich ausschließlich neue Elemente abrufen.

>[!NOTE]
>
>Während die Client-Konsole von Campaign die Aktivität **[!UICONTROL Inkrementelle Abfrage]** mit einer integrierten Planung versieht, behandelt die Web-Benutzeroberfläche von Campaign diese Funktion getrennt. Um die Ausführungen inkrementeller Abfragen zu planen, fügen Sie vor der Aktivität **[!UICONTROL Inkrementelle Abfrage]** die Aktivität **[!UICONTROL Planung]** im Workflow hinzu. [Informationen dazu, wie Sie die Aktivität „Planung“ konfigurieren](scheduler.md)

Die Aktivität **[!UICONTROL Inkrementelle Abfrage]** kann zu verschiedenen Zwecken eingesetzt werden:

* Segmentierung von Populationen, um die Zielgruppe für eine Nachricht, Zielgruppe oder andere Vorgänge zu definieren.
* Export von Daten.  Verwenden Sie die Aktivität beispielsweise, um regelmäßig neue Protokolle in Dateien zu exportieren. Dies ist für externe Berichte oder Business Intelligence-Tools nützlich.

Die bereits bei früheren Ausführungen ausgewählte Population wird im Workflow gespeichert. Zwei Workflows, die aus derselben Vorlage gestartet werden, verwenden nicht dasselbe Protokoll. Zwei Aufgaben, die auf derselben inkrementellen Abfrage im selben Workflow basieren, verwenden jedoch dasselbe Protokoll.

Wenn das Ergebnis einer inkrementellen Abfrage bei einer ihrer Ausführungen gleich 0 ist, wird der Workflow bis zur nächsten geplanten Ausführung der Abfrage ausgesetzt. Die auf die inkrementelle Abfrage folgenden Transitionen und Aktivitäten werden nicht vor der folgenden Ausführung verarbeitet.

## Konfigurieren der Aktivität „Inkrementelle Abfrage“ {#incremental-query-configuration}

Führen Sie die folgenden Schritte aus, um die Aktivität **Inkrementelle Abfrage** zu konfigurieren:

[Beschreibung: Screenshot der Benutzeroberfläche zur Konfiguration für die Aktivität „Inkrementelle Abfrage“ in Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Fügen Sie die Aktivität **Inkrementelle Abfrage** in Ihren Workflow ein.

1. Wählen Sie im Abschnitt **[!UICONTROL Zielgruppe]** die **Zielgruppendimension** und klicken Sie dann auf **[!UICONTROL Fortsetzen]**.

   Die Zielgruppendimension bestimmt die vom Vorgang betroffene Population wie Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer oder Abonnierende. Standardmäßig wird die Zielgruppe aus den Empfängerinnen und Empfängern ausgewählt. [Erfahren Sie mehr über Zielgruppendimensionen](../../audience/about-recipients.md#targeting-dimensions)

1. Verwenden Sie den Abfrage-Modeler, um Ihre Abfrage zu definieren, ähnlich wie Sie eine Zielgruppe beim Entwerfen einer neuen E-Mail erstellen. [Erfahren Sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md)

1. Wählen Sie im Abschnitt **[!UICONTROL Verarbeitete Daten]** den zu verwendenden inkrementellen Modus aus:

   * **[!UICONTROL Ergebnisse der vorherigen Ausführung ausschließen]**: Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen.

     Die bereits in früheren Ausführungen ausgewählten Einträge können ab dem Tag, an dem sie ausgewählt wurden, bis zu einer Höchstzahl von Tagen protokolliert werden. Verwenden Sie zum Festlegen dieses Werts das Feld **[!UICONTROL Verlaufsumfang in Tagen]**. Wenn dieser Wert null ist, werden die Empfangenden nie aus dem Protokoll gelöscht.

   * **[!UICONTROL Datumsfeld verwenden]**: Diese Option schließt Ergebnisse früherer Ausführungen basierend auf einem bestimmten Datumsfeld aus. Wählen Sie das gewünschte Datumsfeld aus der Liste der Attribute aus, die für die ausgewählte Zielgruppendimension verfügbar sind. Bei den anschließenden Ausführungen des Workflows werden nur Daten abgerufen, die nach dem Datum der letzten Ausführung geändert oder erstellt wurden.

     Nach der ersten Ausführung des Workflows wird das Feld **[!UICONTROL Letztes Ausführungsdatum]** verfügbar. Es gibt das Datum an, das für die nächste Ausführung verwendet wird, und wird bei jeder Ausführung des Workflows automatisch aktualisiert. Sie können diesen Wert entsprechend Ihren Anforderungen manuell überschreiben.

   >[!NOTE]
   >
   >Der Modus **[!UICONTROL Datumsfeld verwenden]** ermöglicht je nach ausgewähltem Datumsfeld größere Flexibilität. Wenn das angegebene Feld beispielsweise einem Änderungsdatum entspricht, ruft der Datumsfeldmodus Daten ab, die kürzlich aktualisiert wurden. Im anderen Modus werden Einträge ausgeschlossen, die schon in einer früheren Ausführung abgerufen worden waren, selbst wenn diese Daten seit der letzten Ausführung des Workflows geändert wurden.

## Beispiel {#incremental-query-example}

Im folgenden Beispiel wird die Konfiguration eines Workflows illustriert, der die Profile in der Adobe Campaign-Datenbank wöchentlich filtert. Er wählt Personen aus, die für den Dienst „Yoga-Newsletter“ angemeldet sind, und sendet diesen eine Begrüßungs-E-Mail.

![Screenshot einer Workflow-Beispielkonfiguration zum Filtern von Profilen, die für den Dienst „Yoga-Newsletter“ angemeldet sind.](../assets/incremental-query-example.png)

Der Workflow umfasst die folgenden Elemente:

* Eine Aktivität vom Typ **[!UICONTROL Planung]**, damit der Workflow jeden Montag um 6 Uhr ausgeführt wird.
* Eine Aktivität vom Typ **[!UICONTROL Inkrementelle Abfrage]**, die bei der ersten Ausführung zunächst den Abruf aller aktuellen Abonnierenden und bei folgenden Ausführungen nur den Abruf der neuen Abonnierenden ermöglicht.
* Eine Aktivität **[!UICONTROL E-Mail-Versand]**.