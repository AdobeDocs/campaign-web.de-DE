---
audience: end-user
title: Pläne und Programme
description: Erfahren Sie, wie Sie in Adobe Campaign Pläne und Programme erstellen und konfigurieren.
source-git-commit: f9b8c0805d816075c5ee9ea9443f50cfead371d1
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Pläne und Programme

Mit Adobe Campaign können Sie Ihre Ordnerhierarchie für Marketingpläne und -programme konfigurieren.

Um sie besser zu organisieren, empfiehlt Adobe die folgende Hierarchie: Planen `>` Programme `>` Kampagnen

* A **plan** kann mehrere Programme enthalten. Sie definiert strategische Ziele für einen bestimmten Zeitraum.
* A **program** kann andere Programme sowie Kampagnen, Workflows und Landingpages enthalten.
* A **Kampagne** kann Sendungen, Workflows und Landingpages enthalten.

## Erstellen und Konfigurieren eines Plans {#create-plan}

Um einen Plan zu erstellen, müssen Sie einen Ordner mit dem Ordnertyp erstellen **[!UICONTROL Plan]** [Erfahren Sie mehr über das Erstellen eines Ordners](create-manage-folder.md).

![](assets/plan_create.png){zoomable="yes"}

Navigieren Sie zu **[!UICONTROL Ordnereinstellungen]** von Ihrem Plan, sie zu verwalten.

![](assets/plan_settings.png){zoomable="yes"}

Sie können **[!UICONTROL Benutzerdefinierte Optionen]**, um das Planungsdatum Ihres Plans festzulegen.

![](assets/plan_options.png){zoomable="yes"}

So verwalten Sie  **[!UICONTROL Benutzerdefinierte Optionen]**:

1. Navigieren Sie zum **[!UICONTROL Schemas]**
1. Wählen Sie die **[!UICONTROL Bearbeitbar]** Schemata in den Filtern
1. Klicken Sie auf das Symbol von **[!UICONTROL Bearbeiten benutzerdefinierter Details]**

![](assets/plan_edit.png){zoomable="yes"}

Sie können sie konfigurieren:

![](assets/plan_customfields.png){zoomable="yes"}

## Programm erstellen und konfigurieren

So erstellen Sie ein Programm in Ihrem Plan ([Erfahren Sie mehr über die Erstellung eines Plans](#create-plan)), müssen Sie sich in Ihrem Plan befinden und einen Ordner mit dem Ordnertyp erstellen **[!UICONTROL Programm]** [Erfahren Sie mehr über das Erstellen eines Ordners](create-manage-folder.md).

![](assets/program_create.png){zoomable="yes"}

Navigieren Sie zu **[!UICONTROL Ordnereinstellungen]** von Ihrem Programm, um es zu verwalten.

![](assets/program_settings.png){zoomable="yes"}

Sie können **[!UICONTROL Benutzerdefinierte Optionen]**, um das Planungsdatum Ihres Programms festzulegen.

![](assets/program_options.png){zoomable="yes"}

So verwalten Sie  **[!UICONTROL Benutzerdefinierte Optionen]**:

1. Navigieren Sie zum **[!UICONTROL Schemas]**
1. Wählen Sie die **[!UICONTROL Bearbeitbar]** Schemata in den Filtern
1. Klicken Sie auf das Symbol von **[!UICONTROL Bearbeiten benutzerdefinierter Details]**

![](assets/program_edit.png){zoomable="yes"}

Sie können sie konfigurieren:

![](assets/program_customfields.png){zoomable="yes"}

## Verknüpfen einer Kampagne mit einem Programm

Sie haben zwei Möglichkeiten, eine Kampagne mit einem Programm zu verknüpfen:

### 1. Weg : Sie haben bereits ein Programm und möchten eine damit verknüpfte Kampagne erstellen

Um eine neue Kampagne mit Ihrem Programm zu verknüpfen, erstellen Sie direkt eine Kampagne im Programm :

![](assets/program_campaign_create.png){zoomable="yes"}

Die **[!UICONTROL Ordner]** -Einstellungen werden automatisch mit dem Pfad zu Ihrem Programm abgelegt.

![](assets/program_campaign_folder.png){zoomable="yes"}

### 2. Weg : Sie haben bereits eine bestehende Kampagne, die mit einem vorhandenen Programm verknüpft werden soll

Navigieren Sie zu **[!UICONTROL Einstellungen]** Schaltfläche der Kampagne, die Sie mit Ihrem Programm verknüpfen möchten:

![](assets/campaign_settings.png){zoomable="yes"}

In **[!UICONTROL Eigenschaften]**, klicken Sie auf die **[!UICONTROL Ordner]** im **[!UICONTROL Ordner]** -Einstellungen, um Ihre **[!UICONTROL Programm]** Ordner.

![](assets/campaign_folder.png){zoomable="yes"}

Wählen Sie **[!UICONTROL Programm]** Ordner und klicken Sie auf **[!UICONTROL Bestätigen]** Schaltfläche und dann auf **[!UICONTROL Speichern und schließen]** Schaltfläche.

![](assets/campaign_linked.png){zoomable="yes"}

Ihre Kampagne ist jetzt in Ihrem Programm aufgeführt:

![](assets/campaign_in_program.png){zoomable="yes"}