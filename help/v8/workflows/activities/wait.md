---
audience: end-user
title: Verwenden der Workflow-Aktivität „Warten“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Warten“ verwenden.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: 023777b88fa5c80e110fcf334517f7cef1c7f1ee
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 92%

---

# Warten {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Aktivität „Warten“"
>abstract="Die Aktivität **Warten** wird verwendet, um die Transition von einer Aktivität zu einer anderen zu verzögern."

Die Aktivität **Warten** ist eine Aktivität zur **Flusskontrolle**. Sie wird verwendet, um einen bestimmten Zeitraum zwischen der Ausführung zweier Aktivitäten zu definieren. Beispielsweise kann man mehrere Tage nach einer E-Mail-Versandaktivität warten, dann die während dieses Zeitraums erfolgten Öffnungen und Klicks analysieren, bevor man weitere Verarbeitungsschritte (Erinnerungs-E-Mail, Zielgruppenerstellung etc.) unternimmt.

## Konfiguration    {#wait-configuration}

Gehen Sie folgendermaßen vor, um die Aktivität **Warten** zu konfigurieren:

1. Fügen Sie eine Aktivität **Warten** zu Ihrem Workflow hinzu.

1. Geben Sie die **Dauer** der Wartezeit zwischen der eingehenden und der ausgehenden Transition an.

1. Wählen Sie die Zeiteinheit im **Zeiträume** -Feld: Sekunden, Minuten, Stunden, Tage.

## Beispiel{#wait-example}

Das folgende Beispiel erläutert die Aktivität **Warten** anhand eines typischen Fallbeispiels. Darin wird eine E-Mail mit einer Einladung zu einem Event verschickt. 24 Stunden nach dem Versand wird ein SMS-Versand an dieselbe Population gesendet.

![](../assets/workflow-wait-example.png)
