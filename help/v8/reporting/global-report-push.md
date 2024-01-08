---
audience: end-user
title: Globale Berichte für den Push-Kanal
description: Allgemeine Berichte für den Push-Kanal
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 34%

---

# Globale Berichte für den Push-Kanal {#campaign-reports-push}

Die globalen Berichte bieten Benutzern einen umfassenden Überblick über Traffic- und Interaktionsmetriken auf Kanalebene.

Navigieren Sie zum **[!UICONTROL Berichte]** innerhalb des **[!UICONTROL Berichterstellung]** Abschnitt. Sie können Ihre Daten nach Berichtsdatum, -ordner oder -regeln filtern. [Weitere Informationen](global-reports.md)

## Versandzusammenfassung {#delivery-summary-push}

### Versandübersicht {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Push-Versand – Übersicht"
>abstract="Die Push-Benachrichtigung **Versandübersicht** KPIs bieten eine gründliche Untersuchung Ihrer Push-Sendungen und liefern detaillierte Einblicke sowie spezifische Daten. Es bietet umfassende Details zu Leistung, Effektivität und Ergebnissen der Sendungen."

Die **[!UICONTROL Versandübersicht]** liefert wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucher mit jedem Push-Benachrichtigungsversand interagieren. Metriken werden nachfolgend beschrieben.

![](assets/global_report_push_delivery_overview.png)

+++ Erfahren Sie mehr über Versandübersichtsmetriken.

* **[!UICONTROL Zu sendende Nachrichten]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten im Verhältnis zur Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Klicks gesamt]**: Gesamtzahl der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

* **[!UICONTROL Fehler]**: Summe der Fehler, die beim Versand und bei der automatischen Rücksendung kumuliert wurden, bezogen auf die Gesamtzahl der gesendeten Nachrichten.

+++

### Zielgruppe {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Push-Zielpopulation"
>abstract="Die **Zielgruppe** Diagramm und Tabelle zeigen Daten zu Ihrer Push-Nachrichten-Audience, einschließlich Informationen zu den zu versendenden Nachrichten und Ausschlüssen."

Die **[!UICONTROL Zielgruppe]** -Tabelle und -diagramm enthält Daten zu Ihren Empfängern für jeden gesendeten Push-Benachrichtigungsversand. Metriken werden nachfolgend beschrieben.

![](assets/global_report_push_targeted_audience.png)

+++ Erfahren Sie mehr über Zielgruppen-Metriken.

* **[!UICONTROL Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Ausschluss]**: Gesamtzahl der Adressen, die bei Anwendung der Regeln während der Analyse ignoriert wurden: fehlende Adresse, in Quarantäne, Blockierungsliste usw.

+++

### Versandstatistiken {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Push-Versandstatistiken"
>abstract="Die **Gesamtstatistik** liefert Informationen zu gesendeten Push-Benachrichtigungen, einschließlich Erfolgsraten, Fehlern und Quarantänen."

Die **[!UICONTROL Versandstatistiken]** in der Tabelle wird der Erfolg jedes Push-Benachrichtigungsversands beschrieben. Metriken werden nachfolgend beschrieben.

![](assets/global_report_push_delivery_statistics.png)

+++ Erfahren Sie mehr über Versandstatistiken-Metriken.

* **[!UICONTROL Nachrichten insgesamt]**: Gesamtzahl der nach der Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler/Bounces]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

* **[!UICONTROL Neu in Quarantäne]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (ungültige Registrierung, Zurückweisung von Nachrichten, Payload-Fehler usw.), in Bezug auf die Anzahl der zu sendenden Nachrichten.

  Die Fehlertypen von Push-Benachrichtigungen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#push-error-types){target="_blank"} aufgelistet.

+++

### Ausschlussgründe {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Push-Ausschlussgründe"
>abstract="Die **Ausschlussgründe** Diagramm und Tabelle veranschaulichen die verschiedenen Gründe, aus denen Benutzerprofile keine Push-Benachrichtigungen erhalten konnten."

Die **[!UICONTROL Ausschlussgründe]** Diagramm und Tabelle zeigen die Gründe an, aus denen verhindert wurde, dass aus den Zielgruppenprofilen ausgeschlossene Benutzerprofile die Nachricht empfangen.

Die Fehlertypen von Push-Benachrichtigungen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#push-error-types){target="_blank"} aufgelistet.

## Versanddurchsatz {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Bericht &quot;Versanddurchsatz&quot;"
>abstract="Die **Versanddurchsatz** Der Bericht enthält detaillierte Informationen zum Durchsatz der Push-Benachrichtigung bei der Bereitstellung der gesamten Plattform innerhalb eines bestimmten Zeitraums."

![](assets/global_report_push_delivery_throughput.png)

Die **[!UICONTROL Versanddurchsatz]** Dieser Bericht bietet umfassende Einblicke in die Effektivität des Push-Benachrichtigungs-Versandsystems und bietet eine detaillierte Zusammenfassung der Erfolgs- und Fehlerquoten über einen bestimmten Zeitraum hinweg.

