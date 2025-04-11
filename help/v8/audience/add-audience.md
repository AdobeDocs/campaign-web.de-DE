---
audience: end-user
title: Auswählen einer bestehenden Zielgruppe
description: Erfahren Sie, wie Sie eine Zielgruppe auswählen
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 57%

---

# Auswählen einer bestehenden Zielgruppe {#add-audience}

>[!CONTEXTUALHELP]
>
In diesem Abschnitt wird beschrieben, wie Sie bei der Definition der Zielgruppe eines E-Mail-Versands eine bestehende Zielgruppe auswählen. Bei der Bestimmung der Hauptzielgruppe eines Versands haben Sie außerdem folgende Möglichkeiten:
* [Erstellen einer einmaligen Zielgruppe](one-time-audience.md) mithilfe des Abfrage-Modelers.
* [Laden einer Zielgruppe aus einer externen Datei](file-audience.md) (nur für E-Mails).

Auf Zielgruppen, die in Sendungen ausgewählt werden können, kann über das Menü **Zielgruppen** links zugegriffen werden. Sie stammen aus mehreren Quellen, z. B. der Client-Konsole, Workflows für Campaign Web-Zielgruppen oder Adobe Experience Platform. [Weitere Informationen zu Zielgruppen](manage-audience.md)

Gehen Sie wie folgt vor, um eine vorhandene Zielgruppe für Ihre Nachricht auszuwählen:

1. Klicken Sie im Abschnitt **Audience** des Assistenten zur Versanderstellung auf die Schaltfläche **[!UICONTROL Audience auswählen]** und wählen Sie dann **[!UICONTROL Audience auswählen]**.

   [Dieser Screenshot zeigt die Schaltfläche **Zielgruppe auswählen** im Assistenten zur Versanderstellung.](assets/create-audience.png){zoomable="yes"}

1. Auf diesem Bildschirm werden alle bestehenden Zielgruppen für den aktuellen Ordner angezeigt.

   [Dieser Screenshot zeigt die Liste der im aktuellen Ordner vorhandenen Zielgruppen.](assets/create-audience2.png){zoomable="yes"}

   Um eine Zielgruppe aus Adobe Experience Platform auszuwählen, suchen Sie im Abschnitt „Filter“ des Bildschirms nach `AEP Audiences folder`. [Weitere Informationen zu Adobe Experience Platform-Zielgruppen](manage-audience.md#monitor)

   [Dieser Screenshot zeigt den Filterabschnitt mit dem ausgewählten AEP Audiences-Ordner.](assets/select-audience-folder.png){zoomable="yes"}

1. Im Filterbereich können Sie auf Filteroptionen zugreifen, um die Zielgruppenliste zu präzisieren. Klicken Sie auf **Regeln hinzufügen**, um auf den Abfrage-Modeler zuzugreifen, mit dem Sie erweiterte Filter für die Liste der Zielgruppen erstellen können. [So verwenden Sie den Abfrage-Modeler](../query/query-modeler-overview.md)

   Sie können z. B. eine Regel definieren, um nach der Herkunft der Zielgruppen zu filtern, wie unten dargestellt:

   [Dieser Screenshot zeigt einen Filter, der auf Zielgruppen basierend auf ihrer Herkunft angewendet wird.](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Klicken Sie auf **Bestätigen**, um Ihre Zielgruppe als Hauptzielgruppe des Versands hinzuzufügen. Anschließend können Sie die Audience mit dem Abfrage-Modellierer einschränken, indem Sie auf die Schaltfläche **Regeln bearbeiten** klicken.

   [Dieser Screenshot zeigt die Schaltfläche **Regeln bearbeiten** zum Verfeinern der Audience.](assets/refine-audience.png){zoomable="yes"}

1. Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Auf diese Weise können Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. [Weitere Informationen](control-group.md)