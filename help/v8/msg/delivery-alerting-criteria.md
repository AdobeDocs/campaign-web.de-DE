---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten können.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 100%

---

# Versandwarnungskriterien {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard für Versandwarnungskriterien"
>abstract="Die Campaign Web-Benutzeroberfläche bietet vordefinierte Warnungskriterien (Sendungen mit geringem Durchsatz oder Sendungen, deren Vorbereitung fehlgeschlagen ist), die Sie Ihrem Dashboard hinzufügen können. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen."

Die Campaign Web-Benutzeroberfläche bietet vordefinierte Warnungskriterien (Sendungen mit geringem Durchsatz oder Sendungen, deren Vorbereitung fehlgeschlagen ist), die Sie Ihrem Dashboard hinzufügen können. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen.

Sie können über das Menü **Versandwarnung** im linken Navigationsbereich auf der Registerkarte **Kriterien** auf die Warnungskriterien zugreifen.

![](assets/alerting-criteria-list.png)

## Vordefinierte Warnungskriterien {#ootb-criteria}

Vordefinierte Warnungskriterien sind in der Campaign Web-Benutzeroberfläche verfügbar. Diese Kriterien decken eine Reihe von Szenarien ab, die unten aufgeführt sind:

* **Versandfehler**: Alle in einem bestimmten Zeitraum geplanten Sendungen mit einem Fehler als Status.
* **Sendungen mit fehlgeschlagener Vorbereitung**: Alle in einem bestimmten Zeitraum geänderten Sendungen, deren Vorbereitung (Zielgruppenberechnung und Inhaltserstellung) fehlgeschlagen ist.
* **Versand mit zu hoher Softbounce-Fehlerrate**: Alle in einem bestimmten Zeitraum geplanten Sendungen, deren Status zumindest „Gestartet“ lautet und deren Softbounce-Fehlerrate über dem festgelegten Prozentsatz liegt.
* **Versand mit zu hoher Hardbounce-Fehlerrate**: Alle in einem bestimmten Zeitraum geplanten Sendungen, deren Status zumindest „Gestartet“ lautet und deren Hardbounce-Fehlerrate über dem festgelegten Prozentsatz liegt.
* **Sendungen mit lange ausstehendem Start**: Alle in einem bestimmten Zeitraum geplanten Sendungen, die sich länger als die definierte Dauer im Status „Start ausstehend“ befinden. „Start ausstehend“ bedeutet, dass die Nachrichten vom System noch nicht berücksichtigt wurden.
* **Sendungen mit geringem Durchsatz**: Alle Sendungen, deren Start länger als die definierte Dauer zurückliegt, die einen niedrigeren als den definierten Prozentsatz an verarbeiteten Nachrichten aufweisen oder deren Durchsatz unter einem definierten Wert liegt.
* **Gestartete Sendungen**: Alle in einem bestimmten Zeitraum geplanten Sendungen, deren Status „Gestartet“ lautet.

>[!NOTE]
>
>Für die oben genannten Kriterien werden auf alle Parameter Standardwerte angewendet. Diese Werte können im Abschnitt **Kriterienparameter** des Versandwarnungs-Dashboards, in dem sie verwendet werden, angepasst werden. [Erfahren Sie, wie Sie mit Dashboards arbeiten.](../msg/delivery-alerting-dashboards.md)

## Erstellen eines Warnungskriteriums {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Erstellen eines Versandwarnungskriteriums"
>abstract="Neben den von Adobe Campaign bereitgestellten vordefinierten Warnungskriterien können Sie auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indikatoren, die in Warnungen hinzugefügt werden sollen"
>abstract="Wählen Sie die Indikatoren aus, die im Bereich „Details“ der E-Mail-Warnungen als Spalten angezeigt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Warnungstyp"
>abstract="Geben Sie den **Warnungstyp** für das Kriterium ein, d. h. den Titel und die Farbe, die neben dem Versandkriterium im Abschnitt „Zusammenfassung“ der Warnungen angezeigt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frequenz des Kriteriums"
>abstract="Steuern Sie die Häufigkeit der Warnungen pro Tag für jeden Versand, der das Kriterium erfüllt."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Erstellen eines Warnungskriteriums"
>abstract="Um eigene Versandfilter zu erstellen, erstellen Sie einen neuen vordefinierten Filter in der Campaign v8-Konsole aus dem Knoten unter **Administration** > **Konfiguration** > **Vordefinierte Filter**."

Gehen Sie wie folgt vor, um ein neues Kriterium zu erstellen:

1. Navigieren Sie im linken Navigationsbereich zum Menü **Versandwarnung** und wählen Sie die Registerkarte **Kriterien** aus.
1. Klicken Sie auf die Schaltfläche **Versandwarnungskriterien erstellen**.
1. Geben Sie einen Titel für das Kriterium an. Der interne Name wird automatisch ausgefüllt und schreibgeschützt.
1. Der **von diesen Kriterien angewendete Versandfilter** ermöglicht es Ihnen, den Umfang des Kriteriums durch Anwendung eines vordefinierten Filters zu verfeinern.

   Im unten abgebildeten Beispiel wurde der Filter **Versand gestartet (critInProgressDeliveries)** ausgewählt, d. h., das Kriterium berücksichtigt nur Sendungen mit dem Status „Gestartet“.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Wenn keiner der vordefinierten Filter Ihren Anforderungen entspricht, können Sie sich an Ihre Admins wenden, um einen eigenen Filter zu erstellen.   Detaillierte Informationen zum Erstellen vordefinierter Filter in der Campaign-Konsole finden Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Dieser Vorgang sollte nur von erfahrenen Benutzenden durchgeführt werden.

1. Wählen Sie im Abschnitt **Indikatoren, die in Warnungen hinzugefügt werden sollen** die Indikatoren aus, die im Bereich „Details“ der E-Mail-Warnungen als Spalten angezeigt werden sollen.

1. Geben Sie den **Warnungstyp** für das Kriterium ein, d. h. den Titel und die Farbe, die neben dem Versandkriterium im Abschnitt „Zusammenfassung“ der Warnungen angezeigt werden sollen.

1. Im Abschnitt **Frequenz des Kriteriums** können Sie die Häufigkeit von Warnungen pro Tag für jeden Versand steuern, der das Kriterium erfüllt:

   * **Dieses Versandkriterium wird in jeder Benachrichtigung wiederholt**: Zeigt einen Versand, der das Kriterium erfüllt, in jeder E-Mail-Warnung des Tages an.
   * **Dieses Versandkriterium wird nur beim ersten Auftreten des Tages gesendet**: Zeigt einen Versand, der das Kriterium erfüllt, nur im ersten Bericht des Tages an, aber wiederholt dies nicht in nachfolgenden E-Mail-Warnungen.
