---
audience: end-user
title: Nachrichten an Abonnenten eines Dienstes senden
description: Hier erfahren Sie, wie Sie Nachrichten an die Abonnenten eines Dienstes senden.
badge: label="Beta"
source-git-commit: e5ef71de970468fce418cc06cb9d2c25c0c40306
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 5%

---


# Nachrichten an Abonnenten eines Dienstes senden

Sie können in Adobe Campaign Anmeldedienste erstellen und Nachrichten an Ihre Abonnenten senden. Erfahren Sie, wie Sie Abonnementdienste in erstellen [diese Seite](../audience//manage-services.md#create-service).

Um Nachrichten an Ihre Abonnenten zu senden, erstellen Sie eine bestimmte Audience, um die Abonnenten zu identifizieren, und erstellen Sie dann den Versand wie unten beschrieben.

1. Erstellen einer Zielgruppe. Weitere Informationen zu Zielgruppen finden Sie in [diese Seite](../audience/create-audience.md).

1. Im **[!UICONTROL Audience erstellen]** Aktivität, erweiterte Attribute anzeigen und **[!UICONTROL Empfänger]** > **[!UICONTROL Abonnements]** > **[!UICONTROL Dienst]**.

   Wählen Sie in diesem Beispiel die Benutzer aus, die den Dienst abonniert haben, der über die **Luma-Newsletter** Beschriftung.

   ![](assets/service-audience-subscribers.png)

1. Speichern Sie die Audience.
1. Erstellen eines Versands. Die Schritte zum Erstellen eines Versands werden im Abschnitt [diese Seite](../msg/gs-messages.md#create-delivery).
1. Navigieren Sie zu Ihren Versandeinstellungen und ändern Sie das standardmäßige Zielgruppen-Mapping in **Abonnements (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. Wählen Sie im Hauptzielbereich des Versands die zuvor erstellte Audience aus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Erstellen Sie den Nachrichteninhalt, testen und senden Sie den Versand, wie im Abschnitt [diesem Abschnitt](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Ihre Nachricht wird nur an die Abonnenten dieses Dienstes gesendet.
