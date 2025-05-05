---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 35%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die mit früheren Versionen verfügbar sind, sind in den [2024](release-notes-24.md) und [2025](release-notes-25.md) aufgeführt.

## Version April &#39;25 {#25-4-release}

**Veröffentlichungsdatum**: Mittwoch, 29. April 2025


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
<p>Der Callcenter-Kanal ist jetzt in der Web-Benutzeroberfläche von Campaign verfügbar. Dieser Kanal bezieht sich auf eine Kommunikationsmethode, die verwendet wird, um Kommunikationen oder Interaktionen zu verwalten und zu verfolgen, die über ein Callcenter abgewickelt werden - in der Regel Telefonanrufe, die von Agenten an Kunden oder Interessenten getätigt werden.</p>
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
<p>Es ist jetzt ein neuer Regel-Builder verfügbar, der Ihnen bei der Definition komplexer Bedingungen in einer verbesserten Benutzeroberfläche hilft. Sie können bei Bedarf vom alten zum neuen Regel-Builder wechseln.</p>
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
<p>Als Campaign-Administrator können Sie jetzt über die Campaign Web-Benutzeroberfläche neue Verbindungen mit externen Systemen einrichten.
Sie können auch vorhandene externe Konten anzeigen, aktualisieren und verwalten.</p>
<p>Weitere Informationen finden Sie in der <a href="../administration/external-account.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#25-4-improvements}

**Allgemeine Verbesserungen an der Benutzeroberfläche**

* Die Optionen Feldbeschreibung, Zu Favoriten hinzufügen und Verteilung von Werten für Schemaattribute sind jetzt in der Benutzeroberfläche besser sichtbar. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../get-started/attributes.md).
* Auf der Benutzeroberfläche werden jetzt Datum und Uhrzeit entsprechend der in den Experience League-Voreinstellungen festgelegten Primärsprache angezeigt. Diese Verbesserung ist nur für mehrere Sprachen verfügbar. Die vollständige Liste der unterstützten Sprachen finden Sie in der [ Dokumentation](https://experienceleague.adobe.com/de/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**E-Mail-Editor**: Um die Barrierefreiheit in der Web-Benutzeroberfläche von Campaign zu verbessern, stehen in der E-Mail-Designer jetzt zwei neue Felder zur Verfügung, die dem `title`- und dem lang-Attribut im `html`-Element Ihres E-Mail-Inhalts entsprechen. Sie können diese Einstellungen zusätzlich zum Feld Preheader im Abschnitt E-Mail-Textkörper definieren. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schemata**

* Sie können jetzt das temporäre Schema einer Liste über die Web-Benutzeroberfläche von Campaign bearbeiten. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../audience/manage-audience.md).
* Sie können jetzt die benutzerdefinierten Felder eines Schemas in einem Beispielbildschirm in der Vorschau anzeigen. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../administration/custom-fields.md#add).
* Benutzerdefinierte Felder können jetzt per Drag-and-Drop in der Liste verschoben werden. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../administration/custom-fields.md#add).


### Neue Funktionen in eingeschränkter Verfügbarkeit {#25-4-features-la}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind auf Kunden beschränkt, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in einer anderen Umgebung bereitgestellt werden. Dazu ist ein Upgrade des Campaign-Servers auf Version 8.7.4 erforderlich.
>
>Weitere Informationen finden Sie auf den folgenden Seiten der Dokumentation: [Wechsel von Campaign Standard zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard-Benutzende](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de).

* **Erstellung eines mehrsprachigen Versands** - Sie können jetzt in der Web-Benutzeroberfläche von Adobe Campaign mehrere E-Mail-Sendungen in verschiedenen Sprachen senden. Mit der Funktion „Mehrsprachiger Versand“ können Sie die Standardsprache Ihres Versands sowie die verschiedenen Sprachen auswählen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in den von Ihnen ausgewählten Sprachen in der Vorschau anzeigen. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../email/edit-content.md).

* **Dynamisches Reporting für mehrsprachige**) - Dynamische Berichte sind jetzt für mehrsprachige E-Mail-Sendungen verfügbar. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](../reporting/global-reports.md).

* **SMS-REST-API-Unterstützung (LA)** - Die REST-API für Transaktionsnachrichten ist jetzt für den SMS-Kanal verfügbar. Wenn sowohl E-Mail als auch Mobiltelefon in der Payload vorhanden sind, können Sie das Feld „wishChannel“ verwenden, um den Kanal anzugeben. Wenn keine E-Mail-Adresse angegeben wird, wird sie standardmäßig verwendet, es sei denn, WishedChannel fordert explizit SMS an. Weitere Informationen finden Sie in der [entsprechenden Dokumentation](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

