---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 777611699d3d4189cdd7d0d7ded66a9b08cf26cd
workflow-type: ht
source-wordcount: 610
ht-degree: 100%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

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

* Die Workflow-Aktivität **Start** wurde hinzugefügt, um die Kompatibilität mit der Client-Konsole zu verbessern. Diese Aktivität ist optional und wird in neuen Workflows nicht standardmäßig eingefügt. Sie wird jedoch automatisch in vorhandene Workflows eingefügt.
  [Weitere Informationen](../workflows/activities/about-activities.md#flow-control)
* Das Feld für die Zeitzonenauswahl in den Einstellungen für den **Zeitplan** eines Versands wurde unter das Feld **Kontaktdatum** verschoben. [Weitere Informationen](../msg/create-deliveries.md#gs-schedule)