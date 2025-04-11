---
audience: end-user
title: Verwendung der Workflow-Aktivität „Und-Verknüpfung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Und-Verknüpfung“ verwenden.
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 45%

---

# Und-Verknüpfung {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Aktivität &quot;Und-Verknüpfung&quot;"
>abstract="Die Aktivität **Und-Verknüpfung** ermöglicht es, die Ausführung verschiedener Workflow-Verzweigungen zu synchronisieren. Sie wird ausgelöst, sobald alle vorangehenden Aktivitäten beendet sind. Dadurch wird sichergestellt, dass bestimmte Aktivitäten abgeschlossen sind, bevor der Workflow ausgeführt wird."

Die Aktivität **Und-Verknüpfung** ist eine Aktivität zur **Flusskontrolle**. Es synchronisiert mehrere Ausführungszweige eines Workflows.

Die ausgehende Transition wird erst Trigger, nachdem alle eingehenden Transitionen aktiviert wurden. Mit anderen Worten, sie wird aktiviert, sobald alle vorherigen Aktivitäten abgeschlossen sind. Dadurch wird sichergestellt, dass bestimmte Aktivitäten abgeschlossen sind, bevor der Workflow ausgeführt wird.

## Konfigurieren der Aktivität „Und-Verknüpfung“ {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Zusammenführungssoptionen"
>abstract="Wählen Sie die Aktivitäten aus, die Sie verknüpfen möchten. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die Sie beibehalten möchten."

Führen Sie die folgenden Schritte aus, um die Aktivität **Und-Verknüpfung** zu konfigurieren:

![Screenshot der Konfigurationsoberfläche für die Aktivität „Und-Verknüpfung“.](../assets/workflow-andjoin.png)

1. Fügen Sie mehrere Aktivitäten hinzu, z. B. Kanalaktivitäten, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Fügen Sie die Aktivität **Und-Verknüpfung** zu einer der Verzweigungen hinzu.
1. Aktivieren Sie **Abschnitt „Zusammenführungsoptionen** alle vorherigen Aktivitäten, die Sie zusammenführen möchten.
1. Wählen Sie in der Dropdown-**** Primär die Population der eingehenden Transition aus, die beibehalten werden soll. Die ausgehende Transition darf nur eine der Populationen der eingehenden Transition enthalten.

## Beispiel {#and-join-example}

Das folgende Beispiel zeigt zwei Workflow-Verzweigungen mit einem E-Mail- und SMS-Versand. Die UND-Verknüpfungs-Trigger, wenn beide eingehenden Transitionen aktiviert sind. Push-Benachrichtigungen werden erst gesendet, nachdem beide Sendungen abgeschlossen sind.

![Beispiel eines Workflows mit zwei Verzweigungen, der den E-Mail- und SMS-Versand gefolgt von Push-Benachrichtigungen anzeigt.](../assets/workflow-andjoin-example.png){zoomable="yes"}