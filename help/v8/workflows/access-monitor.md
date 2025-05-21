---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 100%

---

# Zugriff und Verwaltung von Workflows {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="In diesem Bildschirm kannn auf die vollständige Liste der Einzel- und Kampagnen-Workflows zugegriffen und ihr aktueller Status sowie das letzte/nächste Ausführungsdatum überprüft und ein neuer Workflow erstellt werden. Zur Registerkarte „Vorlage“ navigieren, um auf verfügbare Workflow-Vorlagen zuzugreifen."

Das Menü **[!UICONTROL Workflows]** bietet Zugriff auf die vollständige Liste der Workflows. Diese Liste enthält die beiden **eigenständigen Workflows**, die auf diesem Bildschirm erstellt wurden, und **Kampagnen-Workflows**, die in einer Kampagne erstellt wurden.

![Bildschirm der Workflow-Liste mit eigenständigen und Kampagnen-Workflows](assets/workflow-list.png){zoomable="yes"}

Jeder Workflow in der Liste zeigt Informationen zum aktuellen [Status](#status), das letzte Mal, wann er ausgeführt oder geändert wurde, sowie das Datum und die Uhrzeit der nächsten geplanten Ausführung an.

Passen Sie die angezeigten Spalten an, indem Sie auf das Symbol **[!UICONTROL Spalte für ein benutzerdefiniertes Layout konfigurieren]** in der oberen rechten Ecke der Liste klicken. Auf diese Weise können Sie zusätzliche Informationen zur Liste hinzufügen, z. B. die letzte fehlerhafte Aktivität eines Workflows oder die angewendete Zielgruppendimension.

Darüber hinaus stehen eine Suchleiste und Filter zur Verfügung, um die Suche innerhalb der Liste zu vereinfachen. Filtern Sie beispielsweise die Workflows so, dass nur die einer Kampagne angehörenden oder die während eines bestimmten Datumsbereichs verarbeiteten Workflows angezeigt werden.

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

Workflow-Vorlagen enthalten vorkonfigurierte Aktivitäten und allgemeine Eigenschaftskonfigurationen, die zur Erstellung neuer Workflows wiederverwendet werden können. 

Erstellen Sie Workflow-Vorlagen aus einem vorhandenen Workflow oder von Grund auf neu. [So erstellen Sie Workflow-Vorlagen](create-workflow.md#workflow-templates)