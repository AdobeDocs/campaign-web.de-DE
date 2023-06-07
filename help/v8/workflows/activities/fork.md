---
audience: end-user
title: Workflow-Aktivität Verzweigung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Verzweigung verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---


# Verzweigung {#fork}

Die **Verzweigung** -Aktivität **Flusssteuerung** Aktivität. Sie können ausgehende Transitionen erstellen, um mehrere Aktivitäten gleichzeitig zu starten.

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

