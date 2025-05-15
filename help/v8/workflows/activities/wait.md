---
audience: end-user
title: Verwenden der Workflow-Aktivität „Warten“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Warten“ verwenden.
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 100%

---

# Warten {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Aktivität „Warten“"
>abstract="Die Aktivität **Warten** wird verwendet, um die Transition von einer Aktivität zu einer anderen zu verzögern."

Die Aktivität **Warten** ist eine Aktivität zur **Flusskontrolle**. Sie lässt eine bestimmte Zeit zwischen der Ausführung zweier Aktivitäten verstreichen. Sie kann beispielsweise verwendet werden, um nach einer E-Mail-Versandaktivität mehrere Tage zu warten und anschließend die während dieser Zeitspanne erfolgten Öffnungen und Klicks zu analysieren, bevor man andere Verarbeitungsschritte wie das Senden einer Erinnerungs-E-Mail oder das Erstellen einer Zielgruppe unternimmt.

## Konfiguration {#wait-configuration}

Gehen Sie folgendermaßen vor, um die Aktivität **Warten** zu konfigurieren:

1. Fügen Sie eine Aktivität **Warten** zu Ihrem Workflow hinzu.

1. Geben Sie die **Dauer** der Wartezeit zwischen der eingehenden und der ausgehenden Transition an.

1. Wählen Sie die Zeiteinheit im Feld **Zeiträume** aus: Sekunden, Minuten, Stunden, Tage.

## Beispiel {#wait-example}

Das folgende Beispiel erläutert die Aktivität **Warten** anhand eines typischen Fallbeispiels. Darin wird eine E-Mail mit einer Einladung zu einem Event verschickt. Nach 24 Stunden wird ein SMS-Versand an dieselbe Population gesendet.

![Beispiel eines Workflows mit der Aktivität „Warten“, um eine SMS 24 Stunden nach einer E-Mail-Einladung zu senden.](../assets/workflow-wait-example.png)