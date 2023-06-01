---
audience: end-user
title: Workflow-Aktivität "Und-Verknüpfung" verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Und-Verknüpfung verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 6ed2c73a5348871348ec4cbdd89fc8119fdbc718
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 21%

---


# Und-Verknüpfung {#join}

Die **Und-Verknüpfung** ermöglicht die Synchronisation mehrerer Ausführungszweige eines Workflows.

Bei einer Und-Verknüpfung wird die ausgehende Transition erst aktiviert, wenn alle eingehenden Transitionen aktiviert wurden, d. h. wenn alle vorangehenden Aktivitäten beendet sind.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Und-Verknüpfung** Aktivität:

1. Hinzufügen mehrerer Aktivitäten wie **Kombinieren** Aktivitäten, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Hinzufügen einer **Und-Verknüpfung** -Aktivität zu einem der Zweige.
1. Im **Zusammenführungsoptionen** alle vorherigen Aktivitäten, denen Sie beitreten möchten.
1. Wählen Sie die **Primärer Satz** in der ausgehenden Transition beibehalten werden.

## Beispiel

Das folgende Beispiel zeigt zwei Workflow-Zweige mit einem E-Mail- und SMS-Versand. Die Und-Verknüpfung wird Trigger, wenn beide eingehende Transitionen aktiviert sind. Die Push-Benachrichtigungen werden dann erst gesendet, nachdem beide Sendungen abgeschlossen sind.

![](../assets/workflow-andjoin-example.png)