---
audience: end-user
title: Senden von Nachrichten an Abonnierende eines Dienstes
description: Hier erfahren Sie, wie Sie Nachrichten an die Abonnentinnen und Abonnenten eines Dienstes senden.
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 95%

---

# Senden von Nachrichten an Abonnierende eines Dienstes {#send-to-subscribers}

Sie können in Adobe Campaign Abonnementdienste erstellen und Nachrichten an Ihre Abonnierenden senden. Erfahren Sie auf [dieser Seite](../audience//manage-services.md#create-service), wie Sie Abonnementdienste erstellen.

Um Nachrichten an Ihre Abonnentinnen und Abonnenten zu senden, erstellen Sie eine bestimmte Zielgruppe, um die Abonnentinnen und Abonnenten zu identifizieren, und erstellen Sie dann den Versand wie unten beschrieben.

1. Erstellen einer Zielgruppe. Es wird automatisch ein neuer Workflow erstellt. [Weitere Informationen zu Zielgruppen](../audience/create-audience.md).

1. Ändern Sie zugunsten einer besseren Lesbarkeit den Namen des Workflows in den Workflow-Einstellungen im Feld **Label**. [Erfahren Sie, wie Sie Workflow-Einstellungen konfigurieren](../workflows/workflow-settings.md)

1. Öffnen Sie die Aktivität **[!UICONTROL Zielgruppe erstellen]** und wählen Sie **[!UICONTROL Zielgruppe erstellen]** aus. [Erfahren Sie, wie Sie die Aktivität „Zielgruppe erstellen“ konfigurieren können](../workflows/activities/build-audience.md).

   ![Screenshot mit der Konfiguration der Aktivität „Zielgruppe erstellen“ in Adobe Campaign](assets/service-create-audience.png){zoomable="yes"}

1. Wählen Sie im Fluss zur Erstellung der Zielgruppe die folgenden benutzerdefinierten Bedingungen aus: Es gibt **[!UICONTROL Abonnements]**, wie beispielsweise **[!UICONTROL Dienst]** ist gleich dem von Ihnen definierten Dienst. In diesem Beispiel wählen Sie Ihren **Luma Yoga-Newsletter** aus.

   ![Screenshot mit dem Fluss zur Erstellung der Zielgruppe mit benutzerdefinierten Bedingungen für Abonnements in Adobe Campaign](assets/service-audience-subscribers.png){zoomable="yes"}

1. Wählen Sie **[!UICONTROL Bestätigen]** aus und klicken Sie auf **[!UICONTROL Starten]**, um den Workflow auszuführen.

1. Erstellen Sie einen Versand. Die Schritte zum Erstellen eines Versands werden auf [dieser Seite](../msg/gs-messages.md#create-delivery) ausgeführt.

1. Navigieren Sie zu Ihren Versandeinstellungen und ändern Sie das standardmäßige Zielgruppen-Mapping in **Abonnements (nms:subscriptions)**.

   ![Screenshot mit den Versandeinstellungen, bei denen das Zielgruppen-Mapping in Adobe Campaign in Abonnements geändert wurde.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Wählen Sie im Hauptzielbereich des Versands die zuvor erstellte Zielgruppe aus.

   ![Screenshot mit dem Abschnitt „Hauptzielgruppe“ des Versands mit der ausgewählten Zielgruppe in Adobe Campaign](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Erstellen Sie den Nachrichteninhalt und testen und senden Sie den Versand, wie in [diesem Abschnitt](../preview-test/preview-test.md) beschrieben.

   ![Screenshot mit dem Versand, der in Adobe Campaign gesendet werden kann](assets/service-delivery-ready.png){zoomable="yes"}

Ihr Versand wird nur den Abonnentinnen und Abonnenten dieses Dienstes zugestellt.