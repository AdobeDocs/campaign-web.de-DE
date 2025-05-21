---
audience: end-user
title: Über schreibgeschützte Workflows
description: Erfahren Sie, warum Workflows schreibgeschützt sind
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 100%

---

# Über schreibgeschützte Workflows {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Dieser Workflow ist schreibgeschützt"
>abstract="Sie können diesen Workflow aufgrund Ihrer Berechtigungen oder des Typs des Workflows nicht bearbeiten."

Einige Workflows sind schreibgeschützt. Integrierte technische Workflows sind immer schreibgeschützt, allerdings kann diese Einschränkung auch für andere Workflow-Typen gelten.

Campaign-Benutzende haben möglicherweise eingeschränkten Zugriff auf Adobe Campaign-Daten. Campaign-Admins können ihnen das Recht gewähren, bestimmte Funktionen anzuzeigen, aber ohne diese bearbeiten oder ändern zu dürfen. Benutzerberechtigungen für Daten sind für Daten- und Prozesssicherheit von entscheidender Bedeutung. Weitere Informationen zum Verwalten von Berechtigungen finden Sie in [diesem Abschnitt](../get-started/permissions.md).

Wenn sich ein Workflow im schreibgeschützten Modus befindet, gilt Folgendes:

* Die Kennzeichnung **[!UICONTROL Schreibgeschützt]** ist neben der Schaltfläche **[!UICONTROL Einstellungen]** zu finden.
* Die Aktionsschaltflächen sind nicht verfügbar

![Schreibgeschützte Workflow-Oberfläche mit der Schaltfläche „Einstellungen“ und deaktivierten Aktionsschaltflächen](assets/readonly-workflow.png){zoomable="yes"}

In einem schreibgeschützten Workflow können Benutzende keine Änderungen vornehmen. Sie sind nicht berechtigt, die Einstellungen der Aktivitäten zu ändern.

![Planungsoberfläche im schreibgeschützten Modus mit deaktivierten Einstellungsoptionen](assets/scheduler-readonly.png){zoomable="yes"}

Benutzende können den Workflow nicht löschen.

![Benutzeroberfläche mit eingeschränkten Rechten zum Löschen von Workflows](assets/readonly-rights.png){zoomable="yes"}

## Typen schreibgeschützter Workflows {#readonly-workflow-types}

Je nach Workflow-Typ kann der schreibgeschützte Modus variieren.

### Kampagnen-Workflows {#readonly-campaign-wf}

Bei einem schreibgeschützten Kampagnen-Workflow können Benutzende nicht auf die Überwachungsschaltfläche zugreifen.

![Campaign-Workflow-Oberfläche im schreibgeschützten Modus mit deaktivierten Überwachungsoptionen](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technische Workflows {#readonly-tech-wf}

Integrierte technische Workflows sind für alle Campaign-Benutzenden schreibgeschützt, auch für Admins. Benutzende können diese jedoch bei Bedarf **aussetzen** oder **stoppen**. Dies sind die einzigen zulässigen Aktionen.

![Technische Workflow-Oberfläche im schreibgeschützten Modus mit Optionen zum Aussetzen oder Stoppen von Workflows](assets/readonly-technical-workflow.png){zoomable="yes"}

Weiterführende Informationen zu technischen Workflows finden Sie in [diesem Abschnitt](https://experienceleague.adobe.com/de/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).