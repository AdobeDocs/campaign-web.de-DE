---
audience: end-user
title: Arbeiten mit Datenverwaltungsaktivitäten in Workflows
description: Erfahren Sie, wie Sie Datenverwaltungsaktivitäten in Adobe Campaign-Web-Workflows verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 5efcdf2da104b86bf3ee37ee7162495c2d99fb48
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 3%

---

# Datenverwaltungsaktivitäten {#data-management}

overview: was sie für welchen Anwendungsfall Sie mit ihnen durchführen können

Liste der verfügbaren Aktivitäten + Kurzbeschreibung + Referenz zum Abschnitt

## Anreicherung {#enrichment}

Die Aktivität Anreicherung wird in der Regel in einem Workflow nach Zielgruppenbestimmungsaktivitäten verwendet. Dadurch können Sie die Zieldaten um zusätzliche Informationen aus der Datenbank erweitern.

Anreicherungsdaten können Folgendes umfassen:

* **Aus derselben Arbeitstabelle** als Zielgruppe für Ihren Workflow:

   *Targeting einer Kundengruppe und Hinzufügen des Felds &quot;Geburtsdatum&quot;zur aktuellen Arbeitstabelle*

* **Aus einer anderen Arbeitstabelle**:

   *Richten Sie eine Gruppe von Kunden ein und fügen Sie die Felder &quot;Betrag&quot;und &quot;Produkttyp&quot;aus der &quot;Kauf&quot;-Tabelle hinzu.*.

Nachdem die Anreicherungsdaten zum Workflow hinzugefügt wurden, können sie in den Aktivitäten verwendet werden, die im Anschluss an die Anreicherungsaktivität hinzugefügt wurden, um Kunden basierend auf ihren Verhaltensweisen, Vorlieben und Anforderungen in verschiedene Gruppen zu unterteilen oder um personalisierte Marketing-Nachrichten und -Kampagnen zu erstellen, die mit höherer Wahrscheinlichkeit bei Ihrer Zielgruppe ankommen.

Sie können beispielsweise der Workflow-Arbeitstabelle Informationen zu Käufen von Kunden hinzufügen und diese Daten verwenden, um E-Mails mit ihrem neuesten Kauf oder dem für diese Käufe ausgegebenen Betrag zu personalisieren.

Gehen Sie wie folgt vor, um Ihrem Workflow die Aktivität Anreicherung hinzuzufügen:

1. Aktivität hinzufügen
1. Attribut auswählen, das als Anreicherungsdaten verwendet werden soll

   Option &quot;Erweiterte Felder anzeigen&quot;auf Schaltfläche

   Hinweis: Attribute aus der Zieldimension

1. Art der Datenerhebung auswählen
1. Anzahl der abzurufenden Datensätze, wenn eine Sammlung mehrerer Datensätze abgerufen werden soll
1. Filter anwenden und Regel erstellen

   einen vorhandenen Filter auswählen, um den Filter zur Wiederverwendung der Ergebnisse des Filters visuell oder in der Codeansicht zu speichern

1. Datensätze mithilfe eines Attributs sortieren

Anreicherungsdaten in Kampagnen nutzen

wo wir die Anreicherungsdaten verwenden können: E-Mail personalisieren, andere Anwendungsfälle?