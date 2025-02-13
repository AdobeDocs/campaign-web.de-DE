---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 93%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind [auf dieser Seite](release-notes-24.md) aufgeführt.

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
<p>Visuelle Fragmente sind vordefinierte visuelle Bausteine, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. Diese Funktion steht nun allen Kundinnen und Kunden mit Serverbuild 8.6.4 und höher zur Verfügung.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
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
<img src="assets/do-not-localize/external-delivery.gif">
<p>Weitere Informationen finden Sie in der <a href="../msg/send-external-deliveries.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

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
<img src="assets/do-not-localize/enumerations.gif">
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
<img src="assets/do-not-localize/options.gif">
<p>Weitere Informationen finden Sie in der <a href="../administration/options.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definieren und Aufrufen von JavaScript-Code</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können nun JavaScript-Code in der Adobe Campaign Web-Benutzeroberfläche erstellen. Auf diese Weise können Sie wiederverwendbare Funktionen erstellen, die in Workflows genutzt werden können, ähnlich wie bei einer Bibliothek.</p>
<img src="assets/do-not-localize/javascript.gif">
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
<p>Der KI-Assistent ist jetzt für Ihre Landingpage-Sendungen verfügbar, sodass Sie Text, Bilder oder vollständige Seiten-Layouts generieren können.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Weitere Informationen zum KI-Assistenten finden Sie in der <a href="../email/generative-lp.md"> Dokumentation </a>.</p>
</td>
</tr>
</tbody>
</table>




### Verbesserungen {#25-1-improvements}

* Anpassen der Anzeige benutzerdefinierter Felder in der Benutzeroberfläche:

   * Sie können nun zusätzliche benutzerdefinierte Felder auswählen, die in der Benutzeroberfläche angezeigt werden sollen.
   * Sie können nun Regeln zum Anzeigen benutzerdefinierter Felder vom Typ „Link“ festlegen, z. B. Listenwerte basierend auf der Eingabe eines anderen Felds beschränken.
   * Flexiblere Anordnung von Feldern in der Benutzeroberfläche: Felder können sich nun über eine einzelne Spalte erstrecken oder zur besseren Organisation in Unterabschnitten gruppiert werden.
   * Sie können nun bestimmte Felder als schreibgeschützt festlegen.

* Filter „Zuletzt verwendet“ und „Favoriten“: Um häufig verwendete Attribute schnell wiederzuverwenden, können Sie sie nun zu Favoriten hinzufügen. Dadurch wird sichergestellt, dass sie für zukünftige Aufgaben problemlos zugänglich sind. Zusätzlich zu den Favoriten können Sie auch die zuletzt ausgewählten Attribute anzeigen und verwenden.

* Externe Konten: Der neue **[!UICONTROL Routing]**-Typ steht beim Erstellen eines neuen externen Kontos zur Auswahl. Damit können Sie ein bestimmtes externes Konto für Ihre externen Sendungen konfigurieren. [Weitere Informationen](../administration/external-account.md#routing)