---
audience: end-user
title: Arbeiten mit Datenverwaltungsaktivitäten in Workflows
description: Erfahren Sie, wie Sie Datenverwaltungsaktivitäten in Adobe Campaign-Web-Workflows verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: ee418ea42bc4568f2ff1f0fe9080825764fee65d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 5%

---

# Datenverwaltungsaktivitäten {#data-management}

overview: was sie für welchen Anwendungsfall Sie mit ihnen durchführen können

Liste der verfügbaren Aktivitäten + Kurzbeschreibung + Referenz zum Abschnitt

## Anreicherung {#enrichment}

description: Fügen Sie eine oder mehrere Anreicherungsdaten hinzu, um den Anwendungsfall für Sendungen zu personalisieren: Abrufen des neuesten Kaufs oder letzten digitalen Abonnements sowie des Gesamtbetrags eines Kaufs und Personalisieren einer E-Mail damit

Prozessanwendungsbeispiel: Abrufen von 4 neuesten Käufen unter 100$ und Personalisieren einer E-Mail mit dieser
1. Aktivität hinzufügen
1. Attribut auswählen, das als Anreicherungsdaten verwendet werden soll

   + Option &quot;Erweiterte Felder anzeigen&quot;
   + i-Taste

   Hinweis: Attribute aus der Zieldimension

1. Art der Datenerhebung auswählen
1. Anzahl der abzurufenden Datensätze, wenn eine Sammlung mehrerer Datensätze abgerufen werden soll
1. Filter anwenden und Regel erstellen

   + existierenden Filter auswählen
   + Filter zur Wiederverwendung speichern
   + Ergebnisse des Filters visuell oder in der Codeansicht anzeigen

1. Datensätze mithilfe eines Attributs sortieren

Anreicherungsdaten in Kampagnen nutzen

wo wir die Anreicherungsdaten verwenden können: E-Mail personalisieren, andere Anwendungsfälle?
