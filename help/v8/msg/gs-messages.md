---
audience: end-user
title: Erste Schritte mit Nachrichten und Sendungen in Campaign v8 Web
description: Erfahren Sie, wie Sie Campaign Web verwenden, um mit Sendungen zu arbeiten und Nachrichten zu senden
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 35%

---

# Erste Schritte mit Nachrichten{#gs-messages}


Mit Adobe Campaign können Sie kanalübergreifende Kampagnen wie E-Mails, SMS und Push-Benachrichtigungen versenden und deren Effektivität mithilfe diverser Berichte messen. Diese Nachrichten werden mittels Sendungen entworfen und gesendet und können für jeden Empfänger personalisiert werden. Diese Sendungen können einzeln oder im Rahmen einer Marketingkampagne durchgeführt werden.

Adobe Campaign v8 enthält die folgenden Versandkanäle:

* **E-Mail-Kanal**: Ein E-Mail-Versand richtet personalisierte elektronische Nachrichten an eine zuvor bestimmte Zielpopulation. Erfahren Sie, wie Sie eine E-Mail erstellen und senden in [diese Seite](../email/create-email.md).

* **SMS-Kanal**: Sendungen über Mobile-Kanäle ermöglichen den Versand personalisierter SMS an die Zielpopulation.  Erfahren Sie, wie Sie SMS erstellen und senden in [diese Seite](../sms/create-sms.md).

* **Mobile-App-Kanal**: Mit Mobile-App-Sendungen können Sie Benachrichtigungen an iOS- und Android-Systeme senden.  Erfahren Sie, wie Sie Push-Benachrichtigungen erstellen und senden in [diese Seite](../push/gs-push.md).

## Erstellen eines Versands {#create-delivery}

Sie können eigenständige Sendungen über die **[!UICONTROL Sendungen]** im linken Menü oder im Kontext einer Marketingkampagne über die Schaltfläche **[!UICONTROL Kampagnen]** Menü links.

>[!BEGINTABS]

>[!TAB Erstellen eines eigenständigen Versands]

Gehen Sie wie folgt vor, um einen eigenständigen Versand zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Sendungen]** im linken Navigationsmenü und klicken Sie auf das **[!UICONTROL Versand erstellen]** Schaltfläche.

   ![](assets/create-a-delivery.png)

1. Wählen Sie einen Kanal für den Versand aus. Weitere Informationen zu Versandkanälen und zum Definieren von Versandinhalten finden Sie in den folgenden Abschnitten:

   * [E-Mail-Kanal](../email/create-email.md)
   * [Push-Benachrichtigungskanal](../push/gs-push.md)
   * [SMS-Kanal](../sms/create-sms.md)

1. Definieren Sie die Versand-Audience für die Hauptzielgruppe und die Kontrollgruppe. Weitere Informationen zu Zielgruppen finden Sie in [diesem Abschnitt](../audience/about-audiences.md).
1. Definieren des Nachrichteninhalts.
1. (Optional) Definieren Sie den Zeitplan für den Versand. Wenn kein Zeitplan definiert ist, werden Nachrichten sofort nach dem Klicken auf die **[!UICONTROL Senden]** Schaltfläche.
1. Klicken Sie auf  **[!UICONTROL Überprüfen und Senden]** -Schaltfläche, um Ihre Einstellungen zu überprüfen.
1. Verwenden Sie die  **[!UICONTROL Inhalt simulieren]** zum Testen Ihres Versands und der Personalisierungseinstellungen. Weitere Informationen zur Nachrichtensimulation finden Sie unter [diesem Abschnitt](../preview-test/preview-test.md).
1. Klicken Sie auf  **[!UICONTROL Vorbereiten]** -Schaltfläche, um die Zielpopulation zu berechnen und die Nachrichten zu erzeugen. Der Vorbereitungsschritt kann einige Minuten dauern. Nach Abschluss der Vorbereitung sind die Nachrichten versandbereit. Im Falle eines Fehlers können Sie die **Protokolle** um Warnhinweise und Warnhinweise zu überprüfen.
1. Überprüfen Sie die Ergebnisse und klicken Sie auf die  **[!UICONTROL Senden]** Schaltfläche zum Starten des Nachrichtenversands.
1. Sobald Nachrichten gesendet wurden, navigieren Sie zum **Berichte** -Abschnitt, um auf Schlüsselmetriken zuzugreifen. Weitere Informationen zu Versandberichten finden Sie in [diesem Abschnitt](../reporting/delivery-reports.md).

>[!TAB Versand in einer Kampagne erstellen]

Gehen Sie wie folgt vor, um einen Versand in einer Kampagne zu erstellen:

1. Erstellen Sie eine Kampagne oder öffnen Sie eine bestehende Kampagne. Weitere Informationen [Marketing-Kampagnen](../campaigns/gs-campaigns.md).
1. Erstellen Sie einen Workflow oder öffnen Sie einen vorhandenen Workflow.
1. Hinzufügen und Konfigurieren eines **[!UICONTROL Audience erstellen]** und klicken Sie auf die `+`Schaltfläche.

   ![](assets/add-delivery-in-wf.png)

   Die **[!UICONTROL Audience erstellen]** -Aktivität wird im Abschnitt [diesem Abschnitt](../workflows/activities/build-audience.md).

1. Wählen Sie eine Versandaktivität aus: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push-Benachrichtigung (Android)]** oder **[!UICONTROL Push-Benachrichtigung (iOS)]**. Erfahren Sie mehr über die Versandkanalaktivitäten in einem Workflow und wie Sie in diesem Versandinhalte definieren [Abschnitt](../workflows/activities/about-activities.md#channel).
1. Starten Sie den Workflow und überprüfen Sie die Protokolle.

Sie können Sendungen auch in einer Kampagne hinzufügen, ohne einen Workflow zu erstellen. Navigieren Sie dazu zum **[!UICONTROL Sendungen]** auf der Registerkarte Ihrer Kampagne klicken und auf die **[!UICONTROL Versand erstellen]** Schaltfläche.

![](assets/new-campaign-delivery.png)

Konfigurationsschritte ähneln den Schritten für eigenständige Sendungen.

Weiterführende Informationen zur Konfiguration einer Kampagne und zur Verwaltung von Sendungen einer Kampagne finden Sie im Abschnitt [diesem Abschnitt](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Hinzufügen von Personalisierung{#personalization}

Nachrichten, die von Adobe Campaign versendet werden, können auf verschiedene Weise personalisiert werden. [Weitere Informationen zu Personalisierungsfunktionen](../personalization/personalize.md).

Verwenden Sie Campaign, um dynamische Inhalte zu erstellen und personalisierte Nachrichten zu versenden. Personalisierungsfunktionen können kombiniert werden, um Ihre Nachrichten zu verbessern und ein individuelles Benutzererlebnis zu schaffen.

Sie können den Nachrichteninhalt wie folgt personalisieren:

* Einfügen von dynamischen **Personalisierungsfeldern**

   Personalisierungsfelder werden für die oberste Ebene der Nachrichtenpersonalisierung verwendet. Sie können jedes in der Datenbank verfügbare Feld aus dem Personalisierungseditor auswählen. Für einen Versand können Sie jedes Feld auswählen, das sich auf die Empfängerin oder den Empfänger, die Nachricht oder den Versand bezieht. Diese Personalisierungsattribute können in die Betreffzeile oder in den Text Ihrer Nachrichten eingefügt werden. [Weitere Informationen](../personalization/personalize.md)

* Einfügen von vordefinierten **Inhaltsbausteinen**

   Campaign verfügt über eine Reihe von Gestaltungsbausteinen, die ein bestimmtes Rendering ermöglichen, das Sie in Ihre Sendungen einfügen können. Sie können zum Beispiel ein Logo, eine Grußbotschaft oder einen Link zur Mirror-Seite der Nachricht hinzufügen. Inhaltsbausteine sind über einen eigenen Eintrag im Personalisierungseditor verfügbar. [Weitere Informationen](../personalization/personalize.md#ootb-content-blocks)

* Erstellen **bedingter Inhalte**

   Konfigurieren Sie bedingte Inhalte, um beispielsweise eine dynamische Personalisierung basierend auf dem Empfängerprofil hinzuzufügen. Textblöcke und/oder Bilder werden eingefügt, wenn eine bestimmte Bedingung erfüllt ist. [Weitere Informationen](../personalization/conditions.md)

* Hinzufügen **personalisierte Angebote**

   Fügen Sie je nach Empfänger-Standort, aktuellem Wetter oder letzter Bestellung personalisierte Angebote in Ihren Nachrichteninhalt ein.


## Sendungen in der Vorschau ansehen und testen

Nachdem der Nachrichteninhalt definiert wurde, können Sie eine Vorschau davon anzeigen, um das Rendering Ihrer Nachrichten zu steuern, und die Personalisierungseinstellungen mit Testprofilen überprüfen. [Weitere Informationen](../preview-test/preview-test.md)


## Versand- und Trackinglogs{#gs-tracking-logs}

Die Überwachung Ihrer Sendungen nach deren Versand ist ein wichtiger Schritt, um sicherzustellen, dass Ihre Marketing-Kampagnen effizient sind und Ihre Kunden erreichen. Sie können nach dem Versand überwachen sowie nachvollziehen, wie Zustellungsfehler und Quarantänen gehandhabt werden.

## Versand duplizieren{#delivery-duplicate}

Sie können eine Kopie eines bestehenden Versands entweder in der Versandliste oder im Versand-Dashboard erstellen.

Gehen Sie wie folgt vor, um einen Versand aus der Versandliste zu duplizieren:

1. Klicken Sie auf die Schaltfläche mit den drei Punkten rechts neben dem Namen des zu duplizierenden Versands.
1. Auswählen  **[!UICONTROL Duplizieren]**.
1. Duplizierung bestätigen: Das neue Versand-Dashboard wird im mittleren Bereich des Bildschirms geöffnet.


Gehen Sie wie folgt vor, um einen Versand über sein Dashboard zu duplizieren:

1. Öffnen Sie den Versand und klicken Sie auf die Schaltfläche  **[!UICONTROL ...Mehr]** im oberen Bereich des Bildschirms.
1. Auswählen  **[!UICONTROL Duplizieren]**.
1. Duplizierung bestätigen: Der neue Versand ersetzt den aktuellen Versand im zentralen Bildschirm.

