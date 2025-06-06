---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Workflow erstellen
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 100%

---

# Erstellen des Workflows {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Liste der Workflows in der Kampagne"
>abstract="Die Registerkarte **Workflows** enthält alle mit der Kampagne verknüpften Workflows. Klicken Sie auf den Namen eines Workflows, um ihn zu bearbeiten. Verwenden Sie die Schaltfläche **Workflow erstellen**, um einen neuen Workflow für diese Kampagne hinzuzufügen."

Sie können eigenständige Workflows oder Workflows innerhalb einer Kampagne erstellen. Der erste Schritt besteht darin, eine Vorlage auszuwählen und ihre allgemeinen Eigenschaften zu definieren. Konfigurieren Sie dann bei Bedarf weitere Einstellungen.

Gehen Sie dazu wie folgt vor:

1. Um einen **eigenständigen Workflow** zu erstellen, navigieren Sie zum Menü **Workflows**. Um einen **Kampagnen-Workflow** zu erstellen, navigieren Sie zum Menü **Kampagnen** und öffnen Sie die Kampagne, für die Sie einen neuen Workflow erstellen möchten.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Workflow erstellen]** in der rechten oberen rechten Ecke des Bildschirms.

   ![Screenshot mit der Schaltfläche „Workflow erstellen“ oben rechts im Bildschirm](assets/workflow-create.png){zoomable="yes"}

1. Wählen Sie im Dialogfeld **Eigenschaften** die Vorlage aus, die zum Erstellen des Workflows verwendet werden soll (Sie können auch die integrierte Standardvorlage verwenden). [Erfahren Sie mehr über Workflow-Vorlagen](#workflow-templates).

1. Geben Sie dem Workflow ein Label. Fügen Sie Ihrem Workflow darüber hinaus eine Beschreibung in das dedizierte Feld im Abschnitt **[!UICONTROL Weitere Optionen]** des Bildschirms hinzu.

1. Erweitern Sie den Abschnitt **[!UICONTROL Weitere Optionen]**, um weitere Einstellungen für den Workflow zu konfigurieren. Auf [dieser Seite](workflow-settings.md#properties) erfahren Sie, wie Sie die Workflow-Eigenschaften konfigurieren.

   ![Screenshot mit dem Abschnitt „Weitere Optionen“ zum Konfigurieren von Workflow-Einstellungen](assets/workflow-additional-options.png){zoomable="yes"}

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Workflow erstellen]** zur Bestätigung der Workflow-Erstellung.

Ihr Workflow wird jetzt erstellt und ist in der Liste der Workflows verfügbar. Sie können auf die zugehörige visuelle Arbeitsfläche zugreifen und mit dem Hinzufügen, Konfigurieren und Orchestrieren der Aufgaben beginnen, die ausgeführt werden sollen. [Erfahren Sie, wie Sie Workflow-Aktivitäten orchestrieren](orchestrate-activities.md)

## Arbeiten mit Workflow-Vorlagen {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Workflow-Vorlagen"
>abstract="Workflow-Vorlagen enthalten vorkonfigurierte Einstellungen und Aktivitäten, die zur Erstellung neuer Workflows wiederverwendet werden können."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="Workflow-Eigenschaften"
>abstract="Workflow-Vorlagen enthalten vorkonfigurierte Einstellungen und Aktivitäten, die zur Erstellung neuer Workflows wiederverwendet werden können. Geben Sie in diesem Bildschirm den Titel der Workflow-Vorlage ein und konfigurieren Sie die zugehörigen Einstellungen wie den internen Namen, Ordner und Ausführungsordner, die Zeitzone und die Supervisorgruppe."

Workflow-Vorlagen enthalten vorkonfigurierte Einstellungen und Aktivitäten, die zur Erstellung neuer Workflows wiederverwendet werden können. Bei der Erstellung eines Workflows wählen Sie die Vorlage Ihres Workflows aus den Workflow-Eigenschaften aus. Standardmäßig wird eine leere Vorlage bereitgestellt.

Sie können eine Vorlage aus einem vorhandenen Workflow erstellen oder eine neue Vorlage von Grund auf erstellen. Beide Methoden werden nachfolgend beschrieben.

>[!BEGINTABS]

>[!TAB Erstellen einer Vorlage aus einem vorhandenen Workflow]

Gehen Sie wie folgt vor, um eine Workflow-Vorlage aus einem vorhandenen Workflow zu erstellen:

1. Öffnen Sie das Menü **Workflows** und navigieren Sie zum Workflow, um ihn als Vorlage zu speichern.
1. Klicken Sie auf die drei Punkte rechts neben dem Namen des Workflows und wählen Sie **Als Vorlage kopieren** aus.

   ![Screenshot mit der Option „Als Vorlage kopieren“ im Workflow-Menü](assets/wf-copy-as-template.png){zoomable="yes"}

1. Bestätigen Sie im Popup-Fenster die Vorlagenerstellung.
1. Markieren Sie in der Arbeitsfläche der Workflow-Vorlage die gewünschten Aktivitäten, fügen Sie sie hinzu und konfigurieren Sie sie.
1. Navigieren Sie zu den **Einstellungen** über die gleichnamige Schaltfläche, um den Namen der Workflow-Vorlage zu ändern und eine Beschreibung einzugeben.
1. Wählen Sie den **Ordner** und den **Ausführungsordner** der Vorlage aus. Der Ordner ist der Speicherort der Workflow-Vorlage. Der Ausführungsordner ist der Ordner, in dem Workflows gespeichert werden, die auf dieser Vorlage basieren.

   ![Screenshot mit den Einstellungen für Ordner und Ausführungsordner in der Workflow-Vorlage](assets/wf-settings-template.png){zoomable="yes"}

   Die anderen Eigenschaften sind bei Workflows üblich. Weitere Informationen finden Sie auf [dieser Seite](workflow-settings.md#properties).

1. Speichern Sie Ihre Änderungen.

Die Workflow-Vorlage ist jetzt in der Vorlagenliste verfügbar. Sie können einen Workflow erstellen, der auf dieser Vorlage basiert. Dieser Workflow wird mit den in der Vorlage definierten Einstellungen und Aktivitäten vorkonfiguriert.

>[!TAB Erstellen einer Vorlage von Grund auf]

Gehen Sie wie folgt vor, um eine neue Workflow-Vorlage von Grund auf zu erstellen:

1. Öffnen Sie das Menü **Workflows** und navigieren Sie zur Registerkarte **Vorlagen**. Die Liste der verfügbaren Workflow-Vorlagen wird angezeigt.
1. Klicken Sie auf **[!UICONTROL Vorlage erstellen]** in der rechten oberen Ecke des Bildschirms.
1. Geben Sie den Titel ein und öffnen Sie die zusätzlichen Optionen, um eine Beschreibung für Ihre Workflow-Vorlage einzugeben.
1. Wählen Sie den Ordner und den Ausführungsordner der Vorlage aus. Der Ordner ist der Speicherort der Workflow-Vorlage. Der Ausführungsordner ist der Ordner, in dem Workflows gespeichert werden, die auf dieser Vorlage basieren.

   ![Screenshot zur Erstellung einer neuen Workflow-Vorlage mit den Einstellungen für Ordner und Ausführungsordner](assets/new-wf-template.png){zoomable="yes"}

   Die anderen Eigenschaften sind bei Workflows üblich. Weitere Informationen finden Sie auf [dieser Seite](workflow-settings.md#properties).

1. Klicken Sie anschließend auf die Schaltfläche **Erstellen**, um Ihre Einstellungen zu bestätigen.
1. Fügen Sie in der Arbeitsfläche der Workflow-Vorlage die gewünschten Aktivitäten hinzu und konfigurieren Sie sie nach Bedarf.

   ![Screenshot mit der Arbeitsfläche für Workflow-Vorlagen zum Hinzufügen und Konfigurieren von Aktivitäten](assets/wf-template-activities.png){zoomable="yes"}

1. Speichern Sie Ihre Änderungen.

Die Workflow-Vorlage ist jetzt in der Vorlagenliste verfügbar. Sie können einen Workflow erstellen, der auf dieser Vorlage basiert. Dieser Workflow wird mit den in der Vorlage definierten Einstellungen und Aktivitäten vorkonfiguriert.

>[!ENDTABS]