---
audience: end-user
title: Verwendung der Workflow-Aktivität „Und-Verknüpfung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Und-Verknüpfung“ verwenden.
badge: label="Beta"
source-git-commit: f5d2cb68b3df42105da9d6b346e6e9c57e14723a
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 83%

---


# Und-Verknüpfung {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Aktivität &quot;UND-Verknüpfung&quot;"
>abstract="Die Aktivität **Und-Verknüpfung** ermöglicht es, die Ausführung verschiedener Workflow-Verzweigungen zu synchronisieren. Sie wird ausgelöst, sobald alle vorangehenden Aktivitäten beendet sind. Auf diese Weise können Sie sicherstellen, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie den Workflow weiter ausführen."

Die Aktivität **Und-Verknüpfung** ist eine Aktivität zur **Flusskontrolle**. Sie ermöglicht es, die Ausführung verschiedener Workflow-Verzwweigungen zu synchronisieren.

Bei dieser Aktivität wird die ausgehende Transition erst aktiviert, wenn alle eingehenden Transitionen aktiviert wurden, d. h. wenn alle vorangehenden Aktivitäten beendet sind. Auf diese Weise können Sie sicherstellen, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie mit der Ausführung des Workflows fortfahren.

## Konfigurieren der Aktivität Und-Verknüpfung{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Konfigurieren der Und-Verknüpfung"
>abstract="Wählen Sie die Aktivitäten aus, denen Sie beitreten möchten. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die Sie beibehalten möchten."

Führen Sie die folgenden Schritte aus, um die Aktivität **Und-Verknüpfung** zu konfigurieren:

![](../assets/workflow-andjoin.png)

1. Fügen Sie mehrere Aktivitäten wie z. B. Kanalaktivitäten hinzu, um mindestens zwei verschiedene Ausführungsverzweigungen zu bilden.
1. Fügen Sie die Aktivität **Und-Verknüpfung** zu einer der Verzweigungen hinzu.
1. Aktivieren Sie im Abschnitt **Zusammenführungsoptionen** alle vorherigen Aktivitäten, denen Sie beitreten möchten.
1. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die Sie beibehalten möchten. Die ausgehende Transition darf nur eine der Populationen der eingehenden Transition enthalten.

## Beispiel{#and-join-example}

Das folgende Beispiel zeigt zwei Workflow-Verzweigungen mit einem E-Mail- und SMS-Versand. Die Und-Verknüpfung wird ausgelöst, wenn beide eingehenden Transitionen aktiviert sind. Die Push-Benachrichtigungen werden erst dann gesendet, wenn beide Sendungen abgeschlossen sind.

![](../assets/workflow-andjoin-example.png)