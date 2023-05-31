---
audience: end-user
title: Verwenden Sie die Workflow-Aktivität Kombinieren .
description: Erfahren Sie, wie Sie die Workflow-Aktivität Kombinieren verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 36%

---


# Kombinieren {#combine}

Diese Aktivität ermöglicht die Verarbeitung von Sets für eingehende Daten. Sie können also verschiedene Populationen vereinen, einen Teil daraus ausschließen oder nur die in jeder der Populationen enthaltenen Datensätze verwenden. Im Folgenden finden Sie die verfügbaren Segmentierungstypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Die **Vereinigung** ermöglicht die Zusammenfassung des Ergebnisses mehrerer Aktivitäten in einer Zielgruppe.
* Die **Schnittmenge** ermöglicht es, nur die Elemente beizubehalten, die den verschiedenen eingehenden Populationen in der Aktivität gemein sind.
* Die **Ausschluss** ermöglicht den Ausschluss von Elementen aus einer Population nach bestimmten Kriterien.

Führen Sie die folgenden Schritte aus, um die **Kombinieren** Aktivität:

1. Fügen Sie Ihre **Kombinieren** -Aktivität zu einer der vorherigen Segmentierungsübergänge hinzu.
1. Wählen Sie den Segmentierungstyp aus: Vereinigung, Schnittmenge oder Ausschluss.
1. Bestätigen Sie die Angaben mit der Schaltfläche **Fortfahren**.
1. Im **Sets zum Verbinden** alle vorherigen Aktivitäten, denen Sie beitreten möchten.

Für **Vereinigung** und **Schnittmenge**, müssen Sie die **Abstimmtyp** zur Definition des Umgangs mit Duplikaten:

    * Nur Schlüssel: Dies ist der Standardmodus. die Aktivität behält nur einen der Datensätze bei, wenn mehrere aus verschiedenen eingehenden Transitionen stammende Datensätze denselben Schlüssel aufweisen. Diese Option kann nur verwendet werden, wenn die eingehenden Populationen homogen sind.
    * Auswahl an Spalten – die Abstimmung erfolgt auf Basis der von Ihnen angegebenen Spalten. Wählen Sie zunächst die die Quelldaten enthaltende Hauptmenge aus und dann die für die Herstellung der Relation zu verwendenden Spalten.

Für **Schnittmenge** und **Ausschluss**, können Sie die **Abschluss generieren** -Option, wenn Sie die verbleibende Population verarbeiten möchten. Das Komplement enthält die Vereinigung der Ergebnisse aller eingehenden Aktivitäten abzüglich der Schnittmenge. Der Aktivität wird daraufhin eine zusätzliche ausgehende Transition hinzugefügt.

Für **Ausschluss**, wählen Sie die **Primärer Satz** aus den eingehenden Transitionen in der **Sets zum Verbinden** Abschnitt. aus der die Elemente der anderen eingehenden Transitionen ausgeschlossen werden sollen. Die eingehenden Transitionen müssen Populationen gleichen Typs enthalten.
