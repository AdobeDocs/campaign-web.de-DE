---
audience: end-user
title: Verwenden Sie die Workflow-Aktivität Warten .
description: Erfahren Sie, wie Sie die Workflow-Aktivität "Warten"verwenden
badge: label="Alpha" type="Positive"
source-git-commit: 9be56c3c9c7a339e1f348ac9c74d425b501c317d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 72%

---


# Warten {#wait}

Die **Warten**-Aktivität ermöglicht das zeitweise Aussetzen der Ausführung eines Teils eines Workflows. Die ausgehende Transition der Aktivität wird nach einer Frist aktiviert, die zwischen einigen Sekunden und mehreren Monaten liegen kann, wodurch die Ausführung der im Anschluss folgenden Aktivitäten ermöglicht wird.

Die **Warten**-Aktivität ermöglicht es, einen bestimmten Zeitraum zwischen der Ausführung zweier Aktivitäten zu definieren. Beispielsweise kann man mehrere Tage nach einer E-Mail-Versandaktivität warten, dann die während dieser Zeitspanne erfolgten Öffnungen und Klicks analysieren, bevor man andere Verarbeitungsschritte (Erinnerungs-E-Mail, Audience-Erstellung etc.) unternimmt.

## Konfiguration    

Führen Sie die folgenden Schritte aus, um die **Warten** Aktivität:

1. Hinzufügen einer **Warten** in Ihren Workflow ein.

1. Bestimmen Sie die **Dauer** der Wartezeit zwischen der Aktivierung der eingehenden und der ausgehenden Transition der Aktivität.

1. Zeiteinheit auswählen **Zeitraum**: Sekunden, Minuten, Stunden.

## Beispiel

Das folgende Beispiel erläutert die **Warten**-Aktivität anhand eines typischen Fallbeispiels. Darin wird eine E-Mail mit einer Einladung zu einem Ereignis verschickt. 24 Stunden nach dem Versand wird ein SMS-Versand an dieselbe Population gesendet.

![](../assets/workflow-wait-example.png)
