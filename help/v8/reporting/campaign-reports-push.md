---
audience: end-user
title: Kampagnenberichte für den Push-Kanal
description: Kampagnenberichte für den Push-Kanal verstehen
badge: label="Beta"
source-git-commit: 72a7cb2577512b9b3dbf239ca664aa8410918ba2
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 42%

---


# Kampagnenberichte für den Push-Kanal {#campaign-reports-push-channel}

Jeder Kampagnenbericht ist in verschiedene Widgets unterteilt, die den Erfolg und die Fehler Ihrer Kampagne detailliert beschreiben. Für den Push-Kanal werden die Berichte und Metriken unten beschrieben. Erfahren Sie, wie Sie auf Ihre Kampagnenberichte zugreifen können in [diese Seite](campaign-reports.md).

## Versandzusammenfassung {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Versandübersicht"
>abstract="Die **Versandübersicht** liefert wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucher mit Ihrem Push-Benachrichtigungsversand interagieren."

Die **[!UICONTROL Versandübersicht]** liefert wichtige Leistungsindikatoren (KPIs), die detaillierte Informationen darüber enthalten, wie Ihre Besucher mit Ihrem Push-Benachrichtigungsversand interagieren. Die Metriken werden nachfolgend beschrieben.

![](assets/campaign-reporting-push-summary.png)


+++Erfahren Sie mehr über die Metriken des Push-Kampagnenberichts.

* **[!UICONTROL Insgesamt gesendet]**: Gesamtzahl der während der Versandvorbereitung verarbeiteten Nachrichten.

* **[!UICONTROL Zugestellt]**: Anzahl der erfolgreich gesendeten Nachrichten im Verhältnis zur Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Fehler]**: Summe der Fehler, die beim Versand und bei der automatischen Rücksendung kumuliert wurden, bezogen auf die Gesamtzahl der gesendeten Nachrichten.

* **[!UICONTROL Klicks insgesamt]**: Gesamtzahl der unterschiedlichen Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

+++

### Statistiken der ursprünglichen Zielgruppe {#delivery-summary-push-initial-target}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Statistiken der ursprünglichen Zielgruppe"
>abstract="Die **Ursprüngliche Zielgruppenstatistiken** zeigt Daten zu Ihren Empfängern an"

Die **[!UICONTROL Ursprüngliche Zielgruppenstatistiken]** zeigt Daten zu Ihren Empfängern an. Die Metriken werden nachfolgend beschrieben.

![](assets/campaign-reporting-push-target.png)


+++Erfahren Sie mehr über die Metriken des Push-Kampagnenberichts.

* **[!UICONTROL Ursprüngliche Zielgruppe]**: Gesamtzahl der Zielgruppenempfängerinnen und -empfänger.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Aufgrund von Regeln abgelehnt]**: Gesamtzahl der Adressen, die während der Analyse beim Anwenden von Regeln ignoriert wurden: fehlende Adresse, in Quarantäne, auf Blockierungsliste usw.

+++

### Ausführungsstatistiken {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Ausführungsstatistiken"
>abstract="Die **Ausführungsstatistiken** -Tabelle zeigt den Erfolg Ihres Versands: Zu sendende Nachrichten, Erfolg, Fehler und neue Quarantänen."

Die **[!UICONTROL Ausführungsstatistiken]** -Tabelle zeigt den Erfolg Ihres Versands. Die Metriken werden nachfolgend beschrieben.

![](assets/campaign-reporting-push-exec.png)


+++Erfahren Sie mehr über die Metriken des Push-Kampagnenberichts.

* **[!UICONTROL Zu versendende Nachricht]**: Gesamtzahl der nach erfolgter Versandvorbereitung zu versendenden Nachrichten.

* **[!UICONTROL Erfolg]**: Anzahl der erfolgreich verarbeiteten Nachrichten im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Fehler]**: Gesamtzahl der über alle Sendungen hinweg kumulierten Fehler und der automatischen Bounce-Verarbeitungen im Verhältnis zur Anzahl der zu versendenden Nachrichten.

* **[!UICONTROL Neue Quarantänen]**: Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (ungültige Registrierung, Zurückweisung von Nachrichten, Payload-Fehler z. B.) in Bezug auf die Anzahl zu sendender Nachrichten.

  Die Fehlertypen von Push-Benachrichtigungen werden im Abschnitt [Dokumentation zu Adobe Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Erzeugte Clickstreams {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Erzeugte Clickstreams"
>abstract="Die **Erzeugte Clickstreams** zeigt die verfügbaren Daten in Bezug auf die Interaktion der Empfänger mit Ihrem Versand an."

Die **[!UICONTROL Erzeugte Clickstreams]** zeigt Daten dazu an, wie Ihre Empfänger mit Ihrem Versand interagiert haben. Die Metriken werden nachfolgend beschrieben.

![](assets/campaign-reporting-push-clicks.png)

+++Erfahren Sie mehr über die Metriken des Push-Kampagnenberichts.

* **[!UICONTROL Einzelklicks]**: Gesamtzahl der unterschiedlichen Empfänger, die mindestens einmal im betreffenden Versand geklickt haben.

* **[!UICONTROL Klicks insgesamt]**: Gesamtzahl der Klicks auf Links in Sendungen.

* **[!UICONTROL Reaktionsrate]**: Verhältnis der Anzahl an Zielgruppenempfängerinnen und -empfängern, die auf einen Versand geklickt haben, in Bezug zur geschätzten Anzahl der Zielgruppenempfängerinnen und -empfänger, die einen Versand geöffnet haben.

+++
