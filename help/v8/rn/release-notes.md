---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62e064b5a2e2c0d8b81755d2a8a9ea04c512e6f2
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 31%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind auf den Seiten für [2024](release-notes-24.md) und [2025](release-notes-25.md) aufgeführt.

## Version Januar &#39;26 {#26-1-release}

_27. Januar 2026_

### Neue Funktionen {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Mehrsprachige Bereitstellungsfunktionen (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Funktion zur Bereitstellung in mehreren Sprachen steht nun allen Kunden zur Verfügung. Mit dieser Funktion können Sie mehrere Nachrichten in verschiedenen Sprachen in der Web-Benutzeroberfläche von Adobe Campaign senden. Sie können die Standardsprache Ihres Versands sowie die verschiedenen Sprachen auswählen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in einer Vorschau in den von Ihnen ausgewählten Sprachen anzeigen. 
<p>Weitere Informationen finden Sie im <a href="../msg/multilingual.md">entsprechenden Handbuch</a>.</p>
<p>Die folgenden Verbesserungen wurden an mehrsprachigen Push-Benachrichtigungen vorgenommen:</p>
<ul>
<li>Sie können jetzt alle Sprachvarianten schnell füllen, indem Sie eine CSV-Datei mit mehrsprachigen Inhalten hochladen. <a href="../msg/multilingual.md#csv-upload">Weitere Informationen</a>
</li>
<li>Rich-Push-Benachrichtigungen werden jetzt unterstützt.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Profilanreicherung in Transaktionsnachrichten (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Funktion Profilanreicherung in Transaktionsnachrichten steht nun allen Kunden (GA) zur Verfügung. Zusätzlich zu E-Mails werden jetzt auch SMS- und Push-Benachrichtigungen unterstützt. Mit dieser Funktion können Sie Transaktionsnachrichten personalisieren, indem Sie Adobe Campaign-Datenbankfelder mit dem Nachrichteninhalt verknüpfen. Sie können Zielgruppen-Mappings, Anreicherungsspalten und einen Abstimmschlüssel auswählen, um präzise Echtzeit-Personalisierung unter Einhaltung der Leistungsschwellen sicherzustellen.</p>
<p>Weitere Informationen finden Sie im <a href="../transactional-messaging/profile-enrichment.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager Live Copies und Sprachkopien</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Durch die Adobe Experience Manager-Inhaltsintegration können Sie direkt in Campaign auf alle in Adobe Experience Manager erstellten Sprach- und Live Copies zugreifen, wenn Sie Sendungen erstellen. Sie können Inhalte in Echtzeit aktualisieren, um die neuesten Adobe Experience Manager-Versionen abzurufen. Durch diese Integration wird die manuelle Synchronisierung von Inhalten zwischen Adobe Experience Manager und Campaign überflüssig, was den mehrsprachigen Kampagnen-Workflow optimiert.</p>
<p>Weitere Informationen finden Sie im <a href="../integrations/aem-multilingual.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Inhaltsexperimente - A/B-Tests</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Mit Inhaltsexperimenten in Adobe Campaign Web können Sie mehrere Varianten von A/B-Tests für die Bereitstellung definieren, um zu messen, welche für Ihre Zielgruppe am besten geeignet ist. Sie können Versandinhalt, Betreff oder Absender variieren, um verschiedene Versionen zu testen und festzustellen, welche Variante die besten Ergebnisse erzielt. Sie können A/B-Tests für verschiedene E-Mail-Elemente durchführen, z. B. Betreffzeile, Absendername und E-Mail-Textinhalt.</p>
<p>Weitere Informationen finden Sie im <a href="../email/ab-testing.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Kontinuierliche Versandaktivität</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Aktivität Versand (fortlaufend) ermöglicht das Hinzufügen neuer Empfänger zu einem bestehenden Versand. Bei diesem Versandtyp muss nicht jedes Mal ein neuer Versand erstellt werden, was ihn effizienter für Benachrichtigungen oder Benachrichtigungen mit geringem Volumen macht, die nach Bedarf gesendet werden. Bei einem fortlaufenden Versand wird eine einzige Versandinstanz erstellt. Alle Versandlogs (broadLog) und Trackinglogs verweisen auf diesen Versand und vereinfachen die Überwachung und das Reporting.</p>
<p>Weitere Informationen finden Sie im <a href="../workflows/activities/continuous-delivery.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Validierungsverwaltung für Kampagnen</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Der Validierungsprozess hilft, mehrere Stakeholder zu koordinieren, und stellt die Qualitätskontrolle vor dem Versand sicher. Verwenden Sie Validierungen, wenn Ihr Unternehmen die Validierung durch verschiedene Teams erfordert, z. B. durch Marketing-Manager, die Inhalte überprüfen, oder durch Datenanalysten, die Zielgruppen validieren.</p>
<p>Weitere Informationen finden Sie im <a href="../campaigns/campaign-approvals.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-1-improvements}

* Dynamische Berichte unterstützen jetzt Push-Benachrichtigungen und SMS. [Weitere Informationen](../reporting/dynamic-reporting/get-started-reporting.md)
* Vordefinierte Filter - Mit der neuen Option „Freigegebener Filter“ können Sie einen vordefinierten Filter für andere Benutzer in Ihrer Organisation verfügbar machen. [Weitere Informationen](../get-started/predefined-filters.md#share-filter)
* In Adobe Experience Manager erstellte Personalisierungsfelder wie Name, E-Mail, Datum und Adresse sind jetzt bei der Verwendung von Inhaltsvorlagen enthalten und verfügbar.
* Die Bewertung der Inhaltsqualität prüft jetzt Probleme mit Lesbarkeit, Kohärenz und Effektivität unabhängig von Markenrichtlinien und erkennt unklare Botschaften, inkonsistenten Ton oder strukturelle Lücken. [Weitere Informationen](../content/brands-score.md)
