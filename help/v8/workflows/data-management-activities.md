---
audience: end-user
title: Arbeiten mit Workflows – Daten-Management-Aktivitäten
description: Erfahren Sie, wie Sie Daten-Management-Aktivitäten in Adobe Campaign Web-Workflows verwenden
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Daten-Management-Aktivitäten {#data-management}

Überblick: wofür sie verwendet werden
welche Anwendungsfälle damit durchgeführt werden können

Liste der verfügbaren Aktivitäten + Kurzbeschreibung + Verweis auf Abschnitt

## Anreicherung {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Anreicherung Aktivität"
>abstract="Die Anreicherungsaktivität ermöglicht es Ihnen, die Zielgruppendaten um zusätzliche Informationen aus der Datenbank zu erweitern. Dies wird in einem Workflow häufig nach den Zielgruppenbestimmungsaktivitäten verwendet.<br/>Nachdem Anreicherungsdaten zum Workflow hinzugefügt wurden, können sie in den Aktivitäten verwendet werden, die nach der Anreicherungsaktivität hinzugefügt wurden, um Kundinnen und Kunden basierend auf ihren Verhaltensweisen, Voreinstellungen und Anforderungen in verschiedene Gruppen zu unterteilen oder um personalisierte Marketing-Nachrichten und -Kampagnen zu erstellen, die Ihre Zielgruppen-Audience mit größerer Wahrscheinlichkeit ansprechen."

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
