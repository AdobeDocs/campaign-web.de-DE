---
audience: end-user
title: Arbeiten mit Ordnern
description: Erfahren Sie, wie Sie in Adobe Campaign einen Ordner verwalten.
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: c7bb533174019d465f273c4fede3b578a40f2bb6
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 54%

---

# Arbeiten mit Ordnern {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="Ordnereigenschaften"
>abstract="Ordnereigenschaften"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="Ordnersicherheit"
>abstract="Ordnersicherheit"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="Ordnereinschränkungen"
>abstract="Ordnereinschränkungen"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Ordnerzeitplan"
>abstract="Ordnerzeitplan"

## Über Ordner

Ordner sind Objekte in Adobe Campaign zur Organisation Ihrer Komponenten und Daten.

Sie können Ordner im Navigationsbaum erstellen, umbenennen, neu anordnen und verschieben. Sie können sie auch Ihren Bedürfnissen entsprechend löschen.

![](assets/folders.png){zoomable="yes"}

Sie können einen Ordnertyp einrichten. Zum Beispiel: ein Ordner mit Sendungen.
Das Symbol des Ordners ändert sich je nach Typ.

## Erstellen eines neuen Ordners

Gehen Sie wie folgt vor, um in der Adobe Campaign Web-Benutzeroberfläche einen neuen Ordner zu erstellen:

1. Navigieren Sie dazu in **[!UICONTROL Explorer]** zu dem Ordner, in dem Sie Ihren neuen Ordner erstellen möchten.
Im Menü **[!UICONTROL …]** finden Sie die Option **[!UICONTROL Neuen Ordner erstellen]**.

![](assets/folder_create.png){zoomable="yes"}

Wenn Sie einen neuen Ordner erstellen, ist der Ordner standardmäßig vom gleichen Typ wie der übergeordnete Ordner.
In unserem Beispiel erstellen wir einen Ordner im Ordner **[!UICONTROL Sendungen]**.

![](assets/folder_new.png){zoomable="yes"}

1. Ändern Sie bei Bedarf den Typ des Ordners, indem Sie auf das Symbol des Ordnertyps klicken, und wählen Sie ihn in der angezeigten Liste aus, wie unten dargestellt:

![](assets/folder_type.png){zoomable="yes"}

Richten Sie den Ordnertyp ein, indem Sie auf die Schaltfläche **[!UICONTROL Bestätigen]** klicken.

Wenn Sie einen Ordner ohne bestimmten Typ erstellen möchten, wählen Sie den Typ **[!UICONTROL Allgemeiner Ordner]** aus.

Sie können auch [Ordner in der Adobe Campaign-Konsole erstellen und verwalten](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/config/configuration/folders-and-views).

## Löschen eines Ordners

>[!CAUTION]
>
>Beim Löschen eines Ordners werden auch alle im Ordner gespeicherten Daten gelöscht.

Um einen Ordner zu löschen, wählen Sie ihn im Baum **[!UICONTROL Explorer]** aus und klicken Sie auf das Menü **[!UICONTROL ...]**.
Wählen Sie **[!UICONTROL Ordner löschen]** aus.

![](assets/folder_delete.png){zoomable="yes"}

## Verteilung der Werte in einem Ordner {#distribution-values-folder}

Die Werteverteilung hilft dabei, den Prozentsatz eines Werts in einer Spalte innerhalb einer Tabelle zu ermitteln.

Um die Verteilung der Werte in einem Ordner zu erfahren, gehen Sie wie folgt vor:

Beispielsweise möchten wir die Werteverteilung der Spalte **Kanal** unter den Sendungen kennen.

Um diese Informationen zu erhalten, gehen Sie zum Ordner **[!UICONTROL Sendungen]** und klicken Sie auf das Symbol **[!UICONTROL Spalten konfigurieren]** .

Klicken Sie im Fenster **[!UICONTROL Spalten konfigurieren]** auf das Symbol **[!UICONTROL Informationen]** der Spalte, die Sie kennen möchten. Klicken Sie dann auf die Schaltfläche **[!UICONTROL Werteverteilung]** .

![](assets/values_deliveries.png){zoomable="yes"}

Sie erhalten den Prozentsatz der Werte in der Spalte **[!UICONTROL Kanal]** .

![](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
> Bei Spalten mit vielen Werten werden nur die ersten zwanzig Werte angezeigt. Eine Benachrichtigung **[!UICONTROL Teillade]** gibt eine Warnung aus.

Sie können auch die Werteverteilung eines Links verwenden.

Klicken Sie in der Attributliste auf die Schaltfläche **+** neben dem gewünschten Link, wie unten dargestellt. Dadurch wird der Link zu den **[!UICONTROL Ausgabespalten]** hinzugefügt. Jetzt können Sie über das Symbol **[!UICONTROL Informationen]** verfügen, über das Sie die Verteilung der Werte anzeigen können. Wenn Sie den Link nicht in den **[!UICONTROL Ausgabespalten]** beibehalten möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Abbrechen]** .

![](assets/values_link.png){zoomable="yes"}

Es ist auch möglich, die Werteverteilung in einem Abfragemodell zu verwenden. [Weitere Informationen finden Sie hier](../query/build-query.md#distribution-of-values-in-a-query).