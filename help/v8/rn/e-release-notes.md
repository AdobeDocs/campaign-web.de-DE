---
title: Frühzeitige Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der nächsten Version der Campaign Web-Benutzeroberfläche
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 202796bbaa26afb0741a5eb3947795ceff7e5414
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 21%

---

# Frühzeitige Versionshinweise {#e-release}

Die Adobe Campaign Web-Benutzeroberfläche bietet kontinuierlich neue Funktionen, Verbesserungen vorhandener Funktionen und Fehlerbehebungen. Alle Änderungen werden am Ende jedes Monats in den [Versionshinweisen](release-notes.md) konsolidiert.

**Die nachfolgenden frühzeitigen Versionshinweise können ohne vorherige Ankündigung bis zum Verfügbarkeitsdatum der Version geändert werden**. Links, Bildschirme und die aktualisierte Dokumentation werden am Veröffentlichungsdatum in den [Versionshinweisen](release-notes.md) veröffentlicht.

## Version Januar &#39;25 {#25-1-release}

**Veröffentlichungsdatum**: 5. Februar 2025

Die folgenden Funktionen und Verbesserungen sind ab Januar verfügbar.

### Funktionen {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Erstellen und Verwenden von visuellen Fragmenten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Visuelle Fragmente sind vordefinierte visuelle Blöcke, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. Diese Funktion steht nun allen Kunden zur Verfügung, die mit Server-Build 8.6.4 und höher arbeiten.</p>
<p>Weitere Informationen finden Sie in der <a href="../content/use-visual-fragments.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Verwenden eines Drittanbietersystems zum Senden von Sendungen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt externe Sendungen und externe Versandvorlagen in der Web-Benutzeroberfläche von Campaign definieren. In diesem Modus werden Nachrichten in eine Eingabedatei kompiliert, die mit Ihrem externen Anbieter geteilt werden kann. Standardmäßig wird der externe Versandmodus für den Briefpostkanal verwendet.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Erstellen von Geschäftsregeln (Typologieregeln)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt Typologien und Typologieregeln in der Adobe Campaign-Web-Oberfläche erstellen. Eine Typologie ist eine Sammlung von Typologieregeln, mit denen Sendungen gesteuert, gefiltert und priorisiert werden können. Typologien stellen sicher, dass Ihre Sendungen immer erforderliche Elemente enthalten (z. B. einen Abmelde-Link oder eine Betreffzeile) und wenden Filterregeln an, um bestimmte Gruppen aus Ihrer Zielgruppe auszuschließen (z. B. Abonnenten, Konkurrenten oder Kunden, die nicht Mitglied des Treueprogramms sind).</p>
<img src="assets/do-not-localize/typology.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Auflistungen verwalten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können Auflistungen jetzt direkt über die Adobe Campaign-Web-Benutzeroberfläche erstellen. Eine Auflistung ist eine Liste von Werten, die vom System zum Ausfüllen von Feldern vorgeschlagen werden. Verwenden Sie Auflistungen, um die Werte dieser Felder zu standardisieren, die Dateneingabe zu unterstützen oder sie in Abfragen zu verwenden.</p>
<img src="assets/do-not-localize/enumerations.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Sie können jetzt in der Web-Benutzeroberfläche von Adobe Campaign auf technische Optionen zugreifen und Ihre eigenen benutzerdefinierten Optionen entsprechend Ihren Anforderungen erstellen. Dies ist besonders nützlich, wenn Sie mit Workflow-Aktivitäten mit JavaScript-Code arbeiten, um Zwischendaten zu speichern.</p>
<img src="assets/do-not-localize/options.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definieren und Aufrufen von JavaScript-Codes</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt JavaScript-Codes in der Web-Benutzeroberfläche von Adobe Campaign erstellen. Auf diese Weise können Sie wiederverwendbare Funktionen erstellen, die in Workflows verwendet werden können, ähnlich wie bei einer Bibliothek.</p>
<img src="assets/do-not-localize/javascript.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#25-1-improvements}

* Anpassen der Anzeige benutzerdefinierter Felder in der Benutzeroberfläche:

   * Sie können jetzt zusätzliche benutzerdefinierte Felder auswählen, die in der Benutzeroberfläche angezeigt werden sollen
   * Sie können jetzt Regeln für die Anzeige benutzerdefinierter Felder vom Typ „Link“ festlegen, z. B. das Beschränken von Listenwerten basierend auf der Eingabe eines anderen Felds
   * Sie können Felder in der Benutzeroberfläche jetzt flexibler anordnen: Felder können sich über eine einzelne Spalte erstrecken oder zur besseren Organisation in Unterabschnitten gruppiert werden
   * Sie können jetzt bestimmte Felder als schreibgeschützt festlegen

* Filter „Zuletzt verwendet“ und „Favoriten“: Um häufig verwendete Attribute schnell wiederzuverwenden, können Sie sie jetzt zu Favoriten hinzufügen. Dadurch wird sichergestellt, dass sie für zukünftige Aufgaben leicht zugänglich sind. Zusätzlich zu den Favoriten können Sie auch die zuletzt ausgewählten Attribute anzeigen und verwenden.


