---
audience: end-user
title: Erste Schritte mit Nachrichten und Sendungen in Campaign v8 Web
description: Erfahren Sie, wie Sie Campaign Web verwenden, um mit Sendungen zu arbeiten und Nachrichten zu senden
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 38%

---

# Erste Schritte mit Nachrichten in Campaign Web {#gs-messages}

Mit Adobe Campaign können Sie kanalübergreifende Kampagnen wie E-Mails, SMS und Push-Benachrichtigungen versenden und deren Effektivität mithilfe diverser Berichte messen. Diese Nachrichten werden mittels Sendungen entworfen und gesendet und können für jeden Empfänger personalisiert werden. Diese Sendungen können einzeln oder im Rahmen einer Marketingkampagne durchgeführt werden.

Adobe Campaign v8 enthält die folgenden Versandkanäle:

* **E-Mail-Kanal**: Ein E-Mail-Versand richtet personalisierte elektronische Nachrichten an eine zuvor bestimmte Zielpopulation. Erfahren Sie, wie Sie eine E-Mail erstellen und senden in [diese Seite](../email/create-email.md).

* **SMS-Kanal**: Sendungen über Mobile-Kanäle ermöglichen den Versand personalisierter SMS an die Zielpopulation.  Erfahren Sie, wie Sie SMS erstellen und senden in [diese Seite](../sms/create-sms.md).

* **Mobile-App-Kanal**: Mit Mobile-App-Sendungen können Sie Benachrichtigungen an iOS- und Android-Systeme senden.  Erfahren Sie, wie Sie Push-Benachrichtigungen erstellen und senden in [diese Seite](../push/gs-push.md).

## Erstellen eines Versands

Sie können eigenständige Sendungen über die **Versand** oder Sendungen im Rahmen einer Marketingkampagne erstellen.

>[!BEGINTABS]

>[!TAB Erstellen eines eigenständigen Versands]

Gehen Sie wie folgt vor, um einen eigenständigen Versand zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Sendungen]** im linken Navigationsmenü und klicken Sie auf das **[!UICONTROL Versand erstellen]** Schaltfläche.
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
1. Sobald Nachrichten gesendet wurden, navigieren Sie zum Abschnitt Berichte , um auf Schlüsselmetriken zuzugreifen. Weitere Informationen zu Versandberichten finden Sie in [diesem Abschnitt](../reporting/reports.md).

>[!TAB Versand in einer Kampagne erstellen]

Gehen Sie wie folgt vor, um einen Versand in einer Kampagne zu erstellen:

1. Erstellen Sie eine Kampagne oder öffnen Sie eine bestehende Kampagne.

Weitere Informationen zur Konfiguration einer Kampagne finden Sie unter

>[!ENDTABS]


## Auswahl der Versandart für Ihre Nachrichten{#gs-send-msg}

Sobald Ihre Nachricht erstellt und ihr Inhalt entworfen und getestet wurde, können Sie wählen, wie Sie sie versenden möchten.

Campaign bietet eine Reihe von Funktionen, um:

* Manuelles Senden von Nachrichten an die Hauptzielgruppe

* Senden von Nachrichten, die einer [Marketing-Kampagne](../campaigns/gs-campaigns.md) zugeordnet sind

* Senden von Nachrichten über einen [Workflow](../workflows/channel-activities.md)


## Hinzufügen von Personalisierung{#personalization}

Nachrichten, die von Adobe Campaign versendet werden, können auf verschiedene Weise personalisiert werden


## Versand- und Trackinglogs{#gs-tracking-logs}

Die Überwachung Ihrer Sendungen nach deren Versand ist ein wichtiger Schritt, um sicherzustellen, dass Ihre Marketing-Kampagnen effizient sind und Ihre Kunden erreichen. Sie können nach dem Versand überwachen sowie nachvollziehen, wie Zustellungsfehler und Quarantänen gehandhabt werden.
