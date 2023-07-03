---
audience: end-user
title: E-Mail-Versandberichte
description: Erfahren Sie, wie Sie auf E-Mail-Versandberichte zugreifen und diese verwenden können
badge: label="Alpha"
source-git-commit: a653fe4329f449a94f8056e4b5f2247bd839b87a
workflow-type: ht
source-wordcount: '1407'
ht-degree: 100%

---

# E-Mail-Versandbericht {#email-report}

Der **E-Mail-Versandbericht** bietet umfassende Einblicke und Daten, die speziell für den E-Mail-Kanal gelten. Er bietet detaillierte Informationen über Leistung, Effektivität und Ergebnisse Ihrer einzelnen Sendungen und verschafft Ihnen einen umfassenden Überblick.

## Versandzusammenfassung {#delivery-summary-email}

* Die Tabelle **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** zeigt Daten zu Ihren Empfängerinnen und Empfängern an:

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger.

   * **[!UICONTROL Zu versenden]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Ausschluss]**: Gesamtzahl der vom Versand an die Zielgruppe ausgeschlossenen Nachrichten.
+++

* **[!UICONTROL Versandstatistiken]**: Die Tabelle gibt Auskunft über den Erfolg Ihres Versands.

  ![](assets/reporting_email_2.png){align="left"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Kampagnen-Berichts.

   * **[!UICONTROL Gesendete Nachricht]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitungen im Verhältnis zur Anzahl der zu versendenden Nachrichten.

   * **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

+++

* **[!UICONTROL Ausschlussgründe]**: Diagramm und Tabelle zeigen die Aufschlüsselung der im Zuge der Analyse abgelehnten Nachrichten nach Regeln.

  ![](assets/reporting_email_3.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehlertyp, der während des Versands erzeugt wird, um anzuzeigen, dass die E-Mail-Adresse ungültig ist.

   * **[!UICONTROL Ungültige Domain]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Domain der E-Mail-Adresse falsch ist oder nicht existiert.

   * **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn das Postfach zu viele Nachrichten enthält.

   * **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

   * **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

   * **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

   * **[!UICONTROL Nicht angemeldet]**: Fehlertyp, wenn das Mobiltelefon der Empfängerin bzw. des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder über keinen Netzempfang verfügte.

+++

## Versanddurchsatz {#delivery-throughtput}

Dieser Bericht enthält detaillierte Informationen zum Versanddurchsatz der gesamten Plattform innerhalb eines bestimmten Zeitraums. Die wichtigste Kennzahl, mit der die Geschwindigkeit des Nachrichtenversands gemessen wird, ist die Anzahl der pro Stunde gesendeten Nachrichten.

## Versandstatistiken {#broadcast-statistics}

* Die Tabelle **[!UICONTROL Versandstatistiken]** enthält die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind.

  ![](assets/reporting_email_4.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Verarbeitete E-Mails]**: Gesamtzahl der Nachrichten, die vom Versand-Server verarbeitet wurden.

   * **[!UICONTROL Zugestellt]**: Prozentualer Anteil der erfolgreich verarbeiteten Nachrichten im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten.

   * **[!UICONTROL Hardbounces]**: Prozentualer Anteil der „Hardbounces“, d. h. permanente Fehler wie etwa eine falsche E-Mail-Adresse, im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten.

   * **[!UICONTROL Softbounces]**: Prozentualer Anteil der „Softbounces“, d. h. temporäre Fehler wie etwa ein voller Posteingang, im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten

   * **[!UICONTROL Öffnungen]**: Prozentualer Anteil der Zielgruppenempfängerinnen und -empfänger, die mindestens einmal eine Nachricht geöffnet haben, im Vergleich zur Gesamtzahl der erfolgreich verarbeiteten Nachrichten.

   * **[!UICONTROL Klicks]**: Prozentsatz der Anzahl der Personen, die mindestens einmal auf einen Versand geklickt haben, im Vergleich zur Anzahl der erfolgreich verarbeiteten Nachrichten.

   * **[!UICONTROL Abmeldungen]**: Prozentualer Anteil der Klicks auf einen Abmelde-Link in Bezug auf die Gesamtzahl der verarbeiteten Nachrichten.
+++

## Unzustellbare Nachrichten und Bounces {#non-deliverables-email}

* Die Tabellen und Diagramme **[!UICONTROL Aufschlüsselung der Fehler nach Typ]** und **[!UICONTROL Aufschlüsselung der Fehler nach Domain]** enthalten die verfügbaren Daten zu möglichen Fehlern, die bei jeder Domain aufgetreten sind.

  Die in diesem Bericht angezeigten Fehler lösen einen Quarantäneprozess aus. Weitere Informationen zur Quarantäneverwaltung finden Sie in der [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=de){target="_blank"}.

  ![](assets/campaign_report_email_6.png)

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehlertyp, der während des Versands erzeugt wird, um anzuzeigen, dass die E-Mail-Adresse ungültig ist.

   * **[!UICONTROL Ungültige Domain]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Domain der E-Mail-Adresse falsch ist oder nicht existiert.

   * **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn das Postfach zu viele Nachrichten enthält.

   * **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

   * **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

   * **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

   * **[!UICONTROL Nicht angemeldet]**: Fehlertyp, wenn das Mobiltelefon der Empfängerin bzw. des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder über keinen Netzempfang verfügte.

+++

## Tracking-Indikatoren {#tracking-indicators-email}

* **[!UICONTROL Versandstatistiken]** bieten wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den für gesendete E-Mails verfügbaren Daten enthalten.

  ![](assets/reporting_email_5.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

   * **[!UICONTROL Unterschiedliche Öffnungen (Unique Opens)]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger, die mindestens einmal eine Nachricht geöffnet haben.

   * **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

   * **[!UICONTROL Klicks auf den Abmelde-Link]**: Anzahl der Klicks auf den Abmelde-Link.

   * **[!UICONTROL Klicks auf den Mirror-Link]**: Anzahl der Klicks auf den Link der Mirrorseite.

   * **[!UICONTROL Schätzung der Weiterleitungen]**: Schätzung der Anzahl der E-Mails, die von den Zielgruppenempfängerinnen und -empfängern weitergeleitet werden.
+++

* Die Tabelle **[!UICONTROL Öffnungs- und Klickrate]** zeigt Daten zu Ihren Empfängerinnen und Empfängern an.

  ![](assets/reporting_email_6.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Gesendet]**: Gesamtzahl der gesendeten Nachrichten.

   * **[!UICONTROL Beschwerden]**: Anzahl der Nachrichten für diese Domain, die von der Empfängerin oder vom Empfänger als unerwünscht gemeldet wurden.

   * **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

   * **[!UICONTROL Klicks]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger, die mindestens einmal in einem Versand geklickt haben.

   * **[!UICONTROL Brutto-Reaktionsrate]**: Prozentualer Anteil der Empfängerinnen und Empfänger, die mindestens einmal in einem Versand geklickt haben, in Bezug auf die Empfängerinnen und Empfänger, die mindestens einmal einen Versand geöffnet haben.
+++

## URLs und Clickstreams {#url-email}

* **[!UICONTROL URLs und Clickstreams]**: Bietet wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den URLs enthalten, auf die während eines Versands am häufigsten geklickt wurde.

  ![](assets/reporting_email_7.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Reaktionsrate]**: Verhältnis der Anzahl an Zielgruppenempfängerinnen und -empfängern, die auf einen Versand geklickt haben, in Bezug zur geschätzten Anzahl der Zielgruppenempfängerinnen und -empfänger, die einen Versand geöffnet haben.

   * **[!UICONTROL Unterschiedliche Klicks (Unique Clicks)]**: Gesamtzahl der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Plattform-Durchschnitt]**: Dieser unter jeder Rate (Reaktivität, Unique Clicks und Klicks insgesamt) angezeigte Wert bezieht sich auf die Gesamtheit der in den letzten sechs Monaten gesendeten Sendungen. Nur Sendungen, die dieselbe Typologie aufweisen und die auf demselben Kanal gesendet wurden, werden berücksichtigt. Testsendungen sind von der Statistik ausgenommen.

+++

* **[!UICONTROL Die 10 meistbesuchten Links]**: Diagramm und Tabelle mit den verfügbaren Daten für das Empfängerverhalten pro Link.

  ![](assets/reporting_email_8.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Prozentsatz]**: Prozentsatz der Benutzerinnen und Benutzer, die mit dem Versand interagiert haben

+++

* **[!UICONTROL Aufschlüsselung der Klicks im Zeitverlauf]**: Das Diagramm enthält die verfügbaren Daten zum Empfängerverhalten pro Link.

  ![](assets/reporting_email_9.png){align="center"}

## Benutzeraktivitäten {#user-activities-email}

* **[!UICONTROL Benutzeraktivitäten]**: Zeigt die Aufschlüsselung der Öffnungen und Klicks in Form eines Diagramms. Sie können den Zeitraum der Zielgruppendaten auswählen: letzter Tag, letzte Stunde oder letzte 30 Minuten.

  ![](assets/reporting_email_10.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

+++

## Tracking-Statistiken {#tracking-statistics}

* **[!UICONTROL Tracking-Statistiken]**: Das Diagramm enthält Statistiken über Öffnungen und Klicks. Sie haben die Möglichkeit, den spezifischen Zeitrahmen für die Zielgruppendaten auszuwählen.

  ![](assets/reporting_email_11.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

+++

## Aufschlüsselung der Öffnungen {#breakdown-opens}

Dieser Bericht zeigt die Aufschlüsselung der Öffnungen nach Betriebssystem, Gerät und Browser für den betreffenden Zeitraum. Für jede Kategorie stehen zwei Diagramme zur Verfügung. Das erste zeigt die Öffnungsstatistiken für Computer und Mobilgeräte an, das zweite nur für Mobilgeräte.
Sie haben die Möglichkeit, von **[!UICONTROL Desktop-Computer und Mobilgeräte]** auf ausschließlich **[!UICONTROL Nur Mobilgeräte]** umzuschalten, um die Genauigkeit der Zielgruppenbestimmung zu erhöhen.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

Dieser Bericht zeigt den Nachrichteninhalt (HTML und/oder Text) mit dem prozentualen Klickanteil für jeden Link. Abmelde-Links in Gestaltungsbausteinen sowie Mirror-Seiten-Links und Angebots-Links werden in der Gesamtklickzahl berücksichtigt, in diesem Bericht jedoch nicht angezeigt.

![](assets/reporting11.png)
