---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten können.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: 7b78b6d710fa88be1be60f514b2fe8219bd04d75
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 50%

---

# Versandwarnungskriterien {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard für Versandwarnungskriterien"
>abstract="Die Campaign Web-Benutzeroberfläche bietet vordefinierte Warnungskriterien (Sendungen mit geringem Durchsatz oder Sendungen, deren Vorbereitung fehlgeschlagen ist), die Sie Ihrem Dashboard hinzufügen können. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen."

Die Web-Benutzeroberfläche von Campaign bietet vordefinierte Warnkriterien, die Sie Ihrem Dashboard hinzufügen können, z. B. Sendungen mit geringem Durchsatz oder Sendungen, bei denen die Vorbereitung fehlgeschlagen ist. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen.

Sie können über das Menü **Versandwarnung** im linken Navigationsbereich auf der Registerkarte **Kriterien** auf die Warnungskriterien zugreifen.

![Liste der Warnungskriterien, die im Menü Versandwarnung angezeigt werden](assets/alerting-criteria-list.png)

## Vordefinierte Warnungskriterien {#ootb-criteria}

Vordefinierte Warnungskriterien sind in der Campaign Web-Benutzeroberfläche verfügbar. Diese Kriterien decken eine Reihe von Szenarien ab, die unten aufgeführt sind:

* **Versandfehler**: Alle in einem bestimmten Zeitraum geplanten Sendungen mit einem Fehler als Status.
* **Sendungen mit fehlgeschlagener Vorbereitung**: Alle in einem bestimmten Zeitraum geänderten Sendungen, deren Vorbereitung (Zielgruppenberechnung und Inhaltserstellung) fehlgeschlagen ist.
* **Versand mit der Fehlerquote für Softbounces**: Jeder Versand, der innerhalb eines definierten Bereichs geplant wurde und einen Status von mindestens „In Bearbeitung“ aufweist sowie eine Fehlerquote für Softbounces, die größer als ein definierter Prozentsatz ist.
* **Versand mit der Fehlerquote für Hardbounces**: Jeder Versand, der innerhalb eines definierten Bereichs geplant ist und einen Status von mindestens „In Bearbeitung“ aufweist sowie eine Fehlerquote für Hardbounces, die größer als ein definierter Prozentsatz ist.
* **Sendungen mit langem ausstehendem Start**: Jeder innerhalb eines definierten Bereichs geplante Versand mit dem Status „Start ausstehend“, der länger als eine definierte Dauer ist. Der Status „Start ausstehend“ bedeutet, dass die Nachrichten vom System noch nicht berücksichtigt wurden.
* **Sendungen mit niedrigem Durchsatz**: Jeder Versand, der länger als eine definierte Dauer gestartet wurde, weniger als einen definierten Prozentsatz verarbeiteter Nachrichten und einen Durchsatz hat, der kleiner als einen definierten Wert ist.
* **Sendungen in Bearbeitung**: Jeder innerhalb eines definierten Bereichs geplante Versand mit dem Status „In Bearbeitung“.

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
>abstract="Indikatoren auswählen, die als Spalten im Abschnitt „Details“ der E-Mail-Warnhinweise angezeigt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Warnungstyp"
>abstract="Geben Sie für **Kriterium den** Warnhinweistyp“ an, d. h. den Titel und die Farbe, die neben dem Versandkriterium im Abschnitt „Zusammenfassung“ der Warnhinweise angezeigt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frequenz des Kriteriums"
>abstract="Steuern Sie die Häufigkeit der Warnungen pro Tag für jeden Versand, der das Kriterium erfüllt."

Gehen Sie wie folgt vor, um ein neues Kriterium zu erstellen:

1. Navigieren Sie zum Menü **Versandwarnung** im linken Navigationsbereich und wählen Sie die Registerkarte **Kriterien** aus.
1. Klicken Sie auf die Schaltfläche **Versandwarnungskriterien erstellen**.
1. Geben Sie einen Titel für das Kriterium an. Der interne Name wird automatisch ausgefüllt und schreibgeschützt.
1. Verwenden Sie den **von diesem Kriterium angewendeten Versandfilter** um den Umfang des Kriteriums durch Anwendung eines vordefinierten Filters zu verfeinern.

   Im unten abgebildeten Beispiel wurde der Filter **Versand gestartet (critInProgressDeliveries)** ausgewählt, d. h., das Kriterium berücksichtigt nur Sendungen mit dem Status „Gestartet“.

   ![Beispiel für Warnungskriterieneigenschaften mit ausgewähltem Filter](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Wenn keiner der vordefinierten Filter Ihren Anforderungen entspricht, können Sie eigene Filter im Menü **Kundenverwaltung** > **Vordefinierte Filter** erstellen. [Weitere Informationen](../get-started/predefined-filters.md)
   >
   >Dieser Vorgang sollte nur von erfahrenen Benutzenden durchgeführt werden.

1. Wählen Sie im Abschnitt **Indikatoren, die in Warnungen hinzugefügt werden sollen** die Indikatoren aus, die im Bereich „Details“ der E-Mail-Warnungen als Spalten angezeigt werden sollen.

1. Geben Sie den **Warnungstyp** für das Kriterium ein, d. h. den Titel und die Farbe, die neben dem Versandkriterium im Abschnitt „Zusammenfassung“ der Warnungen angezeigt werden sollen.

1. Verwenden Sie den **Kriterienfrequenz**, um die Häufigkeit der Warnhinweise pro Tag für jeden Versand zu steuern, der dieses Kriterium erfüllt:

   * **Dieses Versandkriterium wird in jeder Benachrichtigung wiederholt**: Zeigt einen Versand, der das Kriterium erfüllt, in jeder E-Mail-Warnung des Tages an.
   * **Dieses Versandkriterium wird nur beim ersten Auftreten des Tages gesendet**: Zeigt einen Versand an, der das Kriterium nur im ersten Bericht des Tages erfüllt, ohne ihn in nachfolgenden E-Mail-Warnhinweisen zu wiederholen.