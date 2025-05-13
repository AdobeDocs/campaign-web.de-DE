---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: b730eeeaab5bfc87e8c9c10b6e25bed0e484fb64
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 94%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind in den [Versionshinweisen 2024](release-notes-24.md) und [Versionshinweisen 2025](release-notes-25.md) aufgeführt.

## Mai &#39;25 Updates {#25-5-release}

<table>
<thead>
<tr>
<th><strong>Bewertung der Markenausrichtung (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Funktion zur Bewertung der Markenausrichtung bietet ein klares Feedback direkt im E-Mail-Designer, sodass Sie sehen können, ob Ihr Inhalt mit dem Ton, dem Stil und den Richtlinien Ihrer Marke übereinstimmt. Diese Funktion ist in Beta verfügbar.</p>
<p>Weitere Informationen finden Sie in der <a href="../content/brands-score.md">entsprechenden Dokumentation</a>.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

## Version April 2025 {#25-4-release}

**Veröffentlichungsdatum**: 29. April 2025

### Neue Funktionen {#25-4-features}

Die folgenden Funktionen stehen allen Benutzenden ab der April-Version zur Verfügung.

<table>
<thead>
<tr>
<th><strong>Callcenter-Kanal</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Der Callcenter-Kanal ist jetzt in der Campaign Web-Benutzeroberfläche verfügbar. Dieser Kanal bezieht sich auf eine Kommunikationsmethode, mit der über ein Callcenter abgewickelte Mitteilungen oder Interaktionen verwalten und verfolgt werden. In der Regel handelt es sich dabei um Telefonanrufe, die von Callcenter-Mitarbeitenden an bestehende oder potenzielle Kundinnen und Kunden erfolgen.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Weitere Informationen finden Sie in der <a href="../call-center/gs-call-center.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Neuer Regel-Builder</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Es ist nun ein neuer Regel-Builder verfügbar, der Sie bei der Definition komplexer Bedingungen in einer verbesserten Benutzeroberfläche unterstützt. Sie können bei Bedarf vom alten zum neuen Regel-Builder wechseln.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Weitere Informationen finden Sie in der <a href="../query/query-modeler-overview.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Erstellen externer Konten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Als Campaign-Admin können Sie nun über die Campaign Web-Benutzeroberfläche neue Verbindungen mit externen Systemen einrichten.
Sie haben zudem die Möglichkeit, vorhandene externe Konten anzuzeigen, zu aktualisieren und zu verwalten.</p>
<p>Weitere Informationen finden Sie in der <a href="../administration/external-account.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#25-4-improvements}

**Allgemeine Verbesserungen an der Benutzeroberfläche**

* Das Feld „Beschreibung“ sowie die Optionen „Zu Favoriten hinzufügen“ und „Werteverteilung“ für Schemaattribute sind jetzt auf der Benutzeroberfläche besser sichtbar. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../get-started/attributes.md).
* Auf der Benutzeroberfläche werden nun Datum und Uhrzeit entsprechend der in den Experience League-Voreinstellungen festgelegten Primärsprache angezeigt. Diese Verbesserung ist nur für einige Sprachen verfügbar. Die vollständige Liste der unterstützten Sprachen finden Sie in der [entsprechenden Dokumentation](https://experienceleague.adobe.com/de/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**E-Mail-Editor**: Um die Barrierefreiheit in der Campaign Web-Benutzeroberfläche zu verbessern, sind im E-Mail-Designer nun zwei neue Felder verfügbar. Sie entsprechen dem Element `title` und dem lang-Attribut im Element `html` Ihres E-Mail-Inhalts. Sie können diese Einstellungen zusätzlich zum Feld „Preheader“ im Abschnitt für den E-Mail-Text definieren. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schemata**

* Sie können nun das temporäre Schema einer Liste über die Campaign Web-Benutzeroberfläche bearbeiten. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../audience/manage-audience.md).
* Sie können nun die benutzerdefinierten Felder eines Schemas in einem Beispielbildschirm in der Vorschau anzeigen. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../administration/custom-fields.md#add).
* Sie können nun benutzerdefinierte Felder per Drag-and-Drop in der Liste verschieben. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../administration/custom-fields.md#add).


### Neue Funktionen in eingeschränkter Verfügbarkeit {#25-4-features-la}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden. Dazu ist ein Upgrade des Campaign-Servers auf die Version 8.7.4 erforderlich.
>
>Weitere Informationen finden Sie auf den folgenden Seiten der Dokumentation: [Wechsel von Campaign Standard zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard-Benutzende](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de).

* **Erstellung eines mehrsprachigen Versands**: In der Adobe Campaign Web-Benutzeroberfläche ist nun die Durchführung mehrerer E-Mail-Sendungen in verschiedenen Sprachen möglich. Mit der Funktion „Mehrsprachiger Versand“ können Sie die Standardsprache Ihres Versands sowie die verschiedenen Sprachen festlegen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in einer Vorschau in den von Ihnen ausgewählten Sprachen anzeigen. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../email/edit-content.md).

* **Dynamische Berichte für mehrsprachige Sendungen**: Dynamische Berichte sind jetzt für mehrsprachige E-Mail-Sendungen verfügbar. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../reporting/global-reports.md).

* **SMS REST API-Unterstützung (LA)**: Das REST-API für Transaktionsnachrichten ist nun für den SMS-Kanal verfügbar. Wenn sowohl „email“ als auch „mobilePhone“ in der Payload vorhanden sind, können Sie den Kanal über das Feld „wishedChannel“ angeben. Ohne Angabe wird standardmäßig „email“ verwendet, es sei denn, „wishedChannel“ fordert explizit SMS an. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

