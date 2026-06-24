---
audience: end-user
title: Verwenden der Workflow-Aktivität „Join“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Join“ verwenden
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '473'
ht-degree: 100%

---

# Join {#join}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Mehrere Workflow-Verzweigungen und Join-Aktivität"
>abstract="Mehrere Verzweigungen werden jetzt unterstützt. Anstatt eine Verzweigung zu verwenden, können Sie auf der Symbolleiste auf „Verzweigung hinzufügen“ klicken. Die Aktivität „Und-Join“ wurde ebenfalls verbessert. Es handelt sich jetzt um eine allgemeine Join-Aktivität, die es Ihnen ermöglicht, zwischen den Join-Optionen UND und ODER zu wählen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Aktivität &quot;UND-Verknüpfung&quot;"
>abstract="Die Aktivität **Und-Verknüpfung** ermöglicht es, die Ausführung verschiedener Workflow-Verzweigungen zu synchronisieren. Sie wird ausgelöst, sobald alle vorangehenden Aktivitäten beendet sind. Auf diese Weise wird sichergestellt, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie mit der Ausführung des Workflows fortfahren."

>[!CONTEXTUALHELP]
>id="acw_orchestration_join"
>title="Aktivität „Zusammenführen“"
>abstract="Mit der Aktivität **Join** können Sie mehrere eingehende Transitionen zusammenführen. Wählen Sie aus, ob der Vorgang fortgesetzt werden soll, wenn alle eingehenden Transitionen abgeschlossen sind (UND) oder wenn eine beliebige eingehende Transition abgeschlossen ist (ODER)."

Die Aktivität **Join** ist eine **Flusssteuerungsaktivität**. Sie synchronisiert mehrere Ausführungszweige eines Workflows.
Sie können auswählen, wie eingehende Transitionen ausgewertet werden sollen:

* **UND:** Wird nur fortgesetzt, nachdem alle ausgewählten eingehenden Transitionen aktiviert wurden.
* **ODER:** Wird fortgesetzt, sobald eine ausgewählte eingehende Transition aktiviert wird.

Wenn **UND** ausgewählt ist, löst diese Aktivität die ausgehende Transition erst aus, nachdem alle eingehenden Transitionen aktiviert wurden. Das heißt, sie wird aktiviert, sobald alle vorangehenden Aktivitäten beendet sind. Auf diese Weise wird sichergestellt, dass bestimmte Aktivitäten abgeschlossen sind, bevor Sie mit der Ausführung des Workflows fortfahren.

Wenn **ODER** ausgewählt ist, wird die Ausführung fortgesetzt, sobald eine der ausgewählten eingehenden Transitionen aktiviert wird. Dabei wird nicht auf jede Verzweigung gewartet.

## Konfigurieren der Join-Aktivität {#join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Zusammenführungssoptionen"
>abstract="Wählen Sie die Aktivitäten aus, die Sie verknüpfen möchten. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die Sie beibehalten möchten."

Führen Sie die folgenden Schritte aus, um die Aktivität **Join** zu konfigurieren:

1. Fügen Sie mehrere Aktivitäten wie z. B. Kanalaktivitäten hinzu, um mindestens zwei verschiedene Ausführungszweige zu bilden. Sie können einen **Verzweigung** verwenden oder einen separaten Zweig mit der Symbolleistenschaltfläche **Verzweigung hinzufügen** (+) hinzufügen. Siehe [Orchestrieren von Aktivitäten](../orchestrate-activities.md#toolbar).

   ![Screenshot mit zwei Verzweigungen.](../assets/workflow-join.png)

1. Fügen Sie eine Aktivität **Join** zu einer beliebigen Verzweigung hinzu.

   ![Screenshot mit hinzugefügter Aktivität „Join“.](../assets/workflow-join2.png)

1. Wählen Sie in den Join-Optionen **UND** oder **ODER** und klicken Sie auf **Weiter**.
1. Aktivieren Sie im Abschnitt **Zusammenführungsoptionen** alle vorherigen Aktivitäten, denen Sie beitreten möchten.
1. Wählen Sie in der Dropdown-Liste **Hauptmenge** die Population der eingehenden Transition aus, die beibehalten werden soll. Die ausgehende Transition darf nur eine der Populationen der eingehenden Transition enthalten.

   >[!NOTE]
   >
   >Das Feld **Hauptmenge** ist nur für die Join-Option **UND** verfügbar.

   ![Screenshot mit konfiguriertem Join.](../assets/workflow-join3.png)

## Beispiel {#join-example}

Das folgende Beispiel zeigt zwei Workflow-Verzweigungen mit einem E-Mail- und SMS-Versand. Die Aktivität **Join**, auf **UND** eingestellt, wird ausgelöst, wenn beide eingehenden Transitionen aktiviert werden. Push-Benachrichtigungen werden erst dann gesendet, wenn beide Sendungen abgeschlossen sind. Wenn Sie die Join-Option auf **ODER** setzen, werden die Push-Benachrichtigungen gesendet, sobald die erste eingehende Versandaktivität abgeschlossen ist.

![Beispiel eines Workflows mit zwei Verzweigungen, der den E-Mail- und SMS-Versand gefolgt von Push-Benachrichtigungen anzeigt](../assets/workflow-join4.png){zoomable="yes"}