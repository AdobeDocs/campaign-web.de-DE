---
audience: end-user
title: Globale Berichte für den SMS-Kanal
description: Grundlegendes zu globalen Berichten für den SMS-Kanal
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 97%

---

# Globale Berichte für den SMS-Kanal {#campaign-reports-sms}

Die globalen Berichte bieten einen umfassenden Überblick über Traffic- und Interaktionsmetriken auf Kanalebene.

Navigieren Sie zum Menü **[!UICONTROL Berichte]** im Abschnitt **[!UICONTROL Reporting]**. Sie können Ihre Daten nach Berichtsdatum, -ordner oder -regeln filtern. [Weitere Informationen](global-reports.md)

## Versandzusammenfassung {#delivery-summary-sms}

### Versandübersicht {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="SMS-Versand – Überblick"
>abstract="Die KPIs zur **SMS-Versandübersicht** bieten einen guten Überblick über Ihren SMS-Versand und detaillierte Informationen zu bestimmten Daten. Sie bieten umfassende Informationen über Leistung, Effektivität und Ergebnisse Ihres Versands."

Der Bericht **[!UICONTROL Versandübersicht]** bietet anhand umfassender KPIs (Key Performance Indicators) detaillierte Erkenntnisse zu den Interaktionsmustern Ihrer Besucherinnen und Besucher bei jedem SMS-Versand. Folgende Metriken sind nachfolgend beschrieben.

![Screenshot des Berichts „Versandübersicht“ mit KPIs für den SMS-Versand](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++Weitere Informationen zu Metriken der Versandübersicht.

* **[!UICONTROL Zu sendende Nachrichten]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Anteil der erfolgreich gesendeten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Clickthrough-Rate]**: Anteil der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

* **[!UICONTROL Fehler]**: Anteil der beim Versand und der automatischen Rücksendung kumulierten Fehler, bezogen auf die Gesamtzahl der gesendeten Nachrichten.

+++

### Zielgruppe {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="SMS-Zielpopulation"
>abstract="Das Diagramm und die Tabelle **Zielpopulation** enthalten Daten zu Ihrer SMS-Zielgruppe, einschließlich Informationen zu den zu sendenden Nachrichten und Ausschlüssen."

Die Tabelle und der Graph **[!UICONTROL Zielgruppe]** enthalten Daten zu den Empfängerinnen und Empfängern jedes gesendeten SMS-Versands. Metriken werden nachfolgend beschrieben.

![Screenshot des Berichts „Zielgruppe“ mit Daten zu Empfängerinnen und Empfängern und Ausschlüssen für SMS-Sendungen](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++Weitere Informationen zu Metriken für Zielgruppen.

* **[!UICONTROL Zielgruppe]**: Gesamtzahl der angesprochenen Empfängerinnen und Empfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Ausschluss]**: Gesamtzahl der Adressen, die während der Analyse beim Anwenden von Regeln ignoriert wurden, z. B. fehlende Adressen, Adressen in Quarantäne, Adressen auf einer Blockierungsliste usw.

+++

### Versandstatistiken {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="SMS-Versandstatistiken"
>abstract="Der Bericht zu **Versandstatistiken** bietet umfassende Einblicke in die gesendete SMS und eine Aufschlüsselung verschiedener Metriken wie Erfolgsraten, Fehlerereignisse und in Quarantäne gestellte Zielgruppen. Diese detaillierte Darstellung ermöglicht eine gründliche Untersuchung der Gesamtleistung und der Ergebnisse des SMS-Versandprozesses."

Die Tabelle **[!UICONTROL Versandstatistiken]** gibt Auskunft über den Erfolg jedes SMS-Versands. Metriken werden nachfolgend beschrieben.

![Screenshot des Berichts „Versandstatistiken“ mit Erfolgsraten, Fehlern und Quarantänen für SMS-Sendungen](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++Weitere Informationen zu Metriken der Versandstatistik.

* **[!UICONTROL Nachrichten gesamt]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten, bezogen auf die Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler/Bounces]**: Gesamtzahl der über alle Sendungen und der automatischen Bounce-Verarbeitungen hinweg kumulierten Fehler im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Neu in Quarantäne]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (z. B. „Unbekannte Nutzerin bzw. unbekannter Nutzer“, „Ungültige Domain“), bezogen auf die Anzahl der zu versendenden Nachrichten.

  Die SMS-Fehlertypen sind in der [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#sms-quarantines){target="_blank"} aufgelistet.

+++

### Ausschlussgründe {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="SMS-Ausschlussgründe"
>abstract="Der Graph und die Tabelle **Ausschlussgründe** veranschaulichen die unterschiedlichen Gründe, aus denen Benutzerprofile keine SMS-Nachrichten erhalten haben."

Der Graph und die Tabelle **[!UICONTROL Ausschlussgründe]** veranschaulichen die Gründe, aus denen Benutzerprofile, die von den Zielprofilen ausgeschlossen wurden, Ihre SMS-Sendungen nicht erhalten haben.

Die E-Mail-Fehlertypen sind in der [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#email-error-types){target="_blank"} aufgelistet.

![Screenshot des Berichts „Ausschlussgründe“ mit Gründen für SMS-Versandausschlüsse](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Versanddurchsatz {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="SMS-Versanddurchsatz"
>abstract="Der Bericht zum **Versanddurchsatz** bietet umfassende Einblicke in die Effizienz des Versandsystems für SMS-Nachrichten und einen detaillierten Überblick über Erfolgs- und Fehlerquoten innerhalb eines bestimmten Zeitraums."

![Screenshot des Berichts „Versanddurchsatz“ mit Erfolgs- und Fehlerraten für SMS-Sendungen im Zeitverlauf](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

Der Bericht **[!UICONTROL Versanddurchsatz]** bietet umfassende Erkenntnisse zur Effektivität des SMS-Versandsystems und eine detaillierte Zusammenfassung der Erfolgs- und Fehlerraten über einen bestimmten Zeitraum.