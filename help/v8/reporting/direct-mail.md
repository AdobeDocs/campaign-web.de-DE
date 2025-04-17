---
audience: end-user
title: Briefpost-Berichte
description: Erfahren Sie, wie Sie auf Briefpost-Berichte zugreifen und diese verwenden können.
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 35%

---

# Briefpost-Versandbericht {#direct-mail-report}

Der **Briefpost-Versandbericht** bietet umfassende Einblicke und Daten, die speziell für Ihren Briefpost-Versand gelten. Sie enthält detaillierte Informationen über Leistung, Effektivität und Ergebnisse einzelner Sendungen und bietet einen vollständigen Überblick.

## Versandzusammenfassung {#delivery-summary-direct-mail}

### Versandübersicht {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Versandübersicht"
>abstract="Die **Versandübersicht** präsentiert wichtige Leistungsmetriken (KPI) mit umfassenden Erkenntnissen zur Interaktion Ihrer Besucherinnen und Besucher mit jedem Briefpostversand. Die Metriken sind unten dargestellt."

Die **[!UICONTROL Versandübersicht]** bietet detaillierte Einblicke in die Besucherinteraktionen mit jedem Briefpost-Versand und zeigt wesentliche Schlüsselleistungsmetriken (KPIs). Die Metriken sind unten dargestellt.

![Diagramm mit Metriken zur Versandübersicht mit wichtigen Leistungsindikatoren für den Briefpost-Versand.](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++ Erfahren Sie mehr über Metriken zur Versandübersicht.

* **[!UICONTROL Zu versendende Nachrichten]**: Gesamtzahl der bei der Versandvorbereitung verarbeiteten Nachrichten.
* **[!UICONTROL Ausgewählt]**: Anzahl der Benutzerprofile, die sich als Zielgruppenprofile für Briefpostnachrichten eignen.
* **[!UICONTROL Auszuschließen]**: Anzahl der Benutzerprofile, die aus den Zielgruppenprofilen ausgeschlossen sind und keine Briefpostnachrichten erhalten.
+++

### Anfängliche Zielgruppenpopulation {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Anfängliche Zielgruppenpopulation"
>abstract="Der Graph **Anfängliche Zielgruppenpopulation** zeigt Daten zu Ihren Empfängerinnen und Empfängern sowie Nachrichten basierend auf den Ergebnissen der Versandvorbereitung an."

Das **[!UICONTROL Zielpopulation]** Diagramm zeigt Daten zu Empfängern an. Metriken werden während der Versandvorbereitung berechnet und umfassen die anfängliche Audience, die Anzahl der zu sendenden Nachrichten und die Anzahl der ausgeschlossenen Empfänger.

![Diagramm der anfänglichen Zielgruppenpopulation mit Zielgruppengröße, zu sendenden Nachrichten und Ausschlüssen.](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Bewegen Sie den Mauszeiger über einen Teil des Diagramms, um die genaue Zahl anzuzeigen.

![Detailansicht des Diagramms der ursprünglichen Zielpopulation mit Hover-Funktion.](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++ Erfahren Sie mehr über die Metriken des Briefpost-Versandberichts.

* **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger.
* **[!UICONTROL Zu versenden]**: Gesamtzahl der nach erfolgter Versandanalyse zu versendenden Nachrichten.
* **[!UICONTROL Ausschluss]**: Gesamtzahl der vom Versand an die Zielgruppe ausgeschlossenen Nachrichten.
+++

### Versandstatistiken {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Versandstatistiken"
>abstract="Der Graph **Versandstatistiken** zeigt den Erfolg Ihres Briefpostversands und die aufgetretenen Fehler an."

Das Diagramm **[!UICONTROL Versandstatistiken]** bietet einen Überblick über die Versandleistung und bietet detaillierte Metriken zur Messung von Erfolg und Effektivität.

![Diagramm mit Versandstatistiken, das Erfolgsraten, Fehler und Quarantänen anzeigt.](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++ Erfahren Sie mehr über die Metriken des Briefpost-Kampagnenberichts.

* **[!UICONTROL Gesendete Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.
* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Vergleich zur Anzahl der zu versendenden Nachrichten.
* **[!UICONTROL Fehler]**: Gesamtzahl der bei Sendungen und automatischer Bounce-Verarbeitung kumulierten Fehler im Vergleich zur Anzahl der zu versendenden Nachrichten.
* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (z. B. unbekannter Nutzer, ungültige Domain), im Vergleich zur Anzahl der zu versendenden Nachrichten.
+++

### Ausschlussgründe {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Versand – Ausschlussgründe"
>abstract="Der Graph **Ausschlussgründe** zeigt die Verteilung der zurückgewiesenen Nachrichten während der Versandvorbereitung, kategorisiert nach den jeweiligen Regeln."

Das Diagramm **[!UICONTROL Ausschlussgründe]** enthält eine Aufschlüsselung der Gründe für die Zurückweisung von Nachrichten während der Versandvorbereitung. Diese Aufschlüsselung ist nach verschiedenen Regeln gegliedert und bietet eine detaillierte Ansicht der Faktoren, die zum Nachrichtenausschluss beitragen. Ausschlussregeln werden in der Dokumentation zu [ v8 (Konsole) ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#email-error-types){_blank}.

![Diagramm „Ausschlussgründe“, das die Verteilung der zurückgewiesenen Nachrichten nach Regel anzeigt.](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++ Erfahren Sie mehr über die Ursachen von Ausschlussmetriken.

* **[!UICONTROL Adresse in Quarantäne]**: Fehlertyp, der erzeugt wird, wenn eine Adresse in Quarantäne gestellt wird.
* **[!UICONTROL Adresse nicht angegeben]**: Fehlertyp, der erzeugt wird, wenn eine Adresse nicht existiert.
* **[!UICONTROL Adresse schlechter Qualität]**: Fehlertyp, der erzeugt wird, wenn der Qualitätsindex der Postanschrift zu niedrig ist.
* **[!UICONTROL Auf die Blockierungsliste gesetzt Adresse]**: Fehlertyp, der erzeugt wurde, als der Empfänger während des Versands auf die Blockierungsliste gesetzt wurde.
* **[!UICONTROL Double]**: Fehlertyp, der erzeugt wurde, als der Empfänger aufgrund nicht eindeutiger Schlüsselwerte ausgeschlossen wurde.
* **[!UICONTROL Kontrollgruppenadresse]**: Die Adresse der Empfängerin oder des Empfängers ist Teil der Kontrollgruppe.
* **[!UICONTROL Größe der Zielgruppe begrenzt]**: Die maximale Versandgröße wurde für die Empfängerin oder den Empfänger erreicht.
+++

### Ausschlüsse {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Ausschlüsse"
>abstract="Die Tabelle **[!UICONTROL Ausschlüsse]** zeigt eine detaillierte Aufschlüsselung der während der Versandvorbereitung zurückgewiesenen Nachrichten nach Regeln an."

Die **[!UICONTROL Ausschlüsse]**-Tabelle enthält eine detaillierte Aufschlüsselung der bei der Versandvorbereitung abgelehnten Nachrichten, die nach bestimmten Regeln kategorisiert ist. Diese Aufschlüsselung bietet ein klares Verständnis der Gründe für Nachrichtenausschlüsse.

![Tabelle „Ausschlüsse“ mit detaillierter Aufschlüsselung der abgelehnten Nachrichten nach Regel.](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

Die verfügbaren Metriken sind die gleichen wie die für die weiter oben beschriebenen [Ausschlussgründe](#direct-mail-delivery-exclusions).