---
audience: end-user
title: Abonnenten verwalten
description: Erfahren Sie, wie Sie Abonnentinnen und Abonnenten eines Dienstes im Adobe Campaign Web verwalten und an sie etwas senden können.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 68%

---

# Abonnenten verwalten {#manage-subscribers}

Wenn Sie einmal einen [Dienst erstellt](manage-services.md#create-service) haben, können Sie Abonnentinnen und Abonnenten hinzufügen, Empfängerinnen und Empfänger abmelden und Nachrichten an die Abonnentinnen und Abonnenten dieses Dienstes senden.

Die Abonnentenverwaltung wird auf dieser Seite beschrieben. Informationen zum Senden von Nachrichten an Ihre Abonnentinnen und Abonnenten finden Sie in [diesem Abschnitt](../msg/send-to-subscribers.md).

## Hinzufügen von Abonnentinnen und Abonnenten zu Ihrem Dienst {#add-subscribers}

Gehen Sie wie folgt vor, um Abonnentinnen und Abonnenten manuell hinzuzufügen.

1. Wählen Sie einen vorhandenen Dienst aus der Liste **[!UICONTROL Anmeldedienste]** aus.

1. Navigieren Sie zu **[!UICONTROL Abonnenten]** Registerkarte und klicken Sie auf **[!UICONTROL Abonnenten hinzufügen]**.

   ![](assets/service-subscribers-tab.png)

1. Wählen Sie die hinzuzufügenden Profile aus der Liste aus und klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Klicks **[!UICONTROL Senden]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> , damit die ausgewählten Empfänger das Abonnement erhalten [Bestätigungsnachricht](manage-services.md#create-confirmation-message) die Sie definiert haben, wenn [Erstellen des Dienstes](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

   >[!NOTE]
   >
   >Wenn Sie **[!UICONTROL Abbrechen]** keine Bestätigungsnachricht an die ausgewählten Profile gesendet, diese jedoch angemeldet sind.

Die hinzugefügten Profile werden im Abschnitt **[!UICONTROL Abonnenten]** Registerkarte. Sie haben jetzt Ihren Dienst abonniert.

## Entfernen von Abonnentinnen und Abonnenten aus Ihrem Dienst {#remove-subscribers}

### Manuelles Abmelden von Empfängerinnen und Empfängern {#manual-unsubscription}

Wenn Sie für Ihren Dienst [Abonnentinnen und Abonnenten](#add-subscribers) hinzugefügt haben, können Sie jeden von Ihnen manuell abmelden. Gehen Sie dazu wie folgt vor.

1. Wählen Sie einen vorhandenen Dienst aus der Liste **[!UICONTROL Anmeldedienste]** aus.

1. Klicken Sie auf das Drei-Punkte-Symbol neben dem Namen der gewünschten Empfängerin bzw. des gewünschten Empfängers und klicken Sie auf **[!UICONTROL Löschen]**.

   ![](assets/service-subscribers-delete.png)

1. Bestätigen Sie den Löschvorgang.

1. Klicks **[!UICONTROL Senden]** , damit der ausgewählte Empfänger die Abmeldung erhält [Bestätigungsnachricht](manage-services.md#create-confirmation-message) die Sie definiert haben, wenn [Erstellen des Dienstes](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

Der Empfänger wird aus der **[!UICONTROL Abonnenten]** und Ihr Dienst nicht mehr abonniert hat.

### Automatisches Abmelden von Empfängerinnen und Empfängern {#automatic-unsubscription}

Ein Anmeldedienst kann von begrenzter Dauer sein. Die Abmeldung von Abonnentinnen und Abonnenten erfolgt automatisch, wenn der Gültigkeitszeitraum abgelaufen ist.

Dieser Zeitraum wird angegeben, wenn der [Dienst erstellt](manage-services.md#create-service) wird. Deaktivieren Sie in **[!UICONTROL Zusätzliche Optionen]** die Option **[!UICONTROL Unbegrenzter Gültigkeitszeitraum]** und legen Sie einen Gültigkeitszeitraum für den Dienst fest.

![](assets/service-create-validity-period.png)

Nach Ablauf der angegebenen Dauer werden alle Abonnentinnen und Abonnenten automatisch von diesem Dienst abgemeldet.
