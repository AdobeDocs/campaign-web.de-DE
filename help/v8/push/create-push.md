---
audience: end-user
title: Erstellen eines Push-Benachrichtigungs-Versands
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Versand für eine Push-Benachrichtigung erstellen
badge: label="Beta"
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 4ea25f0877fd3f0ab02f3023f041bd040e0530a3
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 38%

---

# Erstellen eines Push-Benachrichtigungs-Versands {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Vorlage für Push-Benachrichtigungen"
>abstract="Wählen Sie eine Vorlage für Push-Benachrichtigungen aus, um Ihren Push-Versand zu starten. Versandvorlagen ermöglichen die einfache Wiederverwendung benutzerdefinierter Inhalte und Einstellungen in allen Kampagnen und Sendungen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Verwenden von Versandvorlagen"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Eigenschaften des Push-Versands"
>abstract="Definieren Sie die Eigenschaften des Push-Versands. Geben Sie den Titel der Push-Benachrichtigung ein und verwenden Sie die **Zusätzliche Optionen** um den internen Namen, den Versandordner und den Code zu konfigurieren. Sie können auch eine benutzerdefinierte Beschreibung eingeben."

Sie können einen eigenständigen Push-Benachrichtigungsversand erstellen oder eine Push-Benachrichtigung im Kontext eines Kampagnen-Workflows erstellen. Die folgenden Schritte beschreiben die Vorgehensweise für einen eigenständigen (einmaligen) Push-Versand. Wenn Sie im Kontext eines Kampagnen-Workflows arbeiten, finden Sie in [diesem Abschnitt](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow) detaillierte Schritte, um einen solchen Versand zu erstellen.

## Push-Versand erstellen {#create-push-delivery}

Gehen Sie wie folgt vor, um einen eigenständigen Push-Versand zu erstellen:

1. Gehen Sie zum Menü **[!UICONTROL Sendungen]** in der linken Leiste, und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

1. Unter dem **[!UICONTROL Kanal]** auswählen **Push-Benachrichtigung** als Kanal verwenden und je nach gewähltem Gerätebetriebssystem eine Vorlage auswählen: Android oder iOS. [Weitere Informationen zu Vorlagen](../msg/delivery-template.md)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![](assets/push_create_1.png)

## Versandeinstellungen konfigurieren {#configure-push-settings}

Konfigurieren Sie Ihre Versandeinstellungen wie unten beschrieben:

1. Geben Sie einen **[!UICONTROL Titel]** für den Versand. Standardmäßig wird der Titel mit dem Titel der ausgewählten Vorlage festgelegt. Sie sollte aktualisiert werden.

1. Durchsuchen Sie die **[!UICONTROL Zusätzliche Optionen]** -Dropdown, um bei Bedarf die Optionen anzupassen. Wenn Ihr Versand auf einem erweiterten Schema basiert, muss **Benutzerdefinierte Optionen** verfügbar sind.

   +++Konfigurieren Sie die folgenden Einstellungen entsprechend Ihren Anforderungen.
   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu.
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner.
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an.
   * **[!UICONTROL Art]**: Geben Sie die Art der E-Mail zu Klassifizierungszwecken an.
+++


## Push-Versand-Audience auswählen {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Push-Benachrichtigungs-Audience definieren"
>abstract="Um die Audience Ihrer Nachricht zu definieren, müssen Sie zunächst die mit dem Push-Versand verknüpfte App auswählen. Standardmäßig wird Ihre Push-Benachrichtigung an alle Abonnenten der Anwendung gesendet. Sie können eine bestimmte Zielgruppe einschränken, indem Sie auf **Zielgruppe auswählen** Schaltfläche. Fügen Sie bei Bedarf eine Kontrollgruppe hinzu, um die Wirkung Ihres Versands zu messen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=de" text="Festlegen einer Kontrollgruppe"


Sie müssen zuerst die App auswählen und dann die Audience für Push-Benachrichtigungen wie unten beschrieben verfeinern:

1. Aus dem **[!UICONTROL Zielgruppe]** wählen Sie die Anwendung aus, die Sie für diesen Versand verwenden möchten. Standardmäßig wird Ihre Push-Benachrichtigung an alle Abonnenten der Anwendung gesendet. Sie können eine bestimmte Zielgruppe einschränken, indem Sie auf **[!UICONTROL Zielgruppe auswählen]** Schaltfläche.

   ![](assets/push_create_2.png)

1. Wählen Sie eine existierende Zielgruppe aus oder erstellen Sie eine eigene Zielgruppe, um die Zielpopulation für Ihren Push-Versand zu verfeinern. Bei Push-Benachrichtigungen ist die Standardeinstellung [Zieldimension](../audience/about-recipients.md#targeting-dimensions) is **Abonnentenanwendung** (nms:appSubscriptionRcp), der mit der Empfängertabelle verknüpft ist.

   Erfahren Sie, wie Sie eine vorhandene Zielgruppe in [diese Seite](../audience/add-audience.md)

   Erfahren Sie, wie Sie eine neue Zielgruppe in erstellen [diese Seite](../audience/one-time-audience.md)

1. Schalten Sie die **[!UICONTROL Kontrollgruppe aktivieren]** -Option, um eine Kontrollgruppe zur Messung der Wirkung Ihres Versands einzurichten. Nachrichten werden nicht an diese Kontrollgruppe gesendet, sodass Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen können, die die Nachricht erhalten haben. [Weitere Informationen](../audience/control-group.md)

## Inhalt der Push-Benachrichtigung definieren {#create-content-push}

Um den Inhalt Ihrer Benachrichtigung zu definieren, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](content-push.md)

![](assets/push_create_5.png)

Auf diesem Bildschirm können Sie auch [Inhalte simulieren](../preview-test/preview-test.md) und [Angebote einrichten](../content/offers.md).

## Versandzeitpunkt planen {#schedule-push}

Um den Versand für ein bestimmtes Datum und eine bestimmte Uhrzeit zu planen, aktivieren Sie die Option **[!UICONTROL Zeitplan aktivieren]**. Nachdem der Versand initiiert wurde, wird die Nachricht automatisch an dem Datum und zu der Uhrzeit gesendet, die Sie für die Empfängerin bzw. den Empfänger festgelegt haben. Weitere Informationen zur Versandplanung finden Sie in [diesem Abschnitt](../msg/gs-messages.md#gs-schedule)

![](assets/push_create_3.png)


## Erweiterte Versandeinstellungen {#adv-push}

Klicken Sie auf **[!UICONTROL Versandeinstellungen konfigurieren]**, um auf erweiterte Optionen in Bezug auf Ihre Versandvorlage zuzugreifen. [Weitere Informationen](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png)
