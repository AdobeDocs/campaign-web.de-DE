---
audience: end-user
title: Verwenden der Workflow-Aktivität „Kombinieren“.
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Kombinieren“ verwenden.
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '950'
ht-degree: 100%

---

# Kombinieren {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Die Aktivität „Kombinieren“"
>abstract="Die Aktivität **Kombinieren** ermöglicht die Segmentierung Ihrer eingehenden Population. Sie können verschiedene Populationen vereinen, einen Teil daraus ausschließen oder nur die in mehreren Zielgruppen enthaltenen Datensätze verwenden."

Die Aktivität **Kombinieren** ist eine Aktivität zur **Zielgruppenbestimmung**. Diese Aktivität ermöglicht die Segmentierung Ihrer eingehenden Population. Sie können verschiedene Populationen vereinen, einen Teil daraus ausschließen oder nur die in mehreren Zielgruppen enthaltenen Datensätze verwenden. Im Folgenden finden Sie die verfügbaren Segmentierungstypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Eine **Vereinigung** fasst das Ergebnis mehrerer Aktivitäten zu einer einzigen Zielgruppe zusammen.
* Durch eine **Schnittmenge** werden nur die Elemente behalten, die den verschiedenen eingehenden Populationen in der Aktivität gemeinsam sind.
* Durch einen **Ausschluss** werden entsprechende Elemente gemäß bestimmten Kriterien aus einer Population ausgeschlossen.

## Konfigurieren der Aktivität „Kombinieren“ {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Optionen für die Zusammenführung von Schnittmengen"
>abstract="Durch eine Schnittmenge werden nur die Elemente behalten, die den verschiedenen eingehenden Populationen in der Aktivität gemeinsam sind. Aktivieren Sie im Abschnitt „Zusammenzuführende Mengen“ alle vorherigen Aktivitäten, die Sie zusammenfügen möchten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Optionen für die Zusammenführung von Ausschlüssen"
>abstract="Durch einen Ausschluss werden entsprechende Elemente gemäß bestimmten Kriterien aus einer Population ausgeschlossen. Aktivieren Sie im Abschnitt „Zusammenzuführende Mengen“ alle vorherigen Aktivitäten, die Sie zusammenfügen möchten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Auswählen des Segmentierungstyps"
>abstract="Wählen Sie aus, wie Zielgruppen kombiniert werden. Eine **Vereinigung** fasst das Ergebnis mehrerer Aktivitäten zu einer einzigen Zielgruppe zusammen. Durch eine **Schnittmenge** werden nur die Elemente behalten, die den verschiedenen eingehenden Populationen in der Aktivität gemeinsam sind. Durch einen **Ausschluss** werden entsprechende Elemente gemäß bestimmten Kriterien aus einer Population ausgeschlossen."

Führen Sie die folgenden Schritte aus, um mit der Aktivität **Kombinieren** zu beginnen:

![](../assets/workflow-combine.png)

1. Fügen Sie mehrere Aktivitäten wie **Zielgruppe erstellen** hinzu, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Fügen Sie die Aktivität **Kombinieren** zu einer der vorherigen Verzweigungen hinzu.
1. Wählen Sie einen der Segmentierungstypen aus: [Vereinigung](#union), [Schnittmenge](#intersection) oder [Ausschluss](#exclusion).
1. Klicken Sie auf **Fortfahren**.
1. Aktivieren Sie im Abschnitt **Zusammenzuführende Mengen** alle vorherigen Aktivitäten, die Sie zusammenfügen möchten.

## Vereinigung {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Abstimmoptionen"
>abstract="Wählen Sie den **Abstimmtyp** aus, um festzulegen, wie Duplikate behandelt werden. Die Option **Schlüssel** ist standardmäßig aktiviert. Das heißt, die Aktivität behält nur ein Element bei, wenn mehrere aus verschiedenen eingehenden Transitionen stammende Elemente denselben Schlüssel aufweisen. Verwenden Sie die Option **Auswahl an Spalten**, um die Liste der Spalten zu definieren, auf die die Datenabstimmung angewendet werden soll. "

Konfigurieren Sie in der Aktivität **Kombinieren** eine **Vereinigung**, indem Sie den **Abstimmtyp** auswählen, um die Verarbeitung von Duplikaten zu definieren:

* **Nur die Schlüssel**: Dies ist der Standardmodus. Die Aktivität behält nur ein Element bei, wenn mehrere aus verschiedenen eingehenden Transitionen stammende Elemente denselben Schlüssel aufweisen. Diese Option kann nur verwendet werden, wenn die eingehenden Populationen homogen sind.
* **Auswahl an Spalten**: Wählen Sie diese Option, um die Liste der Spalten zu definieren, auf die die Datenabstimmung angewendet werden soll. Wählen Sie zunächst die Hauptmenge (die Quelldaten) aus, und dann die für den Join zu verwendenden Spalten.

## Schnittmenge {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Abstimmoptionen für Schnittmengen"
>abstract="Wählen Sie den **Abstimmtyp** aus, um festzulegen, wie Duplikate behandelt werden. Die Option **Schlüssel** ist standardmäßig aktiviert. Das heißt, die Aktivität behält nur ein Element bei, wenn mehrere aus verschiedenen eingehenden Transitionen stammende Elemente denselben Schlüssel aufweisen. Verwenden Sie die Option **Auswahl an Spalten**, um die Liste der Spalten zu definieren, auf die die Datenabstimmung angewendet werden soll. "

Konfigurieren Sie in der Aktivität **Kombinieren** eine **Schnittmenge**, indem Sie diese zusätzlichen Schritte ausführen: 

1. Wählen Sie den **Abstimmtyp**, um festzulegen, wie Duplikate behandelt werden. Siehe den Abschnitt [Vereinigung](#union).
1. Aktivieren Sie die Option **Komplement erzeugen**, wenn Sie auch die nicht in der Schnittmenge enthaltene Population verwenden möchten. Das Komplement enthält die Vereinigung der Ergebnisse aller eingehenden Aktivitäten abzüglich der Schnittmenge. Der Aktivität wird daraufhin eine zusätzliche ausgehende Transition hinzugefügt.

## Ausschluss  {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Ausschlussregeln"
>abstract="Bei Bedarf können die eingehenden Tabellen angepasst werden. Um eine Zielgruppe aus einer anderen Dimension auszuschließen, setzen Sie diese Zielgruppe auf dieselbe Zielgruppendimension wie die Hauptzielgruppe zurück. Klicken Sie im Abschnitt „Ausschlussregeln“ auf „Regel hinzufügen“ und geben Sie die Bedingungen für die Dimensionsänderung an. Die Datenabstimmung wird entweder über ein Attribut oder einen Join durchgeführt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Auswählen von Sets, die kombiniert werden sollen"
>abstract="Wählen Sie im Abschnitt **Zusammenzuführende Mengen** die **Hauptmenge** aus den eingehenden Transitionen. Dies ist die Menge, aus der Elemente ausgeschlossen werden. Die anderen Mengen stimmen mit Elementen überein, bevor sie aus der Primärmenge ausgeschlossen werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Ausschlussregeln"
>abstract="Bei Bedarf können die eingehenden Tabellen angepasst werden. Um eine Zielgruppe aus einer anderen Dimension auszuschließen, setzen Sie diese Zielgruppe auf dieselbe Zielgruppendimension wie die Hauptzielgruppe zurück. Klicken Sie im Abschnitt „Ausschlussregeln“ auf „Regel hinzufügen“ und geben Sie die Bedingungen für die Dimensionsänderung an. Die Datenabstimmung wird entweder über ein Attribut oder einen Join durchgeführt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Kombinieren von „Komplement erzeugen“"
>abstract="Aktivieren Sie die Option „Komplement erzeugen“, um die verbleibende Population in einer zusätzlichen Transition zu verarbeiten."

Konfigurieren Sie in der Aktivität **Kombinieren** einen **Ausschluss**, indem Sie diese zusätzlichen Schritte ausführen: 

1. Wählen Sie im Abschnitt **Zusammenzuführende Mengen** die **Hauptmenge** aus den eingehenden Transitionen. Dies ist die Menge, aus der Elemente ausgeschlossen werden. Die anderen Mengen stimmen mit Elementen überein, bevor sie aus der Primärmenge ausgeschlossen werden.
1. Bei Bedarf können die eingehenden Tabellen angepasst werden. Um eine Zielgruppe aus einer anderen Dimension auszuschließen, setzen Sie diese Zielgruppe auf dieselbe Zielgruppendimension wie die Hauptzielgruppe zurück. Klicken Sie im Abschnitt **Ausschlussregeln** auf **Regel hinzufügen** und geben Sie die Bedingungen für die Dimensionsänderung an. Die Datenabstimmung wird entweder über ein Attribut oder einen Join durchgeführt.
1. Aktivieren Sie die Option **Komplement erzeugen**, wenn Sie auch die nicht in der Schnittmenge enthaltene Population verwenden möchten. Siehe den Abschnitt [Schnittmenge](#intersection).

## Beispiele {#combine-examples}

Im folgenden Beispiel verwendet die Aktivität **Kombinieren** eine **Vereinigung**, um alle Profile der beiden Abfragen abzurufen: Personen zwischen 18 und 27 Jahren und Personen zwischen 34 und 40 Jahren.

![](../assets/workflow-union-example.png)

Das folgende Beispiel zeigt die **Schnittmenge** zwischen zwei Abfrageaktivitäten. Sie ruft Profile ab, die zwischen 18 und 27 Jahre alt sind und deren E-Mail-Adresse angegeben wurde.

![](../assets/workflow-intersection-example.png)

Folgendes **Ausschluss**-Beispiel zeigt zwei Abfragen, die zum Filtern von Profilen konfiguriert wurden, die zwischen 18 und 27 Jahre alt sind und über eine Adobe-E-Mail-Domain verfügen. Die Profile mit einer Adobe-E-Mail-Domain werden aus dem ersten Satz ausgeschlossen.

![](../assets/workflow-exclusion-example.png)