---
audience: end-user
title: Pläne und Programme
description: Erfahren Sie, wie Sie Pläne und Programme in Adobe Campaign erstellen und konfigurieren können.
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 100%

---

# Pläne und Programme {#plan-and-programs}

Adobe Campaign ermöglicht Ihnen das Konfigurieren Ihrer Ordnerhierarchie für Marketing-Pläne und -Programme.

Um sie besser zu organisieren, empfiehlt Adobe die folgende Hierarchie: Plan `>` Programme `>` Kampagnen.

* Ein **Plan** kann mehrere Programme enthalten. Er definiert strategische Ziele für einen bestimmten Zeitraum.
* Ein **Programm** kann weitere Programme, Kampagnen, Workflows und Landingpages enthalten.
* Eine **Kampagne** kann Sendungen, Workflows und Landingpages enthalten.

## Erstellen und Konfigurieren eines Plans {#create-plan}

Um einen Plan zu erstellen, müssen Sie einen Ordner mit dem Ordnertyp **[!UICONTROL Plan]** erstellen. [Erfahren Sie mehr über das Erstellen eines Ordners](../get-started/work-with-folders.md).

![](assets/plan_create.png){zoomable="yes"}

Navigieren Sie zu den **[!UICONTROL Ordnereinstellungen]** Ihres Plans, um ihn zu verwalten.

![](assets/plan_settings.png){zoomable="yes"}

Sie können **[!UICONTROL benutzerdefinierte Optionen]** definieren, um das Planungsdatum Ihres Plans festzulegen.

![](assets/plan_options.png){zoomable="yes"}

Verwalten der **[!UICONTROL benutzerdefinierten Optionen]**:

1. Navigieren Sie zu den **[!UICONTROL Schemata]**
1. Wählen Sie in den Filtern die **[!UICONTROL bearbeitbaren]** Schemata aus.
1. Klicken Sie auf das Symbol **[!UICONTROL Benutzerdefinierte Details bearbeiten]**

![](assets/plan_edit.png){zoomable="yes"}

Sie können sie konfigurieren:

![](assets/plan_customfields.png){zoomable="yes"}

## Erstellen und Konfigurieren eines Programms

Um ein Programm in Ihrem Plan zu erstellen ([hier erfahren Sie mehr über das Erstellen eines Plans](#create-plan)), müssen Sie sich in Ihrem Plan befinden und einen Ordner mit dem Ordnertyp **[!UICONTROL Programm]** erstellen. [Hier erfahren Sie mehr über das Erstellen eines Ordners](../get-started/work-with-folders.md).

![](assets/program_create.png){zoomable="yes"}

Navigieren Sie zu den **[!UICONTROL Ordnereinstellungen]** Ihres Programms, um es zu verwalten.

![](assets/program_settings.png){zoomable="yes"}

Sie können **[!UICONTROL benutzerdefinierte Optionen]** definieren, um das Planungsdatum Ihres Programms festzulegen.

![](assets/program_options.png){zoomable="yes"}

So verwalten Sie die **[!UICONTROL benutzerdefinierten Optionen]**:

1. Navigieren Sie zu den **[!UICONTROL Schemata]**
1. Wählen Sie in den Filtern die **[!UICONTROL bearbeitbaren]** Schemata aus.
1. Klicken Sie auf das Symbol **[!UICONTROL Benutzerdefinierte Details bearbeiten]**

![](assets/program_edit.png){zoomable="yes"}

Sie können sie konfigurieren:

![](assets/program_customfields.png){zoomable="yes"}

## Verknüpfen einer Kampagne mit einem Programm

Sie haben zwei Möglichkeiten, eine Kampagne mit einem Programm zu verknüpfen:

### Möglichkeit 1: Sie verfügen bereits über ein Programm und möchten eine damit verknüpfte Kampagne erstellen.

Um eine neue Kampagne mit Ihrem Programm zu verknüpfen, erstellen Sie Ihre Kampagne direkt im Programm:

![](assets/program_campaign_create.png){zoomable="yes"}

Die **[!UICONTROL Ordnereinstellungen]** werden automatisch mit dem Pfad zu Ihrem Programm gespeichert.

![](assets/program_campaign_folder.png){zoomable="yes"}

### Möglichkeit 2: Sie verfügen bereits über eine bestehende Kampagne und möchten sie mit einem vorhandenen Programm verknüpfen.

Navigieren Sie zur Schaltfläche **[!UICONTROL Einstellungen]** der Kampagne, die Sie mit Ihrem Programm verknüpfen möchten:

![](assets/campaign_settings.png){zoomable="yes"}

Klicken Sie in ihren **[!UICONTROL Eigenschaften]** auf das Symbol **[!UICONTROL Ordner]** in den **[!UICONTROL Ordnereinstellungen]**, um Ihren **[!UICONTROL Programmordner]** zu wählen.

![](assets/campaign_folder.png){zoomable="yes"}

Wählen Sie Ihren **[!UICONTROL Programmordner]** aus und klicken Sie auf die Schaltfläche **[!UICONTROL Bestätigen]** und dann auf die Schaltfläche **[!UICONTROL Speichern und schließen]**.

![](assets/campaign_linked.png){zoomable="yes"}

Ihre Kampagne wird jetzt in Ihrem Programm aufgeführt:

![](assets/campaign_in_program.png){zoomable="yes"}
