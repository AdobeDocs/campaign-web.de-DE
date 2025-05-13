---
audience: end-user
title: Verwendung der Workflow-Aktivität „Und-Verknüpfung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Und-Verknüpfung“ verwenden.
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: ht
source-wordcount: '262'
ht-degree: 100%

---

# Und-Verknüpfung {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Aktivität &quot;Und-Verknüpfung&quot;"
>abstract="Die Aktivität **Und-Verknüpfung** ermöglicht es, die Ausführung verschiedener Workflow-Verzweigungen zu synchronisieren. Sie wird ausgelöst, sobald alle vorangehenden Aktivitäten beendet sind. Auf diese Weise wird sichergestellt, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie mit der Ausführung des Workflows fortfahren."

Die Aktivität **Und-Verknüpfung** ist eine Aktivität zur **Flusskontrolle**. Sie synchronisiert mehrere Ausführungszweige eines Workflows.

Bei dieser Aktivität wird die ausgehende Transition erst aktiviert, nachdem alle eingehenden Transitionen aktiviert wurden. Das heißt, sie wird aktiviert, sobald alle vorangehenden Aktivitäten beendet sind. Auf diese Weise wird sichergestellt, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie mit der Ausführung des Workflows fortfahren.

## Konfigurieren der Aktivität „Und-Verknüpfung“ {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Zusammenführungssoptionen"
>abstract="Wählen Sie die Aktivitäten aus, die Sie verknüpfen möchten. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die Sie beibehalten möchten."

Führen Sie die folgenden Schritte aus, um die Aktivität **Und-Verknüpfung** zu konfigurieren:

![Screenshot mit der Benutzeroberfläche für die Konfiguration der Aktivität „Und-Verknüpfung“](../assets/workflow-andjoin.png)

1. Fügen Sie mehrere Aktivitäten wie z. B. Kanalaktivitäten hinzu, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Fügen Sie die Aktivität **Und-Verknüpfung** zu einer der Verzweigungen hinzu.
1. Aktivieren Sie im Abschnitt **Zusammenführungsoptionen** alle vorherigen Aktivitäten, denen Sie beitreten möchten.
1. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die beibehalten werden soll. Die ausgehende Transition darf nur eine der Populationen der eingehenden Transition enthalten.

## Beispiel {#and-join-example}

Das folgende Beispiel zeigt zwei Workflow-Verzweigungen mit einem E-Mail- und SMS-Versand. Die Und-Verknüpfung wird ausgelöst, wenn beide eingehenden Transitionen aktiviert werden. Push-Benachrichtigungen werden erst dann gesendet, wenn beide Sendungen abgeschlossen sind.

![Beispiel eines Workflows mit zwei Verzweigungen, der den E-Mail- und SMS-Versand gefolgt von Push-Benachrichtigungen anzeigt](../assets/workflow-andjoin-example.png){zoomable="yes"}