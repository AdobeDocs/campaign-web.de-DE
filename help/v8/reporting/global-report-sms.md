---
audience: end-user
title: Allgemeine Berichte für den SMS-Kanal
description: Allgemeine Berichte für den SMS-Kanal
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 19%

---

# Allgemeine Berichte für den SMS-Kanal {#campaign-reports-sms}

Die globalen Berichte bieten Benutzern einen umfassenden Überblick über Traffic- und Interaktionsmetriken auf Kanalebene.

Navigieren Sie zum **[!UICONTROL Berichte]** innerhalb des **[!UICONTROL Berichterstellung]** Abschnitt. Sie können Ihre Daten nach Berichtsdatum, -ordner oder -regeln filtern. [Weitere Informationen](global-reports.md)

## Versandzusammenfassung {#delivery-summary-sms}

### Versandübersicht {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="SMS-Versand – Überblick"
>abstract="Die **Übersicht über den SMS-Versand** KPIs bieten eine gründliche Zusammenfassung Ihres SMS-Versands mit detaillierten Einblicken und spezifischen Daten. Es liefert umfassende Informationen über Leistung, Effektivität und Ergebnisse Ihrer Sendungen."

Die **[!UICONTROL Versandübersicht]** bietet umfassende KPIs (Key Performance Indicators), die einen umfassenden Einblick in die Interaktionsmuster Ihrer Besucher bei jedem SMS-Versand bieten. Die folgenden Metriken sind unten beschrieben.

![](assets/global_report_sms_delivery_overview.png)

+++ Erfahren Sie mehr über Versandübersichtsmetriken.

* **[!UICONTROL Zu sendende Nachrichten]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Prozentsatz der erfolgreich gesendeten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten

* **[!UICONTROL Clickthrough-Rate]**: Prozentsatz der unterschiedlichen Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

* **[!UICONTROL Fehler]**: Prozentsatz der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Gesamtzahl der gesendeten Nachrichten.

+++

### Zielgruppe {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="SMS-Zielpopulation"
>abstract="Das Diagramm und die Tabelle für **Zielgruppenbestimmung** Daten bezüglich Ihrer SMS-Audience präsentieren, einschließlich Informationen zu den zu sendenden Nachrichten und Ausschlüssen."

Die **[!UICONTROL Zielgruppe]** -Tabelle und -diagramm enthält Daten zu Ihren Empfängern für jeden gesendeten SMS-Versand. Metriken werden nachfolgend beschrieben.

![](assets/global_report_sms_targeted_audience.png)

+++ Erfahren Sie mehr über Zielgruppen-Metriken.

* **[!UICONTROL Zielgruppe]**: Gesamtzahl der Zielgruppenempfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Ausschluss]**: Gesamtzahl der Adressen, die bei Anwendung der Regeln während der Analyse ignoriert wurden: fehlende Adresse, in Quarantäne, Blockierungsliste usw.

+++

### Versandstatistiken {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="SMS-Versandstatistiken"
>abstract="Die **Versandstatistiken** bietet umfassende Einblicke in die gesendete SMS und eine Aufschlüsselung verschiedener Metriken wie Erfolgsraten, Fehlerereignisse und in Quarantäne gestellte Zielgruppen. Diese detaillierte Darstellung ermöglicht eine gründliche Untersuchung der Gesamtleistung und der Ergebnisse des SMS-Versandprozesses."

Die **[!UICONTROL Versandstatistiken]** in der Tabelle wird der Erfolg jedes SMS-Versands beschrieben. Metriken werden nachfolgend beschrieben.

![](assets/global_report_sms_delivery_statistics.png)

+++ Erfahren Sie mehr über Versandstatistiken-Metriken.

* **[!UICONTROL Nachrichten insgesamt]**: Gesamtzahl der nach der Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler/Bounces]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitung in Bezug auf die Zahl der zu sendenden Nachrichten.

* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannter Nutzer, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

  Die SMS-Fehlertypen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#sms-quarantines){target="_blank"} aufgelistet.

+++

### Ausschlussgründe {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="SMS-Ausschlussgründe"
>abstract="Die **Ausschlussgründe** Diagramm und Tabelle veranschaulichen die unterschiedlichen Ursachen, aus denen Benutzerprofile keine SMS-Nachrichten erhalten konnten."

Die **[!UICONTROL Ausschlussgründe]** Diagramm und Tabelle zeigen die Gründe an, aus denen verhindert wurde, dass aus den Zielgruppenprofilen ausgeschlossene Benutzerprofile Ihre SMS-Sendungen erhalten.

Die Fehlertypen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Versanddurchsatz {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="SMS-Versanddurchsatz"
>abstract="Die **Versanddurchsatz** bietet umfassende Einblicke in die Effizienz des SMS-Versandsystems und bietet einen detaillierten Überblick über Erfolg und Fehlerrate innerhalb eines bestimmten Zeitraums."

![](assets/global_report_sms_delivery_throughput.png)

Die **[!UICONTROL Versanddurchsatz]** bietet umfassende Einblicke in die Effektivität des SMS-Versandsystems und bietet eine detaillierte Zusammenfassung der Erfolgs- und Fehlerquoten über einen bestimmten Zeitraum.
