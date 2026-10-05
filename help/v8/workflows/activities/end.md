---
audience: end-user
title: Verwenden der Workflow-Aktivität „Ende“
description: Informationen zum Verwenden der Workflow-Aktivität „Ende“
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 100%
---
# Ende {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Endaktivität"
>abstract="Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Wenn mehr als eine eingehende Transition verfügbar ist, den Abschnitt **Zusammenzuführende Mengen** verwenden, um auszuwählen, welche Transitionen mit der Aktivität verbunden werden sollen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Zusammenzuführende Mengen"
>abstract="Markieren Sie die vorherigen Aktivitäten, die als eingehende Transitionen der Aktivität **Ende** verbunden werden sollen. Die ausgewählten Aktivitäten werden dann mit der Aktivität **Ende** verbunden. Dieser Abschnitt wird nur angezeigt, wenn mehr als eine eingehende Transition für die Verbindung mit der Aktivität verfügbar ist."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Externes Signal"
>abstract="Platzhalter für den Abschnitt „Externes Signal“ in den Parametern der Endaktivität. Nur für orchestrierte Kampagnen verfügbar. NICHT LÖSCHEN"

Die Aktivität **Ende** ist eine Aktivität zur **Flusskontrolle**. Damit können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität ist optional.

Die Aktivität unterstützt mehrere eingehende Transitionen, wenn mehr als eine eingehende Transition verfügbar ist.

Aktivieren Sie im Abschnitt **Zusammenzuführende Mengen** die vorherigen Aktivitäten, die Sie als eingehende Transitionen der Aktivität **Ende** verbinden möchten. Die ausgewählten Aktivitäten werden dann mit der Aktivität **Ende** auf der Workflow-Arbeitsfläche verknüpft.

![Konfigurationsprozess für die Workflow-Deduplizierung](../assets/workflow-end.png)
