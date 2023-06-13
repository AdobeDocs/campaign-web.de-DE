---
audience: end-user
title: Workflow-Aktivität Verzweigung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Verzweigung verwenden.
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 19%

---


# Verzweigung {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Verzweigung Aktivität"
>abstract="Eine Verzweigung erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten."

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Verzweigung** Aktivität:

1. Hinzufügen einer **Verzweigung** -Aktivität zu Ihrem Workflow hinzu.
1. Klicken **Transition hinzufügen** um eine neue ausgehende Transition hinzuzufügen. Standardmäßig sind zwei Transitionen definiert.
1. Fügen Sie jedem Ihrer Transitionen einen Titel hinzu.

## Beispiel

Im folgenden Beispiel verwenden wir zwei **Verzweigung** Aktivitäten:

* Vor den beiden Abfragen, um sie gleichzeitig auszuführen.
* Senden Sie eine E-Mail und eine SMS gleichzeitig an die Zielpopulation.

![](../assets/workflow-fork-example.png)

