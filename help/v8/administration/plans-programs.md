---
audience: end-user
title: Pläne und Programme
description: Erfahren Sie, wie Sie Pläne und Programme in Adobe Campaign erstellen und konfigurieren können.
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 1a751aed6d5185e700dafb1de2afd88300dfcd79
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 96%

---

# Pläne und Programme {#plan-and-programs}

Adobe Campaign ermöglicht Ihnen das Konfigurieren Ihrer Ordnerhierarchie für Marketing-Pläne und -Programme.

Um diese Komponenten besser zu organisieren, empfiehlt Adobe die folgende Hierarchie: Plan `>` Programme `>` Kampagnen.

* Ein **Plan** kann mehrere Programme enthalten. Er definiert strategische Ziele für einen bestimmten Zeitraum.
* Ein **Programm** kann sowohl weitere Programme als auch Kampagnen, Workflows und Landingpages enthalten.
* Eine **Kampagne** kann Sendungen, Workflows und Landingpages enthalten.

## Erstellen und Konfigurieren eines Plans {#create-plan}

Um einen Plan zu erstellen, erstellen Sie einen Ordner mit dem Ordnertyp **[!UICONTROL Plan]**. [Weitere Informationen zum Erstellen eines Ordners](../get-started/work-with-folders.md)

![Screenshot zur Erstellung eines Ordners vom Typ „Plan“](assets/plan_create.png){zoomable="yes"}

Navigieren Sie zu den **[!UICONTROL Ordnereinstellungen]** Ihres Plans, um ihn zu verwalten.

![Screenshot mit den Ordnereinstellungen für einen Plan](assets/plan_settings.png){zoomable="yes"}

Sie können **[!UICONTROL benutzerdefinierte Optionen]** definieren und das Planungsdatum für Ihren Plan festlegen.

![Screenshot mit den benutzerdefinierten Optionen für einen Plan](assets/plan_options.png){zoomable="yes"}

So verwalten Sie die **[!UICONTROL benutzerdefinierten Optionen]**:

1. Navigieren Sie zu den **[!UICONTROL Schemata]**.
1. Wählen Sie mit den Filtern die **[!UICONTROL bearbeitbaren]** Schemata aus.
1. Klicken Sie auf das Schema.

![Screenshot zur Bearbeitung benutzerdefinierter Details für einen Plan](assets/plan_edit.png){zoomable="yes"}

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**.

   ![](assets/plan_edit2.png){zoomable="yes"}

Konfigurieren Sie die benutzerdefinierten Optionen:

![Screenshot zur Konfiguration von benutzerdefinierten Feldern für einen Plan](assets/plan_customfields.png){zoomable="yes"}

## Erstellen und Konfigurieren eines Programms

Um ein Programm in Ihrem Plan zu erstellen ([weitere Informationen zum Erstellen eines Plans](#create-plan)), navigieren Sie zu Ihrem Plan und erstellen Sie einen Ordner mit dem Ordnertyp **[!UICONTROL Programm]**. [Erfahren Sie mehr zum Erstellen eines Ordners](../get-started/work-with-folders.md).

![Screenshot zur Erstellung eines Programmordners](assets/program_create.png){zoomable="yes"}

Navigieren Sie zu den **[!UICONTROL Ordnereinstellungen]** Ihres Programms, um es zu verwalten.

![Screenshot mit den Ordnereinstellungen für ein Programm](assets/program_settings.png){zoomable="yes"}

Sie können **[!UICONTROL benutzerdefinierte Optionen]** definieren und das Planungsdatum für Ihr Programm festlegen.

![Screenshot mit den benutzerdefinierten Optionen für ein Programm](assets/program_options.png){zoomable="yes"}

So verwalten Sie die **[!UICONTROL benutzerdefinierten Optionen]**:

1. Navigieren Sie zu den **[!UICONTROL Schemata]**.
1. Wählen Sie mit den Filtern die **[!UICONTROL bearbeitbaren]** Schemata aus.
1. Klicken Sie auf das Schema.

![Screenshot zur Bearbeitung benutzerdefinierter Details für ein Programm](assets/program_edit.png){zoomable="yes"}

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**.

   ![](assets/program_edit2.png){zoomable="yes"}

Konfigurieren Sie die benutzerdefinierten Optionen:

![Screenshot zur Konfiguration von benutzerdefinierten Feldern für ein Programm](assets/program_customfields.png){zoomable="yes"}

## Verknüpfen einer Kampagne mit einem Programm

Sie haben zwei Möglichkeiten, eine Kampagne mit einem Programm zu verknüpfen:

### Möglichkeit 1: Sie verfügen bereits über ein Programm und möchten eine damit verknüpfte Kampagne erstellen.

Um eine neue Kampagne mit Ihrem Programm zu verknüpfen, erstellen Sie die Kampagne direkt im Programm:

![Screenshot zur Erstellung einer Kampagne innerhalb eines Programms](assets/program_campaign_create.png){zoomable="yes"}

Die **[!UICONTROL Ordnereinstellungen]** werden automatisch mit dem Pfad zu Ihrem Programm aufgefüllt.

![Screenshot mit den Ordnereinstellungen für eine mit einem Programm verknüpfte Kampagne](assets/program_campaign_folder.png){zoomable="yes"}

### Möglichkeit 2: Sie verfügen bereits über eine bestehende Kampagne und möchten sie mit einem vorhandenen Programm verknüpfen.

Navigieren Sie zur Schaltfläche **[!UICONTROL Einstellungen]** der Kampagne, die Sie mit Ihrem Programm verknüpfen möchten:

![Screenshot mit der Schaltfläche „Einstellungen“ für eine Kampagne](assets/campaign_settings.png){zoomable="yes"}

Klicken Sie in ihren **[!UICONTROL Eigenschaften]** auf das Symbol **[!UICONTROL Ordner]** unter den **[!UICONTROL Ordnereinstellungen]**, um Ihren **[!UICONTROL Programmordner]** zu wählen.

![Screenshot mit der Ordnerauswahl zum Verknüpfen einer Kampagne mit einem Programm](assets/campaign_folder.png){zoomable="yes"}

Wählen Sie Ihren **[!UICONTROL Programmordner]** aus, klicken Sie auf die Schaltfläche **[!UICONTROL Bestätigen]** und dann auf die Schaltfläche **[!UICONTROL Speichern und schließen]**.

![Screenshot einer mit einem Programm verknüpften Kampagne](assets/campaign_linked.png){zoomable="yes"}

Ihre Kampagne wird jetzt in Ihrem Programm aufgeführt.

![Screenshot einer in einem Programm aufgelisteten Kampagne](assets/campaign_in_program.png){zoomable="yes"}