---
audience: end-user
title: Globale Berichte für den SMS-Kanal
description: Grundlegendes zu globalen Berichten für den SMS-Kanal
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 54%

---

# Globale Berichte für den SMS-Kanal {#campaign-reports-sms}

Die globalen Berichte bieten den Benutzenden einen umfassenden Überblick über Traffic- und Interaktionsmetriken auf Kanalebene.

Navigieren Sie zum Menü **[!UICONTROL Berichte]** im Abschnitt **[!UICONTROL Berichterstellung]**. Sie können Ihre Daten nach Berichtsdatum, Ordner oder Regeln filtern. [Weitere Informationen](global-reports.md)

## Versandzusammenfassung {#delivery-summary-sms}

### Versandübersicht {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="SMS-Versand – Überblick"
>abstract="Die KPIs zur **SMS-Versandübersicht** bieten einen guten Überblick über Ihren SMS-Versand und detaillierte Informationen zu bestimmten Daten. Sie bieten umfassende Informationen über Leistung, Effektivität und Ergebnisse Ihres Versands."

Der **[!UICONTROL Versandübersicht]** bietet umfassende KPIs (Key Performance Indicators), die detaillierte Einblicke in die Interaktionsmuster Ihrer Besuchenden bei jedem SMS-Versand bieten. Folgende Metriken sind nachfolgend beschrieben.

![Screenshot des Berichts mit der Versandübersicht, der die wichtigsten Leistungsindikatoren für den SMS-Versand zeigt.](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++Erfahren Sie mehr über Versandübersichtsmetriken.

* **[!UICONTROL Zu sendende Nachrichten]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Anteil der erfolgreich gesendeten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Clickthrough-Rate]**: Anteil der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

* **[!UICONTROL Fehler]**: Prozentsatz der Fehler, die beim Versand und bei der automatischen Rücksendung kumuliert wurden, bezogen auf die Gesamtzahl der gesendeten Nachrichten.

+++

### Zielgruppe {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="SMS-Zielpopulation"
>abstract="Das Diagramm und die Tabelle für die **Zielgruppenpopulation** enthalten Daten, die sich auf Ihre SMS-Zielgruppe beziehen, einschließlich Informationen zu zu versendenden Nachrichten und Ausschlüssen."

Die Tabelle und der Graph **[!UICONTROL Zielgruppe]** enthalten Daten zu den Empfängerinnen und Empfängern jedes gesendeten SMS-Versands. Metriken werden nachfolgend beschrieben.

![Screenshot des Berichts Zielgruppe mit Daten zu Empfängern und Ausschlüssen für SMS-Sendungen.](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++Erfahren Sie mehr über Zielgruppen-Metriken.

* **[!UICONTROL Zielgruppe]**: Gesamtzahl der angesprochenen Empfängerinnen und Empfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Ausschluss]**: Gesamtzahl der Adressen, die während der Analyse beim Anwenden von Regeln ignoriert wurden, z. B. fehlende Adresse, in Quarantäne oder auf einer Blockierungsliste.

+++

### Versandstatistiken {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="SMS-Versandstatistiken"
>abstract="Der Bericht zu **Versandstatistiken** bietet umfassende Einblicke in die gesendete SMS und eine Aufschlüsselung verschiedener Metriken wie Erfolgsraten, Fehlerereignisse und in Quarantäne gestellte Zielgruppen. Diese detaillierte Darstellung ermöglicht eine gründliche Untersuchung der Gesamtleistung und der Ergebnisse des SMS-Versandprozesses."

Die **[!UICONTROL Versandstatistiken]** gibt Auskunft über den Erfolg jedes SMS-Versands. Metriken werden nachfolgend beschrieben.

![Screenshot des Berichts Versandstatistiken mit Erfolgsraten, Fehlern und Quarantänen für SMS-Sendungen.](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++Erfahren Sie mehr über Versandstatistik-Metriken.

* **[!UICONTROL Nachrichten gesamt]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler/Bounces]**: Gesamtzahl der bei Sendungen und automatischer Bounce-Verarbeitung akkumulierten Fehler im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (z. B. unbekannter Nutzer, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

  Die SMS-Fehlertypen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#sms-quarantines){target="_blank"} aufgelistet.

+++

### Ausschlussgründe {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="SMS-Ausschlussgründe"
>abstract="Der Graph und die Tabelle **Ausschlussgründe** veranschaulichen die unterschiedlichen Gründe, aus denen Benutzerprofile keine SMS-Nachrichten erhalten haben."

Der Graph und die Tabelle **[!UICONTROL Ausschlussgründe]** veranschaulichen die Gründe, aus denen Benutzerprofile, die von den Zielprofilen ausgeschlossen wurden, Ihre SMS-Sendungen nicht erhalten haben.

Die E-Mail-Fehlertypen werden in der [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#email-error-types){target="_blank"} aufgelistet.

![Screenshot des Berichts „Ausschlussgründe“ mit Gründen für SMS-Versandausschlüsse.](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Versanddurchsatz {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="SMS-Versanddurchsatz"
>abstract="Der Bericht zum **Versanddurchsatz** bietet umfassende Einblicke in die Effizienz des Versandsystems für SMS-Nachrichten und einen detaillierten Überblick über Erfolgs- und Fehlerquoten innerhalb eines bestimmten Zeitraums."

![Screenshot des Berichts zum Versanddurchsatz, der die Erfolgs- und Fehlerquoten der SMS-Sendungen im Zeitverlauf zeigt.](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

Der **[!UICONTROL Versanddurchsatz]** bietet umfassende Einblicke in die Effektivität des SMS-Nachrichtenversand-Systems und bietet eine detaillierte Zusammenfassung der Erfolgs- und Fehlerquoten über einen bestimmten Zeitraum.