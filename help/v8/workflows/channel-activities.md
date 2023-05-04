---
audience: end-user
title: Arbeiten mit Workflows – Kanalaktivitäten
description: Erfahren Sie, wie Sie Kanalaktivitäten in Adobe Campaign Web-Workflows verwenden.
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 26%

---

# Kanalaktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketingkampagnen über mehrere Kanäle hinweg automatisieren und ausführen, z. B. E-Mail, SMS oder Push-Benachrichtigungen. Mit Adobe Campaign-Workflows können Sie Kanalaktivitäten in der Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen Trigger-Aktionen basierend auf dem Kundenverhalten durchgeführt werden können.

Sie können beispielsweise eine Begrüßungs-E-Mail-Kampagne erstellen, die eine Reihe von Nachrichten über verschiedene Kanäle wie E-Mail, SMS und Push-Benachrichtigungen enthält. Sie können auch eine Folgenachricht senden, nachdem ein Kunde einen Kauf getätigt hat, oder eine personalisierte Geburtstagsnachricht per SMS an einen Kunden senden.

Mithilfe von Kanalaktivitäten können Sie umfassende, personalisierte Kampagnen erstellen, die Kunden über mehrere Touchpoints hinweg ansprechen und Konversionen fördern.

Kanalaktivitäten können über die Palette auf der linken Bildschirmseite im Bereich Kanäle aufgerufen werden.

## E-Mail {#email}

Beschreibung, welchen Anwendungsfall Sie ausführen können (gängige andere Aktivitäten, die Sie vor oder nach der Aktivität verknüpfen können)

wie die Aktivität hinzugefügt und konfiguriert wird

Beispiel einer konfigurierten Aktivität in einem Workflow


Die E-Mail-Versandaktivität ermöglicht den Versand von E-Mails innerhalb eines Workflows.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Die E-Mail-Empfänger werden im Vorfeld der Aktivität im selben Workflow mithilfe einer Audience-Zielgruppenbestimmungsaktivität definiert.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->