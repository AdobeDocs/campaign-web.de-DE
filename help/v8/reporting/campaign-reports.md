---
audience: end-user
title: Kampagnenberichte
description: Erfahren Sie, wie Sie auf Kampagnenberichte zugreifen und diese verwenden können
badge: label="Alpha" type="Positive"
source-git-commit: 875b7edac9696af227273a02357d5431f6a1e8ab
workflow-type: tm+mt
source-wordcount: '1682'
ht-degree: 8%

---

# Kampagnenberichte {#campaign-reports}

Der Kampagnenbericht ist in verschiedene Widgets unterteilt, die den Erfolg und die Fehler Ihrer Kampagne detailliert beschreiben.

Die Seite Kampagnenbericht wird mit den folgenden Tabs angezeigt:

* [E-Mail-Kanal](#email-channel)
* [SMS-Kanal](#sms-channel)
* [Push-Kanal](#push-channel)

Um auf Ihren Kampagnenbericht zuzugreifen, klicken Sie im Dashboard Ihrer Kampagne auf Berichte .

![](assets/campaign_report_email_13.png)

## E-Mail-Kanal {#email-channel}

### Versandzusammenfassung {#delivery-summary-email}

* **[!UICONTROL Versandübersicht]** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucher mit Ihrem E-Mail-Versand interagieren.

  ![](assets/campaign_report_email_1.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Gesendete Summe]**: Gesamtzahl der bei der Versandanalyse verarbeiteten Nachrichten.

   * **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten

   * **[!UICONTROL Bounces]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Gesamtzahl der gesendeten Nachrichten.

   * **[!UICONTROL Unique Opens]**: Gesamtzahl der Zielgruppenempfänger, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

+++

* **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** -Tabelle zeigt Daten zu Ihren Empfängern an:

  ![](assets/campaign_report_email_2.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger

   * **[!UICONTROL Zu sendende Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Nach Regeln abgelehnt]**: Gesamtzahl der im Zuge der Regelanalyse ignorierten Adressen: Adresse fehlt, in Quarantäne, auf Blockierungsliste usw.

+++

* **[!UICONTROL Ausführungsstatistiken]** -Tabelle zeigt den Erfolg Ihres Versands.

  ![](assets/campaign_report_email_3.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Zu sendende Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten in Bezug auf die Anzahl der zu sendenden Nachrichten.

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

   * **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), in Bezug auf die Zahl der zu sendenden Nachrichten.

+++

* **[!UICONTROL Reaktionsstatistiken]** enthält die verfügbaren Daten zur Empfängeraktivität für Ihren Versand.

  ![](assets/campaign_report_email_4.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Unique Opens]**: Gesamtzahl der Zielgruppenempfänger, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Abmeldungen]**: Anzahl der Empfänger, die in dem betreffenden Zeitraum auf Abmeldungen geklickt haben

   * **[!UICONTROL Mirrorseite]**: Anzahl der Empfänger, die auf den Mirrorseiten-Link geklickt haben

   * **[!UICONTROL Forwards]**: Anzahl der Empfänger, die geklickt haben, die die E-Mail weitergeleitet haben
+++

* **[!UICONTROL Erzeugte Clickstreams]** zeigt Daten dazu an, wie Ihre Empfänger mit Ihrem Versand interagiert haben.

  ![](assets/campaign_report_email_5.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Reaktivität]**: Prozentualer Anteil der Zielgruppenempfänger, die in einen Versand geklickt haben, in Bezug auf die geschätzte Anzahl der Zielgruppenempfänger, die einen Versand geöffnet haben.

+++

### Unzustellbare E-Mails {#non-deliverables-email}

* **[!UICONTROL Verteilung der Fehler nach Typ]** und **[!UICONTROL Verteilung der Fehler nach Domain]** Tabellen und Diagramme enthalten die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind.

  ![](assets/campaign_report_email_6.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehler bei ungültigen E-Mail-Adressen.

   * **[!UICONTROL Ungültige Domain]**: Fehler bei ungültigen oder inexistenten E-Mail-Domains.

   * **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn der Posteingang der Empfänger zu viele Nachrichten enthält.

   * **[!UICONTROL Konto deaktiviert]**: Fehler, wenn eine Adresse nicht mehr existiert.

   * **[!UICONTROL Abgelehnt]**: Fehlertyp, der erzeugt wird, wenn eine Adresse von einem ISP (Internet Access Provider) z. B. aufgrund der Anwendung einer Sicherheitsregel (Anti-Spam-Software) zurückgewiesen wird.

   * **[!UICONTROL Unerreichbar]**: Fehler in der Verteilungskette der Nachricht (Vorfall beim SMTP-Server, zeitweilig unerreichbare Domain usw.).

   * **[!UICONTROL Nicht angemeldet]**: Fehlertyp, der angibt, dass das Mobiltelefon des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder vom Netzwerk getrennt war.

+++

### Tracking-Indikatoren {#tracking-indicators-email}

* **[!UICONTROL Versandstatistiken]** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen zu den für gesendete E-Mails verfügbaren Daten enthalten.

  ![](assets/campaign_report_email_7.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten in Bezug auf die Anzahl der zu sendenden Nachrichten.

   * **[!UICONTROL Unique Opens]**: Gesamtzahl der Zielgruppenempfänger, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Klicks auf den Ausschluss-Link]**: Anzahl der Klicks auf den Abmelde-Link.

   * **[!UICONTROL Klicks auf den Mirrorlink]**: Anzahl der Klicks auf den Mirrorseite-Link.

   * **[!UICONTROL Schätzung der Weiterleitungen]**: Schätzung der Anzahl der E-Mails, die von den Zielgruppenempfängern weitergeleitet werden.
+++

* **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** zeigt Daten zu Ihren Empfängern an.

  ![](assets/campaign_report_email_8.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Gesendet]**: Gesamtzahl der gesendeten Nachrichten

   * **[!UICONTROL Beschwerden]**: Anzahl der Nachrichten für diese Domain, die vom Empfänger als unerwünscht gemeldet wurden.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Klicks]**: Anzahl unterschiedlicher Zielgruppenempfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Brutto-Reaktionsrate]**: Prozentualer Anteil der Empfänger, die mindestens einmal im betreffenden Versand geklickt haben, in Bezug auf die Empfänger, die mindestens einmal den betreffenden Versand geöffnet haben.
+++

### URLs und Clickstreams {#url-email}

* **[!UICONTROL URLs und Clickstreams]** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen zu den URLs enthalten, auf die während eines Versands am häufigsten geklickt wurde.

  ![](assets/campaign_report_email_9.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Reaktivität]**: Prozentualer Anteil der Zielgruppenempfänger, die in einen Versand geklickt haben, in Bezug auf die geschätzte Anzahl der Zielgruppenempfänger, die einen Versand geöffnet haben.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

+++

* **[!UICONTROL Die 10 am häufigsten besuchten Links]** Diagramm und Tabelle enthalten die verfügbaren Daten für das Empfängerverhalten pro Link.

  ![](assets/campaign_report_email_10.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Prozentsatz]**: Prozentsatz der Benutzer, die mit dem Versand interagiert haben

+++

* **[!UICONTROL Zeitliche Klickverteilung]** -Diagramm enthält die verfügbaren Daten zum Empfängerverhalten pro Link.

  ![](assets/campaign_report_email_11.png)

### Benutzeraktivitäten {#user-activities-email}

* **[!UICONTROL Benutzeraktivitäten]** zeigt die Verteilung der Öffnungen und Klicks in Form eines Diagramms.

  ![](assets/campaign_report_email_12.png)

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

+++

## SMS-Kanal {#sms-channel}

### Versandzusammenfassung {#delivery-summary-sms}

* **[!UICONTROL Versandübersicht]** bietet wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zur Interaktion Ihrer Besucher mit Ihrem SMS-Versand enthalten.

  ![](assets/campaign_report_sms_1.png)

  +++ Erfahren Sie mehr über SMS-Kampagnenberichtsmetriken.

   * **[!UICONTROL Gesendete Summe]**: Gesamtzahl der bei der Versandanalyse verarbeiteten Nachrichten.

   * **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Gesamtzahl der gesendeten Nachrichten.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

+++

* **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** -Tabelle zeigt Daten zu Ihren Empfängern an:

  ![](assets/campaign_report_sms_2.png)

  +++ Erfahren Sie mehr über SMS-Kampagnenberichtsmetriken.

   * **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger

   * **[!UICONTROL Zu sendende Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Nach Regeln abgelehnt]**: Gesamtzahl der im Zuge der Regelanalyse ignorierten Adressen: Adresse fehlt, in Quarantäne, auf Blockierungsliste usw.

+++

* **[!UICONTROL Ausführungsstatistiken]** -Tabelle zeigt den Erfolg Ihres Versands:

  ![](assets/campaign_report_sms_3.png)

  +++ Erfahren Sie mehr über SMS-Kampagnenberichtsmetriken.

   * **[!UICONTROL Zu sendende Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten in Bezug auf die Anzahl der zu sendenden Nachrichten.

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

   * **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), in Bezug auf die Zahl der zu sendenden Nachrichten.

+++

* **[!UICONTROL Erzeugte Clickstreams]** -Tabelle zeigt Daten dazu an, wie Ihre Empfänger mit Ihrem Versand interagiert haben:

  ![](assets/campaign_report_sms_4.png)

  +++ Erfahren Sie mehr über SMS-Kampagnenberichtsmetriken.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Reaktivität]**: Prozentualer Anteil der Zielgruppenempfänger, die in einen Versand geklickt haben, in Bezug auf die geschätzte Anzahl der Zielgruppenempfänger, die einen Versand geöffnet haben.

+++

## Push-Kanal {#push-channel}

### Versandzusammenfassung {#delivery-summary-push}

* **[!UICONTROL Versandübersicht]** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucher mit Ihrem Push-Benachrichtigungsversand interagieren.

  +++ Erfahren Sie mehr über die Metriken des Push-Kampagnen-Berichts.

   * **[!UICONTROL Gesendete Summe]**: Gesamtzahl der bei der Versandanalyse verarbeiteten Nachrichten.

   * **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Gesamtzahl der gesendeten Nachrichten.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

+++

* **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** -Tabelle zeigt Daten zu Ihren Empfängern an:

  +++ Erfahren Sie mehr über die Metriken des Push-Kampagnen-Berichts.

   * **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger

   * **[!UICONTROL Zu sendende Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Nach Regeln abgelehnt]**: Gesamtzahl der im Zuge der Regelanalyse ignorierten Adressen: Adresse fehlt, in Quarantäne, auf Blockierungsliste usw.

+++

* **[!UICONTROL Ausführungsstatistiken]** -Tabelle zeigt den Erfolg Ihres Versands:

  +++ Erfahren Sie mehr über die Metriken des Push-Kampagnen-Berichts.

   * **[!UICONTROL Zu sendende Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten in Bezug auf die Anzahl der zu sendenden Nachrichten.

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

   * **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), in Bezug auf die Zahl der zu sendenden Nachrichten.

+++

* **[!UICONTROL Erzeugte Clickstreams]** -Tabelle zeigt Daten dazu an, wie Ihre Empfänger mit Ihrem Versand interagiert haben:

  +++ Erfahren Sie mehr über die Metriken des Push-Kampagnen-Berichts.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Reaktivität]**: Prozentualer Anteil der Zielgruppenempfänger, die in einen Versand geklickt haben, in Bezug auf die geschätzte Anzahl der Zielgruppenempfänger, die einen Versand geöffnet haben.

+++
