---
audience: end-user
title: Erstellen Ihrer erste Abfrage mithilfe des Abfrage-Modelers
description: Erfahren Sie, wie Sie Ihre erste Abfrage im Abfrage-Modeler in Adobe Campaign Web erstellen.
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '2310'
ht-degree: 73%

---


# Erstellen Ihrer ersten Abfrage {#build-query}

Um mit der Erstellung einer Abfrage zu beginnen, greifen Sie je nach der Aktion, die Sie ausführen wollen, vom gewünschten Speicherort aus auf den Abfrage-Modeler zu. Der Abfrage-Modellierer wird mit einer leeren Arbeitsfläche geöffnet. Klicken Sie auf die Schaltfläche **+**, um den ersten Knoten der Abfrage zu konfigurieren.

Sie können zwei Elementtypen hinzufügen:

* **Filterkomponenten** (benutzerdefinierte Bedingung, Zielgruppe auswählen, vordefinierter Filter) ermöglichen es Ihnen, eigene Regeln zu erstellen, eine Zielgruppe auszuwählen oder einen vordefinierten Filter zu verwenden, um Ihre Abfrage zu verfeinern. Sie werden zu Beginn Ihrer Abfrage und bei gepunkteten Transitionen hinzugefügt. [Erfahren Sie, wie Sie mit Filterkomponenten arbeiten können](#filtering)

  Beispiel: *Empfänger, die den Newsletter „Sport“ abonniert haben*, *Empfänger in New York*, *Empfänger in San Francisco*

  ![Beispiel für das Hinzufügen von Filterkomponenten zu einer Abfrage.](assets/query-add-component.png){zoomable="yes"}

* Mit **Gruppenoperatoren** (AND, OR, EXCEPT) können Sie Filterkomponenten im Diagramm gruppieren. Sie werden bei vorhandenen Transitionen vor einer Filterkomponente hinzugefügt. [Erfahren Sie, wie man mit Operatoren arbeitet](#filtering)

  Beispiel: *Empfängerinnen und Empfänger, die den Newsletter „Sport“ abonniert haben **UND**in New York **ODER**San Francisco leben*

  ![Beschreibung: Beispiel für das Hinzufügen von Gruppenoperatoren zu einer Abfrage.](assets/query-add-operator.png){zoomable="yes"}

## Werteverteilung in einer Abfrage {#distribution-values-query}

Die Werteverteilung zeigt den Prozentsatz jedes Werts eines Felds in einer Tabelle auf der Grundlage der aktuellen Abfrageparameter an. Die Kenntnis der Werteverteilung innerhalb einer Abfrage hilft, die Segmentierung zu verfeinern.

Um auf diese Option zuzugreifen, klicken Sie in Ihrer Abfrage auf die Schaltfläche zur Attributauswahl, wie unten dargestellt. Klicken Sie dann auf das Symbol **[!UICONTROL Informationen]** neben dem ausgewählten Attribut. Sie können auf die Schaltfläche **[!UICONTROL Werteverteilung]** zugreifen.

![Beschreibung: Zugriff auf die Option „Werteverteilung“ in einer Abfrage.](assets/values_query.png){zoomable="yes"}

>[!NOTE]
>
>* Bei Feldern mit vielen Werten werden nur die ersten zwanzig Werte angezeigt. In solchen Fällen werden Sie von einer Benachrichtigung **[!UICONTROL Teillast]** gewarnt.
>* Die Option **[!UICONTROL Werteverteilung]** ist in jeder Attributauswahl verfügbar. [Erfahren Sie, wie Sie Attribute auswählen](../get-started/attributes.md)
>* Mithilfe der **[!Aerweiterten Filter]** können Sie Bedingungen zu den Ergebnissen hinzufügen. [Weitere Informationen finden Sie hier](../get-started/work-with-folders.md#filter-the-values).

## Hinzufügen von Filterkomponenten {#filtering}

Filterkomponenten ermöglichen es Ihnen, eine Abfrage mithilfe von folgenden Filtern zu verfeinern:

* **[Benutzerdefinierte Bedingungen](#custom-condition)**: Filtern Sie eine Abfrage, indem Sie Ihre eigene Bedingung mit Attributen aus der Datenbank und erweiterten Ausdrücken erstellen.
* **[Zielgruppen](#audiences)**: Filtern Sie eine Abfrage, indem Sie eine vorhandene Zielgruppe verwenden.
* **[Vordefinierter Filter](#predefined-filters)**: Filtern Sie eine Abfrage mit vorhandenen vordefinierten Filtern.

### Konfigurieren einer benutzerdefinierten Bedingung {#custom-condition}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Benutzerdefinierte Bedingung"
>abstract="Benutzerdefinierte Bedingungen filtern Komponenten, mit denen Sie Ihre Abfrage filtern können, indem Sie Ihre eigene Bedingung mit Attributen aus der Datenbank und erweiterten Ausdrücken erstellen."

Gehen Sie wie folgt vor, um Ihre Abfrage mit einer benutzerdefinierten Bedingung zu filtern:

1. Klicken Sie auf die Schaltfläche **+** auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Benutzerdefinierte Bedingung]** aus. Der Eigenschaftenbereich für benutzerdefinierte Bedingungen wird auf der rechten Seite geöffnet.

1. Wählen Sie **Feld „Attribut** das Attribut aus der Datenbank aus, das Sie zum Erstellen Ihrer Bedingung verwenden möchten. Die Attributliste enthält alle Attribute aus Ihrer Campaign-Datenbank, einschließlich der Attribute aus verknüpften Tabellen. [Erfahren Sie, wie Sie Attribute auswählen und zu den Favoriten hinzufügen](../get-started/attributes.md)

   ![Auswählen von Attributen für eine benutzerdefinierte Bedingung in einer Abfrage.](assets/query-custom-condition-fields.png){zoomable="yes"}

   >[!NOTE]
   >
   >Mit der Schaltfläche **Ausdruck bearbeiten** können Sie den Ausdruckseditor von Campaign Web verwenden, um einen Ausdruck manuell mithilfe von Feldern aus der Datenbank und Hilfsfunktionen zu definieren. [Erfahren Sie, wie Sie Ausdrücke bearbeiten](expression-editor.md)

1. Wählen Sie in der Dropdown-Liste den anzuwendenden Operator aus. Es stehen verschiedene Operatoren zur Verfügung. Beachten Sie, dass die in der Dropdown-Liste verfügbaren Operatoren vom Datentyp des Attributs abhängen.

   +++Liste der verfügbaren Operatoren

   | Operator | Zweck | Beispiel |
   |---|---|---|
   | Gleich | Die zurückgegebenen Daten stimmen vollständig mit dem in der zweiten Spalte angegebenen Wert überein. | Nachname (@lastName) gleich „Jones“ gibt nur Empfänger zurück, deren Nachname Jones ist. |
   | Ungleich | Die ausgegebenen Daten unterscheiden sich vom angegebenen Wert. | Sprache (@language) ist ungleich &#39;Englisch&#39;. |
   | Größer als | Die ausgegebenen Daten übersteigen den angegebenen Wert. | Alter (@age) größer als 50 gibt alle Werte größer als „50“ zurück, z. B. „51“, „52“. |
   | Kleiner als | Der ausgegebene Wert unterschreitet den eingegebenen Wert. | Erstellungsdatum (@created) vor &#39;DaysAgo(100)&#39; gibt alle Empfänger zurück, die vor weniger als 100 Tagen erstellt wurden. |
   | Größer als oder gleich | Die ausgegebenen Daten sind identisch mit oder übersteigen den angegebenen Wert. | Alter (@age) größer oder gleich „30“ gibt alle Empfänger ab 30 zurück. |
   | Kleiner als oder gleich | Die ausgegebenen Daten sind identisch mit oder unterschreiten den angegebenen Wert. | Mit Alter (@age) kleiner oder gleich „60“ werden alle Empfänger mit einem Alter von 60 Jahren oder jünger zurückgegeben. |
   | Eingeschlossen in | Die ausgegebenen Daten sind in den angegebenen Werten enthalten. Diese Werte müssen durch ein Komma getrennt werden. | Das Geburtsdatum (@birthDate) ist in &#39;12/10/1979,12/10/1984&#39; enthalten und gibt die Empfänger zurück, die zwischen diesen Daten geboren wurden. |
   | Ist nicht enthalten in | Funktioniert wie der Operator Ist enthalten in . Hier werden Empfänger anhand der eingegebenen Werte ausgeschlossen. | Das Geburtsdatum (@birthDate) ist nicht in &#39;12/10/1979,12/10/1984&#39; enthalten. Empfänger, die innerhalb dieser Daten geboren wurden, werden nicht zurückgegeben. |
   | Ist leer | Gibt Ergebnisse zurück, die einem leeren Wert in der zweiten Spalte Wert entsprechen. | „Mobiltelefon (@mobilePhone) ist leer“ gibt alle Empfängerinnen und Empfänger zurück, die keine Mobiltelefonnummer haben. |
   | Ist nicht leer | Negative Form des Operators „Ist leer“. Es ist nicht nötig, Daten in die zweite Wert-Spalte einzugeben. | E-Mail (@email) ist nicht leer. |
   | Beginnt mit | Gibt Ergebnisse zurück, die mit dem eingegebenen Wert beginnen. | Kundennummer (@account) beginnt mit &#39;32010&#39;. |
   | Beginnt nicht mit | Gibt Ergebnisse zurück, die nicht mit dem eingegebenen Wert beginnen. | Konto # (@account) beginnt nicht mit „20“. |
   | Enthält | Gibt Ergebnisse zurück, die mindestens den eingegebenen Wert enthalten. | E-Mail-Domain (@domain) enthält „mail“. Gibt alle Domain-Namen zurück, die „mail“ enthalten, z. B. „gmail.com“. |
   | Enthält nicht | Die ausgegebenen Daten enthalten den angegebenen Wert nicht. | E-Mail-Domain (@domain) enthält nicht „vo“. Domänennamen, die „vo“ enthalten, wie z. B. „voila.fr“, werden nicht in den Ergebnissen angezeigt. |
   | Ist wie | Ähnlich wie beim Operator „Enthält“ können Sie damit ein Platzhalterzeichen % in den Wert einfügen. | Nachname (@lastName) ist wie &#39;Me%er&#39;. Das Platzhalterzeichen dient als „Joker“, um Namen wie „Jones“ zu finden. |
   | Ist nicht wie | Ähnlich wie beim Operator „Enthält“ können Sie damit ein Platzhalterzeichen % in den Wert einfügen. | Nachname (@lastName) nicht wie „Schmi%t“. Empfänger mit dem Nachnamen „Smith“ werden nicht zurückgegeben. |

+++

1. Legen Sie im Feld **Wert** den erwarteten Wert fest. Sie können auch den Web-Ausdruckseditor von Campaign verwenden, um einen Ausdruck manuell mithilfe von Feldern aus der Datenbank und Hilfsfunktionen zu definieren. Klicken Sie dazu auf die Schaltfläche **Ausdruck bearbeiten**. [Erfahren Sie, wie Sie Ausdrücke bearbeiten](expression-editor.md)

   *Abfragebeispiel, in dem alle Profile im Alter von 21 Jahren oder älter zurückgegeben werden:*

   ![Beispiel einer Abfrage mit Profilen ab 21 Jahren.](assets/query-custom-condition.png){zoomable="yes"}

   Für Attribute vom Typ „Datum“ sind vordefinierte Werte bei Verwendung der Option **[!UICONTROL Voreinstellungen]** verfügbar.

   ![Beispiel für die Verwendung von Datumsvorgaben in einer Abfrage.](assets/date-presets.png){zoomable="yes"}

#### Benutzerdefinierte Bedingungen für verknüpfte Tabellen (1:1- und 1:n-Relation){#links}

Mit benutzerdefinierten Bedingungen können Sie Tabellen abfragen, die mit der aktuell von Ihrer Regel verwendeten Tabelle verknüpft sind. Dazu gehören Tabellen mit einer 1:1-Relation oder Sammlungstabellen (1:n-Relation).

Navigieren Sie bei einer **1:1-Relation** zur verknüpften Tabelle, wählen Sie das gewünschte Attribut aus und definieren Sie den erwarteten Wert.

Sie können auch direkt eine Tabellenverknüpfung in der Auswahl **Wert** auswählen und bestätigen. In diesem Fall müssen die für die ausgewählte Tabelle verfügbaren Werte mit einer speziellen Auswahl ausgewählt werden, wie im folgenden Beispiel gezeigt.

+++Abfragebeispiel

Hier geht es bei der Abfrage um Marken mit der Bezeichnung „Laufen“.

1. Navigieren Sie durch die Tabelle **Marke** und wählen Sie das Attribut **Titel**.

   ![Screenshot der Brand-Tabelle](assets/1-1-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Definieren Sie den erwarteten Wert für das Attribut.

   ![Beispiel für einen definierten erwarteten Wert](assets/1-1-table.png){zoomable="yes"}{width="85%" align="center"}

Hier ist ein Abfragebeispiel, bei dem eine Tabellenverknüpfung direkt ausgewählt wurde. Die verfügbaren Werte für diese Tabelle müssen über eine spezielle Auswahl ausgewählt werden.

![Beispiel für eine Abfrage](assets/1-1-table-direct.png){zoomable="yes"}{width="85%" align="center"}

+++

Für eine **1:n-Relation** können Sie Unterbedingungen definieren, um Ihre Abfrage zu verfeinern, wie im folgenden Beispiel gezeigt.

+++Abfragebeispiel

In unserem Beispiel zielt die Abfrage auf Empfängerinnen und Empfänger ab, die im Zusammenhang mit dem BrewMaster-Produkt Einkäufe getätigt haben, und zwar für einen Gesamtbetrag von mindestens 100 USD.

1. Wählen Sie die Tabelle **Käufe** und bestätigen Sie.

   ![Screenshot der Tabelle „Einkauf“](assets/1-N-collection.png){zoomable="yes"}{width="50%" align="center"}

1. Es wird eine ausgehende Transition hinzugefügt, die die Erstellung von Unterbedingungen ermöglicht.

   ![Beispiel einer ausgehenden Transition](assets/1-n-subcondition.png){zoomable="yes"}{width="85%" align="center"}

1. Wählen Sie das Attribut **Preis** und Zielkäufe von 1000 USD oder mehr

   ![Screenshot des Preisattributs](assets/1-n-price.png){zoomable="yes"}{width="85%" align="center"}

1. Fügen Sie Unterbedingungen hinzu, die Ihren Anforderungen entsprechen. In unserem Beispiel haben wir eine Bedingung für Profile hinzugefügt, die ein BrewMaster-Produkt erworben haben.

   ![Beispiel für Unterbedingungen](assets/custom-condition-1-N.png){zoomable="yes"}{width="85%" align="center"}

+++

#### Arbeiten mit aggregierten Daten {#aggregate}

Mit benutzerdefinierten Bedingungen können Sie Aggregierungsvorgänge ausführen. Wählen Sie dazu direkt ein Attribut aus einer Sammlungstabelle aus:

1. Navigieren Sie durch die gewünschte Sammlungstabelle und wählen Sie das Attribut aus, für das Sie einen Aggregierungsvorgang durchführen möchten.

   ![Screenshot der Attributliste](assets/aggregate-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Aktivieren Sie im Eigenschaften-Fenster die Option **Daten aggregieren** und wählen Sie die gewünschte Aggregierungsfunktion aus.

   ![Screenshot der Option „Daten aggregieren“](assets/aggregate.png){zoomable="yes"}{width="85%" align="center"}

### Auswählen einer Zielgruppe {#audiences}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Zielgruppe auswählen"
>abstract="Wenn Sie die Option **Zielgruppe auswählen** verwenden, können Sie die Zielgruppe auswählen, die Sie zum Filtern Ihrer Abfrage verwenden möchten."

Gehen Sie wie folgt vor, um Ihre Abfrage mithilfe einer vorhandenen Zielgruppe zu filtern:

1. Klicken Sie auf die Schaltfläche **+** auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Zielgruppe auswählen]** aus.

1. Der Bereich mit den Eigenschaften **Zielgruppe auswählen** wird auf der rechten Seite geöffnet. Wählen Sie die Zielgruppe aus, die Sie zum Filtern Ihrer Abfrage verwenden möchten.

   *Abfragebeispiel, in dem alle Profile der Zielgruppe „Festivalbesuchende“ zurückgegeben werden:*

   ![Screenshot eines Abfragebeispiels](assets/query-audience.png){zoomable="yes"}

### Verwenden eines vordefinierten Filters {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Vordefinierter Filter"
>abstract="Wenn Sie die Option **Vordefinierter Filter** verwenden, können Sie einen vordefinierten Filter aus der Liste der benutzerdefinierten Filter oder aus den Favoriten auswählen."

Gehen Sie wie folgt vor, um Ihre Abfrage mithilfe eines vordefinierten Filters zu filtern:

1. Klicken Sie auf die Schaltfläche **+** auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Vordefinierter Filter]** aus.

1. Der Bereich mit den Eigenschaften **Vordefinierter Filter** wird auf der rechten Seite geöffnet. Wählen Sie einen Filter aus der Liste der vordefinierten Filter oder aus den Favoriten aus.

   *Abfragebeispiel, in dem alle Profile zurückgegeben werden, die dem vordefinierten Filter „Inaktive Kunden“ entsprechen:*

   ![Screenshot eines Abfragebeispiels](assets/query-predefined-filter.png){zoomable="yes"}

### Kopieren und Einfügen von Komponenten {#copy}

Mithilfe des Abfrage-Modelers können Sie eine oder mehrere Filterkomponenten kopieren und am Ende einer Transition einfügen. Dieser Vorgang kann in der aktuellen Abfragearbeitsfläche oder in einer beliebigen Arbeitsfläche innerhalb Ihrer Instanz ausgeführt werden.

>[!NOTE]
>
>Die kopierte Auswahl wird beibehalten, solange Sie in Ihrer Instanz arbeiten. Wenn Sie sich abmelden und wieder anmelden, steht Ihre Auswahl nicht mehr zum Einfügen zur Verfügung.

Gehen Sie wie folgt vor, um Filterkomponenten zu kopieren und einzufügen:

1. Klicken Sie in der Abfragearbeitsfläche auf die Filterkomponente, die Sie kopieren möchten. Um mehrere Komponenten auszuwählen, verwenden Sie das Tool zur Mehrfachauswahl in der Symbolleiste oben rechts auf der Arbeitsfläche.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Kopieren]** im Eigenschaften-Fenster der Komponente oder in der blauen Leiste unten im Bildschirm, wenn Sie mehrere Komponenten ausgewählt haben.

   | Kopieren einer einzelnen Komponente | Kopieren mehrerer Komponenten |
   |  ---  |  ---  |
   | ![](assets/copy-single-component.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} | ![](assets/copy-multiple-components.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |

1. Um die Komponente(n) einzufügen, klicken Sie auf die Schaltfläche „+“ am Ende der gewünschten Transition und wählen Sie **(n) Elemente einfügen**.

   ![Beispiel für das Einfügen der Komponenten](assets/copy-paste.png){zoomable="yes"}

## Kombinieren von Filterkomponenten mit Operatoren {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Gruppe"
>abstract="In diesem Bereich können Sie den Operator ändern, mit dem Filterbedingungen verknüpft werden."

Jedes Mal, wenn Sie zu Ihrer Abfrage eine neue Filterkomponente hinzufügen, wird diese automatisch durch einen **UND**-Operator mit der anderen Komponente verknüpft. Dadurch werden die Ergebnisse der beiden Filterkomponenten kombiniert.

In diesem Beispiel haben wir für die zweite Transition neue Zielgruppentyp-Filterkomponenten hinzugefügt. Die Komponente ist mit der vordefinierten Filterbedingung durch einen **UND**-Operator verknüpft, d. h., die Abfrageergebnisse enthalten Empfängerinnen und Empfänger, auf die der vordefinierte Filter „Wohnhaft in Madrid“ zutrifft UND die zur Zielgruppe „Rabattjäger“ gehören.

![Beispiel einer Abfrage](assets/query-operator.png){zoomable="yes"}

Um den Operator für die Verknüpfung der Filterbedingungen zu ändern, klicken Sie darauf und wählen Sie den gewünschten Operator im Bereich **Gruppe** aus, der sich rechts öffnet.

Die folgenden Operatoren sind verfügbar:

* **UND (Schnittmenge)**: Kombiniert Ergebnisse, die allen Filterkomponenten in den ausgehenden Transitionen entsprechen.
* **ODER (Vereinigung)**: Umfasst Ergebnisse, die mindestens einer der Filterkomponenten in den ausgehenden Transitionen entsprechen.
* **AUSSER (Ausschluss)**: Schließt Ergebnisse aus, die allen Filterkomponenten in der ausgehenden Transition entsprechen.

![Beispiel einer Abfrage](assets/query-operator-change.png){zoomable="yes"}

Darüber hinaus können Sie Zwischengruppen von Komponenten erstellen, indem Sie auf die Schaltfläche **+** auf einer Transition klicken. Auf diese Weise können Sie einen Operator an dieser bestimmten Stelle hinzufügen, um mehrere Komponenten zu gruppieren und Ihre Abfrage zu verfeinern.

Im folgenden Beispiel haben wir eine Zwischengruppe erstellt, um Ergebnisse aus den Zielgruppen „Zu belohnende VIP“ oder „Super VIP“ einzubeziehen.

![Beispiel einer Abfrage](assets/query-intermediate-group.png){zoomable="yes"}

## Überprüfen und Validieren einer Abfrage

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Regeleigenschaften"
>abstract="Nachdem Sie Ihre Abfrage auf der Arbeitsfläche erstellt haben, können Sie sie über den Bereich **Regeleigenschaften** auf der rechten Seite überprüfen.<br/>In diesem Bereich können Sie die resultierenden Daten anzeigen, eine SQL-Code-Version der Abfrage abrufen und die Anzahl der Zieleinträge überprüfen.<br/>Verwenden Sie die Schaltfläche **Filter auswählen oder speichern**, um Ihre Abfrage als vordefinierten Filter zu speichern oder den Inhalt der Arbeitsfläche durch einen vorhandenen Filter zu ersetzen."

Nachdem Sie Ihre Abfrage auf der Arbeitsfläche erstellt haben, können Sie sie über den Bereich **Regeleigenschaften** auf der rechten Seite überprüfen. Dieser Bereich wird beim Einrichten einer Abfrage zum Erstellen einer Zielgruppe angezeigt. Verfügbare Operationen sind:

* **Ergebnisse anzeigen:** Zeigt die aus Ihrer Abfrage resultierenden Daten an.
* **Code-Ansicht**: Zeigt eine Code-basierte Version der Abfrage in SQL an.
* **Berechnen**: Aktualisiert und zeigt die Anzahl der Einträge an, auf die Ihre Abfrage abzielt.
* **Filter auswählen oder speichern**: Wählen Sie einen vorhandenen vordefinierten Filter aus, um ihn in der Arbeitsfläche zu verwenden, oder speichern Sie Ihre Abfrage als neu vordefinierten Filter, um sie später erneut zu verwenden. [Erfahren Sie, wie Sie mit vordefinierten Filtern arbeiten](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Wählen Sie im Bereich mit den Regeleigenschaften einen vordefinierten Filter aus, um die in der Arbeitsfläche erstellte Abfrage durch den ausgewählten Filter zu ersetzen.

Wenn Ihre Abfrage fertig ist, klicken Sie auf die Schaltfläche **[!UICONTROL Bestätigen]** in der rechten oberen Ecke, um sie zu speichern.

Sie können Ihre Abfrage jederzeit ändern, indem Sie sie öffnen. Beachten Sie, dass beim Öffnen einer vorhandenen Abfrage diese in einer vereinfachten Ansicht angezeigt wird, ohne dass die Schaltflächen **+** angezeigt werden. Um der Abfrage neue Elemente hinzuzufügen, wählen Sie eine Komponente oder einen Operator auf der Arbeitsfläche aus, um die Schaltflächen **+** anzuzeigen.

![Beispiel einer Abfrage](assets/edit-audience.png){zoomable="yes"}

