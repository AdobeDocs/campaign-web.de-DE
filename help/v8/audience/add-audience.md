---
audience: end-user
title: Auswählen einer bestehenden Zielgruppe
description: Erfahren Sie, wie Sie eine Zielgruppe auswählen
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: d05b6f9fec0e56f90d3fe51014fc11d2ed87bb66
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 88%

---


# Auswählen einer bestehenden Zielgruppe {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Auswählen einer bestehenden Zielgruppe"
>abstract="Durchsuchen Sie die Liste, um eine vorhandene Zielgruppe auszuwählen. Verwenden Sie das Symbol „Filter anzeigen“, um die Liste zu filtern, oder wählen Sie einen bestimmten Ordner aus."

In diesem Abschnitt wird beschrieben, wie Sie bei der Definition der Zielgruppe eines E-Mail-Versands eine bestehende Audience auswählen.

Außerdem haben Sie folgende Möglichkeiten:

* Erstellen Sie eine neue Zielgruppe. [Weitere Informationen](segment-builder.md)
* Laden Sie eine Zielgruppe aus einer externen Datei (nur für E-Mails). [Weitere Informationen](file-audience.md)
* Verwenden Sie eine Adobe Experience Platform-Audience. [Weitere Informationen](aep-audience.md).


Gehen Sie wie folgt vor, um eine vorhandene Audience für Ihre Nachricht auszuwählen:

1. Klicken Sie im Abschnitt **Audience** des Assistenten zur Versanderstellung auf die Schaltfläche **[!UICONTROL Audience auswählen]**.

   ![](assets/create-audience.png)

1. Klicken Sie auf **[!UICONTROL Audience auswählen]**, um eine bestehende Audience zu verwenden. Um eine neue Audience zu erstellen, die in dieser E-Mail verwendet werden soll, wählen Sie **Eigene erstellen**. Näheres dazu finden Sie in [diesem Abschnitt](segment-builder.md).

   Auf diesem Bildschirm werden alle vorhandenen Zielgruppen für den aktuellen Ordner angezeigt.

   ![](assets/create-audience2.png)

   Zielgruppen werden über das linke Menü **Zielgruppen** erstellt. Sie können auch in der Client-Konsole erstellt werden.

   Um Adobe Experience Platform-Zielgruppen zu nutzen, müssen Sie die Integration mit Zielen konfigurieren. Weitere Informationen finden Sie in der Dokumentation zu [Adobe Experience Platform-Zielen](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=de){target="_blank"}.

   >[!IMPORTANT]
   >
   >In dieser Produktversion sind beim Erstellen von Regeln, beim Auswählen der Zielgruppe eines Versands oder beim Erstellen einer Zielgruppe in einem Workflow einige vordefinierte Filter nicht in der Benutzeroberfläche verfügbar. Sie können sie weiterhin verwenden. [Weitere Informationen](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

1. Wählen Sie eine Zielgruppe aus und klicken Sie auf **Auswählen**.
1. Verwenden Sie das Symbol **Filter anzeigen**, um die Filteroptionen anzuzeigen. Klicken Sie auf **Regeln hinzufügen**, um auf den Regel-Builder zuzugreifen: Mit dem Regel-Builder können Sie erweiterte Filter für die Liste der Zielgruppen erstellen. In diesem [Abschnitt](segment-builder.md) erfahren Sie, wie Sie den Regel-Builder verwenden.

   ![](assets/create-audience4.png)

1. Klicken Sie auf **Speichern**.

Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Dadurch lässt sich das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. Weiterführende Informationen finden Sie in [diesem Abschnitt](control-group.md).