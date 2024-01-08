---
audience: end-user
title: Senden von Nachrichten an Abonnentinnen und Abonnenten eines Dienstes
description: Hier erfahren Sie, wie Sie Nachrichten an die Abonnentinnen und Abonnenten eines Dienstes senden.
badge: label="Beta"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: cd7e2bb325b4e571018a8e04ffa0eaef74fe6768
workflow-type: ht
source-wordcount: '185'
ht-degree: 100%

---

# Senden von Nachrichten an Abonnentinnen und Abonnenten eines Dienstes

Sie können in Adobe Campaign Anmeldedienste erstellen und Nachrichten an Ihre Abonnentinnen und Abonnenten senden. Erfahren Sie auf [dieser Seite](../audience//manage-services.md#create-service), wie Sie Abonnementdienste erstellen.

Um Nachrichten an Ihre Abonnentinnen und Abonnenten zu senden, erstellen Sie eine bestimmte Zielgruppe, um die Abonnentinnen und Abonnenten zu identifizieren, und erstellen Sie dann den Versand wie unten beschrieben.

1. Erstellen einer Zielgruppe. Weitere Informationen über Zielgruppen finden Sie auf [dieser Seite](../audience/create-audience.md).

1. Zeigen Sie in der Aktivität **[!UICONTROL Zielgruppe erstellen]** die erweiterten Attribute an und wählen Sie **[!UICONTROL Empfänger]** > **[!UICONTROL Abonnements]** > **[!UICONTROL Dienst]**.

   Wählen Sie in diesem Beispiel die Benutzenden aus, die den Dienst mit der Kennzeichnung **Luma-Newsletter** abonnieren.

   ![](assets/service-audience-subscribers.png)

1. Speichern Sie die Zielgruppe.
1. Erstellen Sie einen Versand. Die Schritte zum Erstellen eines Versands werden auf [dieser Seite](../msg/gs-messages.md#create-delivery) ausgeführt.
1. Navigieren Sie zu Ihren Versandeinstellungen und ändern Sie das standardmäßige Zielgruppen-Mapping in **Abonnements (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. Wählen Sie im Hauptzielbereich des Versands die zuvor erstellte Zielgruppe aus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Erstellen Sie den Nachrichteninhalt und testen und senden Sie den Versand, wie in [diesem Abschnitt](../preview-test/preview-test.md) ausgeführt.

   ![](assets/service-delivery-ready.png)

Ihre Versand wird nur den Abonnentinnen und Abonnenten dieses Dienstes zugestellt.
