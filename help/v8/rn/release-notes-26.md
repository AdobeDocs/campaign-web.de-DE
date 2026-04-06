---
title: Frühere Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Versionen der Campaign-Web-Benutzeroberfläche 2026
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: be38a0d27ae805ac64f0c951e5ea470cd1feb859
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 22%

---

# Versionshinweise für 2026 {#2026-release}

Auf dieser Seite werden alle Änderungen und Verbesserungen aufgelistet, die in **Versionen aus 2026** verfügbar sind. Die neuesten Versionshinweise finden Sie auf [dieser Seite](release-notes.md).

## Version Februar &#39;26 {#26-2-release}

_17. Februar 2026_

### Neue Funktionen {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>Ansicht „Zeitleiste“ im Kampagneninventar</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Das Kampagneninventar enthält jetzt eine Zeitleisten -Ansicht, mit der Sie Kampagnen im Zeitverlauf visualisieren und verwalten können: Wechseln zwischen Liste und Zeitleiste, Navigieren nach Woche, Monat oder Tag, Verwenden der Schaltfläche Heute , um zum aktuellen Datum zu springen, und Öffnen von Kampagnendetails (Status, Workflows, Sendungen) in einem rechten Bedienfeld - mit denselben Filtern und Suchvorgängen wie die Listenansicht.</p>
<p>Weitere Informationen finden Sie im <a href="../campaigns/manage-campaigns.md#timeline">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schema-Authoring (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können Schemata jetzt direkt über die Web-Benutzeroberfläche von Campaign erstellen und verwalten. Mit dieser Funktion können Sie neue Tabellen erstellen, vorhandene Schemata erweitern und benutzerdefinierte Formulare erstellen. Sie können benutzerdefinierte Datenstrukturen definieren, um Ihre spezifischen Geschäftsanforderungen zu unterstützen, ohne Zugriff auf die Client-Konsole zu benötigen.</p>
<p>Hinweis: Diese Funktion ist nur für eine bestimmte Gruppe von Unternehmen verfügbar (eingeschränkte Verfügbarkeit) und wird in einer zukünftigen Version global eingeführt.</p>
<p>Weitere Informationen finden Sie im <a href="../administration/schemas.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

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
<th><strong>Inhaltsexperimente – A/B-Tests</strong><br/></th> 
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
<th><strong>Aktivität „Versand (fortlaufend)“</strong><br/></th> 
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
<th><strong>Verwaltung der Genehmigung von Kampagnen</strong><br/></th> 
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
