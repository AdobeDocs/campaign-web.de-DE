---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Workflow-Aktivitäten ausgeführt werden
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c134f930b253a8d4463f438176fc54e09ea21a48
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 98%

---


# Workflow-Aktivitäten {#workflow-activities}

## Zielgruppenbestimmungsaktivitäten {#targeting}

Inhalt TBD

<!--à reformuler-->Mit diesen Aktivitäten können Sie eine oder mehrere Zielgruppen erstellen, indem Sie Mengen definieren und diese Mengen durch Bilden von Schnittmengen, Vereinigungsmengen oder Ausschlüssen aufteilen oder kombinieren.

### Zielgruppe aufbauen {#build-audience}

### Kombinieren {#combine}

### Anreicherung {#enrichment}

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


## Kanalaktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketing-Kampagnen über mehrere Kanäle hinweg automatisieren und ausführen, z. B. E-Mail, SMS oder Push-Benachrichtigungen. Mit Adobe Campaign-Workflows können Sie Kanalaktivitäten in der Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf dem Kundenverhalten Aktionen ausgelöst werden können.

Sie können beispielsweise eine Begrüßungs-E-Mail-Kampagne erstellen, die eine Reihe von Nachrichten über verschiedene Kanäle wie E-Mail, SMS und Push-Benachrichtigungen enthält. Sie können auch eine Folgenachricht senden, nachdem eine Kundin oder ein Kunde einen Kauf getätigt hat, oder eine personalisierte Geburtstagsnachricht per SMS an eine Kundin bzw. einen Kunden senden.

Mithilfe von Kanalaktivitäten können Sie umfassende, personalisierte Kampagnen erstellen, die Kundinnen und Kunden über mehrere Touchpoints hinweg ansprechen und Konversionen fördern.

Kanalaktivitäten können über die Palette auf der linken Bildschirmseite im Bereich „Kanäle“ aufgerufen werden.

### E-Mail {#email}

Beschreibung, welchen Anwendungsfall Sie ausführen können (gängige andere Aktivitäten, die Sie vor oder nach der Aktivität verknüpfen können)

wie die Aktivität hinzugefügt und konfiguriert wird

Beispiel einer konfigurierten Aktivität in einem Workflow


Die Aktivität „E-Mail-Versand“ ermöglicht das Konfigurieren eines E-Mail-Versands innerhalb eines Workflows.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Die Empfängerinnen und Empfänger der E-Mails werden im Vorfeld der Aktivität im selben Workflow mithilfe einer Audience-Zielgruppenbestimmungsaktivität definiert.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Push-Benachrichtigung (Android) {#push-android}

### Push-Benachrichtigung (iOS) {#push-ios}

## Flusssteuerungsaktivitäten {#flow-control}

Inhalt TBD

<!--à reformuler-->Mit diesen Aktivitäten können Sie eine oder mehrere Zielgruppen erstellen, indem Sie Mengen definieren und diese Mengen durch Bilden von Schnittmengen, Vereinigungsmengen oder Ausschlüssen aufteilen oder kombinieren.

Flusssteuerungsaktivitäten dienen zur Koordinierung der Workflow-Aktivitäten.

### Verzweigung {#fork}

### Und-Verknüpfung {#join}


### Warten {#wait}

### Ende {#end}

## Daten-Management-Aktivitäten {#data-management}

Überblick: wofür sie verwendet werden
welche Anwendungsfälle damit durchgeführt werden können

Liste der verfügbaren Aktivitäten + Kurzbeschreibung + Verweis auf Abschnitt

