---
audience: end-user
title: Erstellen Sie Ihre erste Abfrage mithilfe des Abfragemodells
description: Erfahren Sie, wie Sie Ihre erste Abfrage in Adobe Campaign Web Query Modeler erstellen.
source-git-commit: cc909bdf7507e66e000297440e31f9b5260f1257
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 15%

---

# Erste Abfrage erstellen {#build-query}

Um mit der Erstellung einer Abfrage zu beginnen, greifen Sie je nach gewünschter Aktion vom gewünschten Speicherort auf das Abfragemodell zu. Das Abfragemodell wird mit einer leeren Arbeitsfläche geöffnet. Klicken Sie auf **+** -Schaltfläche, um den ersten Knoten Ihrer Abfrage zu konfigurieren.

Sie können zwei Elementtypen hinzufügen:

* **Komponenten filtern** (Benutzerdefinierte Bedingung, Zielgruppe auswählen, vordefinierter Filter) ermöglichen es Ihnen, eigene Regeln zu erstellen, eine Zielgruppe oder einen vordefinierten Filter auszuwählen, um Ihre Abfrage zu verfeinern. [Erfahren Sie, wie Sie mit Filterkomponenten arbeiten](#filtering)

  Beispiel:

  *Empfänger, die den Newsletter &quot;Sport&quot;abonniert haben*. *Empfänger mit Wohnsitz in New York*, *Empfänger mit Wohnsitz in San Francisco*

* **Gruppenoperatoren** (AND, OR, EXCEPT) ermöglichen es Ihnen, die Filterkomponenten im Diagramm nach Ihren Bedürfnissen zu gruppieren. [Erfahren Sie, wie Sie mit Operatoren arbeiten.](#filtering)

  Beispiel:

  *Empfänger, die den Newsletter &quot;Sport&quot;abonniert haben **UND**die in New York leben **ODER**San Francisco*.

![](assets/query-add-component.png)

## Hinzufügen von Filterkomponenten {#filtering}

Filterkomponenten ermöglichen es Ihnen, Ihre Abfrage mithilfe von:

* **Benutzerdefinierte Bedingungen**: Filtern Sie Ihre Abfrage, indem Sie Ihre eigene Bedingung mit Attributen aus der Datenbank und erweiterten Ausdrücken erstellen.
* **Zielgruppen**: Filtern Sie Ihre Abfrage mit einer vorhandenen Zielgruppe.
* **Vordefinierter Filter**: Filtern Sie Ihre Abfrage mit vorhandenen vordefinierten Filtern.

### Benutzerdefinierte Bedingung konfigurieren

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Benutzerdefinierte Bedingung"
>abstract="Benutzerdefinierte Bedingung"

Gehen Sie wie folgt vor, um Ihre Abfrage mit einer benutzerdefinierten Bedingung zu filtern:

1. Klicken Sie auf **+** auf dem gewünschten Knoten klicken und **[!UICONTROL Benutzerdefinierte Bedingung]**. Der Bereich mit den benutzerdefinierten Bedingungseigenschaften wird auf der rechten Seite geöffnet.

1. Im **Attribut** -Feld das Attribut aus der Datenbank auswählen, das Sie zum Erstellen Ihrer Bedingung verwenden möchten. Die Attributliste enthält alle Attribute aus Ihrer Campaign-Datenbank, einschließlich der mit Ihrer Tabelle verknüpften Attribute.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Die Schaltfläche Ausdruck bearbeiten ermöglicht die Verwendung des Ausdruckseditors für Campaign-Webausdrücke, um mithilfe von Feldern aus der Datenbank und Hilfsfunktionen einen Ausdruck manuell zu definieren.

1. Wählen Sie in der Dropdown-Liste den anzuwendenden Operator aus. Es stehen verschiedene Operatoren zur Verfügung. Beachten Sie, dass die in der Dropdown-Liste verfügbaren Operatoren vom Datentyp des ausgewählten Attributs abhängen.

   ++ + Liste der verfügbaren Operatoren

   | Operator | Zweck | Beispiel |
   |  ---  |  ---  |  ---  |
   | Gleich | Die ausgegebenen Daten stimmen vollständig mit dem angegebenen Wert überein. | Nachname (@lastName) gleich &#39;Jones&#39;, gibt nur Empfänger zurück, deren Nachname Jones ist. |
   | Ungleich | Die ausgegebenen Daten unterscheiden sich vom angegebenen Wert. | Sprache (@language) ungleich &#39;Englisch&#39; |
   | Größer als | Die ausgegebenen Daten übersteigen den angegebenen Wert. | Alter (@age) über 50</strong>, gibt alle Werte zurück, die größer als &#39;50&#39; sind, d. h. &#39;51&#39;, &#39;52&#39; usw. |
   | Kleiner als | Die ausgegebenen Daten unterschreiten den angegebenen Wert. | Erstellungsdatum (@created) vor &#39;DaysAgo(100)&#39;</strong>zurückgibt alle Empfänger zurück, die vor weniger als 100 Tagen erstellt wurden. |
   | Größer als oder gleich | Die ausgegebenen Daten sind identisch mit oder übersteigen den angegebenen Wert. | Alter (@age) größer/gleich &#39;30&#39;</strong>, gibt alle Empfänger ab 30 Jahren zurück. |
   | Kleiner als oder gleich | Die ausgegebenen Daten sind identisch mit oder unterschreiten den angegebenen Wert. | Alter (@age) kleiner oder gleich &#39;60&#39;</strong>, gibt alle Empfänger im Alter von 60 Jahren oder weniger zurück. |
   | Enthalten in | Die ausgegebenen Daten sind in den angegebenen Werten enthalten. Die Werte werden durch Kommata getrennt. | Das Geburtsdatum (@birthDate) ist in &#39;12/10/1979,12/10/1984&#39; enthalten, gibt die Empfänger zurück, die zwischen diesen Daten geboren wurden. |
   | Nicht enthalten | Funktioniert wie der Operator Ist im . Im vorliegenden Beispiel sollen die Empfänger anhand der eingegebenen Werte ausgeschlossen werden. | Das Geburtsdatum (@birthDate) ist nicht in &#39;12/10/1979,12/10/1984&#39; enthalten. Im Gegensatz zum vorherigen Beispiel werden innerhalb dieser Datumswerte geborene Empfänger nicht zurückgegeben. |
   | Ist leer | Die ausgegebenen Daten enthalten keinen Wert in der entsprechenden Spalte. | Mobiltelefon (@mobilePhone) ist leer; gibt alle Empfänger zurück, für die keine Mobiltelefonnummer angegeben wurde. |
   | Ist nicht leer | Negative Form des Operators ist leer . Es ist nicht erforderlich, Daten in die zweite Wert -Spalte einzutragen. | E-Mail (@email) ist nicht leer. |
   | Beginnt mit | Die ausgegebenen Daten beginnen mit dem angegebenen Wert. | Kundennummer (@account) beginnt mit &#39;32010&#39;. |
   | Beginnt nicht mit | Die ausgegebenen Daten beginnen nicht mit dem angegebenen Wert. | Kundennummer (@account) beginnt nicht mit &#39;20&#39; |
   | Enthält | Die ausgegebenen Daten enthalten den angegebenen Wert. | E-Mail-Domain (@domain) enthält &#39;mail&#39;</strong>gibt alle Domänennamen zurück, die &quot;mail&quot;enthalten. Die Domain &#39;gmail.com&#39; wird also ebenfalls zurückgegeben. |
   | Enthält nicht | Die ausgegebenen Daten enthalten den angegebenen Wert nicht. | E-Mail-Domain (@domain) enthält nicht &#39;vo&#39;</strong>. In diesem Fall werden Domänennamen, die &quot;vo&quot;enthalten, nicht zurückgegeben. Der Domänenname &quot;voila.fr&quot;wird nicht in den Ergebnissen angezeigt. |
   | Ist wie | Ist wie ähnelt dem Operator Enthält sehr. Damit können Sie einen Platzhalterzeichen % in den Wert einfügen. | Nachname (@lastName) wie &quot;Jon%s&quot;. Hier wird das Platzhalterzeichen als &quot;Joker&quot;verwendet, um den Namen &quot;Jones&quot;zu finden, falls der Benutzer den fehlenden Buchstaben zwischen &quot;n&quot;und &quot;s&quot;vergessen hat. |
   | Ist nicht wie | Ist wie ähnelt dem Operator Enthält sehr. Damit können Sie einen Platzhalterzeichen % in den Wert einfügen. | Nachname (@lastName) nicht wie &quot;Schmi%t&quot;. Hier werden die Empfänger, deren Nachname &#39;Schmi%t&#39; lautet, nicht zurückgegeben. |

+++

1. Im **Wert** -Feld den erwarteten Wert festlegen. Sie können auch den Campaign-Web-Ausdruckseditor verwenden, um einen Ausdruck manuell mithilfe von Feldern aus der Datenbank und Hilfsfunktionen zu definieren. Klicken Sie dazu auf die Schaltfläche **Ausdruck bearbeiten** Schaltfläche.

   *Abfragebeispiel, in dem alle Profile im Alter von 21 Jahren oder älter zurückgegeben werden:*

   ![](assets/query-custom-condition.png)

### Auswählen einer Zielgruppe

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Zielgruppe auswählen"
>abstract="Zielgruppe auswählen"

Gehen Sie wie folgt vor, um Ihre Abfrage nach einer existierenden Audience zu filtern:

1. Klicken Sie auf **+** Schaltfläche auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Zielgruppe auswählen]**.

1. Die **Zielgruppe auswählen** Eigenschaftenfenster wird auf der rechten Seite geöffnet. Wählen Sie die Zielgruppe aus, die Sie zum Filtern Ihrer Abfrage verwenden möchten.

   *Abfragebeispiel, in dem alle Profile der Audience &quot;Festival Goers&quot;zurückgegeben werden:*

   ![](assets/query-audience.png)

### Verwenden eines vordefinierten Filters

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Vordefinierter Filter"
>abstract="Vordefinierter Filter"

Gehen Sie wie folgt vor, um Ihre Abfrage mithilfe eines vordefinierten Filters zu filtern:

1. Klicken Sie auf **+** auf dem gewünschten Knoten klicken und **[!UICONTROL Vordefinierter Filter]**.

1. Die **Vordefinierter Filter** Eigenschaftenfenster wird auf der rechten Seite geöffnet. Wählen Sie einen vordefinierten Filter aus der Liste der benutzerdefinierten Filter oder aus Favoriten aus.

   *Abfragebeispiel, das alle Profile zurückgibt, die dem vordefinierten Filter &quot;Inaktive Kunden&quot;entsprechen:*

   ![](assets/query-predefined-filter.png)

## Kombinieren von Filterkomponenten mit Operatoren {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Gruppe"
>abstract="Gruppe"

Jedes Mal, wenn Sie Ihrer Abfrage eine neue Filterkomponente hinzufügen, wird diese von einem AND-Operator automatisch mit der anderen Komponente verknüpft. Dies bedeutet, dass die Ergebnisse aus beiden Filterkomponenten in den Abfrageergebnissen kombiniert werden.

In diesem Beispiel haben wir für die zweite Transition eine neue Filterkomponente vom Typ Zielgruppe hinzugefügt. Die Komponente ist mit der vordefinierten Filtertypbedingung mit einem AND -Operator verknüpft, d. h. die Abfrageergebnisse enthalten Empfänger, die auf den vordefinierten Filter &quot;Madrider&quot; UND der Audience &quot;Rabattjäger&quot; ausgerichtet sind.

![](assets/query-operator.png)

Um den Operator zu ändern, der für die Verknüpfung der Filterbedingungen verwendet wird, klicken Sie darauf und wählen Sie den gewünschten Operator im rechten Bereich Gruppieren aus.

Die verfügbaren Operatoren sind:

* **AND (Schnittmenge)**: Kombiniert Ergebnisse aus allen Filterkomponenten in den ausgehenden Transitionen.
* **ODER (Vereinigung)**: Umfasst Ergebnisse aus mindestens einer der Filterkomponenten in die ausgehenden Transitionen.
* **AUSSER (Ausschluss)**: Schließt Ergebnisse aus allen Filterkomponenten in der ausgehenden Transition aus.

![](assets/query-operator-change.png)

## Abfrage überprüfen und validieren

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Eigenschaften der Regel"
>abstract="Eigenschaften der Regel"

Nachdem Sie Ihre Abfrage auf der Arbeitsfläche erstellt haben, können Sie sie mit der **Regeleigenschaften** Bereich auf der rechten Seite. Verfügbare Vorgänge sind:

* **Ergebnisse anzeigen:** Zeigt die aus Ihrer Abfrage resultierenden Daten an.
* **Codeansicht**: Zeigt eine code-basierte Version der Abfrage in SQL an.
* **berechnen**: Aktualisiert und zeigt die Anzahl der Datensätze an, auf die Ihre Abfrage zutrifft.
* **Filter auswählen oder speichern**: Wählen Sie einen vorhandenen vordefinierten Filter aus, der auf der Arbeitsfläche verwendet werden soll, oder speichern Sie Ihre Abfrage als vordefinierten Filter, um sie später erneut zu verwenden. [Erfahren Sie, wie Sie mit vordefinierten Filtern arbeiten](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Wählen Sie im Bereich Regeleigenschaften einen vordefinierten Filter aus, um die in der Arbeitsfläche erstellte Abfrage durch den ausgewählten Filter zu ersetzen.
