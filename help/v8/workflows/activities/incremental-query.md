---
audience: end-user
title: Verwenden der Workflow-Aktivität „Inkrementelle Abfrage“
description: Informationen dazu, wie Sie die Workflow-Aktivität „Inkrementelle Abfrage“ verwenden
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 35%

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

Die Aktivität **Inkrementelle Abfrage** ist eine **Targeting**-Aktivität, mit der Sie Datenbankabfragen nach einem bestimmten Zeitplan durchführen können. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch können Sie nur neue Elemente als Ziel auswählen.

>[!NOTE]
>
>Während die Client-Konsole von Campaign die Aktivität **[!UICONTROL Inkrementelle Abfrage]** mit einer integrierten Planung versieht, behandelt die Web-Benutzeroberfläche von Campaign diese Funktion getrennt. Um inkrementelle Abfrageausführungen zu planen, fügen Sie eine Aktivität **[!UICONTROL Planung]** im Workflow vor der Aktivität **[!UICONTROL Inkrementelle Abfrage]** hinzu. [Informationen dazu, wie Sie die Aktivität „Planung“ konfigurieren](scheduler.md)

Die Aktivität **[!UICONTROL Inkrementelle Abfrage]** kann für verschiedene Zwecke verwendet werden:

* Segmentieren von Kontakten, um die Zielgruppe einer Nachricht oder eines anderen Vorgangs zu definieren.
* Export von Daten.  Verwenden Sie die Aktivität zum Beispiel, um regelmäßig neue Protokolle in Dateien zu exportieren. Dies ist für externe Reporting- oder Business Intelligence-Tools nützlich.

Die bereits bei früheren Ausführungen ausgewählte Population wird im Workflow gespeichert. Zwei Workflows, die aus derselben Vorlage gestartet wurden, verwenden nicht dasselbe Protokoll. Zwei Aufgaben, die auf derselben inkrementellen Abfrage im selben Workflow basieren, verwenden jedoch dasselbe Protokoll.

Wenn das Ergebnis einer inkrementellen Abfrage während einer ihrer Ausführungen gleich 0 ist, pausiert der Workflow bis zur nächsten programmierten Ausführung der Abfrage. Die Übergänge und Aktivitäten, die der inkrementellen Abfrage folgen, werden nicht vor der nächsten Ausführung verarbeitet.

## Konfigurieren der Aktivität „Inkrementelle Abfrage“ {#incremental-query-configuration}

Führen Sie die folgenden Schritte aus, um die Aktivität **Inkrementelle Abfrage** zu konfigurieren:

[Beschreibung: Screenshot der Konfigurationsoberfläche für die Aktivität Inkrementelle Abfrage in Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Fügen Sie die Aktivität **Inkrementelle Abfrage** in Ihren Workflow ein.

1. Wählen Sie im Abschnitt **[!UICONTROL Zielgruppe]** die Dimension **Zielgruppenbestimmung** und klicken Sie dann auf **[!UICONTROL Weiter]**.

   Die Zielgruppendimension definiert die Population, auf die sich der Vorgang bezieht, z. B. Empfänger, Vertragsbegünstigte, Benutzer oder Abonnenten. Standardmäßig wird die Zielgruppe aus den Empfängerinnen und Empfängern ausgewählt. [Erfahren Sie mehr über Zielgruppendimensionen](../../audience/about-recipients.md#targeting-dimensions)

1. Verwenden Sie den Abfrage-Modellierer, um Ihre Abfrage zu definieren, ähnlich wie Sie eine Zielgruppe beim Entwerfen einer neuen E-Mail erstellen. [Erfahren Sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md)

1. Wählen Sie im Abschnitt **[!UICONTROL Verarbeitete Daten]** den zu verwendenden inkrementellen Modus aus:

   * **[!UICONTROL Ergebnisse der vorherigen Ausführung ausschließen]**: Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen.

     Datensätze, die bereits in früheren Ausführungen als Ziel ausgewählt wurden, können für eine maximale Anzahl von Tagen ab dem Tag protokolliert werden, an dem sie als Ziel ausgewählt wurden. Verwenden Sie das Feld **[!UICONTROL Verlauf in Tagen]**, um diesen Wert festzulegen. Wenn dieser Wert null ist, werden die Empfangenden nie aus dem Protokoll gelöscht.

   * **[!UICONTROL Datumsfeld verwenden]**: Mit dieser Option werden Ergebnisse früherer Ausführungen auf der Grundlage eines bestimmten Datumsfelds ausgeschlossen. Wählen Sie das gewünschte Datumsfeld aus der Liste der für die ausgewählte Zielgruppendimension verfügbaren Attribute aus. Bei nachfolgenden Ausführungen des Workflows werden nur Daten abgerufen, die nach dem letzten Ausführungsdatum geändert oder erstellt wurden.

     Nach der ersten Ausführung des Workflows wird das Feld **[!UICONTROL Letztes Ausführungsdatum]** verfügbar. Er gibt das Datum für die nächste Ausführung an und wird bei jeder Ausführung des Workflows automatisch aktualisiert. Sie können diesen Wert entsprechend Ihren Anforderungen manuell überschreiben.

   >[!NOTE]
   >
   >Der **[!UICONTROL Datumsfeld verwenden]** bietet je nach ausgewähltem Datumsfeld mehr Flexibilität. Wenn das angegebene Feld beispielsweise einem Änderungsdatum entspricht, ruft der Datumsfeldmodus die zuletzt aktualisierten Daten ab. Der andere Modus schließt Aufzeichnungen aus, die bereits in einer vorherigen Ausführung angesprochen wurden, selbst wenn sie seit der letzten Ausführung des Workflows geändert wurden.

## Beispiel {#incremental-query-example}

Das folgende Beispiel zeigt die Konfiguration eines Workflows, der wöchentlich Profile in der Adobe Campaign-Datenbank filtert. Sie richtet sich an Personen, die sich für den Yoga-Newsletter angemeldet haben, und sendet ihnen eine Begrüßungs-E-Mail.

![Screenshot einer Beispiel-Workflow-Konfiguration zum Filtern von Profilen, die für den Yoga-Newsletter-Service abonniert wurden.](../assets/incremental-query-example.png)

Der Workflow umfasst die folgenden Elemente:

* Eine **[!UICONTROL Planung]**-Aktivität, die den Workflow jeden Montag um 6 Uhr morgens ausführt.
* Eine Aktivität **[!UICONTROL Inkrementelle Abfrage]** die während der ersten Ausführung alle aktuellen Abonnenten und bei nachfolgenden Ausführungen nur neue Abonnenten abfragt.
* Eine Aktivität **[!UICONTROL E-Mail-Versand]**.