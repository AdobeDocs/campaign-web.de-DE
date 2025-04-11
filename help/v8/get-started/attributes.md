---
audience: end-user
title: Auswählen von Attributen und Hinzufügen dieser Auswahl zu Favoriten
description: Erfahren Sie, wie Sie mit Attributen arbeiten und einfach auf bevorzugte und zuletzt verwendete Attribute zugreifen können.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: c0c9c5da3369e55269411b7348004006cd3c139e
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 35%

---

# Auswählen von Attributen und Hinzufügen dieser Auswahl zu Favoriten {#folders}

In der Web-Benutzeroberfläche von Campaign können Benutzer je nach ausgeführter Aktion Attribute aus der Datenbank an verschiedenen Stellen auswählen. Beispielsweise können Attribute beim Definieren der Ausgabespalten für einen Briefpost-Versand oder eine zu extrahierende Datei ausgewählt werden. Ebenso können Attribute ausgewählt werden, wenn der Abfrage-Modellierer zum Erstellen von Regeln, Filtern oder Zielgruppen verwendet wird.

![Wählen Sie Attribute über die Datenbankschnittstelle aus und zeigen Sie Attributoptionen an.](assets/attributes-list.png)

Um häufig verwendete Attribute schnell wiederzuverwenden, fügen Sie sie zu den Favoriten hinzu. Dadurch wird sichergestellt, dass sie für zukünftige Aufgaben problemlos zugänglich sind. Zusätzlich zu den Favoriten können Benutzer die zuletzt ausgewählten Attribute anzeigen und verwenden.

Die Oberfläche bietet außerdem das Tool „Werteverteilung“, mit dem Sie die Verteilung der Attributwerte in einer Tabelle visualisieren können. Dieses Tool hilft bei der Identifizierung des Bereichs und der Häufigkeit von Werten und stellt so die Datenkonsistenz beim Erstellen von Abfragen oder Ausdrücken sicher.

## Favoriten und zuletzt verwendete Attribute {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favoriten und zuletzt ausgewertet"
>abstract="Das Menü **[!UICONTROL Favoriten und zuletzt ausgewertet]** in der Attributauswahl bietet eine organisierte Ansicht von Attributen, die Sie den Favoriten hinzugefügt haben, sowie eine Liste der zuletzt verwendeten Attribute. Bevorzugte Attribute werden zuerst angezeigt, gefolgt von den zuletzt verwendeten Attributen, sodass Sie die benötigten Attribute leicht finden können."

Das Menü **[!UICONTROL Favoriten und Zuletzt verwendet]** in der Attributauswahl bietet eine organisierte Ansicht von Attributen, die zu den Favoriten hinzugefügt wurden, sowie eine Liste von kürzlich verwendeten Attributen. Favoritenattribute werden zuerst angezeigt, gefolgt von kürzlich verwendeten Attributen, damit Sie die erforderlichen Attribute leicht finden können.

![Menü „Favoriten“ und „Zuletzt verwendete Attribute“ mit den bevorzugten und zuletzt verwendeten Attributen.](assets/attributes-favorites.png)

Um ein Attribut zu den Favoriten hinzuzufügen, bewegen Sie den Mauszeiger über die Informationsschaltfläche und wählen Sie das Sternsymbol aus. Das Attribut wird dann automatisch zur Favoritenliste hinzugefügt. Um ein Attribut aus den Favoriten zu entfernen, klicken Sie erneut auf das Sternsymbol.

Benutzer können bis zu 20 Attribute zu Favoriten hinzufügen. Jedem Benutzer in einer Organisation werden die Attribute „Favorit“ und „Zuletzt verwendet“ zugeordnet, um die Barrierefreiheit auf verschiedenen Computern sicherzustellen und ein nahtloses Erlebnis auf allen Geräten zu ermöglichen.

## Bestimmen der Werteverteilung in einer Tabelle {#distribution}

Mit **Schaltfläche „Werteverteilung** im Informationsbereich eines Attributs können Benutzer die Werteverteilung für dieses Attribut innerhalb der Tabelle analysieren. Diese Funktion ist hilfreich, um die verfügbaren Werte, ihre Anzahl und Prozentsätze zu verstehen. Außerdem lassen sich Probleme wie inkonsistente Groß- und Kleinschreibung beim Erstellen von Abfragen oder Ausdrücken vermeiden.

![Benutzeroberfläche des Tools Werteverteilung , in der die Anzahl und der Prozentsatz der Attributwerte angezeigt werden.](assets/attributes-distribution-values.png)

Bei Attributen mit einer großen Anzahl von Werten zeigt das Tool nur die ersten zwanzig an. In solchen Fällen weist eine **[!UICONTROL Partiallast]**-Benachrichtigung auf diese Einschränkung hin. Wenden Sie erweiterte Filter an, um die angezeigten Ergebnisse zu verfeinern und sich auf bestimmte Werte oder Teilmengen von Daten zu konzentrieren. Ausführliche Anleitungen zur Verwendung von Filtern finden Sie [hier](../get-started/work-with-folders.md#filter-the-values).

Weitere Informationen zur Verwendung des Tools „Werteverteilung“ in verschiedenen Kontexten finden Sie in den folgenden Abschnitten:

* [Werteverteilung in einem Ordner](../get-started/work-with-folders.md##distribution-values-folder)
* [Werteverteilung in einer Abfrage](../query/build-query.md#distribution-values-query)