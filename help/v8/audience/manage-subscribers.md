---
audience: end-user
title: Verwalten von Abonnentinnen und Abonnenten
description: Erfahren Sie, wie Sie Abonnentinnen und Abonnenten eines Dienstes i Adobe Campaign Web verwalten und wie Sie an sie versenden.
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 100%

---

# Verwalten von Abonnentinnen und Abonnenten {#manage-subscribers}

Wenn Sie einmal einen [Dienst erstellt](manage-services.md#create-service) haben, können Sie Abonnentinnen und Abonnenten hinzufügen, Empfängerinnen und Empfänger abmelden und Nachrichten an die Abonnentinnen und Abonnenten dieses Dienstes senden.

Die Abonnentenverwaltung wird auf dieser Seite beschrieben. Informationen zum Senden von Nachrichten an Ihre Abonnentinnen und Abonnenten finden Sie in [diesem Abschnitt](../msg/send-to-subscribers.md).

## Hinzufügen von Abonnentinnen und Abonnenten zu Ihrem Dienst {#add-subscribers}

Gehen Sie wie folgt vor, um Abonnentinnen und Abonnenten manuell hinzuzufügen.

1. Wählen Sie einen vorhandenen Dienst aus der Liste **[!UICONTROL Anmeldedienste]** aus.

1. Navigieren Sie zu der Registerkarte **[!UICONTROL Abonnierende]** und klicken Sie auf **[!UICONTROL Abonnierende hinzufügen]**.

   ![Screenshot mit der Registerkarte „Abonnierende“ in der Benutzeroberfläche der Abonnementdienste.](assets/service-subscribers-tab.png){zoomable="yes"}

1. Wählen Sie die hinzuzufügenden Profile aus der Liste aus und klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![Screenshot mit der Benutzeroberfläche für die Profilauswahl zum Hinzufügen von Abonnierenden](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Senden]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->, damit die ausgewählten Empfängerinnen und Empfänger die [Bestätigungsnachricht](manage-services.md#create-confirmation-message) für das Abonnement erhalten, die Sie beim [Erstellen des Dienstes](manage-services.md#create-service) definiert haben.

   ![Screenshot mit der Benutzeroberfläche für die Bestätigungsnachricht zum Hinzufügen von Abonnierenden](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >Wenn Sie **[!UICONTROL Abbrechen]** auswählen, wird keine Bestätigungsnachricht an die ausgewählten Profile gesendet, aber sie sind angemeldet.

Die hinzugefügten Profile werden in der Registerkarte **[!UICONTROL Abonnierende]** angezeigt. Sie haben jetzt Ihren Dienst abonniert.

## Entfernen von Abonnentinnen und Abonnenten aus Ihrem Dienst {#remove-subscribers}

### Manuelles Abmelden von Profilen {#manual-unsubscription}

Wenn Sie für Ihren Dienst [Abonnentinnen und Abonnenten](#add-subscribers) hinzugefügt haben, können Sie jeden von Ihnen manuell abmelden. Gehen Sie dazu wie folgt vor.

1. Wählen Sie einen vorhandenen Dienst aus der Liste **[!UICONTROL Anmeldedienste]** aus.

1. Klicken Sie auf das Drei-Punkte-Symbol neben dem Namen der gewünschten Empfängerin bzw. des gewünschten Empfängers und wählen Sie **[!UICONTROL Löschen]** aus.

   ![Screenshot mit der Option „Löschen“ für die Abmeldung von Profilen](assets/service-subscribers-delete.png){zoomable="yes"}

1. Bestätigen Sie den Löschvorgang.

1. Klicken Sie auf **[!UICONTROL Senden]**, damit die ausgewählte Empfängerin bzw. der Empfänger die [Bestätigungsnachricht](manage-services.md#create-confirmation-message) für die Abmeldung erhält, die Sie beim [Erstellen des Dienstes](manage-services.md#create-service) definiert haben.

   ![Screenshot mit der Benutzeroberfläche für die Bestätigungsnachricht für die Abmeldung von Profilen](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

Die Empfängerin bzw. der Empfänger wird aus der Registerkarte **[!UICONTROL Abonnierende]** entfernt und hat Ihren Dienst nicht länger abonniert.

### Automatisches Abmelden von Empfängerinnen und Empfängern {#automatic-unsubscription}

Ein Anmeldedienst kann von begrenzter Dauer sein. Die Abmeldung von Profilen erfolgt automatisch, wenn der Gültigkeitszeitraum abgelaufen ist.

Dieser Zeitraum wird angegeben, wenn der [Dienst erstellt](manage-services.md#create-service) wird. Deaktivieren Sie in **[!UICONTROL Zusätzliche Optionen]** die Option **[!UICONTROL Unbegrenzter Gültigkeitszeitraum]** und legen Sie einen Gültigkeitszeitraum für den Dienst fest.

![Screenshot der Konfiguration des Gültigkeitszeitraums für einen Abonnementdienst](assets/service-create-validity-period.png){zoomable="yes"}

Nach Ablauf der angegebenen Dauer werden alle Abonnentinnen und Abonnenten automatisch von diesem Dienst abgemeldet.