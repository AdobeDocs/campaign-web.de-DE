---
audience: end-user
title: Durchsuchen, Suchen und Filtern von Listen
description: Erfahren Sie, wie Sie Listen in Campaign Web v8 durchsuchen und filtern
badge: label="Alpha"
source-git-commit: 065108e7ac4d682dc3f3de63303be8353b145757
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 100%

---


# Durchsuchen, Suchen und Filtern von Listen {#list-screens}

Die meisten Links aus dem linken Navigationsmenü zeigen Listen von Objekten an, wie zum Beispiel die Liste der **Sendungen** oder **Kampagnen**. Einige dieser Listenbildschirme sind schreibgeschützt. Sie können die Listenanzeige anpassen und diese Listen wie unten beschrieben filtern.

Um einen Filter zu entfernen, klicken Sie auf die Schaltfläche **Alle löschen**.

## Anpassen von Listenbildschirmen {#custom-lists}

Die Listen werden in Spalten angezeigt. Sie können auch zusätzliche Informationen anzeigen, indem Sie die Spaltenkonfiguration ändern. Klicken Sie dazu auf das Symbol **Spalte für ein benutzerdefiniertes Layout konfigurieren** in der oberen rechten Ecke der Liste.

![](assets/config-columns.png){width="70%" align="left" zoomable="yes"}

Im Bildschirm **Spalten konfigurieren** können Sie Spalten hinzufügen oder entfernen und die Reihenfolge ändern, in der sie angezeigt werden.

Für diese Einstellungen:

![](assets/columns.png){width="70%" align="left" zoomable="yes"}

enthält die Liste beispielsweise die folgenden Spalten:

![](assets/column-sample.png){width="70%" align="left" zoomable="yes"}

Verwenden Sie den Umschalter **Erweiterte Attribute anzeigen**, um alle Attribute für die aktuelle Liste anzuzeigen. [Weitere Informationen](#adv-attributes)

## Sortieren der Daten {#sort-lists}

Sie können zudem auch Elemente in der Liste sortieren, indem Sie auf eine beliebige Spaltenüberschrift klicken. Ein Aufwärts- oder Abwärtspfeil zeigt an, dass die Liste in dieser Spalte sortiert ist.

Bei numerischen Spalten oder Datumsspalten bedeutet der **Aufwärtspfeil**, dass die Liste in aufsteigender Reihenfolge sortiert ist, während ein **Abwärtspfeil** eine absteigende Reihenfolge kennzeichnet. Bei Zeichenfolge- oder alphanumerischen Spalten werden die Werte in alphabetischer Reihenfolge aufgeführt.

## Integrierte Filter {#list-built-in-filters}

Um Elemente schneller zu finden, können Sie die Suchleiste verwenden oder die Liste nach kontextuellen Kriterien filtern.

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

Sie können beispielsweise Sendungen nach Status, Kanal, Kontaktdatum oder Ordner filtern. Sie können auch Tests ausblenden.

## Benutzerdefinierte Filter{#list-custom-filters}

Um benutzerdefinierte Datenfilter zu erstellen, navigieren Sie zum unteren Rand der Filter und klicken Sie auf die Schaltfläche **Regeln hinzufügen**.

Ziehen Sie auf dem Bildschirm **Erweiterte Filter** Attribute per Drag-and-Drop, um Ihre Filterkriterien zu erstellen.

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

Verwenden Sie den Umschalter **Erweiterte Attribute anzeigen**, um alle Attribute für die aktuelle Liste anzuzeigen. [Weitere Informationen](#adv-attributes)

## Verwenden von erweiterten Attributen {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Anzeigen von erweiterten Attributen"
>abstract="In der Attributliste werden standardmäßig nur die häufigsten Attribute angezeigt. Verwenden Sie diesen Umschalter, um einen Filter mit erweiterten Attributen zu erstellen."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Erweiterte Felder des Regel-Builders"
>abstract="Konfigurieren Sie erweiterte Filter mit erweiterten Feldern."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Erweiterte Attribute des Regel-Builders"
>abstract="Verwenden Sie erweiterte Attribute, um Ihre Regel zu definieren."


Standardmäßig werden in den Konfigurationsbildschirmen der Attributliste und der Filter nur die häufigsten Attribute angezeigt. Attribute, die im Datenschema als `advanced`-Attribute gesetzt wurden, werden in den Konfigurationsbildern ausgeblendet.

Aktivieren Sie den Umschalter **Erweiterte Attribute anzeigen**, um alle verfügbaren Attribute für die aktuelle Liste anzuzeigen: Die Attributliste wird sofort aktualisiert.


![](assets/adv-toggle.png){width="70%" align="left" zoomable="yes"}
