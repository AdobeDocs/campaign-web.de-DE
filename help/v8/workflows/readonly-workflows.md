---
audience: end-user
title: Über schreibgeschützte Workflows
description: Erfahren Sie, warum Workflows schreibgeschützt sind
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 21%

---

# Über schreibgeschützte Workflows {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="This workflow is read only"
>abstract="You cannot edit this workflow due to your rights or the type of the workflow."

Campaign-Benutzende haben möglicherweise eingeschränkten Zugriff auf Adobe Campaign-Daten. Ein Campaign-Administrator kann ihnen das Recht gewähren, bestimmte Funktionen anzuzeigen, sie jedoch nicht zu bearbeiten oder zu ändern. Benutzerberechtigungen für -Daten sind unerlässlich, um Daten- und Prozesssicherheit zu gewährleisten. Weitere Informationen zur Berechtigungsverwaltung in Campaign finden [ in diesem Abschnitt ](../get-started/permissions.md).

Wenn sich ein Workflow im schreibgeschützten Modus befindet, gilt Folgendes:

* Die Meldung **[!UICONTROL Schreibgeschützt]** wird neben der Schaltfläche **[!UICONTROL Einstellungen]** angezeigt.
* Die Aktionsschaltflächen sind nicht verfügbar.

![Schreibgeschützte Workflow-Benutzeroberfläche mit der Schaltfläche „Einstellungen“ und den deaktivierten Aktionsschaltflächen.](assets/readonly-workflow.png){zoomable="yes"}

In einem schreibgeschützten Workflow können Benutzende keine Änderungen vornehmen. Sie dürfen die Einstellungen der Aktivitäten nicht ändern.

![Scheduler-Oberfläche im schreibgeschützten Modus mit deaktivierten Einstellungsoptionen.](assets/scheduler-readonly.png){zoomable="yes"}

Benutzende können den Workflow nicht löschen.

![Benutzeroberfläche mit eingeschränkten Rechten zum Löschen von Workflows.](assets/readonly-rights.png){zoomable="yes"}

## Typen schreibgeschützter Workflows {#readonly-workflow-types}

Je nach Workflow-Typ kann der schreibgeschützte Modus variieren.

### Kampagnen-Workflows {#readonly-campaign-wf}

In einem schreibgeschützten Kampagnen-Workflow kann der/die Benutzende nicht auf die Schaltfläche Überwachung zugreifen.

![Campaign-Workflow-Benutzeroberfläche im schreibgeschützten Modus mit deaktivierten Überwachungsoptionen.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technische Workflows {#readonly-tech-wf}

Integrierte technische Workflows sind für alle Campaign-Benutzer (einschließlich Administratoren) schreibgeschützt. Benutzende können diese jedoch bei Bedarf **aussetzen** oder **stoppen**. Dies sind die einzigen zulässigen Aktionen.

![Technische Workflow-Oberfläche im schreibgeschützten Modus mit Optionen zum Anhalten oder Stoppen von Workflows.](assets/readonly-technical-workflow.png){zoomable="yes"}

Weiterführende Informationen zu technischen Workflows finden Sie in [diesem Abschnitt](https://experienceleague.adobe.com/de/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).