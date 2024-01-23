---
audience: end-user
title: Senden von Nachrichten an Abonnentinnen und Abonnenten eines Dienstes
description: Hier erfahren Sie, wie Sie Nachrichten an die Abonnentinnen und Abonnenten eines Dienstes senden.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: ad8d99ca73bebccae9ee7466bda566cdc465fb26
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 61%

---

# Senden von Nachrichten an Abonnentinnen und Abonnenten eines Dienstes {#send-to-subscribers}

Sie können in Adobe Campaign Anmeldedienste erstellen und Nachrichten an Ihre Abonnentinnen und Abonnenten senden. Erfahren Sie, wie Sie Abonnementdienste erstellen in [diese Seite](../audience//manage-services.md#create-service).

Um Nachrichten an Ihre Abonnentinnen und Abonnenten zu senden, erstellen Sie eine bestimmte Zielgruppe, um die Abonnentinnen und Abonnenten zu identifizieren, und erstellen Sie dann den Versand wie unten beschrieben.

1. Erstellen einer Zielgruppe. Ein neuer Workflow wird automatisch erstellt. [Weitere Informationen zu Zielgruppen](../audience/create-audience.md)

1. Um die Lesbarkeit zu verbessern, ändern Sie den Namen des Workflows in den Workflow-Einstellungen. **Titel** -Feld. [Erfahren Sie, wie Sie Workflow-Einstellungen konfigurieren](../workflows/workflow-settings.md)

1. Öffnen Sie die **[!UICONTROL Audience erstellen]** und wählen Sie **[!UICONTROL Erstellen einer Zielgruppe]**. [Erfahren Sie, wie Sie eine Aktivität „Zielgruppe erstellen“ konfigurieren können](../workflows/activities/build-audience.md)

   ![](assets/service-create-audience.png)

1. Wählen Sie im Erstellungsablauf der Zielgruppe die folgenden benutzerdefinierten Bedingungen aus: **[!UICONTROL Abonnements]** vorhanden sind, z. B. **[!UICONTROL Dienst]** entspricht dem von Ihnen definierten Dienst. Wählen Sie in diesem Beispiel Ihre **Luma-Yoga-Newsletter**.

   ![](assets/service-audience-subscribers.png)

1. Auswählen **[!UICONTROL Bestätigen]** und klicken **[!UICONTROL Starten]** , um den Workflow auszuführen.

1. Erstellen Sie einen Versand. Die Schritte zum Erstellen eines Versands werden auf [dieser Seite](../msg/gs-messages.md#create-delivery) ausgeführt.
1. Navigieren Sie zu Ihren Versandeinstellungen und ändern Sie das standardmäßige Zielgruppen-Mapping in **Abonnements (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. Wählen Sie im Hauptzielbereich des Versands die zuvor erstellte Zielgruppe aus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Erstellen Sie den Nachrichteninhalt und testen und senden Sie den Versand, wie in [diesem Abschnitt](../preview-test/preview-test.md) ausgeführt.

   ![](assets/service-delivery-ready.png)

Ihre Versand wird nur den Abonnentinnen und Abonnenten dieses Dienstes zugestellt.
