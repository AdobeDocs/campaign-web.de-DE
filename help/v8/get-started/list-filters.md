---
audience: end-user
title: Durchsuchen und Filtern von Listen
description: Erfahren Sie, wie Sie Listen in Campaign Web v8 durchsuchen und filtern
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%

---

# Durchsuchen und Filtern von Listen {#list-screens}

Die meisten Links aus dem linken Navigationsmenü zeigen Listen von Objekten an, wie z. B. die Liste der **Sendungen** oder **Kampagnen**. Einige dieser Listenbildschirme sind schreibgeschützt. Sie können die Listenanzeige anpassen und diese Listen wie unten beschrieben filtern.

## Anpassen von Listenbildschirmen {#custom-lists}

Die Listen werden in Spalten angezeigt. Sie können auch zusätzliche Informationen anzeigen, indem Sie die Spaltenkonfiguration ändern. Klicken Sie dazu auf das Symbol **Spalte für ein benutzerdefiniertes Layout konfigurieren** in der oberen rechten Ecke der Liste.

[Screenshot mit dem Symbol „Spalte konfigurieren“, das zum Anpassen des Layouts von Listenspalten verwendet wird](assets/config-columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Im Bildschirm **Spalten konfigurieren** können Sie Spalten hinzufügen oder entfernen und die Reihenfolge ändern, in der sie angezeigt werden.

Sie können die Reihenfolge Ihrer Liste entweder durch **Ziehen und Ablegen** oder durch Verwendung der **Nach-oben- und Nach-unten-Taste** ändern.

[Screenshot zur Veranschaulichung, wie Listenspalten per Drag-and-Drop oder Pfeilschaltflächen neu angeordnet werden können](assets/list-reorder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Für diese Einstellungen:

[Screenshot mit beispielhaften Spalteneinstellungen im Bildschirm „Spalten konfigurieren“](assets/columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

enthält die Liste beispielsweise die folgenden Spalten:

[Screenshot der resultierenden Liste mit Spalten, die gemäß den Beispieleinstellungen konfiguriert wurden](assets/column-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

## Sortieren der Daten {#sort-lists}

Sie können Elemente in der Liste sortieren, indem Sie auf eine beliebige Spaltenüberschrift klicken. Ein Aufwärts- oder Abwärtspfeil zeigt an, dass die Liste anhand dieser Spalte sortiert ist.

Bei numerischen Spalten oder Datumsspalten bedeutet der **Aufwärtspfeil**, dass die Liste in aufsteigender Reihenfolge sortiert ist, während ein **Abwärtspfeil** eine absteigende Reihenfolge kennzeichnet. Bei Zeichenfolge- oder alphanumerischen Spalten werden die Werte in alphabetischer Reihenfolge aufgeführt.

## Filter {#list-built-in-filters}

Um Elemente schneller zu finden, können Sie die Suchleiste verwenden oder die Liste nach Kontextkriterien filtern.

[Screenshot mit Filteroptionen zum Verfeinern der Listenansicht](assets/filter.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Detaillierte Informationen zur Verwendung von Filtern und zur Erstellung eigener benutzerdefinierter Filter finden Sie in [diesem Abschnitt](../query/filter.md).

<!--
## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

Only the most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes set as `advanced` attributes in the data schema are hidden from the configuration screens.

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list updates instantly.

[The screenshot shows the Display advanced attributes toggle used to reveal hidden attributes in the rule builder palette.](assets/adv-toggle.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}
-->