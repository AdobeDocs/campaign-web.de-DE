---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Version vom 26. März {#26-3-release}

### Neue Funktionen {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Schema-Authoring (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Funktion zur Schemaerstellung ist jetzt für alle Kunden (GA) verfügbar. Mit dieser Funktion können Sie Schemata direkt über die Web-Benutzeroberfläche von Campaign erstellen und verwalten. Sie können neue Tabellen erstellen, vorhandene Schemata erweitern und benutzerdefinierte Formulare erstellen. Sie können benutzerdefinierte Datenstrukturen definieren, um Ihre spezifischen Geschäftsanforderungen zu unterstützen, ohne Zugriff auf die Client-Konsole zu benötigen.</p>
<p>Weitere Informationen finden Sie im <a href="../administration/schemas.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Designs in der E-Mail Designer (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Designs bieten ein verbessertes Authoring-Erlebnis für E-Mails, indem sie es Ihnen ermöglichen, wiederverwendbare Designstile zu definieren, die Ihren Markenrichtlinien entsprechen. Sie können jetzt Design-Variablen in Fragmenten verwenden, um eine konsistente Formatierung Ihrer E-Mail-Vorlagen sicherzustellen. Mit dieser Funktion können Sie E-Mails schneller mit vordefinierten Modulen erstellen, die Inhaltselemente wie Titel, Beschreibungen, Bilder und Links abstrahieren und dabei die Markenkonsistenz wahren.</p>
<p>Hinweis: Diese Funktion ist nur für eine bestimmte Gruppe von Unternehmen verfügbar (eingeschränkte Verfügbarkeit) und wird in einer zukünftigen Version global eingeführt.</p>
<p>Weitere Informationen finden Sie im <a href="../email/apply-email-themes.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integration von benutzerdefinierten Firefly-Modellen und Drittanbieter-Image-Generierungsmodellen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ermöglichen Sie die nahtlose Integration von standardmäßigen und benutzerdefinierten Firefly-Modellen zusammen mit genehmigten Bildmodellen von Drittanbietern, um die Flexibilität, Kontrolle und Markenausrichtung beim Erzeugen von Bildern zu verbessern.</p>
<p>Wählen Sie das richtige Modell für Ihre Anforderungen:</p>
<ul><li> <strong>Adobe-Modell</strong> (unterstützt von Firefly Image Model 4) für die sofortige Bildgenerierung ohne zusätzliche Einrichtung</li><li> <strong>Partnermodell</strong> (unterstützt von Gemini 2.5 Flash) für spezielle Funktionen</li><li><strong>Benutzerdefinierte Modelle</strong> (markenspezifische Modelle, die auf Ihren eigenen Assets trainiert wurden) für die Generierung innerhalb der Marke, die genau auf Ihre Markenidentität, Ihren Stil und Ihre visuellen Richtlinien abgestimmt ist.</li></ul>
<p>Weitere Informationen finden Sie im <a href="../content/generative-models.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Versandaktivität automatisieren</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Workflow<strong>Aktivität „Automatisierter Versand</strong> ist jetzt in der Workflow-Palette verfügbar. Sie können damit Versandaktionen (Vorbereiten, Testversand durchführen, Vorbereiten und starten usw.) direkt in Ihrem Workflow erstellen oder ausführen. Wählen Sie einen außerhalb des Workflows erstellten Versand aus, um ihn bei jeder Ausführung wiederzuverwenden, oder erstellen Sie bei jeder Ausführung der Aktivität einen neuen Versand aus einer Vorlage.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Weitere Informationen finden Sie in der <a href="../workflows/activities/automated-delivery.md"> Dokumentation .</p>
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

<p><strong>Mehrere Verzweigungen</strong> werden jetzt unterstützt. Anstatt einen <strong>Verzweigung</strong> zu verwenden, können Sie auf der Symbolleiste auf <strong>Verzweigung hinzufügen</strong> klicken. Die Aktivität <strong>UND-Verknüpfung</strong> wurde ebenfalls verbessert. Es handelt sich jetzt um eine generische Aktivität <strong>Zusammenführen</strong> mit der Sie zwischen den Optionen für UND- und ODER-Zusammenführungen wählen können.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Weitere Informationen finden Sie auf den Dokumentationsseiten <a href="../workflows/orchestrate-activities.md#toolbar">Aktivitäten </a> und <a href="../workflows/activities/join.md">Zusammenführen</a> .</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-3-improvements}

* Die **Start**-Workflow-Aktivität wurde hinzugefügt, um die Kompatibilität mit der Client-Konsole zu verbessern. Diese Aktivität ist optional und wird in neuen Workflows nicht standardmäßig eingefügt. Es wird jedoch automatisch zu vorhandenen Workflows hinzugefügt.
  [Weitere Informationen](../workflows/activities/about-activities.md#flow-control)
* Das Feld für die Zeitzonenauswahl in den **Zeitplan**-Einstellungen eines Versands wurde unter das Feld **Kontaktdatum** verschoben. [Weitere Informationen](../msg/create-deliveries.md#gs-schedule)