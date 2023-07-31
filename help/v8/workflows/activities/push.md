---
audience: end-user
title: Verwenden der Workflow-Aktivität „Push-Benachrichtigung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Push-Benachrichtigung“ verwenden
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 100%

---


# Push-Benachrichtigung {#push-activity}

Die Versandaktivität **Push-Benachrichtigung** ermöglicht es Ihnen, das Senden einer Push-Benachrichtigung in einem Workflow zu konfigurieren.

>[!BEGINTABS]

>[!TAB Push-Benachrichtigung (Android)]

1. Fügen Sie nach dem Erstellen und Konfigurieren eines neuen Workflows die Aktivität „Zielgruppe aufbauen“ hinzu, um eine vorhandene Zielgruppe auszuwählen, oder verwenden Sie den Regel-Builder, um Ihre eigene Abfrage zu definieren.

1. Fügen Sie eine Kanalaktivität „Push-Benachrichtigung (Android)“ in Ihren Workflow ein.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Wählen Sie Ihre Aktivität aus. Wählen Sie im Versandmenü die Vorlagen aus, die Sie für diesen Versand verwenden möchten. Weitere Informationen zu Vorlagen

1. Klicken Sie auf „Versand erstellen“, um Ihren Push-Benachrichtigungs-Versand zu konfigurieren. Weiterführende Informationen zum Versand von Push-Benachrichtigungen (Android) finden Sie auf dieser Seite.

1. Sobald der Versand fertig ist, navigieren Sie zu Ihrem Workflow und klicken Sie auf „Starten“, um den Workflow zu starten.

1. Standardmäßig wird durch die Initiierung eines Versand-Workflows die Vorbereitungsphase der Nachricht ausgelöst, ohne dass die Nachricht sofort versendet wird.

   Klicken Sie im erweiterten Menü Ihrer Kanalaktivität der Push-Benachrichtigung (Android) auf „Überprüfen und Senden“, um den Versand zu bestätigen.

1. Klicken Sie im Dashboard Ihres Push-Benachrichtigungs-Versands auf „Senden“.

>[!TAB Push-Benachrichtigung (iOS)]

1. Fügen Sie nach dem Erstellen und Konfigurieren eines neuen Workflows die Aktivität „Zielgruppe aufbauen“ hinzu, um eine vorhandene Zielgruppe auszuwählen, oder verwenden Sie den Regel-Builder, um Ihre eigene Abfrage zu definieren.

1. Fügen Sie eine Kanalaktivität „Push-Benachrichtigung (iOS)“ in Ihren Workflow ein.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Wählen Sie Ihre Aktivität aus. Wählen Sie im Versandmenü die Vorlagen aus, die Sie für diesen Versand verwenden möchten. Weitere Informationen zu Vorlagen

1. Klicken Sie auf „Versand erstellen“, um Ihren Push-Benachrichtigungs-Versand zu konfigurieren. Weiterführende Informationen zum Versand von Push-Benachrichtigungen (iOS) finden Sie auf dieser Seite.

1. Sobald der Versand fertig ist, navigieren Sie zu Ihrem Workflow und klicken Sie auf „Starten“, um den Workflow zu starten.

1. Standardmäßig wird durch die Initiierung eines Versand-Workflows die Vorbereitungsphase der Nachricht ausgelöst, ohne dass die Nachricht sofort versendet wird.

   Klicken Sie im erweiterten Menü der Kanalaktivität Push-Benachrichtigung (iOS) auf „Überprüfen und senden“, um den Versand zu bestätigen.

1. Klicken Sie im Dashboard Ihres Push-Benachrichtigungs-Versands auf „Senden“.

>[!ENDTABS]