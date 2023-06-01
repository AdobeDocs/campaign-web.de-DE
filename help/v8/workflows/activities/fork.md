---
audience: end-user
title: Workflow-Aktivität Verzweigung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Verzweigung verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 31%

---


# Verzweigung {#fork}

Eine **Verzweigung** erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten.

Die Aktivität **Verzweigung** ermöglicht insbesondere die unabhängige Ausführung verschiedener Aktivitäten innerhalb desselben Workflows.

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

