---
audience: end-user
title: E-Mail-Versandberichte
description: Erfahren Sie, wie Sie auf E-Mail-Versandberichte zugreifen und diese verwenden können
badge: label="Beta"
source-git-commit: 3c679ad284f15a46885829b68c8ebea1e99e2b98
workflow-type: tm+mt
source-wordcount: '2254'
ht-degree: 68%

---

# E-Mail-Versandbericht {#email-report}

Der **E-Mail-Versandbericht** bietet umfassende Einblicke und Daten, die speziell für den E-Mail-Kanal gelten. Er bietet detaillierte Informationen über Leistung, Effektivität und Ergebnisse Ihrer einzelnen Sendungen und verschafft Ihnen einen umfassenden Überblick.

## Versandzusammenfassung {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Versandberichte"
>abstract="Auf der Registerkarte **Senden** Ihres Berichts erhalten Sie einen umfassenden Einblick in die Interaktionen Ihrer Besucherinnen und Besucher mit Ihren Sendungen und in etwaige Fehler, die bei ihnen aufgetreten sind."

### Anfängliche Zielpopulation {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Anfängliche Zielpopulation"
>abstract="Die **Ursprungspopulation** -Diagramm zeigt Daten zu Ihren Empfängern und Nachrichten basierend auf den Ergebnissen der Versandvorbereitung an."

Die **[!UICONTROL Ursprungspopulation]** -Diagramm zeigt Daten zu Ihren Empfängern an. Die Metriken werden bei der Versandvorbereitung berechnet und zeigen: die Anfangs-Audience, die Anzahl der zu sendenden Nachrichten und die Anzahl der ausgeschlossenen Empfänger.

![](assets/reporting_email_1.png){width="50%" align="left" zoomable="yes"}

Bewegen Sie den Mauszeiger über einen Abschnitt des Diagramms, um die genaue Zahl anzuzeigen.

![](assets/reporting_email_1.1.png){width="50%" align="left" zoomable="yes"}


+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger.

* **[!UICONTROL Zu versenden]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

* **[!UICONTROL Ausschluss]**: Gesamtzahl der von der Zielpopulation ausgeschlossen Empfänger.
+++

### Versandstatistiken {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Versandstatistiken"
>abstract="Die **Versandstatistiken** -Diagramm zeigt den Erfolg Ihres Versands und die aufgetretenen Fehler."


Die **[!UICONTROL Versandstatistiken]** -Diagramm zeigt den Erfolg Ihres Versands an. Die Metriken werden nachfolgend beschrieben.

![](assets/reporting_email_2.png){width="50%" align="left" zoomable="yes"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Kampagnen-Berichts.

* **[!UICONTROL Gesendete Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitungen im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

+++

### Ausschlussgründe  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Versandstatistiken"
>abstract="Die **Ausschlussgründe** Diagramm und Tabelle zeigen die Verteilung der bei der Versandvorbereitung zurückgewiesenen Nachrichten nach Regeln."


Die **[!UICONTROL Ausschlussgründe]** Diagramm und Tabelle zeigen die Verteilung der bei der Versandvorbereitung zurückgewiesenen Nachrichten nach Regeln. Ausschlussregeln werden im Abschnitt [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Unbekannter Nutzer]**: Fehlertyp, der während des Versands erzeugt wird, um anzuzeigen, dass die E-Mail-Adresse ungültig ist.

* **[!UICONTROL Ungültige Domain]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Domain der E-Mail-Adresse falsch ist oder nicht existiert.

* **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Versandversuchen erzeugt wird, wenn das Empfängerpostfach zu viele Nachrichten enthält.

* **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

* **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

* **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

* **[!UICONTROL Nicht angemeldet]**: Fehlertyp, wenn das Mobiltelefon der Empfängerin bzw. des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder über keinen Netzempfang verfügte.

+++

## Versanddurchsatz {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Versanddurchsatz"
>abstract="Der Bericht **Versanddurchsatz** enthält detaillierte Informationen zum Versanddurchsatz der gesamten Plattform innerhalb eines bestimmten Zeitraums."

Dieser Bericht enthält detaillierte Informationen zum Versanddurchsatz der gesamten Plattform innerhalb eines bestimmten Zeitraums. Die wichtigste Kennzahl, mit der die Geschwindigkeit des Nachrichtenversands gemessen wird, ist die Anzahl der pro Stunde gesendeten Nachrichten.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## Versandstatistiken {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Versandstatistiken"
>abstract="Die **Versandstatistiken** enthält die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind."

Die Tabelle **[!UICONTROL Broadcast-Statistiken]** enthält die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind. Die Metriken werden nachfolgend beschrieben.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Verarbeitete E-Mails]**: Gesamtzahl der Nachrichten, die vom Versand-Server verarbeitet wurden.

* **[!UICONTROL Zugestellt]**: Prozentualer Anteil der erfolgreich verarbeiteten Nachrichten im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten.

* **[!UICONTROL Hardbounces]**: Prozentualer Anteil der „Hardbounces“, d. h. permanente Fehler wie etwa eine falsche E-Mail-Adresse, im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten.

* **[!UICONTROL Softbounces]**: Prozentualer Anteil der „Softbounces“, d. h. temporäre Fehler wie etwa ein voller Posteingang, im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten

* **[!UICONTROL Öffnungen]**: Prozentualer Anteil der Zielgruppenempfängerinnen und -empfänger, die mindestens einmal eine Nachricht geöffnet haben, im Vergleich zur Gesamtzahl der erfolgreich verarbeiteten Nachrichten.

* **[!UICONTROL Klicks]**: Prozentsatz der Anzahl der Personen, die mindestens einmal auf einen Versand geklickt haben, im Vergleich zur Anzahl der erfolgreich verarbeiteten Nachrichten.

* **[!UICONTROL Abmeldungen]**: Prozentualer Anteil der Klicks auf einen Abmelde-Link in Bezug auf die Gesamtzahl der verarbeiteten Nachrichten.
+++

## Unzustellbare Nachrichten {#non-deliverables-email}

###  zur Aufschlüsselung der Fehler nach Typ {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title=" zur Aufschlüsselung der Fehler nach Typ"
>abstract="Die **Verteilung der Fehler nach Typ** -Tabelle und -Diagramm enthalten die verfügbaren Daten für jeden aufgetretenen Fehlertyp: unbekannter Nutzer, Postfach voll, ungültige Domäne und mehr."

Die **[!UICONTROL Verteilung der Fehler nach Typ]** Tabelle und Diagramm enthalten die verfügbaren Daten für den Fehlertyp. Die Metriken werden nachfolgend beschrieben.

Die in diesem Bericht angezeigten Fehler lösen einen Quarantäneprozess aus. Weitere Informationen zur Quarantäneverwaltung finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=de){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Unbekannter Nutzer]**: Fehlertyp, der während des Versands erzeugt wird, um anzuzeigen, dass die E-Mail-Adresse ungültig ist.

* **[!UICONTROL Ungültige Domain]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Domain der E-Mail-Adresse falsch ist oder nicht existiert.

* **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Versandversuchen erzeugt wird, wenn das Empfängerpostfach zu viele Nachrichten enthält.

* **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

* **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

* **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

* **[!UICONTROL Nicht angemeldet]**: Fehlertyp, wenn das Mobiltelefon der Empfängerin bzw. des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder über keinen Netzempfang verfügte.

+++


### Verteilung der Fehler nach Domain {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Verteilung der Fehler nach Domain"
>abstract="Die **Verteilung der Fehler nach Domain** -Tabelle und -diagramm zeigen die verfügbaren Daten für jeden aufgetretenen Fehlertyp in Abhängigkeit von der jeweiligen Domäne an."


Die **[!UICONTROL Verteilung der Fehler nach Domain]** -Tabelle und -Diagramm zeigen die verfügbaren Daten zu Fehlern an, die bei jeder Domäne aufgetreten sind.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Klicken Sie auf das Symbol neben dem Namen der einzelnen Domänen, um Details anzuzeigen.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Die verfügbaren Metriken sind mit denen der Variablen [Verteilung der Fehler nach Typ](#email-delivery-breakdown-type) weiter oben beschrieben.

## Tracking-Indikatoren {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Tracking-Berichte"
>abstract="Die Registerkarte **Tracking** Ihres Berichts enthält wertvolle Daten, darunter das Empfängerverhalten pro Link, die Aufschlüsselung von Öffnungen und Klicks sowie detaillierte Informationen zu den am häufigsten angeklickten URLs während eines Versands."


### Versandstatistiken  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Versandstatistiken"
>abstract="Die **Versandstatistiken** bietet wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den für gesendete E-Mails verfügbaren Daten liefern: Erfolg, Öffnungen, Klicks und mehr."


Die **[!UICONTROL Versandstatistiken]** bietet wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den für gesendete E-Mails verfügbaren Daten enthalten. Die Metriken werden nachfolgend beschrieben.

![](assets/reporting_email_5.png){align="center"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Unterschiedliche Öffnungen (Unique Opens)]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger, die mindestens einmal eine Nachricht geöffnet haben.

* **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

* **[!UICONTROL Klicks auf den Abmelde-Link]**: Anzahl der Klicks auf den Abmelde-Link.

* **[!UICONTROL Klicks auf den Mirror-Link]**: Anzahl der Klicks auf den Link der Mirrorseite.

* **[!UICONTROL Schätzung der Weiterleitungen]**: Schätzung der Anzahl der E-Mails, die von den Zielgruppenempfängerinnen und -empfängern weitergeleitet werden.
+++

### Öffnungs- und Klickrate {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Öffnungs- und Klickrate"
>abstract="Die Tabelle **Öffnungs- und Klickrate** zeigt Daten bezüglich der Interaktionen Ihrer Empfängerinnen und Empfänger mit dem Versand an."



Die **[!UICONTROL Öffnungs- und Klickrate]** zeigt Daten zu Ihren Empfängern an. Die Metriken werden nachfolgend beschrieben.

![](assets/reporting_email_6.png){align="center"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Gesendet]**: Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Beschwerden]**: Anzahl der Nachrichten für diese Domain, die von der Empfängerin oder vom Empfänger als unerwünscht gemeldet wurden.

* **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

* **[!UICONTROL Klicks]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger, die mindestens einmal in einem Versand geklickt haben.

* **[!UICONTROL Brutto-Reaktionsrate]**: Prozentualer Anteil der Empfängerinnen und Empfänger, die mindestens einmal in einem Versand geklickt haben, in Bezug auf die Empfängerinnen und Empfänger, die mindestens einmal einen Versand geöffnet haben.
+++

## URLs und Clickstreams {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URLs und Clickstreams"
>abstract="Die **URLs und Clickstreams** liefert wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den URLs enthalten, auf die während eines Versands am häufigsten geklickt wurde."


Die **[!UICONTROL URLs und Clickstreams]** liefert wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den URLs enthalten, auf die während eines Versands am häufigsten geklickt wurde.

![](assets/reporting_email_7.png){align="center"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Reaktionsrate]**: Verhältnis der Anzahl an Zielgruppenempfängerinnen und -empfängern, die auf einen Versand geklickt haben, in Bezug zur geschätzten Anzahl der Zielgruppenempfängerinnen und -empfänger, die einen Versand geöffnet haben.

* **[!UICONTROL Unterschiedliche Klicks (Unique Clicks)]**: Gesamtzahl der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

* **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

* **[!UICONTROL Plattform-Durchschnitt]**: Dieser unter jeder Rate (Reaktivität, Unique Clicks und Klicks insgesamt) angezeigte Wert bezieht sich auf die Gesamtheit der in den letzten sechs Monaten gesendeten Sendungen. Nur Sendungen, die dieselbe Typologie aufweisen und die auf demselben Kanal gesendet wurden, werden berücksichtigt. Testsendungen sind von der Statistik ausgenommen.

+++

### Die 10 meistbesuchten Links {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="Die 10 meistbesuchten Links"
>abstract="Die **Die 10 am häufigsten besuchten Links** Diagramm und Tabelle enthalten die verfügbaren Daten für das Empfängerverhalten pro Link."


Die **[!UICONTROL Die 10 am häufigsten besuchten Links]** Diagramm und Tabelle enthalten die verfügbaren Daten für das Empfängerverhalten pro Link.

![](assets/reporting_email_8.png){align="center"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

* **[!UICONTROL Prozentsatz]**: Prozentsatz der Benutzerinnen und Benutzer, die mit dem Versand interagiert haben

+++

### Aufschlüsselung der Klicks im Zeitverlauf {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="Aufschlüsselung der Klicks im Zeitverlauf"
>abstract="Die **Zeitliche Klickverteilung** -Diagramm zeigt die verfügbaren Daten für das Empfängerverhalten pro Link."


Die **[!UICONTROL Zeitliche Klickverteilung]** -Diagramm enthält die verfügbaren Daten zum Empfängerverhalten pro Link.

![](assets/reporting_email_9.png){align="center"}

## Benutzeraktivitäten {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget „Benutzeraktivitäten“"
>abstract="Das Diagramm **Benutzeraktivitäten** zeigt die Aufschlüsselung der Öffnungen und Klicks in Form eines Diagramms. Sie können den Zeitraum der Zielgruppendaten auswählen: letzter Tag, letzte Stunde oder letzte 30 Minuten."

Die **[!UICONTROL Benutzeraktivitäten]** zeigt die Öffnungs- und Klickverteilung in Form eines Diagramms an. Sie können den Zeitraum der Zielgruppendaten auswählen: letzter Tag, letzte Stunde oder letzte 30 Minuten.

![](assets/reporting_email_10.png){align="center"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

* **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

+++

## Tracking-Statistiken {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widget „Tracking-Statistiken“"
>abstract="Das Diagramm **Tracking-Statistiken** liefert Statistiken über Öffnungen und Klicks. Sie haben die Möglichkeit, den spezifischen Zeitrahmen für die Zielgruppendaten auszuwählen."

Das Diagramm **[!UICONTROL Tracking-Statistiken]** liefert Statistiken über Öffnungen und Klicks. Sie haben die Möglichkeit, den spezifischen Zeitrahmen für die Zielgruppendaten auszuwählen.

![](assets/reporting_email_11.png){align="center"}

+++Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

* **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

* **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

+++

## Aufschlüsselung der Öffnungen {#breakdown-opens}

### Öffnungsverteilung nach Gerät {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Aufschlüsselung nach Gerät"
>abstract="Die **Aufschlüsselung nach Gerät** zeigt die Verteilung der Öffnungen nach Gerät für den Zeitraum an. Für jede Kategorie werden zwei Diagramme verwendet. Das erste zeigt Statistiken zu Öffnungen auf Computern und Mobilgeräten. Die zweite zeigt die genaue Anzahl und den genauen Prozentsatz für jeden Gerätetyp an."

Die **Aufschlüsselung nach Gerät** zeigt die Verteilung der Öffnungen nach Gerät für den jeweiligen Zeitraum an: PCs, Android-Geräte, Apple-Geräte usw.

Für jede Kategorie werden zwei Diagramme verwendet. Das erste zeigt Statistiken zu Öffnungen auf Computern und Mobilgeräten. Die zweite zeigt die genaue Anzahl und den genauen Prozentsatz für jeden Gerätetyp an.

![](assets/reporting_email_13.png){align="center"}


### Öffnungsverteilung nach Betriebssystem {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Verteilung nach Betriebssystem"
>abstract="Die **Aufschlüsselung nach Betriebssystem** zeigt die Verteilung der Öffnungen nach Betriebssystem für den betreffenden Zeitraum an. Das erste Diagramm zeigt Statistiken zu Öffnungen auf Computern und Mobilgeräten. Die zweite zeigt die genaue Anzahl und den genauen Prozentsatz für jedes Betriebssystem an."

Die **Aufschlüsselung nach Betriebssystem** zeigt die Verteilung der Öffnungen nach Betriebssystem für den jeweiligen Zeitraum an: Windows-Systeme, Android-Systeme, iOS-Systeme usw.

Für jede Kategorie werden zwei Diagramme verwendet. Die erste zeigt Statistiken über Öffnungen auf einem Computer und mobilen Betriebssystemen an. Die zweite zeigt die genaue Anzahl und den genauen Prozentsatz für jedes Betriebssystem an.

![](assets/reporting_email_13.1.png){align="center"}

### Öffnungsverteilung nach Browser {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Aufschlüsselung nach Browser"
>abstract="Die **Aufschlüsselung nach Browser** zeigt die Verteilung der Öffnungen nach Browser für den Zeitraum an. Das erste Diagramm zeigt Statistiken zu Öffnungen auf Computern und Mobilgeräten. Die zweite zeigt die genaue Anzahl und den genauen Prozentsatz für jeden Browser an."

Die **Aufschlüsselung nach Browser** zeigt die Öffnungsverteilung nach Browser an: Chrome, Safari, Internet Explorer usw.

Für jede Kategorie werden zwei Diagramme verwendet. Die erste zeigt Statistiken über Öffnungen auf einem Computer und mobilen Betriebssystemen an. Die zweite zeigt die genaue Anzahl und den genauen Prozentsatz für jeden Browser an.

![](assets/reporting_email_13.2.png){align="center"}


## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Hotclicks-Bericht"
>abstract="Der Bericht **Hotclicks** zeigt den E-Mail-Inhalt (HTML und/oder Text) mit dem prozentualen Klickanteil für jeden Link. Gestaltungsbausteine, Abmelde-Links, Mirrorseiten-Links und Angebots-Links werden bei der Gesamtanzahl der Klicks berücksichtigt, jedoch nicht im Bericht angezeigt."

Dieser Bericht zeigt den Nachrichteninhalt (HTML und/oder Text) mit dem prozentualen Klickanteil für jeden Link. Gestaltungsbausteine, Abmelde-Links, Mirrorseiten-Links und Angebots-Links werden bei der Gesamtanzahl der Klicks berücksichtigt, jedoch nicht im Bericht angezeigt.

![](assets/reporting11.png)
