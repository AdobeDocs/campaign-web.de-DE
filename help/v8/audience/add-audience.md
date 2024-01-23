---
audience: end-user
title: Auswählen einer bestehenden Zielgruppe
description: Erfahren Sie, wie Sie eine Zielgruppe auswählen
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: 68c3a19122912d730b739549ed5b37e8a34a61df
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 82%

---


# Auswählen einer bestehenden Zielgruppe {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Auswählen einer bestehenden Zielgruppe"
>abstract="Durchsuchen Sie die Liste, um eine vorhandene Zielgruppe auszuwählen. Verwenden Sie das Symbol „Filter anzeigen“, um die Liste zu filtern, oder wählen Sie einen bestimmten Ordner aus."

In diesem Abschnitt wird beschrieben, wie Sie bei der Definition der Zielgruppe eines E-Mail-Versands eine bestehende Zielgruppe auswählen. Bei der Bestimmung der Hauptzielgruppe eines Versands haben Sie außerdem folgende Möglichkeiten:

* [Erstellen einer einmaligen Zielgruppe](one-time-audience.md) Verwendung des Abfragemodells.
* [Laden einer Zielgruppe aus einer externen Datei](file-audience.md) (nur für E-Mails).

Auf Zielgruppen, die in Sendungen ausgewählt werden können, kann über das Menü **Zielgruppen** links zugegriffen werden. Sie stammen aus verschiedenen Quellen, wie z. B. der Client-Konsole, den Zielgruppen-Workflows für Campaign Web oder Adobe Experience Platform. [Erfahren Sie, wie Sie Zielgruppen überwachen und verwalten.](manage-audience.md)

Gehen Sie wie folgt vor, um eine vorhandene Zielgruppe für Ihre Nachricht auszuwählen:

1. Klicken Sie im Abschnitt **Zielgruppe** des Assistenten zur Versanderstellung auf die Schaltfläche **[!UICONTROL Zielgruppe auswählen]**

   ![](assets/create-audience.png)

1. Klicken Sie auf **[!UICONTROL Zielgruppe auswählen]**, um eine bestehende Zielgruppe zu verwenden. Auf diesem Bildschirm werden alle vorhandenen Zielgruppen für den aktuellen Ordner angezeigt.

   ![](assets/create-audience2.png)

   Um eine Zielgruppe aus Adobe Experience Platform auszuwählen, navigieren Sie im Filterabschnitt des Bildschirms zum `AEP Audiences folder`.

   ![](assets/select-audience-folder.png)

1. Im Filterbereich können Sie auf Filteroptionen zugreifen, um die Zielgruppenliste zu präzisieren. Klicken Sie dazu auf **Regeln hinzufügen** , um auf das Abfragemodell zuzugreifen, mit dem Sie erweiterte Filter für die Zielgruppenliste erstellen können. [Erfahren Sie, wie Sie das Abfragemodell verwenden](../query/query-modeler-overview.md)

1. Klicken Sie auf **Bestätigen**, um Ihre Zielgruppe als Hauptzielgruppe des Versands hinzuzufügen. Danach können Sie die Audience mithilfe des Abfragemodells weiter einschränken, indem Sie auf die **Regeln bearbeiten** Schaltfläche.

   ![](assets/refine-audience.png)

   Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Dadurch lässt sich das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. [Weitere Informationen](control-group.md)
