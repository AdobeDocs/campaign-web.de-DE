---
audience: end-user
title: Allgemeine Berichte für den Briefpost-Kanal
description: Weitere Informationen zu globalen Berichten für den Briefpost-Kanal
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 45%

---

# Allgemeine Berichte für den Briefpost-Kanal {#global-report-direct}

Die globalen Berichte bieten Benutzern einen umfassenden Überblick über Traffic- und Interaktionsmetriken auf Kanalebene.

Navigieren Sie zum **[!UICONTROL Berichte]** innerhalb des **[!UICONTROL Berichterstellung]** Abschnitt. Sie können Ihre Daten nach Berichtsdatum, -ordner oder -regeln filtern. [Weitere Informationen](global-reports.md)

## Versandzusammenfassung {#delivery-summary-direct}

### Versandübersicht {#delivery-overview-direct}

Die **[!UICONTROL Versandübersicht]** präsentiert wichtige Leistungsmetriken (KPIs) mit umfassenden Einblicken in die Interaktion Ihrer Besucher mit jedem E-Mail-Versand. Die Metriken sind unten dargestellt.

![](assets/global_report_email_delivery_overview.png){align="center"}

+++ Erfahren Sie mehr über Versandübersichtsmetriken.

* **[!UICONTROL Zu sendende Nachrichten]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten im Verhältnis zur Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Fehler]**: Summe der Fehler, die beim Versand und bei der automatischen Rücksendung kumuliert wurden, bezogen auf die Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Abmeldungen]**: Anzahl der Empfänger, die auf Abmeldungen geklickt haben.
+++

### Zielgruppe {#delivery-summary-direct-initial-target}

Tabelle und Diagramm für **[!UICONTROL Zielgruppe]** zeigt Daten zu Ihren Empfängern mit detaillierten Metriken an, die unten bereitgestellt werden.

![](assets/global_report_email_targeted_audience.png){align="center"}

+++ Erfahren Sie mehr über Zielgruppen-Metriken.

* **[!UICONTROL Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Ausschluss]**: Gesamtzahl der Adressen, die bei Anwendung der Regeln während der Analyse ignoriert wurden: fehlende Adresse, in Quarantäne, Blockierungsliste usw.

+++

### Versandstatistiken {#delivery-summary-direct-exec-stats}

Die **[!UICONTROL Versandstatistiken]** bietet eine Aufschlüsselung des Erfolgs jedes Briefpost-Versands mit detaillierten Metriken, die unten beschrieben werden.

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++ Erfahren Sie mehr über Versandstatistiken-Metriken.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler/Bounces]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

+++

### Ausschlussgründe {#causes-exclusion}

![](assets/global_report_email_exclusions.png){align="center"}

Das Diagramm und die Tabelle Ausschlüsse veranschaulichen die Gründe, aus denen verhindert wurde, dass aus den Zielgruppenprofilen ausgeschlossene Benutzerprofile die Nachricht empfangen.

## Versanddurchsatz {#delivery-throughput}

Dieser Bericht enthält umfassende Informationen zum Versanddurchsatz innerhalb eines bestimmten Zeitraums. Die Schlüsselmetrik, mit der die Geschwindigkeit des Nachrichtenversands gemessen wird, ist die Anzahl der pro Stunde gesendeten Nachrichten.

## Unzustellbare Nachrichten {#non-deliverables-direct}

### Aufschlüsselung der Fehler nach Typen {#delivery-summary-direct-breakdown-per-type}

Die **[!UICONTROL Verteilung der Fehler nach Typ]** -Tabelle und -diagramm enthält die Daten zu potenziellen Fehlern in verschiedenen Domänen, wobei spezifische Metriken unten bereitgestellt werden.

Die in diesem Bericht angezeigten Fehler lösen einen Quarantäneprozess aus. Weitere Informationen zur Quarantäneverwaltung finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=de){target="_blank"}.

+++ Erfahren Sie mehr über die Verteilung der Fehler nach Typmetriken.

* **[!UICONTROL Unbekannter Nutzer]**: Fehler, der beim Versand erzeugt wird, um anzugeben, dass die Adresse ungültig ist.

* **[!UICONTROL Ungültige Domain]**: Fehler, der beim Versand erzeugt wird, um anzugeben, dass die Domain der Adresse falsch ist oder nicht existiert.

* **[!UICONTROL Postfach voll]**: Fehlertyp, der nach fünf fehlgeschlagenen Versandversuchen erzeugt wird, wenn das Empfängerpostfach zu viele Nachrichten enthält.

* **[!UICONTROL Account deaktiviert]**: Fehlertyp, der beim Senden eines Versands erzeugt wird, um anzuzeigen, dass die Adresse nicht mehr existiert.

* **[!UICONTROL Verweigert]**: Fehlertyp, der erzeugt wird, wenn eine Adresse vom IAP (Internet Access Provider) abgelehnt wird, z. B. nach Anwendung einer Sicherheitsregel (Anti-Spam-Software).

* **[!UICONTROL Unerreichbar]**: Fehlertyp, der in der Verteilungskette der Nachricht auftritt: Vorfall im SMTP-Relais, Domain vorübergehend unerreichbar, usw.

* **[!UICONTROL Nicht angemeldet]**: Fehlertyp, wenn das Mobiltelefon der Empfängerin bzw. des Empfängers zum Zeitpunkt des Versands ausgeschaltet war oder über keinen Netzempfang verfügte.

+++

### Aufschlüsselung der Fehler nach Domain {#delivery-summary-email-breakdown-per-domain}

Die **[!UICONTROL Verteilung der Fehler nach Domain]** -Tabelle und -Diagramm zeigen die Daten zu potenziellen Fehlern in den einzelnen Domänen. Die Metriken sind dieselben wie die der Tabelle und des Graphen **[!UICONTROL Aufschlüsselung der Fehler nach Typen]** weiter oben.
