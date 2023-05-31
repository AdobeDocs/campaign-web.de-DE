---
audience: end-user
title: E-Mail-Workflow-Aktivität verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität E-Mail verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 6af0b460a3c81f063a855b2fabba221b43e4ebb9
workflow-type: tm+mt
source-wordcount: '50'
ht-degree: 74%

---


# E-Mail {#email}

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow

-->


Die Aktivität „E-Mail-Versand“ ermöglicht das Konfigurieren eines E-Mail-Versands innerhalb eines Workflows.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Die Empfängerinnen und Empfänger der E-Mails werden im Vorfeld der Aktivität im selben Workflow mithilfe einer Audience-Zielgruppenbestimmungsaktivität definiert.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
