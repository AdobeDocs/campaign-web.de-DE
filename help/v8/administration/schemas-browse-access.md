---
title: Durchsuchen von und Zugreifen auf Schemata
description: Erfahren Sie, wie Sie in der Benutzeroberfläche Schemata durchsuchen und darauf zugreifen können.
exl-id: deafd171-0a3f-4ba2-8fa4-09661d8cdb3e
source-git-commit: c6da1a4cb21c1346982303a29364cf97e26b4f4a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 90%

---

# Zugreifen auf und Konfigurieren von Schemata {#access}

>[!CONTEXTUALHELP]
>id="acw_schema_action_data"
>title="Aktionen zur Datenbearbeitung"
>abstract="Konfigurieren Sie die Aktionen, die für die Detaillisten- und Listenbildschirme des Schemas verfügbar sind. Aktivieren Sie **[!UICONTROL Schreibgeschützt]**, um den Detailbildschirm als schreibgeschützt festzulegen und Aktionen aus der Liste zu entfernen. Aktivieren Sie **[!UICONTROL Löschen nicht zulassen]** um die Löschaktion aus den Detaillisten- und Listenbildschirmen zu entfernen."

Auf Schemata kann über das Menü **[!UICONTROL Administration]** > **[!UICONTROL Schemata]** zugegriffen werden.

![Bildschirm mit der Liste der Schemata samt verfügbaren Schemata und Filtern](assets/schemas-list.png)

Auf diesem Bildschirm können Sie alle vorhandenen Schemata anzeigen. Es stehen Filter zur Verfügung, mit denen Sie die Liste einschränken können, um beispielsweise nur bearbeitbare Schemata anzuzeigen.

Um ein Schema zu öffnen, wählen Sie seinen Namen aus. Eine detaillierte Schemaansicht wird angezeigt.

![Bildschirm mit Schemadetails samt Schemaeigenschaften und -inhalten](assets/schema-details.png)

## Übersicht über das Schema {#overview}

Auf der Registerkarte **[!UICONTROL Übersicht]** finden Sie eine allgemeine Ansicht des Schemas:

* Im Abschnitt **[!UICONTROL Eigenschaften]** werden wichtige Informationen angezeigt, z. B. der Schemaname, der Namespace und der zugehörige Tabellenname.

* Der Abschnitt **[!UICONTROL Schemadefinition]** zeigt Details zur Schemadefinition an, z. B. den für die Datenabstimmung verwendeten Primärschlüssel und seine Verknüpfungen mit anderen Tabellen.

  Klicken Sie auf die Schaltfläche **[!UICONTROL Schemavorschau]**, um die verschiedenen Felder und Links anzuzeigen, aus denen das Schema besteht. Auf diese Weise können Sie die vollständige Struktur eines Schemas überprüfen. Wenn das Schema mit benutzerdefinierten Feldern erweitert wurde, können Sie alle Erweiterungen visualisieren.

* Im Abschnitt **[!UICONTROL Inhalt]** wird der XML-Inhalt des Schemas angezeigt, sodass Sie zwischen der Quelle und der generierten Syntax wechseln können.

## Schemadaten {#data}

Die Registerkarte **[!UICONTROL Daten]** enthält Informationen zu den Schemadaten.

![Registerkarte „Daten“ des Schemas mit Datenstruktur und Attributen](assets/schemas-data.png)

## Anpassen der Bildschirmanzeige {#screen-def}

Mit der Bildschirmdefinition können Sie konfigurieren, wie Schemafelder in der Benutzeroberfläche angezeigt und bearbeitet werden. Sie können Standardspalten für Listenansichten konfigurieren, festlegen, welche benutzerdefinierten Felder in Detailbildschirmen angezeigt werden, Sammlungslisten hinzufügen, um zugehörige Daten anzuzeigen, und Felder in Abschnitte mit Trennzeichen und Sichtbarkeitskriterien organisieren.

So greifen Sie auf die Bildschirmdefinition zu:

1. Navigieren Sie zum Menü **[!UICONTROL Schemata]** und suchen Sie mithilfe der Filter nach bearbeitbaren Schemata.

   ![Bildschirm mit der Liste der Schemata samt verfügbaren Schemata und Filtern](assets/schemas-list2.png)

1. Wählen Sie den Schemanamen in der Liste aus, um das Schema zu öffnen, und klicken Sie in der Ansicht der Schemadetails auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**, um die Bildschirmdefinition aufzurufen.

   ![Bildschirm mit der Liste der Schemata samt verfügbaren Schemata und Filtern](assets/schemas-list3.png)

   Die verschiedenen Listen ermöglichen es Ihnen, Elemente mithilfe der Pfeilsymbole nach oben und unten neu anzuordnen oder sie per Drag-and-Drop abzulegen. Um Elemente zu entfernen, klicken Sie auf das Papierkorbsymbol in einer bestimmten Zeile oder wählen Sie **[!UICONTROL Alle löschen]** über das Symbol mit den Auslassungspunkten aus.

   ![Abschnitt „Allgemein“ der Bildschirmdefinition](assets/schemas-general.png)

In der Bildschirmdefinition haben Sie folgende Möglichkeiten:

* [Standardlistenspalten konfigurieren](schemas-list-columns.md) – Konfigurieren Sie, welche Spalten in Listenansichten standardmäßig angezeigt werden.
* [Benutzerdefinierte Felder bearbeiten](schemas-custom-fields.md) – Konfigurieren Sie, welche benutzerdefinierten Felder auf Detailbildschirmen angezeigt werden, und organisieren Sie sie in Abschnitte.
* [Sammlungslisten hinzufügen](schemas-collection-lists.md) – Fügen Sie Sammlungslisten hinzu, um verwandte Daten in Profilbildern anzuzeigen.
