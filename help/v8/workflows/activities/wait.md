---
audience: end-user
title: Verwenden Sie die Workflow-Aktivität Warten .
description: Erfahren Sie, wie Sie die Workflow-Aktivität "Warten"verwenden
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 39%

---


# Warten {#wait}

Die **Warten** -Aktivität **Flusssteuerung** Aktivität. Er wird verwendet, um einen bestimmten Zeitraum zwischen der Ausführung zweier Aktivitäten zu ermöglichen. Beispielsweise kann man mehrere Tage nach einer E-Mail-Versandaktivität warten, dann die während dieser Zeitspanne erfolgten Öffnungen und Klicks analysieren, bevor man andere Verarbeitungsschritte (Erinnerungs-E-Mail, Audience-Erstellung etc.) unternimmt.

## Konfiguration    

Führen Sie die folgenden Schritte aus, um die **Warten** Aktivität:

1. Hinzufügen einer **Warten** in Ihren Workflow ein.

1. Geben Sie die **Dauer** der Wartezeit zwischen der eingehenden und der ausgehenden Transition.

1. Wählen Sie die Zeiteinheit im **Zeiträume** -Feld: Sekunden, Minuten, Stunden.

## Beispiel

Das folgende Beispiel erläutert die **Warten**-Aktivität anhand eines typischen Fallbeispiels. Darin wird eine E-Mail mit einer Einladung zu einem Ereignis verschickt. 24 Stunden nach dem Versand wird ein SMS-Versand an dieselbe Population gesendet.

![](../assets/workflow-wait-example.png)
