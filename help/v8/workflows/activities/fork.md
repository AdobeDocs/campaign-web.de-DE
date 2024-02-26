---
audience: end-user
title: Verwenden der Workflow-Aktivität „Verzweigung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Verzweigung“ verwenden.
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 100%

---

# Verzweigung  {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Aktivität „Verzweigung“"
>abstract="Eine **Verzweigung** erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transitionen von Verzweigungsaktivitäten"
>abstract="Standardmäßig werden zwei Transitionen mit einer **Verzweigungsaktivität** erstellt. Klicken Sie auf die Schaltfläche **Transition hinzufügen**, um eine zusätzliche ausgehende Transition zu definieren, und geben Sie deren Titel ein."

Die Aktivität **Verzweigung** ist eine Aktivität zur **Flusssteuerung**. Sie erstellt ausgehende Transitionen, um mehrere Aktivitäten parallel zu starten.

## Konfigurieren der Verzweigungsaktivität{#fork-configuration}

Führen Sie die folgenden Schritte aus, um die Aktivität **Verzweigung** zu konfigurieren:

![](../assets/workflow-fork.png)

1. Fügen Sie Ihrem Workflow eine Aktivität **Verzweigung** hinzu.
1. Klicken Sie auf **Transition hinzufügen**, um eine neue ausgehende Transition hinzuzufügen. Standardmäßig sind zwei Transitionen definiert.
1. Fügen Sie jeder Ihrer Transitionen einen Titel hinzu.

## Beispiel{#fork-example}

Im folgenden Beispiel verwenden wir zwei Aktivitäten vom Typ **Verzweigung**:

* Eine vor den beiden Abfragen, damit sie gleichzeitig ausgeführt werden.
* Eine nach dem Schnittpunkt, um eine E-Mail und eine SMS gleichzeitig an die Zielpopulation zu senden.

![](../assets/workflow-fork-example.png)
