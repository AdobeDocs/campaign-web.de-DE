---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 32%

---

# Versandwarnungskriterien {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard für Versandwarnungskriterien"
>abstract="Die Campaign Web-Benutzeroberfläche bietet vordefinierte Kriterien für Warnhinweise (Sendungen mit geringem Durchsatz, Sendungen, deren Vorbereitung fehlgeschlagen ist usw.), die Sie Ihrem Dashboard hinzufügen können. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen."

Die Campaign-Webbenutzeroberfläche bietet vordefinierte Warnungsbedingungen (Sendungen mit geringem Durchsatz, Sendungen, deren Vorbereitung fehlgeschlagen ist usw.), die Sie Ihrem Dashboard hinzufügen können. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen.

Auf Warnungsbedingungen kann über das Menü **Versandwarnung** im linken Navigationsbereich unter dem **Kriterien** Registerkarte.

![](assets/alerting-criteria-list.png)

## Vordefinierte Warnungsbedingungen {#ootb-criteria}

Vordefinierte Warnungsbedingungen sind in der Campaign-Webbenutzeroberfläche verfügbar. Diese Kriterien decken eine Reihe von Szenarien ab, die unten aufgeführt sind:

* **Versandfehler**: Alle in einem bestimmten Zeitraum geplanten Sendungen mit einem Fehler als Status.
* **Sendungen mit fehlgeschlagener Vorbereitung**: Alle in einem bestimmten Zeitraum geänderten Sendungen, deren Vorbereitung (Zielgruppenberechnung und Inhaltserstellung) fehlgeschlagen ist.
* **Versand mit zu hoher Softbounce-Fehlerrate**: Alle in einem bestimmten Zeitraum geplanten Sendungen, deren Status mindestens Gestartet lautet und deren Softbounce-Fehlerrate über dem definierten Prozentsatz liegt.
* **Versand mit zu hoher Hardbounce-Fehlerrate**: Alle in einem bestimmten Zeitraum geplanten Sendungen, deren Status mindestens Gestartet lautet und deren Hardbounce-Fehlerrate über dem definierten Prozentsatz liegt.
* **Sendungen mit lange ausstehendem Start**: Alle in einem bestimmten Zeitraum geplanten Sendungen, deren Status Start ausstehend die definierte Dauer überschreitet, Status Start ausstehend bedeutet, dass die Nachrichten vom System noch nicht berücksichtigt wurden.
* **Sendungen mit geringem Durchsatz**: Alle Sendungen, deren Start länger als die definierte Dauer zurückliegt, die einen niedrigeren als den definierten Prozentsatz an verarbeiteten Nachrichten aufweisen und deren Durchsatz unter einem definierten Wert liegt.
* **Gestartete Sendungen**: Alle in einem bestimmten Zeitraum geplanten Sendungen mit dem Status Gestartet .

>[!NOTE]
>
>Standardwerte werden auf alle Parameter für die oben genannten Kriterien angewendet. Diese Werte können im Abschnitt **Bedingungsparameter** des Versandwarnungs-Dashboards, in dem sie verwendet werden. [Erfahren Sie, wie Sie mit Dashboards arbeiten.](../msg/delivery-alerting-dashboards.md)

## Erstellen eines Kriteriums für einen Warnhinweis {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Versandwarnungskriterien erstellen"
>abstract="Zusätzlich zu den von Adobe Campaign bereitgestellten vordefinierten Kriterien für einen Warnhinweis können Sie auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indikatoren, die in Warnungen hinzugefügt werden sollen"
>abstract="Wählen Sie die Indikatoren aus, die im Abschnitt „Details“ der E-Mail-Warnhinweise als Spalten angezeigt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Warnungstyp"
>abstract="Geben Sie den **Warnhinweistyp** für das Kriterium an, d. h. das Label und die Farbe, die neben der Versandbedingung im Abschnitt „Zusammenfassung“ der Warnhinweise angezeigt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frequenz des Kriteriums"
>abstract="Sie können die Häufigkeit der Warnhinweise pro Tag für jeden Versand steuern, der das Kriterium erfüllt."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Erstellen eines Kriteriums für einen Warnhinweis"
>abstract="Um eigene Versandfilter zu erstellen, erstellen Sie einen neuen vordefinierten Filter in der Campaign v8-Konsole aus dem Knoten unter **Administration** > **Konfiguration** > **Vordefinierte Filter**."

Gehen Sie wie folgt vor, um ein neues Kriterium zu erstellen:

1. Navigieren Sie zum **Delivery Triglering** im linken Navigationsbereich und wählen Sie die **Kriterien** Registerkarte.
1. Klicken Sie auf **Versandwarnungsbedingungen erstellen** Schaltfläche.
1. Geben Sie eine Bezeichnung für das Kriterium an. Der interne Name wird automatisch ausgefüllt und schreibgeschützt.
1. Die **Von diesen Kriterien angewendeter Versandfilter** ermöglicht es Ihnen, den Umfang der Bedingung durch Anwendung eines vordefinierten Filters zu verfeinern.

   Im folgenden Beispiel wird die Variable **Gestartete Sendungen (critInProgressDeliveries)** ausgewählt wurde, d. h., die Bedingung berücksichtigt nur Sendungen mit dem Status &quot;Gestartet&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Wenn keiner der vordefinierten Filter Ihren Anforderungen entspricht, können Sie sich an Ihren Administrator wenden, um einen eigenen Filter zu erstellen.  Detaillierte Informationen zum Erstellen vordefinierter Filter in der Campaign-Konsole finden Sie im Abschnitt [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Dieser Vorgang darf nur von fortgeschrittenen Benutzern durchgeführt werden.

1. Im **In Warnhinweisen hinzuzufügende Indikatoren** die Indikatoren auswählen, die im Bereich &quot;Details&quot;der E-Mail-Warnungen als Spalten angezeigt werden sollen.

1. Geben Sie den **Warnhinweistyp** für das Kriterium an, d. h. das Label und die Farbe, die neben der Versandbedingung im Abschnitt „Zusammenfassung“ der Warnhinweise angezeigt werden sollen.

1. Die **Bedingungsfrequenz** können Sie die Häufigkeit von Warnungen pro Tag für jeden Versand steuern, der die Bedingung erfüllt:

   * **Dieses Versandkriterium wird in jeder Benachrichtigung wiederholt**: Zeigt einen Versand an, der die Bedingung erfüllt, in jeder E-Mail-Warnung des Tages.
   * **Dieses Versandkriterium wird nur am ersten Vorkommen des Tages gesendet**: Zeigt einen Versand, der die Bedingung erfüllt, nur im ersten Bericht des Tages an, nicht wiederholt in nachfolgenden E-Mail-Warnungen.
