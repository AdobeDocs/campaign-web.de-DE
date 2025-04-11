---
audience: end-user
title: Pläne und Programme
description: Erfahren Sie, wie Sie Pläne und Programme in Adobe Campaign erstellen und konfigurieren können.
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 23%

---

# Pläne und Programme {#plan-and-programs}

Adobe Campaign ermöglicht Ihnen das Konfigurieren Ihrer Ordnerhierarchie für Marketing-Pläne und -Programme.

Um diese Komponenten besser zu organisieren, empfiehlt Adobe die folgende Hierarchie: `>` planen `>` Kampagnen.

* Ein **Plan** kann mehrere Programme enthalten. Sie definiert strategische Ziele für einen bestimmten Zeitraum.
* Ein **Programm** kann andere Programme sowie Kampagnen, Workflows und Landingpages enthalten.
* Eine **Kampagne** kann Sendungen, Workflows und Landingpages enthalten.

## Erstellen und Konfigurieren eines Plans {#create-plan}

Um einen Plan zu erstellen, erstellen Sie einen Ordner mit dem Ordnertyp **[!UICONTROL Plan]**. [Weitere Informationen zum Erstellen eines Ordners](../get-started/work-with-folders.md)

![Screenshot zur Erstellung eines Planungsordners](assets/plan_create.png){zoomable="yes"}

Navigieren Sie zu den **[!UICONTROL Ordnereinstellungen]** Ihres Plans, um ihn zu verwalten.

![Screenshot mit den Ordnereinstellungen für einen Plan](assets/plan_settings.png){zoomable="yes"}

Definieren Sie **[!UICONTROL Benutzerdefinierte Optionen]** und legen Sie das Planungsdatum Ihres Plans fest.

![Screenshot mit den benutzerdefinierten Optionen für einen Plan](assets/plan_options.png){zoomable="yes"}

So verwalten Sie die **[!UICONTROL benutzerdefinierten Optionen]**:

1. Navigieren Sie zu **[!UICONTROL Schemata]**.
1. Wählen Sie die **[!UICONTROL bearbeitbaren]** Schemata in den Filtern aus.
1. Klicken Sie auf **[!UICONTROL Symbol Benutzerdefinierte]** bearbeiten .

![Screenshot zur Bearbeitung benutzerdefinierter Details für einen Plan](assets/plan_edit.png){zoomable="yes"}

Konfigurieren Sie die benutzerdefinierten Optionen:

![Screenshot der Konfiguration von benutzerdefinierten Feldern für einen Plan](assets/plan_customfields.png){zoomable="yes"}

## Erstellen und Konfigurieren eines Programms

Um ein Programm in Ihrem Plan zu erstellen ([Weitere Informationen zum Erstellen eines Plans](#create-plan), navigieren Sie zu Ihrem Plan und erstellen Sie einen Ordner mit dem Ordnertyp **[!UICONTROL Programm]**. [Weitere Informationen zum Erstellen eines Ordners](../get-started/work-with-folders.md).

![Screenshot zur Erstellung eines Programmordners](assets/program_create.png){zoomable="yes"}

Navigieren Sie zu den **[!UICONTROL Ordnereinstellungen]** Ihres Programms, um es zu verwalten.

![Screenshot mit den Ordnereinstellungen für ein Programm](assets/program_settings.png){zoomable="yes"}

Definieren Sie **[!UICONTROL Benutzerdefinierte Optionen]** und legen Sie das Planungsdatum Ihres Programms fest.

![Screenshot mit den benutzerdefinierten Optionen für ein Programm](assets/program_options.png){zoomable="yes"}

So verwalten Sie die **[!UICONTROL benutzerdefinierten Optionen]**:

1. Navigieren Sie zu **[!UICONTROL Schemata]**.
1. Wählen Sie die **[!UICONTROL bearbeitbaren]** Schemata in den Filtern aus.
1. Klicken Sie auf **[!UICONTROL Symbol Benutzerdefinierte]** bearbeiten .

![Screenshot zur Bearbeitung benutzerdefinierter Details für ein Programm](assets/program_edit.png){zoomable="yes"}

Konfigurieren Sie die benutzerdefinierten Optionen:

![Screenshot der Konfiguration von benutzerdefinierten Feldern für ein Programm](assets/program_customfields.png){zoomable="yes"}

## Verknüpfen einer Kampagne mit einem Programm

Sie haben zwei Möglichkeiten, eine Kampagne mit einem Programm zu verknüpfen:

### Möglichkeit 1: Sie verfügen bereits über ein Programm und möchten eine damit verknüpfte Kampagne erstellen.

Um eine neue Kampagne mit Ihrem Programm zu verknüpfen, erstellen Sie die Kampagne direkt im Programm.

![Screenshot zur Erstellung einer Kampagne innerhalb eines Programms](assets/program_campaign_create.png){zoomable="yes"}

Die **[!UICONTROL Ordner]**-Einstellungen werden automatisch mit dem Pfad zu Ihrem Programm aufgefüllt.

![Screenshot mit den Ordnereinstellungen für eine mit einem Programm verknüpfte Kampagne](assets/program_campaign_folder.png){zoomable="yes"}

### Möglichkeit 2: Sie verfügen bereits über eine bestehende Kampagne und möchten sie mit einem vorhandenen Programm verknüpfen.

Klicken Sie auf die **[!UICONTROL Einstellungen]** der Kampagne, die Sie mit Ihrem Programm verknüpfen möchten.

![Screenshot mit der Schaltfläche „Einstellungen“ für eine Kampagne](assets/campaign_settings.png){zoomable="yes"}

Klicken Sie in **[!UICONTROL Eigenschaften]** auf das Symbol **[!UICONTROL Ordner]** in den **[!UICONTROL Ordner]**-Einstellungen, um Ihren Ordner **[!UICONTROL Programm]** auszuwählen.

![Screenshot mit der Ordnerauswahl zum Verknüpfen einer Kampagne mit einem Programm](assets/campaign_folder.png){zoomable="yes"}

Wählen Sie **[!UICONTROL Ordner]** Programm“ aus, klicken Sie auf die Schaltfläche **[!UICONTROL Bestätigen]** und klicken Sie anschließend auf die Schaltfläche **[!UICONTROL Speichern und schließen]**.

![Screenshot einer mit einem Programm verknüpften Kampagne](assets/campaign_linked.png){zoomable="yes"}

Ihre Kampagne ist jetzt in Ihrem Programm aufgeführt.

![Screenshot einer in einem Programm aufgelisteten Kampagne](assets/campaign_in_program.png){zoomable="yes"}