---
audience: end-user
title: Verwenden der Workflow-Aktivität „Warten“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Warten“ verwenden.
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: ht
source-wordcount: '162'
ht-degree: 100%

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

1. Wählen Sie die Zeiteinheit im Feld **Zeiträume**: Sekunden, Minuten, Stunden.

## Beispiel{#wait-example}

Das folgende Beispiel erläutert die Aktivität **Warten** anhand eines typischen Fallbeispiels. Darin wird eine E-Mail mit einer Einladung zu einem Event verschickt. 24 Stunden nach dem Versand wird ein SMS-Versand an dieselbe Population gesendet.

![](../assets/workflow-wait-example.png)
