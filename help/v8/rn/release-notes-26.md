---
title: Frühere Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Versionen der Campaign Web-Benutzeroberfläche 2026
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 6ed3a17593d0dc7bda55d9f90fc27526c09d99ed
workflow-type: ht
source-wordcount: '2025'
ht-degree: 100%

---

# Versionshinweise für 2026 {#2026-release}

Auf dieser Seite werden alle Änderungen und Verbesserungen aufgelistet, die in **Versionen 2026** verfügbar sind. Die neuesten Versionshinweise finden Sie auf [dieser Seite](release-notes.md).

## Version Juli 2026 {#26-7-release}

_28. Juli 2026_

### Neue Funktionen {#26-7-features}

<table>
<thead>
<tr>
<th><strong>Angebotsverwaltung</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können Angebote jetzt durchgängig direkt über die Campaign Web-Benutzeroberfläche verwalten. Konfigurieren Sie Angebotsumgebungen und -platzierungen, erstellen Sie Ihren Angebotskatalog und Ihre Kategorien, erstellen Sie Angebote mit Eignungsregeln und Prioritätsgewichtungen und validieren und stellen Sie sie für die Verwendung in Ihren Sendungen bereit. Erweiterte Konfigurationen sind weiterhin in der Client-Konsole verfügbar.</p>
<p>Weitere Informationen finden Sie in der <a href="../offers/gs-offer-management.md">detaillierten Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Markenkonfiguration</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Technische Admins können jetzt Marken direkt über die Web-Benutzeroberfläche von Campaign erstellen und konfigurieren, ohne die Client-Konsole zu verwenden. Alle Markeneinstellungen, einschließlich Identität, Subdomain und Protokolle, E-Mail-Header-Parameter und URL-Tracking-Parameter, sind jetzt in der Web-Benutzeroberfläche verfügbar.</p>
<p>Weitere Informationen finden Sie in der <a href="../administration/branding/branding-configure.md">detaillierten Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Öffentliche Ressourcen im E-Mail-Designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Beim Hinzufügen von Bildern zu Ihren E-Mails können Sie jetzt <strong>öffentliche Ressourcen</strong> auswählen. Auf diese Weise können Sie ein Bild auswählen, das bereits in Ihrer Adobe Campaign-Instanz verfügbar ist, z. B. eine zuvor in den E-Mail-Designer importierte Datei oder eine öffentliche Ressource, die über die Client-Konsole hochgeladen wurde.</p>
<p>Weitere Informationen finden Sie in der <a href="../email/content-components.md#image">detaillierten Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Workflow-Aktivität „Laden (RDBMS)“</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Aktivität <strong>Laden (RDBMS)</strong> ist jetzt in der Web-Benutzeroberfläche von Campaign verfügbar. Verwenden Sie diese Aktivität, um Daten direkt aus einer externen relationalen Datenbank in Ihren Workflow zu laden. Die extrahierten Daten stehen während des gesamten Workflows zur Verfügung und können für die Zielgruppenbestimmung, die Anreicherung oder die weitere Datenverarbeitung verwendet werden.</p>
<p>Weitere Informationen finden Sie in der <a href="../workflows/activities/data-loading-rdbms.md">detaillierten Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Dynamische JavaScript-Seiten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Mit dynamischen JavaScript-Seiten (JSSP) können Sie Server-seitige Seiten erstellen, die dynamische Inhalte generieren, wenn über eine URL darauf zugegriffen wird, z. B. benutzerdefinierte APIs, Exporte oder Web-Anwendungslogik. Sie können diese Seiten jetzt direkt über die Web-Benutzeroberfläche von Campaign erstellen, ändern, duplizieren und löschen.</p>
<p>Weitere Informationen finden Sie im <a href="../administration/dynamic-javascript-pages.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-7-improvements}

* Die folgenden Verbesserungen wurden an der **Konfiguration benutzerdefinierter Schemata** vorgenommen:
  * Der neue Abschnitt **Aktionsdaten** ermöglicht es Ihnen, die für die Einträge eines benutzerdefinierten Schemas verfügbaren Aktionen zu beschränken, unabhängig von den für einzelne Ordner konfigurierten Sicherheitsregeln. [Weitere Informationen](../administration/schemas-action-data.md)
  * **Benutzerdefinierte Filter** wurden im Abschnitt **Konfiguration der Bestandsliste** hinzugefügt. Damit können Sie auswählen, welche Attribute als Schnellzugriffsfelder im Filterbereich der Listenansicht angezeigt werden. [Weitere Informationen](../administration/schemas-custom-filters.md)

* Die folgenden Verbesserungen wurden an **Workflows** vorgenommen:
  * Das Löschen einer Workflow-Aktivität ist jetzt flexibler: Wenn die Aktivität nachfolgende Aktivitäten hat, können Sie entweder alle löschen, nur die ausgewählte Aktivität löschen oder sie löschen und dabei die nachfolgenden Aktivitäten in einer neuen Verzweigung beibehalten. [Weitere Informationen](../workflows/orchestrate-activities.md#delete-activity)
  * Sie können jetzt eine Transition zwischen zwei Workflow-Aktivitäten trennen, ohne eine der Aktivitäten zu löschen. Auf diese Weise können Sie ein Workflow-Diagramm neu organisieren, z. B. um eine Gruppe von Aktivitäten, die Sie beibehalten möchten, vorübergehend beiseite zu legen, ohne sie löschen und neu erstellen zu müssen. [Weitere Informationen](../workflows/orchestrate-activities.md#disconnect-transition)
  * Horizontale und vertikale Bildlaufleisten werden jetzt um die Workflow-Arbeitsfläche herum angezeigt, sodass Sie in großen Workflows durch Ziehen direkt zu dem Bereich navigieren können, den Sie anzeigen möchten. [Weitere Informationen](../workflows/orchestrate-activities.md)
  * Beim Speichern oder Starten/Neustarten eines Workflows wird jetzt eine Warnung angezeigt, wenn eine andere Benutzerin bzw. ein anderer Benutzer den Workflow in der Web-Benutzeroberfläche oder der Client-Konsole geändert hat, seit Sie ihn geöffnet haben. Sie können die anderen Änderungen mit Ihren eigenen überschreiben, den Workflow neu laden, um die neueste Version zu erhalten, oder den Vorgang abbrechen.

* **Absender-E-Mail-Adresse**: Sie können jetzt das Feld **Absender-E-Mail** Ihrer Sendungen mithilfe der Option **NmsDelivery_senderAddressMask** auf eine vordefinierte Liste von Adressen beschränken. [Weitere Informationen](../administration/options.md#restrict-sender-address)
* **Login-Fehlermeldungen** wurden verbessert: Wenn ein Anmeldeversuch fehlschlägt, zeigt die Web-Benutzeroberfläche jetzt eine spezifischere Fehlermeldung für mehrere Szenarien an (z. B. wenn der Benutzerin bzw. dem Benutzer keine Sicherheitszone zugewiesen ist oder ihre bzw. seine IP-Adresse eingeschränkt ist).

## Version Juni 2026 {#26-6-release}

_16. Juni 2026_

### Verbesserungen {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* Sie können jetzt Daten aus jedem Listenbildschirm einschließlich der Trackinglogs exportieren. Suchen Sie Ihre Liste und klicken Sie einfach auf die Schaltfläche „Exportieren“. Der Export umfasst die derzeit geladenen Zeilen und berücksichtigt die auf dem Bildschirm angezeigten Spalten sowie aktive Suchen oder Filter. [Weitere Informationen](../get-started/list-filters.md)

* Die Workflow-Aktivitäten **Deduplizierung** und **Ende** unterstützen jetzt mehrere eingehende Transitionen. Wenn mehr als eine eingehende Transition verfügbar ist, verwenden Sie den Abschnitt **Zusammenzuführende Mengen** in der Aktivität
um die zu verbindenden Transitionen auszuwählen. Weitere Informationen finden Sie auf den folgenden Seiten: [Deduplizierung](../workflows/activities/deduplication.md), [Ende](../workflows/activities/end.md)

* Erweiterte Parameter werden jetzt im Abschnitt **Anreicherungsdaten** der Workflow-Aktivitäten **Zielgruppe erstellen** (Abfragetyp) und **Anreicherung** angezeigt. Mit diesen Parametern können Sie die Struktur von Anreicherungsdaten optimieren, einschließlich Gruppierung, Deduplizierung, Verarbeitung von Primärschlüsseln und Daten eingehender Ereignisse. [Weitere Informationen](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->

## Version April 2026 {#26-4-release}

_29. April 2026_

### Verbesserung {#26-4-improvement}

Der Abschnitt **Anreicherungsdaten** ist jetzt in der Workflow-Aktivität **Zielgruppe erstellen** verfügbar (Abfrageart). Sie können **zusätzliche Daten** direkt in der Campaign Web-Benutzeroberfläche anzeigen, hinzufügen, bearbeiten und entfernen. Wie bei der Aktivität **Anreicherung** können Sie einzelne Anreicherungsattribute, Sammlungs-Links und Ausdrücke hinzufügen.

[Weitere Informationen](../workflows/activities/build-audience.md)

## Version März 2026 {#26-3-release}

24. _März_ 2026_

### Neue Funktionen {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Schemaerstellung (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Funktion zur Schemaerstellung ist jetzt für alle Kundinnen und Kunden verfügbar (GA). Mit dieser Funktion können Sie Schemata direkt über die Campaign Web-Benutzeroberfläche erstellen und verwalten. Sie können neue Tabellen erstellen, vorhandene Schemata erweitern und benutzerdefinierte Formulare erstellen. Sie können benutzerdefinierte Datenstrukturen definieren, die Ihre spezifischen Geschäftsanforderungen zu unterstützen, ohne Zugriff auf die Client-Konsole zu benötigen.</p>
<p>Weitere Informationen finden Sie im <a href="../administration/schemas.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Designs im E-Mail-Designer (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Designs bieten ein verbessertes Authoring-Erlebnis für E-Mails, indem sie es Ihnen ermöglichen, wiederverwendbare Design-Stile zu definieren, die Ihren Markenrichtlinien entsprechen. Sie können jetzt Design-Variablen in Fragmenten verwenden, um eine konsistente Formatierung Ihrer E-Mail-Vorlagen sicherzustellen. Mit dieser Funktion können Sie E-Mails schneller mit vordefinierten Modulen erstellen, die Inhaltselemente wie Titel, Beschreibungen, Bilder und Links abstrahieren, und dabei die Markenkonsistenz wahren.</p>
<p>Hinweis: Diese Funktion ist nur für eine bestimmte Gruppe von Unternehmen verfügbar (eingeschränkte Verfügbarkeit) und wird in einer zukünftigen Version global eingeführt.</p>
<p>Weitere Informationen finden Sie im <a href="../email/apply-email-themes.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integration von benutzerdefinierten Firefly-Modellen und Bildgenerierungsmodellen von Drittanbietern</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Aktivieren Sie die nahtlose Integration von standardmäßigen und benutzerdefinierten Firefly-Modellen zusammen mit genehmigten Bildmodellen von Drittanbietern, um die Flexibilität, Kontrolle und Markenausrichtung beim Erzeugen von Bildern zu verbessern.</p>
<p>Wählen Sie das richtige Modell für Ihre Anforderungen:</p>
<ul><li> <strong>Adobe-Modell</strong> (unterstützt von Firefly Image Model 4) für die sofortige Bildgenerierung ohne zusätzliches Setup</li><li> <strong>Partnermodell</strong> (unterstützt von Gemini 2.5 Flash) für spezielle Funktionen</li><li><strong>Benutzerdefinierte Modelle</strong> (markenspezifische Modelle, die mit Ihren eigenen Assets trainiert wurden) für die markenkonforme Generierung, die genau auf Ihre Markenidentität, Ihren Stil und Ihre visuellen Richtlinien abgestimmt ist.</li></ul>
<p>Weitere Informationen finden Sie im <a href="../content/generative-models.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Aktivität „Automatischer Versand“</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Workflow-Aktivität <strong>Automatischer Versand</strong> ist jetzt in der Workflow-Palette verfügbar. Sie können damit Versandaktionen (vorbereiten, einen Testversand durchführen, vorbereiten und starten) direkt in Ihrem Workflow erstellen und ausführen. Wählen Sie einen außerhalb des Workflows erstellten Versand aus, um ihn bei jeder Ausführung wiederzuverwenden, oder erstellen Sie bei jeder Ausführung der Aktivität einen neuen Versand aus einer Vorlage.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Weitere Informationen finden Sie in der <a href="../workflows/activities/automated-delivery.md">ausführlichen Dokumentation.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Mehrere Workflow-Verzweigungen und Join-Aktivität</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong>Mehrere Verzweigungen</strong> werden jetzt unterstützt. Anstatt eine <strong>Verzweigung</strong> zu verwenden, können Sie in der Symbolleiste auf <strong>Verzweigung hinzufügen</strong> klicken. Die Aktivität <strong>UND-Verknüpfung</strong> wurde ebenfalls verbessert. Es handelt sich um eine generische <strong>Join</strong>-Aktivität, bei der Sie die Möglichkeit haben, zwischen UND- und ODER-Verknüpfungen zu wählen.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Weitere Informationen finden Sie auf den Dokumentationsseiten zu <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrierungsaktivitäten</a> und <a href="../workflows/activities/join.md">Join</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-3-improvements}

* Die Workflow-Aktivität **Start** wurde hinzugefügt, um die Kompatibilität mit der Client-Konsole zu verbessern. Diese Aktivität ist optional und wird in neuen Workflows nicht standardmäßig eingefügt. Sie wird jedoch automatisch zu vorhandenen Workflows hinzugefügt.
  [Weitere Informationen](../workflows/activities/about-activities.md#flow-control)
* Das Feld für die Zeitzonenauswahl in den Einstellungen für den **Zeitplan** eines Versands wurde unter das Feld **Kontaktdatum** verschoben. [Weitere Informationen](../msg/create-deliveries.md#gs-schedule)

## Version Februar 2026 {#26-2-release}

_17. Februar 2026_

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
<th><strong>Ansicht „Timeline“ im Kampagneninventar</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Das Kampagneninventar enthält jetzt eine Timeline-Ansicht, mit der Sie Kampagnen im Zeitverlauf visualisieren und verwalten können: Wechseln zwischen Liste und Timeline, Navigation nach Woche, Monat oder Tag, Verwenden der Schaltfläche „Heute“, um zum aktuellen Datum zu springen, und Öffnen von Kampagnendetails (Status, Workflows, Sendungen) in einem Panel auf der rechten Seite – mit denselben Filtern und Suchvorgängen wie in der Listenansicht.</p>
<p>Weitere Informationen finden Sie im <a href="../campaigns/manage-campaigns.md#timeline">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schemaerstellung (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können Schemata jetzt direkt über die Campaign Web-Benutzeroberfläche erstellen und verwalten. Mit dieser Funktion können Sie neue Tabellen erstellen, vorhandene Schemata erweitern und benutzerdefinierte Formulare erstellen. Sie können benutzerdefinierte Datenstrukturen definieren, die Ihre spezifischen Geschäftsanforderungen zu unterstützen, ohne Zugriff auf die Client-Konsole zu benötigen.</p>
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

## Version Januar 2026 {#26-1-release}

_27. Januar 2026_

### Neue Funktionen {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Mehrsprachige Versandfunktionen (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Funktion für den Versand in mehreren Sprachen steht nun allen Kundinnen und Kunden zur Verfügung. Mit dieser Funktion können Sie mehrere Nachrichten in verschiedenen Sprachen in der Adobe Campaign Web-Benutzeroberfläche senden. Sie können die Standardsprache Ihres Versands sowie die verschiedenen Sprachen festlegen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in einer Vorschau in den von Ihnen ausgewählten Sprachen anzeigen. 
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
<p>Die Funktion zur Profilanreicherung in Transaktionsnachrichten steht nun allen Kundinnen und Kunden zur Verfügung (GA). Zusätzlich zu E-Mails werden jetzt auch SMS- und Push-Benachrichtigungen unterstützt. Mit dieser Funktion können Sie Transaktionsnachrichten personalisieren, indem Sie Adobe Campaign-Datenbankfelder mit dem Nachrichteninhalt verknüpfen. Sie können Zielgruppen-Mappings, Anreicherungsspalten und einen Abstimmschlüssel auswählen, um präzise Echtzeit-Personalisierung unter Einhaltung der Leistungsschwellen sicherzustellen.</p>
<p>Weitere Informationen finden Sie im <a href="../transactional-messaging/profile-enrichment.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Live Copies und Sprachkopien aus Adobe Experience Manager</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Durch die Integration von Inhalten aus Adobe Experience Manager können Sie direkt in Campaign auf alle in Adobe Experience Manager erstellten Sprachkopien und Live Copies zugreifen, wenn Sie Sendungen erstellen. Sie können Inhalte in Echtzeit aktualisieren, um die neuesten Versionen aus Adobe Experience Manager abzurufen. Durch diese Integration wird die manuelle Synchronisierung von Inhalten zwischen Adobe Experience Manager und Campaign überflüssig, was den Workflow für mehrsprachige Kampagnen optimiert.</p>
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
<p>Mit Inhaltsexperimenten in Adobe Campaign Web können Sie mehrere Varianten von A/B-Tests für den Versand definieren, um zu messen, welche für Ihre Zielgruppe am besten geeignet ist. Sie können Versandinhalt, Betreff oder Absender variieren, um verschiedene Versionen zu testen und festzustellen, welche Variante die besten Ergebnisse erzielt. Sie können A/B-Tests für verschiedene E-Mail-Elemente durchführen, z. B. Betreffzeile, Absendername und E-Mail-Textinhalt.</p>
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
<p>Die Aktivität „Versand (fortlaufend)“ ermöglicht das Hinzufügen neuer Empfänger bzw. Empfängerinnen zu einem bestehenden Versand. Bei diesem Versandtyp muss nicht jedes Mal ein neuer Versand erstellt werden, was ihn effizienter für Warnhinweise für geringes Volumen oder Benachrichtigungen macht, die bei Bedarf gesendet werden. Bei einem fortlaufenden Versand wird eine einzige Versandinstanz erstellt. Alle Versandlogs (broadLog) und Trackinglogs verweisen auf diesen Versand und vereinfachen das Monitoring und das Reporting.</p>
<p>Weitere Informationen finden Sie im <a href="../workflows/activities/continuous-delivery.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Verwaltung der Kampagnenvalidierung</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Der Validierungsprozess hilft, mehrere Stakeholder zu koordinieren, und stellt die Qualitätskontrolle vor dem Versand sicher. Verwenden Sie Validierungen, wenn Ihre Organisation die Validierung durch verschiedene Teams erfordert, z. B. durch das Marketing-Management, das Inhalte überprüft, oder durch das Datenanalyse-Team, das Zielgruppen validiert.</p>
<p>Weitere Informationen finden Sie im <a href="../campaigns/campaign-approvals.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-1-improvements}

* Dynamische Berichte unterstützen jetzt Push-Benachrichtigungen und SMS. [Weitere Informationen](../reporting/dynamic-reporting/get-started-reporting.md)
* Vordefinierte Filter – Mit der neuen Option „Freigegebener Filter“ können Sie einen vordefinierten Filter für andere Benutzende in Ihrer Organisation verfügbar machen. [Weitere Informationen](../get-started/predefined-filters.md#share-filter)
* In Adobe Experience Manager erstellte Personalisierungsfelder wie „Name“, „E-Mail“, „Datum“ und „Adresse“ sind jetzt bei der Verwendung von Inhaltsvorlagen enthalten und verfügbar.
* Bei der Bewertung der Inhaltsqualität werden nun unabhängig von den Markenrichtlinien Aspekte wie Lesbarkeit, Kohärenz und Effektivität geprüft, um unklare Botschaften, inkonsistenten Ton oder strukturelle Lücken aufzudecken. [Weitere Informationen](../content/brands-score.md)
