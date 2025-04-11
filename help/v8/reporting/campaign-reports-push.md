---
audience: end-user
title: Kampagnenberichte für den Push-Kanal
description: Grundlegendes zu Kampagnenberichten für den Push-Kanal
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 64%

---

# Kampagnenberichte für den Push-Kanal {#campaign-reports-push-channel}

Jeder Kampagnenbericht ist in verschiedene Widgets unterteilt, die den Erfolg und die Fehler Ihrer Kampagne detailliert beschreiben. Im Folgenden werden die Berichte und Metriken für den Push-Kanal beschrieben. Auf [ Seite erfahren Sie, wie Sie auf Ihre Kampagnenberichte ](campaign-reports.md).

## Versandzusammenfassung {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Versandübersicht"
>abstract="Der Bericht **Versandübersicht** bietet wichtige Performance-Indikatoren (KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucherinnen und Besucher mit dem Versand Ihrer Push-Benachrichtigungen interagieren."

Der Bericht **[!UICONTROL Versandübersicht]** bietet wichtige Performance-Indikatoren (KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucherinnen und Besucher mit dem Versand Ihrer Push-Benachrichtigungen interagieren. Metriken werden nachfolgend beschrieben.

![Versandzusammenfassungsmetriken, die im Bericht Versandübersicht angezeigt werden](assets/campaign-reporting-push-summary.png){zoomable="yes"}

+++Erfahren Sie mehr über die Metriken für Push-Kampagnenberichte.

* **[!UICONTROL Zu sendende Nachrichten]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten im Verhältnis zur Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Fehler]**: Gesamtzahl der Fehler, die beim Versand und bei der automatischen Rücksendung kumuliert wurden, bezogen auf die Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Klicks gesamt]**: Gesamtzahl der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

+++

### Statistiken der ursprünglichen Zielgruppe {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Statistiken der ursprünglichen Zielgruppe"
>abstract="Die **Ursprüngliche Zielgruppenstatistiken** zeigt Daten zu Ihren Empfängerinnen und Empfängern an."

Die Tabelle **[!UICONTROL Statistiken der anfänglichen Zielgruppe]** zeigt Daten zu Ihren Empfängerinnen und Empfängern an. Metriken werden nachfolgend beschrieben.

![Im Bericht werden Statistiken zur ursprünglichen Zielgruppe angezeigt](assets/campaign-reporting-push-target.png){zoomable="yes"}

+++Erfahren Sie mehr über die Metriken für Push-Kampagnenberichte.

* **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Aufgrund von Regeln abgelehnt]**: Gesamtzahl der Adressen, die während der Analyse beim Anwenden von Regeln ignoriert wurden, z. B. fehlende Adresse, in Quarantäne oder auf Blockierungsliste.

+++

### Ausführungsstatistiken {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Ausführungsstatistiken"
>abstract="Die Tabelle **Ausführungsstatistiken** zeigt den Erfolg Ihres Versands: Zu sendende Nachrichten, Erfolg, Fehler und Neu in Quarantäne."

Die Tabelle **[!UICONTROL Ausführungsstatistiken]** zeigt den Erfolg Ihres Versands im Detail. Metriken werden nachfolgend beschrieben.

![Im Bericht angezeigte Ausführungsstatistiken](assets/campaign-reporting-push-exec.png){zoomable="yes"}

+++Erfahren Sie mehr über die Metriken für Push-Kampagnenberichte.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler]**: Gesamtzahl der bei Sendungen und automatischer Bounce-Verarbeitung akkumulierten Fehler im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (z. B. ungültige Registrierung, Nachrichtenablehnung oder Payload-Fehler), im Verhältnis zur Anzahl der zu versendenden Nachrichten.

  Die Fehlertypen von Push-Benachrichtigungen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=de#push-error-types){target="_blank"} aufgelistet.

+++

### Generierte Clickstreams {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Generierte Clickstreams"
>abstract="Die Tabelle **Generierte Clickstreams** zeigt Daten dazu an, wie Ihre Empfängerinnen und Empfänger mit Ihrem Versand interagiert haben."

Die Tabelle **[!UICONTROL Generierte Clickstreams]** zeigt Daten dazu an, wie Ihre Empfängerinnen und Empfänger mit Ihrem Versand interagiert haben. Metriken werden nachfolgend beschrieben.

![Generierte Clickstreams werden im Bericht angezeigt](assets/campaign-reporting-push-clicks.png){zoomable="yes"}

+++Erfahren Sie mehr über die Metriken für Push-Kampagnenberichte.

* **[!UICONTROL Einzelklicks]**: Gesamtzahl der unterschiedlichen Empfängerinnen und Empfänger, die einen Versand mindestens einmal angeklickt haben.

* **[!UICONTROL Klicks gesamt]**: Gesamtzahl der Klicks auf Links in Sendungen.

* **[!UICONTROL Reaktionsrate]**: Verhältnis der Anzahl an Zielgruppenempfängerinnen und -empfängern, die auf einen Versand geklickt haben, in Bezug zur geschätzten Anzahl der Zielgruppenempfängerinnen und -empfänger, die einen Versand geöffnet haben.

+++