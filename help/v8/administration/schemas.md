---
title: Arbeiten mit Schemata
description: Erfahren Sie, wie Sie mit Schemata arbeiten.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 100%

---

# Arbeiten mit Schemata {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemata"
>abstract="**[!DNL Adobe Campaign]** verwendet XML-basierte Schemata, um die physische und logische Struktur von Daten innerhalb der Anwendung zu definieren. Auf diesem Bildschirm können Sie alle vorhandenen Schemata anzeigen und auf die Details eines Schemas zugreifen, indem Sie dessen Namen in der Liste auswählen. Es stehen Filter zur Verfügung, mit denen Sie die Liste einschränken können und z. B. nur bearbeitbare Schemata anzeigen."

## Über Schemata {#about}

**[!DNL Adobe Campaign]** verwendet XML-basierte Schemata, um die physische und logische Struktur von Daten innerhalb der Anwendung zu definieren. Ein Schema ist ein mit einer Datenbanktabelle verknüpftes XML-Dokument, mit dem folgende Aspekte definiert werden: 

* die SQL-Tabellenstruktur, wie Tabellenname, Felder und Beziehungen
* die XML-Datenstruktur, wie Elemente, Attribute, Hierarchie, Typen, Standardwerte und Label

Schemata spielen eine wichtige Rolle bei folgenden Aktivitäten:

* Zuordnen von Anwendungsdaten zu Datenbanktabellen.
* Definieren von Beziehungen zwischen Datenobjekten.
* Angeben der Struktur und der Eigenschaften jedes Felds.

Jede Entität in Adobe Campaign verfügt über ein dediziertes Schema, was die Datenkonsistenz und -organisation gewährleistet.

Detaillierte Informationen zu Schemata finden Sie in der [Dokumentation zur Campaign-Konsole](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

## Zugreifen auf Schemata über die Web-Benutzeroberfläche {#access}

Auf Schemata kann über das Menü **[!UICONTROL Administration]** > **[!UICONTROL Schemata]** zugegriffen werden.

![Bildschirm mit der Liste der Schemata samt verfügbaren Schemata und Filtern](assets/schemas-list.png)

Auf diesem Bildschirm können Sie alle vorhandenen Schemata anzeigen. Es stehen Filter zur Verfügung, mit denen Sie die Liste einschränken können, um beispielsweise nur bearbeitbare Schemata anzuzeigen.

Um ein Schema zu öffnen, wählen Sie seinen Namen aus. Eine detaillierte Schemaansicht wird angezeigt.

![Bildschirm mit Schemadetails samt Schemaeigenschaften und -inhalten](assets/schema-details.png)

### Übersicht über das Schema {#overview}

Auf der Registerkarte **[!UICONTROL Übersicht]** finden Sie eine allgemeine Ansicht des Schemas:

* Im Abschnitt **[!UICONTROL Eigenschaften]** werden wichtige Informationen angezeigt, z. B. der Schemaname, der Namespace und der zugehörige Tabellenname.

* Der Abschnitt **[!UICONTROL Schemadefinition]** zeigt Details zur Schemadefinition an, z. B. den für die Datenabstimmung verwendeten Primärschlüssel und seine Verknüpfungen mit anderen Tabellen.

  Klicken Sie auf die Schaltfläche **[!UICONTROL Schemavorschau]**, um die verschiedenen Felder und Links anzuzeigen, aus denen das Schema besteht. Auf diese Weise können Sie die vollständige Struktur eines Schemas überprüfen. Wenn das Schema mit benutzerdefinierten Feldern erweitert wurde, können Sie alle Erweiterungen visualisieren.

* Im Abschnitt **[!UICONTROL Inhalt]** wird der XML-Inhalt des Schemas angezeigt, sodass Sie zwischen der Quelle und der generierten Syntax wechseln können.

### Schemadaten {#data}

Die Registerkarte **[!UICONTROL Daten]** enthält Informationen zu den Schemadaten.

![Registerkarte „Daten“ des Schemas mit Datenstruktur und Attributen](assets/schemas-data.png)

## Bearbeiten benutzerdefinierter Felder {#fields}

Benutzerdefinierte Felder sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zu vorkonfigurierten Schemata hinzugefügt werden. Sie ermöglichen es Ihnen, Schemata anzupassen, indem neue Attribute entsprechend den Anforderungen Ihrer Organisation eingefügt werden. 

Benutzerdefinierte Felder können auf verschiedenen Bildschirmen angezeigt werden, z. B. in den Profildetails der Campaign Web-Benutzeroberfläche. Sie können steuern, welche Felder sichtbar sind und wie sie in der Oberfläche angezeigt werden. Klicken Sie dazu im Menü **[!UICONTROL Schemata]** auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**.

![Bildschirm für benutzerdefinierte Felder mit bearbeitbaren Attributen](assets/schemas-custom.png)

Klicken Sie auf **[!UICONTROL Vorschau]**, um die benutzerdefinierten Felder auf einem Beispielbildschirm anzuzeigen.

Detaillierte Informationen zum Bearbeiten von benutzerdefinierten Feldern in einem Schema finden Sie unter [Konfigurieren benutzerdefinierter Felder](../administration/custom-fields.md).