---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
badge: label="Beta"
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: 5649745c4c1c43d8d4e02dc0fc98d0ea365fb83e
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 97%

---

# Zugriff und Verwaltung von Workflows {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="In diesem Bildschirm kannn auf die vollständige Liste der Einzel- und Kampagnen-Workflows zugegriffen und ihr aktueller Status sowie das letzte/nächste Ausführungsdatum überprüft und ein neuer Workflow erstellt werden. Navigieren Sie zum Tab &quot;Vorlagen&quot;, um auf verfügbare Workflow-Vorlagen zuzugreifen."

Das Menü **[!UICONTROL Workflows]** bietet Zugriff auf die vollständige Liste der Workflows. Diese Liste enthält die beiden **eigenständigen Workflows**, die auf diesem Bildschirm erstellt wurden, und **Kampagnen-Workflows**, die in einer Kampagne erstellt wurden.

![](assets/workflow-list.png)

Jeder Workflow in der Liste zeigt Informationen zum aktuellen [Status](#status), das letzte Mal, wann er ausgeführt oder geändert wurde, sowie das Datum und die Uhrzeit der nächsten geplanten Ausführung an.

Sie können die angezeigten Spalten anpassen, indem Sie auf das Symbol **[!UICONTROL Spalte für ein benutzerdefiniertes Layout konfigurieren]** in der oberen rechten Ecke der Liste klicken. Auf diese Weise können Sie zusätzliche Informationen zur Liste hinzufügen, z. B. die letzte fehlerhafte Aktivität eines Workflows oder die angewendete Zielgruppendimension.

Darüber hinaus stehen eine Suchleiste und Filter zur Verfügung, um die Suche innerhalb der Liste zu erleichtern. Sie können beispielsweise die Workflows so filtern, dass nur die einer Kampagne angehörenden oder die während eines bestimmten Datumsbereichs verarbeiteten Workflows angezeigt werden.

Um einen Workflow zu duplizieren oder zu löschen, klicken Sie auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **[!UICONTROL Duplizieren]** bzw. **[!UICONTROL Löschen]**.

>[!NOTE]
>
>Sie können einen laufenden Workflow duplizieren, ihn jedoch nicht löschen.

## Status von Workflows {#status}

Workflows können mehrere Status aufweisen:

* **[!UICONTROL Entwurf]**: Der Workflow wurde erstellt und gespeichert.
* **[!UICONTROL In Bearbeitung]**: Der Workflow wird derzeit ausgeführt.
* **[!UICONTROL Abgeschlossen]**: Die Ausführung des Workflows ist abgeschlossen.
* **[!UICONTROL Ausgesetzt]**: Der Workflow wurde angehalten.
* **[!UICONTROL Fehlerhaft]**: Beim Workflow ist ein Fehler aufgetreten. Öffnen Sie den Workflow und greifen Sie auf die Protokolle und Aufgaben zu, um den Fehler zu identifizieren und zu beheben. [Erfahren Sie, wie Sie Protokolle und Aufgaben überwachen.](start-monitor-workflows.md#logs-tasks)

Ausführliche Informationen zum Starten und Überwachen der Workflow-Ausführung finden Sie auf [dieser Seite](start-monitor-workflows.md).

## Workflow-Vorlagen {#templates}

Die Registerkarte **[!UICONTROL Vorlagen]** enthält alle verfügbaren Workflow-Vorlagen.

Workflow-Vorlagen enthalten vorkonfigurierte Aktivitäten und allgemeine Eigenschaftskonfigurationen, die zur Erstellung neuer Workflows wiederverwendet werden können. Sie werden über die Client-Konsole erstellt. [Erfahren Sie, wie Sie mit Vorlagen arbeiten können](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html?lang=de#workflow-templates)
