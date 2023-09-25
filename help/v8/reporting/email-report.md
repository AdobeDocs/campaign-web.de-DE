---
audience: end-user
title: E-Mail-Versandberichte
description: Erfahren Sie, wie Sie auf E-Mail-Versandberichte zugreifen und diese verwenden können
badge: label="Beta"
source-git-commit: 9693d4b0ca6f870b8f23b950050a68ac2674db5d
workflow-type: tm+mt
source-wordcount: '1932'
ht-degree: 67%

---

# E-Mail-Versandbericht {#email-report}

Der **E-Mail-Versandbericht** bietet umfassende Einblicke und Daten, die speziell für den E-Mail-Kanal gelten. Er bietet detaillierte Informationen über Leistung, Effektivität und Ergebnisse Ihrer einzelnen Sendungen und verschafft Ihnen einen umfassenden Überblick.

## Versandzusammenfassung {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Berichterstellung"
>abstract="he **Senden** -Tab Ihres Berichts erhalten Sie einen umfassenden Einblick in die Interaktionen Ihrer Besucher mit Ihren Sendungen und in etwaige Fehler, die bei ihnen aufgetreten sind."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="anfängliches Zielgruppen-Widget"
>abstract="Die **Ursprungspopulation der Zielgruppe** -Diagramm zeigt Daten zu Ihren Empfängern und zum Erfolg Ihres Versands an."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Widget &quot;Versandstatistiken&quot;"
>abstract="Die **Versandstatistiken** -Diagramm zeigt den Erfolg Ihres Versands und die aufgetretenen Fehler."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Widget &quot;Versandstatistiken&quot;"
>abstract="Die Tabelle Ausschlussgründe zeigt die Verteilung der während der Vorbereitung zurückgewiesenen Nachrichten nach Regeln."

* **[!UICONTROL Ursprungspopulation der Zielgruppe]** -Diagramm zeigt Daten zu Ihren Empfängern an:

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger.

   * **[!UICONTROL Zu liefern]**: Gesamtzahl der nach der Versandvorbereitung zu versendenden Nachrichten.

   * **[!UICONTROL Ausschluss]**: Gesamtzahl der vom Versand an die Zielgruppe ausgeschlossenen Nachrichten.
+++

* **[!UICONTROL Versandstatistiken]** -Diagramm zeigt den Erfolg Ihres Versands an.

  ![](assets/reporting_email_2.png){align="left"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Kampagnen-Berichts.

   * **[!UICONTROL Nachricht gesendet]**: Gesamtzahl der nach der Versandvorbereitung zu versendenden Nachrichten.

   * **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

   * **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitungen im Verhältnis zur Anzahl der zu versendenden Nachrichten.

   * **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

+++

* **[!UICONTROL Ausschlussgründe]**: Diagramm und Tabelle zeigen die Aufschlüsselung der im Zuge der Analyse abgelehnten Nachrichten nach Regeln.

  ![](assets/reporting_email_3.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehlertyp, der während des Versands erzeugt wird, um anzuzeigen, dass die E-Mail-Adresse ungültig ist.

   * **[!UICONTROL Ungültige Domain]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Domain der E-Mail-Adresse falsch ist oder nicht existiert.

   * **[!UICONTROL Postfach voll]**: Fehler, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn der Posteingang der Empfänger zu viele Nachrichten enthält.

   * **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

   * **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

   * **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

   * **[!UICONTROL Nicht angemeldet]**: Fehler, wenn das Mobiltelefon des Empfängers bei Versand der Nachricht ausgeschaltet war oder über keinen Netzempfang verfügte.

+++

## Versanddurchsatz {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Versanddurchsatz Widget"
>abstract="Die **Versanddurchsatz** enthält detaillierte Informationen zum Versanddurchsatz der gesamten Plattform innerhalb eines bestimmten Zeitraums."

Dieser Bericht enthält detaillierte Informationen zum Versanddurchsatz der gesamten Plattform innerhalb eines bestimmten Zeitraums. Die wichtigste Kennzahl, mit der die Geschwindigkeit des Nachrichtenversands gemessen wird, ist die Anzahl der pro Stunde gesendeten Nachrichten.

## Versandstatistiken {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Widget &quot;Versandstatistiken&quot;"
>abstract="Die **Versandstatistiken** enthält die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind."

* Die Tabelle **[!UICONTROL Versandstatistiken]** enthält die verfügbaren Daten zu Fehlern, die bei jeder Domain aufgetreten sind.

  ![](assets/reporting_email_4.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Verarbeitete E-Mails]**: Gesamtzahl der Nachrichten, die vom Versand-Server verarbeitet wurden.

   * **[!UICONTROL Zugestellt]**: Prozentualer Anteil der erfolgreich verarbeiteten Nachrichten im Vergleich zur Gesamtzahl der verarbeiteten Nachrichten.

   * **[!UICONTROL Hardbounces]**: Prozentualer Anteil der Hardbounces, permanenten Fehler wie eine falsche E-Mail-Adresse in Bezug auf die Gesamtzahl der verarbeiteten E-Mails.

   * **[!UICONTROL Softbounces]**: Prozentualer Anteil der Softbounces, temporäre Fehler wie einen vollständigen Posteingang in Bezug auf die Gesamtzahl der verarbeiteten E-Mails

   * **[!UICONTROL Öffnungen]**: Prozentualer Anteil der Zielgruppenempfängerinnen und -empfänger, die mindestens einmal eine Nachricht geöffnet haben, im Vergleich zur Gesamtzahl der erfolgreich verarbeiteten Nachrichten.

   * **[!UICONTROL Klicks]**: Prozentsatz der Anzahl der Personen, die mindestens einmal auf einen Versand geklickt haben, im Vergleich zur Anzahl der erfolgreich verarbeiteten Nachrichten.

   * **[!UICONTROL Abmeldungen]**: Prozentualer Anteil der Klicks auf einen Abmelde-Link in Bezug auf die Gesamtzahl der verarbeiteten Nachrichten.
+++

## Unzustellbare Nachrichten und Bounces {#non-deliverables-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Verteilung der Fehler nach Typ-Widget"
>abstract="Die **Verteilung der Fehler nach Typ** Tabelle und Diagramm enthalten die verfügbaren Daten für jeden aufgetretenen Fehlertyp."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Verteilung der Fehler nach Domain-Widget"
>abstract="Die **Verteilung der Fehler nach Domain** -Tabelle und -Diagramm enthalten die verfügbaren Daten für jeden Fehlertyp, der je nach Domäne aufgetreten ist."

* Die Tabellen und Diagramme **[!UICONTROL Aufschlüsselung der Fehler nach Typ]** und **[!UICONTROL Aufschlüsselung der Fehler nach Domain]** enthalten die verfügbaren Daten zu möglichen Fehlern, die bei jeder Domain aufgetreten sind.

  Die in diesem Bericht angezeigten Fehler lösen einen Quarantäneprozess aus. Weitere Informationen zur Quarantäneverwaltung finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=de){target="_blank"}.

  ![](assets/campaign_report_email_6.png)

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Unbekannter Nutzer]**: Fehlertyp, der während des Versands erzeugt wird, um anzuzeigen, dass die E-Mail-Adresse ungültig ist.

   * **[!UICONTROL Ungültige Domain]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Domain der E-Mail-Adresse falsch ist oder nicht existiert.

   * **[!UICONTROL Postfach voll]**: Fehler, der nach fünf fehlgeschlagenen Zustellversuchen erzeugt wird, wenn der Posteingang der Empfänger zu viele Nachrichten enthält.

   * **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

   * **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

   * **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

   * **[!UICONTROL Nicht angemeldet]**: Fehler, wenn das Mobiltelefon des Empfängers bei Versand der Nachricht ausgeschaltet war oder über keinen Netzempfang verfügte.

+++

## Tracking-Indikatoren {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Tracking-Berichte"
>abstract="Die **Tracking** -Tab Ihres Berichts enthält wertvolle Daten, darunter das Empfängerverhalten pro Link, die Öffnungs- und Klickverteilung sowie detaillierte Informationen zu den am häufigsten angeklickten URLs während eines Versands."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Widget &quot;Versandstatistiken&quot;"
>abstract="Die **Versandstatistiken** Widget bietet wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen zu den für gesendete E-Mails verfügbaren Daten enthalten."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Widget zur Öffnungs- und Klickrate"
>abstract="Die **Öffnungs- und Klickrate** zeigt Daten bezüglich der Interaktion Ihrer Empfänger mit Ihrem Versand an."

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

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URLs und Clickstreams Widget"
>abstract="Die **URLs und Clickstreams** bietet wichtige Leistungsindikatoren (Key Performance Indicators, KPIs), die detaillierte Informationen zu den URLs enthalten, auf die während eines Versands am häufigsten geklickt wurde."

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

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget &quot;Benutzeraktivitäten&quot;"
>abstract="Die **Benutzeraktivitäten** -Diagramm zeigt die Verteilung der Öffnungen und Klicks in Form eines Diagramms. Sie können den Zeitraum der Zielgruppendaten auswählen: letzter Tag, letzte Stunde oder letzte 30 Minuten."

* **[!UICONTROL Benutzeraktivitäten]**: Zeigt die Aufschlüsselung der Öffnungen und Klicks in Form eines Diagramms. Sie können den Zeitraum der Zielgruppendaten auswählen: letzter Tag, letzte Stunde oder letzte 30 Minuten.

  ![](assets/reporting_email_10.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

+++

## Tracking-Statistiken {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Trackingstatistiken-Widget"
>abstract="Die **Trackingstatistiken** -Diagramm bietet Statistiken zu Öffnungen und Klicks. Sie haben die Möglichkeit, den spezifischen Zeitrahmen für die Zielgruppendaten auszuwählen."

* **[!UICONTROL Tracking-Statistiken]**: Das Diagramm enthält Statistiken über Öffnungen und Klicks. Sie haben die Möglichkeit, den spezifischen Zeitrahmen für die Zielgruppendaten auszuwählen.

  ![](assets/reporting_email_11.png){align="center"}

  +++ Erfahren Sie mehr über die Metriken des E-Mail-Versandberichts.

   * **[!UICONTROL Klicks]**: Gesamtzahl der Klicks auf Links in Sendungen.

   * **[!UICONTROL Öffnungen]**: Anzahl der unterschiedlichen Zielgruppenempfängerinnen und -empfänger dieser Domain, die mindestens einmal eine Nachricht geöffnet haben.

+++

## Aufschlüsselung der Öffnungen {#breakdown-opens}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Aufschlüsselung nach Gerät"
>abstract="Die **Aufschlüsselung nach Gerät** zeigt die Verteilung der Öffnungen nach Gerätetyp für den betreffenden Zeitraum an. Das erste Diagramm zeigt Statistiken über Öffnungen auf einem Computer und Mobilgeräten. Das zweite stellt Statistiken dar, die sich nur auf Öffnungen auf Mobilgeräten beziehen."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Aufschlüsselung nach Betriebssystem"
>abstract="Die **Aufschlüsselung nach Betriebssystem** zeigt die Verteilung der Öffnungen nach Betriebssystem für den betreffenden Zeitraum an. Das erste Diagramm zeigt Statistiken über Öffnungen auf einem Computer und Mobilgeräten. Das zweite stellt Statistiken dar, die sich nur auf Öffnungen auf Mobilgeräten beziehen."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Aufschlüsselung nach Browser"
>abstract="Die **Aufschlüsselung nach Browser** zeigt die Verteilung der Öffnungen nach Browser für den betreffenden Zeitraum an. Das erste Diagramm zeigt Statistiken über Öffnungen auf einem Computer und Mobilgeräten. Das zweite stellt Statistiken dar, die sich nur auf Öffnungen auf Mobilgeräten beziehen."


Dieser Bericht zeigt die Öffnungsverteilung nach Betriebssystem, Geräteart und Browser für den ausgewählten Zeitraum. Für jede Kategorie stehen zwei Diagramme zur Verfügung. Das erste zeigt die Öffnungsstatistiken für Computer und Mobilgeräte an, das zweite nur für Mobilgeräte.

Sie haben die Möglichkeit, von **[!UICONTROL Desktop-Computer und Mobilgeräte]** auf ausschließlich **[!UICONTROL Nur Mobilgeräte]** umzuschalten, um die Genauigkeit der Zielgruppenbestimmung zu erhöhen.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Hotclicks-Bericht"
>abstract="Die **Hotclicks** zeigt den E-Mail-Inhalt (HTML und/oder Text) mit dem prozentualen Klickanteil für jeden Link. Gestaltungsbausteine, Abmelde-Links, Mirrorseiten-Links und Angebotslinks werden bei der Gesamtanzahl der Klicks berücksichtigt, jedoch nicht im Bericht angezeigt."

Dieser Bericht zeigt den Nachrichteninhalt (HTML und/oder Text) mit dem prozentualen Klickanteil für jeden Link. Gestaltungsbausteine, Abmelde-Links, Mirrorseiten-Links und Angebotslinks werden bei der Gesamtanzahl der Klicks berücksichtigt, jedoch nicht im Bericht angezeigt.

![](assets/reporting11.png)
