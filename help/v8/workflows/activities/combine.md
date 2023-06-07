---
audience: end-user
title: Verwenden Sie die Workflow-Aktivität Kombinieren .
description: Erfahren Sie, wie Sie die Workflow-Aktivität Kombinieren verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 25%

---


# Kombinieren {#combine}

Diese Aktivität ermöglicht die Segmentierung Ihrer eingehenden Population. Sie können also verschiedene Populationen vereinen, einen Teil daraus ausschließen oder nur die in jeder der Populationen enthaltenen Datensätze verwenden. Im Folgenden finden Sie die verfügbaren Segmentierungstypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Die **Vereinigung** ermöglicht die Zusammenfassung des Ergebnisses mehrerer Aktivitäten in einer Zielgruppe.
* Die **Schnittmenge** ermöglicht es, nur die Elemente beizubehalten, die den verschiedenen eingehenden Populationen in der Aktivität gemein sind.
* Die **Ausschluss** ermöglicht den Ausschluss von Elementen aus einer Population nach bestimmten Kriterien.

## Allgemeine Konfiguration {#general}

Führen Sie die folgenden Schritte aus, um mit der Konfiguration der **Kombinieren** Aktivität:

1. Hinzufügen mehrerer Aktivitäten wie **Audience erstellen** Aktivitäten, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Hinzufügen einer **Kombinieren** -Aktivität zu einem der vorherigen Zweige.
1. Wählen Sie den Segmentierungstyp aus: [Vereinigung](#union), [Schnittmenge](#intersection) oder [Ausschluss](#exclusion).
1. Bestätigen Sie die Angaben mit der Schaltfläche **Fortfahren**.
1. Im **Sets zum Verbinden** alle vorherigen Aktivitäten, denen Sie beitreten möchten.

## Vereinigung {#union}

Für **Vereinigung**, müssen Sie die **Abstimmtyp** zur Definition des Umgangs mit Duplikaten:

* **Nur die Schlüssel** – Standardmodus; die Aktivität behält nur einen der Datensätze bei, wenn mehrere aus verschiedenen eingehenden Transitionen stammende Datensätze denselben Schlüssel aufweisen. Diese Option kann nur verwendet werden, wenn die eingehenden Populationen homogen sind.
* **Auswahl an Spalten** – die Abstimmung erfolgt auf Basis der von Ihnen angegebenen Spalten. Wählen Sie zunächst die die Quelldaten enthaltende Hauptmenge aus und dann die für die Herstellung der Relation zu verwendenden Spalten.

## Schnittmenge {#intersection}

Für **Schnittmenge** müssen Sie die folgenden zusätzlichen Schritte ausführen:

1. Wählen Sie die **Abstimmtyp** , um festzulegen, wie Duplikate verarbeitet werden. Siehe den Abschnitt [Vereinigung](#union).
1. Sie können die **Abschluss generieren** -Option, wenn Sie die verbleibende Population verarbeiten möchten. Das Komplement enthält die Vereinigung der Ergebnisse aller eingehenden Aktivitäten abzüglich der Schnittmenge. Der Aktivität wird daraufhin eine zusätzliche ausgehende Transition hinzugefügt.

## Ausschluss {#exclusion}

Für **Ausschluss** müssen Sie die folgenden zusätzlichen Schritte ausführen:

1. Im **Sets zum Verbinden** auswählen, wählen Sie die **Primärer Satz** aus den eingehenden Transitionen. aus der die Elemente der anderen eingehenden Transitionen ausgeschlossen werden sollen. Die eingehenden Transitionen müssen Populationen gleichen Typs enthalten.
1. Bei Bedarf können die eingehenden Tabellen angepasst werden. Um eine Zielgruppe aus einer anderen Dimension auszuschließen, muss diese Zielgruppe auf dieselbe Zielgruppendimension wie die Hauptzielgruppe zurückgesetzt werden. Klicken Sie dazu auf **Regel hinzufügen** im **Ausschlussregeln** und geben Sie die Bedingungen für die Dimensionsänderung an. Die Abstimmung der Daten erfolgt entweder über ein Attribut oder einen Join.
1. Sie können die **Abschluss generieren** -Option, wenn Sie die verbleibende Population verarbeiten möchten. Siehe den Abschnitt [Schnittmenge](#intersection).

## Beispiele

Im folgenden Beispiel wurde ein **Vereinigung** die alle Profile der beiden Abfragen abruft: Personen zwischen 18 und 27 Jahren und Personen zwischen 34 und 40 Jahren.

![](../assets/workflow-union-example.png)

Das folgende Beispiel zeigt die **Schnittmenge** zwischen zwei Abfrageaktivitäten. Es wird hier zum Abrufen von Profilen verwendet, die zwischen 18 und 27 Jahre alt sind und deren E-Mail-Adresse angegeben wurde.

![](../assets/workflow-intersection-example.png)

Folgendes **Ausschluss** zeigt zwei Abfragen, die zum Filtern von Profilen konfiguriert wurden, die zwischen 18 und 27 Jahre alt sind und die eine E-Mail-Domain der Adobe haben. Die Profile mit einer Adobe-E-Mail-Domain werden dann aus der ersten Gruppe ausgeschlossen.

![](../assets/workflow-exclusion-example.png)


