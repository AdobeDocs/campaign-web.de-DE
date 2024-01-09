---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Workflow erstellen
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 6694976596909226cadbb0997c6663ec17a9e39b
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 100%

---


# Erstellen des Workflows {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workflow-Eigenschaften"
>abstract="Wählen Sie in diesem Bildschirm die Vorlage aus, die zum Erstellen des Workflows verwendet werden soll, und geben Sie einen Titel an. Erweitern Sie den Abschnitt ZUSÄTZLICHE OPTIONEN, um weitere Einstellungen wie den internen Namen des Workflows, seine Ordner, die Zeitzone und die Gruppe der Verantwortlichen zu konfigurieren. Es wird dringend empfohlen, eine Gruppe von Verantwortlichen auszuwählen, damit Benutzerinnen und Benutzer benachrichtigt werden, wenn Fehler auftreten."


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Liste der Workflows in der Kampagne"
>abstract="Die Registerkarte **Workflows** enthält alle mit der Kampagne verknüpften Workflows. Klicken Sie auf den Namen eines Workflows, um ihn zu bearbeiten. Verwenden Sie die Schaltfläche **Workflow erstellen**, um einen neuen Workflow für diese Kampagne hinzuzufügen."


Sie können eigenständige Workflows oder Workflows innerhalb einer Kampagne erstellen. Der erste Schritt besteht darin, eine Vorlage auszuwählen und ihre allgemeinen Eigenschaften zu definieren. Anschließend können Sie bei Bedarf weitere Einstellungen konfigurieren.

Gehen Sie dazu wie folgt vor:

1. Um einen **eigenständigen Workflow** zu erstellen, navigieren Sie zum Menü **Workflows**.

   Um einen **Kampagnen-Workflow** zu erstellen, navigieren Sie zum Menü **Kampagnen** und öffnen Sie die Kampagne, für die Sie einen neuen Workflow erstellen möchten.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Workflow erstellen]** in der rechten oberen rechten Ecke des Bildschirms.

   ![](assets/workflow-create.png)

1. Wählen Sie im Dialogfeld **Eigenschaften** die Vorlage aus, die zum Erstellen des Workflows verwendet werden soll (Sie können auch die integrierte Standardvorlage verwenden). Weitere Informationen zu Vorlagen finden Sie im [folgenden Abschnitt](#work-with-workflow-templates-workflow-templates).

1. Geben Sie dem Workflow einen Titel. Darüber hinaus empfehlen wir dringend, Ihrem Workflow eine Beschreibung im dedizierten Feld im Abschnitt **[!UICONTROL Zusätzliche Optionen]** des Bildschirms hinzuzufügen.

1. Erweitern Sie den Abschnitt **[!UICONTROL Zusätzliche Optionen]**, um weitere Einstellungen für den Workflow zu konfigurieren. Erfahren Sie auf [dieser Seite](workflow-settings.md#properties), wie Sie die Workflow-Eigenschaften konfigurieren.

   ![](assets/workflow-additional-options.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Workflow erstellen]** zur Bestätigung der Workflow-Erstellung.

Ihr Workflow wurde jetzt erstellt und ist in der Liste der Workflows verfügbar. Sie können jetzt auf die visuelle Arbeitsfläche zugreifen und mit dem Hinzufügen, Konfigurieren und Orchestrieren der Aufgaben beginnen, die ausgeführt werden sollen. Erfahren Sie auf [dieser Seite](orchestrate-activities.md), wie Sie Workflow-Aktivitäten orchestrieren.

## Arbeiten mit Workflow-Vorlagen {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Workflow-Vorlagen"
>abstract="Workflow-Vorlagen enthalten vorkonfigurierte Einstellungen und Aktivitäten, die zur Erstellung neuer Workflows wiederverwendet werden können."

Workflow-Vorlagen enthalten vorkonfigurierte Einstellungen und Aktivitäten, die zur Erstellung neuer Workflows wiederverwendet werden können. Bei der Erstellung eines Workflows können Sie die Vorlage Ihres Workflows aus den Workflow-Eigenschaften auswählen. Standardmäßig wird eine leere Vorlage bereitgestellt.

Sie können eine Vorlage aus einem vorhandenen Workflow erstellen oder eine neue Vorlage von Grund auf erstellen. Beide Methoden werden nachfolgend beschrieben.

>[!BEGINTABS]

>[!TAB Erstellen einer Vorlage aus einem vorhandenen Workflow]

Gehen Sie wie folgt vor, um eine Workflow-Vorlage aus einem vorhandenen Workflow zu erstellen:

1. Öffnen Sie das Menü **Workflows** und navigieren Sie zum Workflow, um ihn als Vorlage zu speichern.
1. Klicken Sie auf die drei Punkte rechts neben dem Namen des Workflows und wählen Sie **Als Vorlage kopieren** aus.

   ![](assets/wf-copy-as-template.png)

1. Bestätigen Sie im Popup-Fenster die Vorlagenerstellung.
1. Markieren Sie in der Arbeitsfläche der Workflow-Vorlage die gewünschten Aktivitäten, fügen Sie sie hinzu und konfigurieren Sie sie.
1. Navigieren Sie zu den **Einstellungen** über die gleichnamige Schaltfläche, um den Namen der Workflow-Vorlage zu ändern und eine Beschreibung einzugeben.
1. Wählen Sie den **Ordner** und den **Ausführungsordner** der Vorlage aus. Der Ordner ist der Speicherort der Workflow-Vorlage. Der Ausführungsordner ist der Ordner, in dem Workflows gespeichert werden, die auf dieser Vorlage basieren.

   ![](assets/wf-settings-template.png)

   Die anderen Eigenschaften sind bei Workflows üblich. Weitere Informationen finden Sie auf [dieser Seite](workflow-settings.md#properties).

1. Speichern Sie Ihre Änderungen.

Die Workflow-Vorlage ist jetzt in der Vorlagenliste verfügbar. Sie können einen Workflow erstellen, der auf dieser Vorlage basiert. Dieser Workflow wird mit den in der Vorlage definierten Einstellungen und Aktivitäten vorkonfiguriert.


>[!TAB Erstellen einer Vorlage von Grund auf]


Gehen Sie wie folgt vor, um eine neue Workflow-Vorlage von Grund auf zu erstellen:

1. Öffnen Sie das Menü **Workflows** und navigieren Sie zur Registerkarte **Vorlagen**. Die Liste der verfügbaren Workflow-Vorlagen wird angezeigt.
1. Klicken Sie auf **[!UICONTROL Vorlage erstellen]** in der rechten oberen Ecke des Bildschirms.
1. Geben Sie den Titel ein und öffnen Sie die zusätzlichen Optionen, um eine Beschreibung für Ihre Workflow-Vorlage einzugeben.
1. Wählen Sie den Ordner und den Ausführungsordner der Vorlage aus. Der Ordner ist der Speicherort der Workflow-Vorlage. Der Ausführungsordner ist der Ordner, in dem Workflows gespeichert werden, die auf dieser Vorlage basieren.

   ![](assets/new-wf-template.png)

   Die anderen Eigenschaften sind bei Workflows üblich. Weitere Informationen finden Sie auf [dieser Seite](workflow-settings.md#properties).

1. Klicken Sie anschließend auf die Schaltfläche **Erstellen**, um Ihre Einstellungen zu bestätigen.
1. Fügen Sie in der Arbeitsfläche der Workflow-Vorlage die gewünschten Aktivitäten hinzu und konfigurieren Sie sie nach Bedarf.

   ![](assets/wf-template-activities.png)

1. Speichern Sie Ihre Änderungen.

Die Workflow-Vorlage ist jetzt in der Vorlagenliste verfügbar. Sie können einen Workflow erstellen, der auf dieser Vorlage basiert. Dieser Workflow wird mit den in der Vorlage definierten Einstellungen und Aktivitäten vorkonfiguriert.

>[!ENDTABS]
