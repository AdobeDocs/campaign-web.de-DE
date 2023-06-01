---
audience: end-user
title: Workflow-Aktivität Anreicherung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Anreicherung verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 93%

---


# Anreicherung {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anreicherung Aktivität"
>abstract="Die Anreicherungsaktivität ermöglicht es Ihnen, die Zielgruppendaten um zusätzliche Informationen aus der Datenbank zu erweitern. Sie wird in der Regel in einem Workflow nach Zielgruppenbestimmungsaktivitäten verwendet.<br/>Nachdem Anreicherungsdaten zum Workflow hinzugefügt wurden, können sie in den Aktivitäten verwendet werden, die nach der Anreicherungsaktivität hinzugefügt wurden, um Kundinnen und Kunden basierend auf ihren Verhaltensweisen, Voreinstellungen und Anforderungen in verschiedene Gruppen zu unterteilen oder um personalisierte Marketing-Nachrichten und -Kampagnen zu erstellen, die Ihre Zielgruppen-Audience mit größerer Wahrscheinlichkeit ansprechen."

Die Anreicherungsaktivität ermöglicht es Ihnen, die Zielgruppendaten um zusätzliche Informationen aus der Datenbank zu erweitern. Dies wird in einem Workflow häufig nach den Zielgruppenbestimmungsaktivitäten verwendet.

Anreicherungsdaten können verschiedene Ursprünge haben:

* **Aus derselben Arbeitstabelle** wie die Zielgruppe in Ihrem Workflow:

   *Targeting einer Kundengruppe und Hinzufügen des Felds „Geburtsdatum“ zur aktuellen Arbeitstabelle*

* **Aus einer anderen Arbeitstabelle**:

   *Targeting einer Kundengruppe und Hinzufügen der Felder „Betrag“ und „Produkttyp“ aus der „Kauf“-Tabelle*.

Nachdem die Anreicherungsdaten zum Workflow hinzugefügt wurden, können sie in den Aktivitäten verwendet werden, die im Anschluss an die Anreicherungsaktivität hinzugefügt wurden, um Kundinnen und Kunden basierend auf ihren Verhaltensweisen, Vorlieben und Anforderungen in verschiedene Gruppen zu unterteilen oder um personalisierte Marketing-Nachrichten und -Kampagnen zu erstellen, die Ihre Zielgruppen-Audience mit größerer Wahrscheinlichkeit ansprechen.

Sie können beispielsweise der Workflow-Arbeitstabelle Informationen zu Käufen von Kundinnen und Kunden hinzufügen und diese Daten verwenden, um E-Mails mit ihrem neuesten Kauf oder dem für diese Käufe ausgegebenen Betrag zu personalisieren.

Gehen Sie wie folgt vor, um Ihrem Workflow die Aktivität „Anreicherung“ hinzuzufügen:

1. Aktivität hinzufügen
1. Attribut auswählen, das für die Anreicherungsdaten verwendet werden soll

   Option „Erweiterte Felder anzeigen“
i-Schaltfläche

   Hinweis: Attribute aus der Zielgruppendimension

1. Art der Datenerhebung auswählen
1. Anzahl der abzurufenden Datensätze, wenn eine Sammlung mehrerer Datensätze abgerufen werden soll
1. Filter anwenden und Regel erstellen

   einen vorhandenen Filter auswählen
Filter zur erneuten Verwendung speichern
Treffer des Filters visuell oder in der Code-Ansicht anzeigen

1. Datensätze mithilfe eines Attributs sortieren

Anreicherungsdaten in Kampagnen nutzen

Wo können die Anreicherungsdaten verwendet werden: E-Mail personalisieren, andere Anwendungsfälle?

