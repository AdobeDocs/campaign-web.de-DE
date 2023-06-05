---
audience: end-user
title: Verwenden der Workflow-Aktivität Push-Benachrichtigung
description: Erfahren Sie, wie Sie die Workflow-Aktivität "Push-Benachrichtigung"verwenden
badge: label="Alpha" type="Positive"
source-git-commit: c0e5902d3ee504aa5aa4e55f18416facfe4020b1
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 3%

---


# Push notification {#push-activity}

Die **Push-Benachrichtigung** Die Versandaktivität ermöglicht den Versand von Push-Benachrichtigungen innerhalb eines Workflows.

>[!BEGINTABS]

>[!TAB Push-Benachrichtigung (Android)]

1. Fügen Sie nach dem Erstellen und Konfigurieren eines neuen Workflows die Aktivität Audience erstellen hinzu, um eine vorhandene Audience auszuwählen, oder verwenden Sie den Regel-Builder, um Ihre eigene Abfrage zu definieren.

1. Fügen Sie die Aktivität Push-Benachrichtigung (Android) in Ihren Workflow ein.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Wählen Sie Ihre Aktivität aus. Wählen Sie im Versandmenü die Vorlagen aus, die Sie für diesen Versand verwenden möchten. Weitere Informationen zu Vorlagen

1. Klicken Sie auf Versand erstellen , um Ihren Push-Benachrichtigungsversand zu konfigurieren. Weiterführende Informationen zum Versand von Push-Benachrichtigungen (Android) finden Sie auf dieser Seite.

1. Sobald der Versand fertig ist, navigieren Sie zu Ihrem Workflow und klicken Sie auf Starten , um den Workflow zu starten.

1. Beim Initiieren eines Versand-Workflows wird standardmäßig die Phase der Nachrichtenvorbereitung Trigger, ohne dass die Nachricht sofort gesendet wird.

   Klicken Sie im erweiterten Menü der Aktivität Android-Kanal (Push notification) auf Überprüfen und senden , um den Versand zu bestätigen.

1. Klicken Sie im Dashboard Ihres Push-Benachrichtigungsversands auf Senden.

>[!TAB Push-Benachrichtigung (iOS)]

1. Fügen Sie nach dem Erstellen und Konfigurieren eines neuen Workflows die Aktivität Audience erstellen hinzu, um eine vorhandene Audience auszuwählen, oder verwenden Sie den Regel-Builder, um Ihre eigene Abfrage zu definieren.

1. Fügen Sie die Aktivität Push-Benachrichtigung (iOS) in Ihren Workflow ein.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Wählen Sie Ihre Aktivität aus. Wählen Sie im Versandmenü die Vorlagen aus, die Sie für diesen Versand verwenden möchten. Weitere Informationen zu Vorlagen

1. Klicken Sie auf Versand erstellen , um Ihren Push-Benachrichtigungsversand zu konfigurieren. Weiterführende Informationen zum Versand von Push-Benachrichtigungen (iOS) finden Sie auf dieser Seite.

1. Sobald der Versand fertig ist, navigieren Sie zu Ihrem Workflow und klicken Sie auf Starten , um den Workflow zu starten.

1. Beim Initiieren eines Versand-Workflows wird standardmäßig die Phase der Nachrichtenvorbereitung Trigger, ohne dass die Nachricht sofort gesendet wird.

   Klicken Sie im erweiterten Menü der Aktivität Push-Benachrichtigung (iOS) auf Überprüfen und senden , um den Versand zu bestätigen.

1. Klicken Sie im Dashboard Ihres Push-Benachrichtigungsversands auf Senden.

>[!ENDTABS]