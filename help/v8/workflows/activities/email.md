---
audience: end-user
title: E-Mail-Workflow-Aktivität verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität E-Mail verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 23%

---


# E-Mail, SMS, Push {#channel}

Mit Adobe Campaign Web können Sie Marketingkampagnen über mehrere Kanäle hinweg automatisieren und ausführen, z. B. E-Mail, SMS oder Push-Benachrichtigungen. Sie können Kanalaktivitäten in der Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen Trigger-Aktionen basierend auf dem Kundenverhalten durchgeführt werden können.

Sie können beispielsweise eine Begrüßungs-E-Mail-Kampagne erstellen, die eine Reihe von Nachrichten über verschiedene Kanäle wie E-Mail, SMS und Push-Benachrichtigungen enthält. Sie können auch eine Folgenachricht senden, nachdem eine Kundin oder ein Kunde einen Kauf getätigt hat, oder eine personalisierte Geburtstagsnachricht per SMS an eine Kundin bzw. einen Kunden senden.

Mithilfe von Kanalaktivitäten können Sie umfassende und personalisierte Kampagnen erstellen, die Kunden über mehrere Touchpoints hinweg ansprechen und Konversionen fördern.

Im Folgenden finden Sie die Schritte zum Hinzufügen einer **Kanal** Aktivität in einem Workflow:

1. Stellen Sie sicher, dass Sie einen **Audience erstellen** Aktivität. Die Audience ist die Hauptzielgruppe Ihres Versands: die Empfänger, die die Nachrichten erhalten. Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Nachrichtenzielgruppe nicht in der Kanalaktivität, sondern im **Audience erstellen** Aktivität. Weitere Informationen finden Sie in [diesem Abschnitt](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Wählen Sie eine Versandaktivität aus: **[!UICONTROL E-Mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Push-Benachrichtigung (Android)]** oder **[!UICONTROL Push-Benachrichtigung (iOS)]**.

1. Wählen Sie eine **Vorlage**. Vorlagen sind vorkonfigurierte Versandeinstellungen, die für die zukünftige Verwendung gespeichert werden. [Weitere Informationen](../../msg/delivery-template.md)

1. Klicken **Versand erstellen** und definieren Ihre Nachricht auf die gleiche Weise wie einen eigenständigen Versand. Hier können Sie auch die Versandeinstellungen definieren, den Inhalt planen und simulieren. [Weitere Informationen](../../msg/gs-messages.md)

1. Navigieren Sie zurück zu Ihrem Workflow und klicken Sie auf **Starten** , um Ihren Workflow zu starten.

   Beim Initiieren eines Versand-Workflows wird standardmäßig die Phase der Nachrichtenvorbereitung Trigger, ohne dass die Nachricht sofort gesendet wird.

1. Klicken **Überprüfen und Senden** aus der Kanalaktivität, um den Versand zu bestätigen.

1. Klicken Sie im Versand-Dashboard auf **Senden**.

## Beispiel

Im Folgenden finden Sie ein kanalübergreifendes Workflow-Beispiel mit einer Segmentierung und zwei Sendungen. Der Workflow richtet sich an alle Kunden, die in Paris leben und an Kaffeemaschinen interessiert sind. Unter dieser Population wird eine E-Mail an die regulären Kunden und eine SMS an die VIP gesendet.

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
