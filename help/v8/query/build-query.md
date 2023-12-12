---
audience: end-user
title: Erstellen Sie Ihre erste Abfrage mithilfe des Abfragemodells
description: Erfahren Sie, wie Sie Ihre erste Abfrage in Adobe Campaign Web Query Modeler erstellen.
source-git-commit: 119b7a65cb39d3cdfb225a673ae6452d2a5359fc
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 13%

---

# Erste Abfrage erstellen {#build-query}

Um mit der Erstellung einer Abfrage zu beginnen, greifen Sie je nach gewünschter Aktion vom gewünschten Speicherort auf das Abfragemodell zu. Das Abfragemodell wird mit einer leeren Arbeitsfläche geöffnet. Klicken Sie auf die Schaltfläche + , um den ersten Knoten Ihrer Abfrage hinzuzufügen.

![](assets/query-add-component.png)

Sie können zwei Elementtypen hinzufügen:

* Filterkomponenten (benutzerdefinierte Bedingung, Zielgruppe auswählen, vordefinierter Filter) ermöglichen es Ihnen, eigene Regeln zu erstellen, eine Zielgruppe auszuwählen oder einen vordefinierten Filter zu wählen, um Ihre Abfrage zu verfeinern.

  Beispiel *Empfänger, die den Newsletter &quot;Sport&quot;abonniert haben*. *Empfänger mit Wohnsitz in New York*, *Empfänger mit Wohnsitz in San Francisco*

* Mit Gruppenoperatoren (AND, OR, EXCEPT) können Sie Filterkomponenten im Diagramm nach Bedarf gruppieren.

  Beispiel: *Empfänger, die den Newsletter &quot;Sport&quot;abonniert haben **UND**die in New York leben **ODER**San Francisco*.

Im Folgenden finden Sie detaillierte Schritte zum Hinzufügen und Kombinieren von Filterkomponenten und Gruppenoperatoren.

## Hinzufügen von Filterkomponenten

Filterkomponenten ermöglichen es Ihnen, Ihre Abfrage mithilfe von:

* **Benutzerdefinierte Bedingungen**: Filtern Sie Ihre Abfrage, indem Sie Ihre eigene Bedingung mit Attributen aus der Datenbank und erweiterten Ausdrücken erstellen.
* **Zielgruppen**: Filtern Sie Ihre Abfrage mit einer vorhandenen Zielgruppe.
* **Vordefinierter Filter**: Filtern Sie Ihre Abfrage mit vorhandenen vordefinierten Filtern.

### Benutzerdefinierte Bedingung erstellen

Gehen Sie wie folgt vor, um Ihre Abfrage mit einer benutzerdefinierten Bedingung zu filtern:

1. Klicken Sie auf die Schaltfläche + auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Benutzerdefinierte Bedingung]**.
1. Der Bereich mit den benutzerdefinierten Bedingungseigenschaften wird auf der rechten Seite geöffnet. Wählen Sie im Feld Attribut das Attribut aus der Datenbank aus, das Sie zum Erstellen Ihrer Bedingung verwenden möchten.

   Die verfügbaren Attribute stellen alle Felder aus Ihrer Campaign-Datenbank dar, einschließlich der Felder aus Tabellen, die mit der Empfängertabelle verknüpft sind.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Die Schaltfläche Ausdruck bearbeiten ermöglicht die Verwendung des Ausdruckseditors für Campaign-Webausdrücke, um mithilfe von Feldern aus der Datenbank und Hilfsfunktionen einen Ausdruck manuell zu definieren.

1. Wählen Sie in der Dropdown-Liste den anzuwendenden Operator aus.

   ++ + Liste der verfügbaren Operatoren

   >[!NOTE]
   >
   >Die verfügbaren Operatoren in der Dropdown-Liste hängen vom Datentyp des ausgewählten Attributs ab.

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

1. Wählen Sie im Feld Wert den erwarteten Wert aus.

   Sie können auch den Campaign-Web-Ausdruckseditor verwenden, um einen Ausdruck manuell mithilfe von Feldern aus der Datenbank und Hilfsfunktionen zu definieren. Klicken Sie dazu auf die Schaltfläche Ausdruck bearbeiten .

   *Beispiel: Abfrage, die alle Profile im Alter von 21 Jahren oder älter zurückgibt*

   ![](assets/query-custom-condition.png)

<!--
querying linked tables
collect additional information on the targeted population, e.g. contract numbers, subscriptions to newsletters or origin.
Select the type of data you want to add. This can be data belonging to the filtering dimension or data stored in linked tables. Select the table which contains the information you want to collect and click Next.

aggregates: Define a calculation mode for the field to be added, such as an aggregate for example.-->

### Auswählen einer Zielgruppe

Gehen Sie wie folgt vor, um Ihre Abfrage nach einer existierenden Audience zu filtern:

1. Klicken Sie auf die Schaltfläche + auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Zielgruppe auswählen]**.

1. Der Bereich Zielgruppeneigenschaften auswählen wird auf der rechten Seite geöffnet. Wählen Sie die Zielgruppe aus, die zum Filtern Ihrer Abfrage verwendet werden soll.

   *Beispiel: Abfrage, die alle Profile der Audience &quot;Festival Goers&quot; zurückgibt*

   ![](assets/query-audience.png)

### Verwenden eines vordefinierten Filters

Gehen Sie wie folgt vor, um Ihre Abfrage mithilfe eines vordefinierten Filters zu filtern:

1. Klicken Sie auf die Schaltfläche + auf dem gewünschten Knoten und wählen Sie **[!UICONTROL Vordefinierter Filter]**.

1. Der Bereich Zielgruppeneigenschaften auswählen wird auf der rechten Seite geöffnet. Wählen Sie einen vordefinierten Filter aus der Liste der benutzerdefinierten Filter oder aus Favoriten aus.

   *Beispiel: Abfrage, die alle Profile zurückgibt, die dem vordefinierten Filter &quot;Inaktive Kunden&quot;entsprechen.*

   ![](assets/query-predefined-filter.png)

## Kombinieren von Filterkomponenten mit Operatoren

Beim Hinzufügen einer Filterkomponente zu Ihrer Abfrage wird automatisch eine neue Transition auf der Arbeitsfläche der Abfrage erstellt und die neue Filterkomponente wird durch einen UND -Operator mit der ersten Komponente verknüpft. Dies bedeutet, dass die Ergebnisse aus beiden Filterkomponenten in den Abfrageergebnissen kombiniert werden.

In diesem Beispiel wird der Arbeitsfläche eine neue Filterkomponente vom Typ Zielgruppe hinzugefügt. Sie wird automatisch bei einer neuen Transition hinzugefügt und mit der vordefinierten Filtertypbedingung mit einem AND -Operator verknüpft. In diesem Fall enthalten die Abfrageergebnisse die Empfänger, die dem vordefinierten Filter &quot;Madrider&quot; UND der Audience &quot;Rabattjäger&quot; angehören.

![](assets/query-operator.png)

Um den Operator zu ändern, der für die Verknüpfung der Filterbedingungen verwendet wird, klicken Sie darauf und wählen Sie den gewünschten Operator im Feld Den Operator können Sie ändern, indem Sie darauf klicken und im rechts geöffneten Gruppenbereich den gewünschten Operator auswählen.

![](assets/query-operator-change.png)

Die verfügbaren Operatoren sind:

* AND (Schnittmenge): kombiniert Ergebnisse aus allen Filterkomponenten der ausgehenden Transitionen.
* ODER (Vereinigung): enthält Ergebnisse aus mindestens einer der Filterkomponenten in den ausgehenden Transitionen.
* AUSSER (Ausschluss): Schließt Ergebnisse aus allen Filterkomponenten der ausgehenden Transition aus.

## Abfrage überprüfen und validieren

Nachdem Sie Ihre Abfrage auf der Arbeitsfläche erstellt haben, können Sie sie über den Bereich Regeleigenschaften auf der rechten Seite überprüfen. Folgende Vorgänge sind verfügbar:

* **Ergebnisse anzeigen:** zeigt die aus Ihrer Abfrage resultierenden Daten an.
* **Codeansicht**: zeigt eine code-basierte Version der Abfrage in SQL an.
* **berechnen**: aktualisiert die Anzahl der Datensätze und zeigt sie an, auf die die Abfrage zutrifft.
* **Filter auswählen oder speichern**: Wählen Sie einen vorhandenen vordefinierten Filter aus, der auf der Arbeitsfläche verwendet werden soll, oder speichern Sie Ihre Abfrage als vordefinierten Filter, um sie später erneut zu verwenden. [Erfahren Sie, wie Sie mit vordefinierten Filtern arbeiten](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Wählen Sie im Bereich Regeleigenschaften einen vordefinierten Filter aus, um die in der Arbeitsfläche erstellte Abfrage durch den ausgewählten Filter zu ersetzen.
