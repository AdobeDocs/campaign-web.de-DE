---
audience: end-user
title: Workflow-Aktivität Inkrementelle Abfrage verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Inkrementelle Abfrage verwenden
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 31%

---

# Inkrementelle Abfrage {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Inkrementelle Abfrage"
>abstract="Verwenden Sie die neue Aktivität Inkrementelle Abfrage , um die Datenbank planmäßig abzufragen. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch lassen sich ausschließlich neue Elemente abrufen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Inkrementelle Abfrage"
>abstract="Die **Inkrementelle Abfrage** -Aktivität **Targeting** -Aktivität, die die Abfrage der Datenbank mithilfe des Abfragemodells ermöglicht. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch lassen sich ausschließlich neue Elemente abrufen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Inkrementeller Abfrageverlauf"
>abstract="Inkrementeller Abfrageverlauf"

Die **Inkrementelle Abfrage** -Aktivität **Targeting** -Aktivität, mit der Sie die Datenbank planmäßig abfragen können. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch lassen sich ausschließlich neue Elemente abrufen.

>[!NOTE]
>
>Während die Campaign-Client-Konsole die **[!UICONTROL Inkrementelle Abfrage]** -Aktivität mit einem integrierten Planer verwendet, behandelt die Campaign-Webbenutzeroberfläche diese Funktion getrennt. Um inkrementelle Abfrageausführungen zu planen, müssen Sie eine **[!UICONTROL Planung]** -Aktivität im Workflow vor der **[!UICONTROL Inkrementelle Abfrage]** -Aktivität. [Erfahren Sie, wie Sie eine Planung konfigurieren](scheduler.md)

**[!UICONTROL Inkrementelle Abfragen]** kommen in verschiedenen Kontexten zum Einsatz:

* Segmentierung von Populationen, um beispielsweise Zielgruppen und Audiences zu definieren
* Exportieren von Daten. Beispielsweise können Sie die Aktivität verwenden, um regelmäßig neue Protokolle in Dateien zu exportieren. Dies kann nützlich sein, wenn Sie Ihre Protokolldaten in externen Berichterstellungs- oder Business Intelligence Tools verwenden möchten.

Die bereits von früheren Ausführungen ausgewählte Population wird im Workflow gespeichert. Das bedeutet, dass zwei Workflows, die aus derselben Vorlage gestartet werden, nicht dasselbe Protokoll verwenden. Zwei Aufgaben, die auf derselben inkrementellen Abfrage im selben Workflow basieren, verwenden jedoch dasselbe Protokoll.

Wenn das Ergebnis einer inkrementellen Abfrage bei einer ihrer Ausführungen gleich 0 ist, wird der Workflow bis zur nächsten geplanten Ausführung der Abfrage ausgesetzt. Die auf die inkrementelle Abfrage folgenden Transitionen und Aktivitäten werden daher nicht vor der folgenden Ausführung verarbeitet.

## Konfigurieren der Aktivität Inkrementelle Abfrage {#incremental-query-configuration}

Führen Sie die folgenden Schritte aus, um die **Inkrementelle Abfrage** Aktivität:

![](../assets/incremental-query.png)

1. Hinzufügen einer **Inkrementelle Abfrage** in Ihren Workflow ein.

1. Im **[!UICONTROL Zielgruppe]** wählen Sie die **Zielgruppendimension** Klicken Sie dann auf **[!UICONTROL Weiter]**.

   Die Zielgruppendimension ermöglicht die Bestimmung der vom Vorgang betroffenen Population: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw. Standardmäßig wird die Zielgruppe aus den Empfängerinnen und Empfängern ausgewählt. [Erfahren Sie mehr über Zielgruppendimensionen](../../audience/about-recipients.md#targeting-dimensions)

1. Verwenden Sie den Abfrage-Modeler, um Ihre Abfrage zu definieren, genauso wie Sie eine Zielgruppe beim Entwerfen einer neuen E-Mail erstellen. [Erfahren sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md)

1. Im **[!UICONTROL Verarbeitete Daten]** wählen Sie den zu verwendenden inkrementellen Modus aus:

   * **[!UICONTROL Ergebnisse der vorherigen Ausführung ausschließen]**: Bei jeder Ausführung der Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen.

     Datensätze, die bereits in früheren Ausführungen enthalten waren, können ab dem Tag, an dem sie kontaktiert wurden, bis zu einer Höchstzahl von Tagen protokolliert werden. Verwenden Sie dazu die **[!UICONTROL Verlauf in Tagen]** -Feld. Wenn dieser Wert null ist, werden die Empfänger nie aus dem Protokoll gelöscht.

   * **[!UICONTROL Datumsfeld verwenden]**: Mit dieser Option können Sie Ergebnisse früherer Ausführungen basierend auf einem bestimmten Datumsfeld ausschließen. Wählen Sie dazu das gewünschte Datumsfeld aus der Liste der Attribute aus, die für die ausgewählte Zielgruppendimension verfügbar sind. Bei den nächsten Ausführungen des Workflows werden nur Daten abgerufen, die nach dem letzten Ausführungsdatum geändert oder erstellt wurden.

     Nach der ersten Ausführung des Workflows wird die **[!UICONTROL Letztes Ausführungsdatum]** -Feld verfügbar. Er gibt das Datum an, das für die nächste Ausführung verwendet wird, und wird bei jeder Ausführung des Workflows automatisch aktualisiert. Sie können diesen Wert auch überschreiben, indem Sie einen neuen eingeben.

   >[!NOTE]
   >
   >Der Modus **[!UICONTROL Datumsfeld verwenden]** ermöglicht je nach ausgewähltem Datumsfeld größere Flexibilität. Wenn das angegebene Feld beispielsweise einem Änderungsdatum entspricht, können Sie im Datumsfeldmodus Daten abrufen, die kürzlich aktualisiert wurden. Im anderen Modus werden jedoch Datensätze ausgeschlossen, die bereits in einer früheren Ausführung ausgewählt wurden, selbst wenn sie seit der letzten Ausführung des Workflows geändert wurden.

## Beispiel {#incremental-query-example}

Das folgende Beispiel zeigt die Konfiguration eines Workflows, der wöchentlich die Profile in der Adobe Campaign-Datenbank filtert, die Abonnenten des Yoga-Newsletter-Dienstes sind, um ihnen eine Willkommens-E-Mail zu senden.

![](../assets/incremental-query-example.png)

Der Workflow ist wie folgt gestaltet:

* Eine **[!UICONTROL Planung]**, damit der Workflow jeden Montag um 6 Uhr ausgeführt wird.
* Eine **[!UICONTROL Inkrementelle Abfrage]**, die bei der ersten Ausführung zunächst den Abruf aller aktuellen Abonnenten, dann bei den folgenden Ausführungen nur den Abruf der im Laufe der Woche dazugekommenen, neuen Abonnenten ermöglicht.
* Ein **[!UICONTROL Email delivery]** -Aktivität.
