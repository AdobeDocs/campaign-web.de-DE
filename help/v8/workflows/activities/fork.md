---
audience: end-user
title: Verwenden der Workflow-Aktivität „Verzweigung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Verzweigung“ verwenden.
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 66%

---


# Verzweigung {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Verzweigung  Aktivität"
>abstract="Eine **Verzweigung** erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transitionen von Verzweigungsaktivitäten"
>abstract="Standardmäßig werden zwei Transitionen mit einem **Verzweigung** -Aktivität. Klicken Sie auf **Transition hinzufügen** -Schaltfläche, um eine zusätzliche ausgehende Transition zu definieren, und geben Sie deren Titel ein."

Die **Verzweigung** -Aktivität **Flusssteuerung** -Aktivität. Sie können ausgehende Transitionen erstellen, um mehrere Aktivitäten gleichzeitig zu starten.

## Konfiguration der Verzweigung{#fork-configuration}

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

