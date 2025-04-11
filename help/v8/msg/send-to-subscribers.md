---
audience: end-user
title: Senden von Nachrichten an Abonnentinnen und Abonnenten eines Dienstes
description: Hier erfahren Sie, wie Sie Nachrichten an die Abonnentinnen und Abonnenten eines Dienstes senden.
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 41%

---

# Senden von Nachrichten an Abonnentinnen und Abonnenten eines Dienstes {#send-to-subscribers}

Sie können Abonnements in Adobe Campaign erstellen und Nachrichten an Ihre Abonnenten senden. Erfahren Sie auf [ Seite , wie Sie Abonnement-Services ](../audience//manage-services.md#create-service).

Um Nachrichten an Ihre Abonnentinnen und Abonnenten zu senden, erstellen Sie eine bestimmte Zielgruppe, um die Abonnentinnen und Abonnenten zu identifizieren, und erstellen Sie dann den Versand wie unten beschrieben.

1. Erstellen einer Zielgruppe. Es wird automatisch ein neuer Workflow erstellt. [Weitere Informationen zu Zielgruppen](../audience/create-audience.md).

1. Ändern Sie zugunsten einer besseren Lesbarkeit den Namen des Workflows in den Workflow-Einstellungen im Feld **Titel**. [Erfahren Sie, wie Sie Workflow-Einstellungen konfigurieren](../workflows/workflow-settings.md).

1. Öffnen Sie die Aktivität **[!UICONTROL Zielgruppe erstellen]** und wählen Sie **[!UICONTROL Zielgruppe erstellen]** aus. [Erfahren Sie, wie Sie die Aktivität „Zielgruppe aufbauen“ konfigurieren](../workflows/activities/build-audience.md).

   ![Screenshot der Konfiguration der Aktivität „Zielgruppe aufbauen“ in Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. Wählen Sie im Ablauf zur Zielgruppenerstellung die folgenden benutzerdefinierten Bedingungen aus: **[!UICONTROL Abonnements]** vorhanden, z. B. **[!UICONTROL Service]** ist gleich dem von Ihnen definierten Service. In diesem Beispiel wählen Sie Ihren **Luma Yoga-Newsletter** aus.

   ![Screenshot, der den Ablauf der Zielgruppenerstellung mit benutzerdefinierten Bedingungen für Abonnements in Adobe Campaign zeigt.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Wählen Sie **[!UICONTROL Bestätigen]** und klicken Sie auf **[!UICONTROL Starten]**, um den Workflow auszuführen.

1. Erstellen Sie einen Versand. Die Schritte zum Erstellen eines Versands werden auf [ Seite ](../msg/gs-messages.md#create-delivery).

1. Navigieren Sie zu Ihren Versandeinstellungen und ändern Sie das standardmäßige Zielgruppen-Mapping in &quot;**(nms:subscriptions)**.

   ![Screenshot mit den Versandeinstellungen, bei denen das Zielgruppen-Mapping in Adobe Campaign in Abonnements geändert wurde.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Wählen Sie im Hauptzielbereich des Versands die zuvor erstellte Zielgruppe aus.

   ![Screenshot, der den Hauptzielabschnitt des Versands mit der ausgewählten Audience in Adobe Campaign zeigt.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Erstellen Sie den Inhalt Ihrer Nachricht, testen Sie ihn und senden Sie den Versand, wie [ diesem Abschnitt beschrieben](../preview-test/preview-test.md).

   ![Screenshot, der den Versand zeigt, der in Adobe Campaign gesendet werden kann.](assets/service-delivery-ready.png){zoomable="yes"}

Ihr Versand wird nur den Abonnentinnen und Abonnenten dieses Dienstes zugestellt.