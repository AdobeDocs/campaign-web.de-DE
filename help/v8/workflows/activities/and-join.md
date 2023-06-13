---
audience: end-user
title: Workflow-Aktivität "Und-Verknüpfung" verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Und-Verknüpfung verwenden.
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 1%

---


# Und-Verknüpfung {#join}

Die **Und-Verknüpfung** -Aktivität **Flusssteuerung** Aktivität. Damit können Sie mehrere Ausführungszweige eines Workflows synchronisieren.

Die ausgehende Transition wird erst dann Trigger, wenn alle eingehenden Transitionen aktiviert wurden, d. h. wenn alle vorangehenden Aktivitäten beendet sind. Auf diese Weise können Sie sicherstellen, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie mit der Ausführung des Workflows fortfahren.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Und-Verknüpfung** Aktivität:

1. Fügen Sie mehrere Aktivitäten wie Kanalaktivitäten hinzu, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Hinzufügen einer **Und-Verknüpfung** -Aktivität zu einem der Zweige.
1. Im **Zusammenführungsoptionen** alle vorherigen Aktivitäten, denen Sie beitreten möchten.
1. Im **Primärer Satz** auswählen, welche eingehende Transition-Population Sie beibehalten möchten. Die ausgehende Transition darf nur eine der eingehenden Populationen enthalten.

## Beispiel

Das folgende Beispiel zeigt zwei Workflow-Zweige mit einem E-Mail- und SMS-Versand. Die Und-Verknüpfung wird Trigger, wenn beide eingehende Transitionen aktiviert sind. Die Push-Benachrichtigungen werden dann erst gesendet, nachdem beide Sendungen abgeschlossen sind.

![](../assets/workflow-andjoin-example.png)