---
audience: end-user
title: E-Mail-Versandberichte
description: Erfahren Sie, wie Sie auf E-Mail-Versandberichte zugreifen und diese verwenden
badge: label="Alpha" type="Positive"
source-git-commit: a8bc3317bc97d429ab6c9abdf5f503a5123f591e
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 26%

---

# Email-Versandbericht {#email-report}

Die **Email-Versandbericht** bietet umfassende Einblicke und Daten, die speziell für den E-Mail-Kanal gelten. Er bietet detaillierte Informationen über Leistung, Effektivität und Ergebnisse Ihrer Sendungen und bietet Ihnen einen umfassenden Überblick.

## Versandzusammenfassung {#delivery-summary-email}

* **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** -Tabelle zeigt Daten zu Ihren Empfängern an:

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger

   * **[!UICONTROL Zu liefern]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Ausschluss]**: Gesamtzahl der vom Versand an die Zielgruppe ausgeschlossenen Nachrichten.
+++

* **[!UICONTROL Versandstatistiken]** -Tabelle zeigt den Erfolg Ihres Versands.

  ![](assets/reporting_email_2.png){align="left"}

  +++ Erfahren Sie mehr über E-Mail-Kampagnen-Berichtsmetriken.

   * **[!UICONTROL Nachricht gesendet]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten in Bezug auf die Anzahl der zu sendenden Nachrichten.

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

   * **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), in Bezug auf die Zahl der zu sendenden Nachrichten.

+++

* **[!UICONTROL Ausschlussgründe]** Diagramm und Tabelle zeigen die Verteilung der im Zuge der Analyse zurückgewiesenen Nachrichten nach Regeln.

  ![](assets/reporting_email_3.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehler bei ungültigen E-Mail-Adressen.

   * **[!UICONTROL Ungültige Domain]**: Fehler bei ungültigen oder inexistenten E-Mail-Domains.

   * **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn der Posteingang der Empfänger zu viele Nachrichten enthält.

   * **[!UICONTROL Konto deaktiviert]**: Fehler, wenn eine Adresse nicht mehr existiert.

   * **[!UICONTROL Abgelehnt]**: Fehlertyp, der erzeugt wird, wenn eine Adresse von einem ISP (Internet Access Provider) z. B. aufgrund der Anwendung einer Sicherheitsregel (Anti-Spam-Software) zurückgewiesen wird.

   * **[!UICONTROL Unerreichbar]**: Fehler in der Verteilungskette der Nachricht (Vorfall beim SMTP-Server, zeitweilig unerreichbare Domain usw.).

   * **[!UICONTROL Nicht angemeldet]**: Fehlertyp, der angibt, dass das Mobiltelefon des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder vom Netzwerk getrennt war.

+++

## Versanddurchsatz {#delivery-throughtput}

Dieser Bericht enthält detaillierte Informationen zum Versanddurchsatz der gesamten Plattform innerhalb eines bestimmten Zeitraums. Die Hauptmetrik, mit der die Geschwindigkeit des Nachrichtenversands gemessen wird, ist die Anzahl der pro Stunde gesendeten Nachrichten.

## Broadcast-Statistiken {#broadcast-statistics}

* **[!UICONTROL Versandstatistiken]** enthält die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind.

  ![](assets/reporting_email_4.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Verarbeitete E-Mails]**: Gesamtzahl der vom Versandserver verarbeiteten Nachrichten.

   * **[!UICONTROL Zugestellt]**: Prozentualer Anteil der erfolgreich verarbeiteten E-Mails in Bezug auf die Gesamtzahl der verarbeiteten E-Mails.

   * **[!UICONTROL Hardbounces]**: Prozentualer Anteil der Hardbounces, permanenten Fehler wie eine falsche E-Mail-Adresse in Bezug auf die Gesamtzahl der verarbeiteten E-Mails.

   * **[!UICONTROL Softbounces]**: Prozentualer Anteil der Softbounces, temporäre Fehler wie einen vollständigen Posteingang in Bezug auf die Gesamtzahl der verarbeiteten E-Mails

   * **[!UICONTROL Öffnungen]**: Prozentualer Anteil der Zielgruppenempfänger, die mindestens einmal die betreffende Nachricht geöffnet haben, in Bezug auf die Gesamtzahl der verarbeiteten E-Mails.

   * **[!UICONTROL Klicks]**: Prozentualer Anteil der Personen, die mindestens einmal im betreffenden Versand geklickt haben, in Bezug auf die Gesamtzahl der verarbeiteten E-Mails.

   * **[!UICONTROL Abmeldungen]**: Prozentualer Anteil der Klicks auf einen Abmelde-Link in Bezug auf die Gesamtzahl der verarbeiteten E-Mails.
+++

## Fehler und Bounces {#non-deliverables-email}

* **[!UICONTROL Verteilung der Fehler nach Typ]** und **[!UICONTROL Verteilung der Fehler nach Domain]** Tabellen und Diagramme enthalten die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind.

  Die in diesem Bericht dargestellten Fehler lösen eine Quarantäne der betroffenen Adressen aus. Weiterführende Informationen zur Quarantäneverwaltung finden Sie im Abschnitt [Quarantäneverwaltung](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=de)

  ![](assets/campaign_report_email_6.png)

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehler bei ungültigen E-Mail-Adressen.

   * **[!UICONTROL Ungültige Domain]**: Fehler bei ungültigen oder inexistenten E-Mail-Domains.

   * **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn der Posteingang der Empfänger zu viele Nachrichten enthält.

   * **[!UICONTROL Konto deaktiviert]**: Fehler, wenn eine Adresse nicht mehr existiert.

   * **[!UICONTROL Abgelehnt]**: Fehlertyp, der erzeugt wird, wenn eine Adresse von einem ISP (Internet Access Provider) z. B. aufgrund der Anwendung einer Sicherheitsregel (Anti-Spam-Software) zurückgewiesen wird.

   * **[!UICONTROL Unerreichbar]**: Fehler in der Verteilungskette der Nachricht (Vorfall beim SMTP-Server, zeitweilig unerreichbare Domain usw.).

   * **[!UICONTROL Nicht angemeldet]**: Fehlertyp, der angibt, dass das Mobiltelefon des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder vom Netzwerk getrennt war.

+++

## Tracking-Indikatoren {#tracking-indicators-email}

* **[!UICONTROL Versandstatistiken]** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen zu den für gesendete E-Mails verfügbaren Daten enthalten.

  ![](assets/reporting_email_5.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten in Bezug auf die Anzahl der zu sendenden Nachrichten.

   * **[!UICONTROL Unique Opens]**: Gesamtzahl der Zielgruppenempfänger, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Klicks auf den Ausschluss-Link]**: Anzahl der Klicks auf den Abmelde-Link.

   * **[!UICONTROL Klicks auf den Mirrorlink]**: Anzahl der Klicks auf den Mirrorseite-Link.

   * **[!UICONTROL Schätzung der Weiterleitungen]**: Schätzung der Anzahl der E-Mails, die von den Zielgruppenempfängern weitergeleitet werden.
+++

* **[!UICONTROL Öffnungs- und Klickrate]** zeigt Daten zu Ihren Empfängern an.

  ![](assets/reporting_email_6.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Gesendet]**: Gesamtzahl der gesendeten Nachrichten

   * **[!UICONTROL Beschwerden]**: Anzahl der Nachrichten für diese Domain, die vom Empfänger als unerwünscht gemeldet wurden.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

   * **[!UICONTROL Klicks]**: Anzahl unterschiedlicher Zielgruppenempfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Brutto-Reaktionsrate]**: Prozentualer Anteil der Empfänger, die mindestens einmal im betreffenden Versand geklickt haben, in Bezug auf die Empfänger, die mindestens einmal den betreffenden Versand geöffnet haben.
+++

## URLs und Clickstreams {#url-email}

* **[!UICONTROL URLs und Clickstreams]** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen zu den URLs enthalten, auf die während eines Versands am häufigsten geklickt wurde.

  ![](assets/reporting_email_7.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Reaktivität]**: Prozentualer Anteil der Zielgruppenempfänger, die in einen Versand geklickt haben, in Bezug auf die geschätzte Anzahl der Zielgruppenempfänger, die einen Versand geöffnet haben.

   * **[!UICONTROL Unique Clicks]**: Gesamtzahl unterschiedlicher Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Plattform-Durchschnitt]**: Dieser unter allen Raten (Reaktivität, Unique Clicks und aufaddierte Klicks) angezeigte Wert bezieht sich auf die Gesamtheit der in den letzten sechs Monaten gesendeten Nachrichten. Nur Sendungen, die dieselbe Typologie aufweisen und die auf demselben Kanal gesendet wurden, werden berücksichtigt. Testsendungen sind von der Statistik ausgenommen.

+++

* **[!UICONTROL Die 10 am häufigsten besuchten Links]** Diagramm und Tabelle enthalten die verfügbaren Daten für das Empfängerverhalten pro Link.

  ![](assets/reporting_email_8.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Prozentsatz]**: Prozentsatz der Benutzer, die mit dem Versand interagiert haben

+++

* **[!UICONTROL Zeitliche Klickverteilung]** -Diagramm enthält die verfügbaren Daten zum Empfängerverhalten pro Link.

  ![](assets/reporting_email_9.png){align="center"}

## Benutzeraktivitäten {#user-activities-email}

* **[!UICONTROL Benutzeraktivitäten]** zeigt die Verteilung der Öffnungen und Klicks in Form eines Diagramms. Sie können den Zeitraum für die Zielgruppenbestimmung von Daten auswählen: letzten Tag oder Stunde oder 30 Minuten.

  ![](assets/reporting_email_10.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

+++

## Tracking-Statistiken {#tracking-statistics}

* **[!UICONTROL Trackingstatistiken]** -Diagramm bietet Statistiken zu Öffnungen und Klicks. Sie haben die Möglichkeit, den spezifischen Zeitrahmen für die Zielgruppendaten auszuwählen.

  ![](assets/reporting_email_11.png){align="center"}

  +++ Erfahren Sie mehr über E-Mail-Versandberichtsmetriken.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl unterschiedlicher Zielgruppenempfänger dieser Domain, die mindestens einmal die betreffende Nachricht geöffnet haben.

+++

## Öffnungsverteilung {#breakdown-opens}

Dieser Bericht zeigt die Öffnungsverteilung nach Betriebssystem, Geräteart und Browser für den ausgewählten Zeitraum. Für jede Kategorie stehen zwei Diagramme zur Verfügung. Das erste zeigt die Öffnungsstatistiken für Computer und Mobilgeräte an, das zweite nur für Mobilgeräte.
Sie haben die Flexibilität, von **[!UICONTROL Fehlerbehebung und mobil]** ausschließlich Zielgruppe **[!UICONTROL Nur für Mobilgeräte]** für eine präzisere Zielgruppenbestimmung.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

Dieser Bericht zeigt den Nachrichteninhalt (HTML und/oder Text) mit dem prozentualen Klickanteil für jeden Link. Abmelde-Links in Gestaltungsbausteinen sowie Mirror-Seiten-Links und Angebots-Links werden in der Gesamtklickzahl berücksichtigt, in diesem Bericht jedoch nicht angezeigt.

![](assets/reporting11.png)
