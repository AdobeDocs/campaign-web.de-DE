---
audience: end-user
title: Workflow-Aktivität Anreicherung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Anreicherung verwenden.
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 26%

---


# Anreicherung {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anreicherung Aktivität"
>abstract="Die Anreicherungsaktivität ermöglicht es Ihnen, die Zielgruppendaten um zusätzliche Informationen aus der Datenbank zu erweitern. Sie wird in der Regel in einem Workflow nach Zielgruppenbestimmungsaktivitäten verwendet.<br/>Nachdem Anreicherungsdaten zum Workflow hinzugefügt wurden, können sie in den Aktivitäten verwendet werden, die nach der Anreicherungsaktivität hinzugefügt wurden, um Kundinnen und Kunden basierend auf ihren Verhaltensweisen, Voreinstellungen und Anforderungen in verschiedene Gruppen zu unterteilen oder um personalisierte Marketing-Nachrichten und -Kampagnen zu erstellen, die Ihre Zielgruppen-Audience mit größerer Wahrscheinlichkeit ansprechen."

Die **Anreicherung** -Aktivität **Targeting** Aktivität. Dadurch können Sie die Zieldaten um zusätzliche Informationen aus der Datenbank erweitern. Sie wird häufig in einem Workflow nach Segmentierungsaktivitäten verwendet.

Anreicherungsdaten können verschiedene Ursprünge haben:

* **Aus derselben Arbeitstabelle** wie die Zielgruppe in Ihrem Workflow:

  *Targeting einer Kundengruppe und Hinzufügen des Felds „Geburtsdatum“ zur aktuellen Arbeitstabelle*

* **Aus einer anderen Arbeitstabelle**:

  *Targeting einer Kundengruppe und Hinzufügen der Felder „Betrag“ und „Produkttyp“ aus der „Kauf“-Tabelle*.

Nachdem die Anreicherungsdaten zum Workflow hinzugefügt wurden, können sie in den Aktivitäten verwendet werden, die nach dem **Anreicherung** Aktivität , um Kunden basierend auf ihren Verhaltensweisen, Vorlieben und Anforderungen in verschiedene Gruppen zu unterteilen oder um personalisierte Marketing-Nachrichten und -Kampagnen zu erstellen, die mit größerer Wahrscheinlichkeit bei Ihrer Zielgruppe ankommen.

Sie können beispielsweise der Workflow-Arbeitstabelle Informationen zu Käufen von Kundinnen und Kunden hinzufügen und diese Daten verwenden, um E-Mails mit ihrem neuesten Kauf oder dem für diese Käufe ausgegebenen Betrag zu personalisieren.

## Allgemeine Konfiguration {#general}

Führen Sie die folgenden Schritte aus, um die **Anreicherung** Aktivität:

1. Hinzufügen von Aktivitäten wie **Audience erstellen** und **Kombinieren** Aktivitäten.
1. Hinzufügen einer **Anreicherung** Aktivität.
1. Klicken **Anreicherungsdaten hinzufügen**.

![](../assets/workflow-enrichment1.png)

Sie können zwei Anreicherungsdaten auswählen: a [Single-Anreicherungsattribut](#single-attribute) aus der Zieldimension oder [Sammlungslink](#collection-link).

## Einzelanreicherungsattribut {#single-attribute}

Hier fügen wir nur ein einziges Anreicherungsattribut hinzu, z. B. das Geburtsdatum. Führen Sie folgende Schritte aus:

1. Klicken Sie in die **Attribut** -Feld.
1. Wählen Sie ein einfaches Feld aus der Zielgruppendimension aus, in unserem Beispiel das Geburtsdatum.
1. Klicken Sie auf **Bestätigen**.

![](../assets/workflow-enrichment2.png)

## Sammlungslink {#collection-link}

In diesem komplexeren Anwendungsfall wählen wir eine Kollektionsrelation aus, die eine 1:n-Relation zwischen Tabellen aufweist. Rufen wir die drei neuesten Käufe ab, die weniger als 100$ betragen. Dazu müssen Sie Folgendes definieren:

* Anreicherungsattribut: die **Gesamtbetrag** field
* die Anzahl der abzurufenden Zeilen: 3
* Filter: Elemente herausfiltern, die größer als 100$ sind
* eine Sortierung: Nachfolgende Sortierung auf der **Bestelldatum** -Feld.

### Attribut hinzufügen

Hier wählen Sie den Kollektionslink aus, der als Anreicherungsdaten verwendet werden soll.

1. Klicken Sie in die **Attribut** -Feld.
1. Klicken **Erweiterte Attribute anzeigen**.
1. Wählen Sie die **Gesamtbetrag** aus dem **Käufe** Tabelle.

![](../assets/workflow-enrichment3.png)

### Kollektionseinstellungen definieren

Definieren Sie dann, wie die Daten erfasst werden und wie viele Datensätze abgerufen werden sollen.

1. Auswählen **Daten sammeln** im **Wählen Sie aus, wie die Daten erfasst werden** Dropdown-Liste.
1. Geben Sie &quot;3&quot;in das Feld **Abzurufende Zeilen (zu erstellende Spalten)** -Feld.

![](../assets/workflow-enrichment4.png)

Wenn Sie beispielsweise den durchschnittlichen Einkaufsbetrag für einen Kunden abrufen möchten, wählen Sie **Aggregierte Daten** und wählen Sie stattdessen **Durchschnittlich** im **Aggregatfunktion** Dropdown-Liste.

![](../assets/workflow-enrichment5.png)

### Filter definieren

Hier definieren wir den Maximalwert für das Anreicherungsattribut. Wir filtern Elemente heraus, die größer als 100$ sind.

1. Klicken **Filter bearbeiten**.
1. Fügen Sie die beiden folgenden Filter hinzu: **Gesamtbetrag** vorhanden UND **Gesamtbetrag** ist kleiner als 100. Der erste Filter filtert NULL-Werte so, wie sie als größter Wert erscheinen würden.
1. Klicken Sie auf **Bestätigen**.

![](../assets/workflow-enrichment6.png)

### Sortierung definieren

Jetzt müssen wir die Sortierung anwenden, um die drei abzurufen **latest** Einkäufe.

1. Aktivieren Sie die **Sortierung aktivieren** -Option.
1. Klicken Sie in die **Attribut** -Feld.
1. Wählen Sie die **Bestelldatum** -Feld.
1. Klicken Sie auf **Bestätigen**.
1. Auswählen **Absteigend** von **Sortieren** Dropdown-Liste.

![](../assets/workflow-enrichment7.png)

<!--

Add other fields
use it in delivery


cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->