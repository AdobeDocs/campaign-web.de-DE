---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 56%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign-Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das eine skalierbare, schrittweise Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals monatlich aktualisiert. Überprüfen Sie sie regelmäßig.

Die Änderungen und Verbesserungen, die mit früheren Versionen verfügbar waren, werden [auf dieser Seite](release-notes-24.md) aufgeführt.

## Version Februar &#39;25 {#25-2-release}

**Veröffentlichungsdatum**: 18. Februar 2025

Die folgenden Funktionen und Verbesserungen sind ab der Version Februar verfügbar.

### Funktionen {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Erstellen von Geschäftsregeln (Typologieregeln)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt Typologien und Typologieregeln in der Adobe Campaign Web-Benutzeroberfläche erstellen. Typologien steuern, filtern und priorisieren den Versand von Sendungen. Typologien überprüfen, ob Sendungen immer obligatorische Komponenten enthalten (z. B. einen Abmelde-Link oder eine Betreffzeile) oder Filterregeln, um Gruppen aus Ihrer Zielgruppe auszuschließen (z. B. Abonnenten, Konkurrenten oder Kunden, die nicht Mitglied im Treueprogramm sind).</p>
<img src="assets/do-not-localize/typology.gif" alt="Abbildung der Erstellung von Typologieregeln in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../administration/typologies.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Zielgruppen-Mappings</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt Zielgruppen-Mappings in der Campaign Web-Benutzeroberfläche erstellen. Zielgruppen-Mappings definieren, wie verschiedene Versandkanäle (E-Mail, SMS, Push-Benachrichtigungen) mit den Datenfeldern eines Schemas verknüpft werden. Das Zielgruppen-Mapping definiert die Zielgruppe: Profile, Vertragsbegünstigte, Benutzer, Abonnenten, Interessenten und andere.</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Abbildung der Erstellung von Zielgruppen-Mappings in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../administration/target-mappings.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schemadetails</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt auf die Details eines Schemas zugreifen, indem Sie dessen Namen in der Liste auswählen. Auf die Bearbeitung benutzerdefinierter Felder kann jetzt über die Schaltfläche <b>Benutzerdefinierte Felder bearbeiten</b> in den Schemadetails zugegriffen werden.</p>
<img src="assets/do-not-localize/schemas.gif" alt="Abbildung von Schemadetails und der Bearbeitung benutzerdefinierter Felder in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../administration/schemas.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

## Version Januar 2025 {#25-1-release}

**Veröffentlichungsdatum**: 5. Februar 2025

Die folgenden Funktionen und Verbesserungen sind ab der Version Januar verfügbar.

### Funktionen {#25-1-features}

<table>
<thead>
<tr>
<th><strong>Erstellen und Verwenden visueller Fragmente</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Visuelle Fragmente sind vordefinierte visuelle Blöcke, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. Diese Funktion steht nun allen Kundinnen und Kunden mit Serverbuild 8.6.4 und höher zur Verfügung.</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Abbildung der Erstellung und Verwendung visueller Fragmente in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../content/use-visual-fragments.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Verwenden eines Drittanbietersystems für Sendungen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>In der Campaign Web-Benutzeroberfläche können nun externe Sendungen und Versandvorlagen definiert werden. In diesem Modus werden Nachrichten in einer Ausgabedatei zusammengefasst, die für einen externen Anbieter freigegeben werden kann. Standardmäßig wird der externe Versandmodus für den Briefpostkanal verwendet.</p>
<img src="assets/do-not-localize/external-delivery.gif" alt="Abbildung der Einrichtung externer Sendungen in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../msg/send-external-deliveries.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Verwalten von Auflistungen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können Auflistungen nun direkt über die Adobe Campaign Web-Benutzeroberfläche erstellen. Eine Auflistung ist eine Liste von Werten, die vom System zum Auffüllen von Feldern vorgeschlagen werden. Verwenden Sie Auflistungen, um die Werte dieser Felder zu standardisieren, die Dateneingabe zu unterstützen oder sie in Abfragen zu verwenden.</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Abbildung der Auflistungsverwaltung in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../administration/enumerations.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Erstellen benutzerdefinierter Optionen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können nun in der Adobe Campaign Web-Benutzeroberfläche auf technische Optionen zugreifen und eigene benutzerdefinierte Optionen entsprechend Ihren Anforderungen erstellen. Dies ist besonders nützlich, wenn Sie mit JavaScript-Code-Workflow-Aktivitäten arbeiten, um Zwischenergebnisse zu speichern.</p>
<img src="assets/do-not-localize/options.gif" alt="Abbildung der Erstellung benutzerdefinierter Optionen in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../administration/options.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>JavaScript-Codes definieren und aufrufen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können nun JavaScript-Code in der Adobe Campaign Web-Benutzeroberfläche erstellen. Auf diese Weise können Sie wiederverwendbare Funktionen erstellen, die in Workflows verwendet werden können, ähnlich wie bei einer Bibliothek.</p>
<img src="assets/do-not-localize/javascript.gif" alt="Abbildung der Erstellung von JavaScript-Code in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weitere Informationen finden Sie in der <a href="../administration/javascript-codes.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Generieren von Landingpages mit dem KI-Assistenten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Der KI-Assistent ist nun für den Versand von Landingpages verfügbar, sodass Sie Text, Bilder oder vollständige Seiten-Layouts generieren können.</p>
<img src="assets/do-not-localize/ai-lp.gif" alt="Abbildung der Verwendung des KI-Assistenten für die Erstellung von Landingpages in der Web-Benutzeroberfläche von Adobe Campaign">
<p>Weiterführende Informationen zum KI-Assistenten finden Sie im <a href="../email/generative-lp.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#25-1-improvements}

* Anpassen der Anzeige benutzerdefinierter Felder in der Benutzeroberfläche:
   * Wählen Sie zusätzliche benutzerdefinierte Felder aus, die auf der Benutzeroberfläche angezeigt werden sollen.
   * Legen Sie Regeln für die Anzeige benutzerdefinierter Felder vom Typ „Link“ fest, z. B. das Beschränken von Listenwerten basierend auf der Eingabe eines anderen Felds.
   * Felder in der Benutzeroberfläche flexibler anordnen: Felder können sich über eine einzelne Spalte erstrecken oder zur besseren Organisation in Unterabschnitten gruppiert werden.
   * Legen Sie bestimmte Felder als schreibgeschützt fest.

* Filter „Zuletzt verwendet“ und „Favoriten“: Zum schnellen Zugriff häufig verwendete Attribute zu den Favoriten hinzufügen. Neben den Favoriten können Sie auch die zuletzt ausgewählten Attribute anzeigen und verwenden.

* Externe Konten: Der neue **[!UICONTROL Routing]**-Typ steht beim Erstellen eines neuen externen Kontos zur Auswahl. Damit können Sie ein bestimmtes externes Konto für Ihre externen Sendungen konfigurieren. [Weitere Informationen](../administration/external-account.md#routing).