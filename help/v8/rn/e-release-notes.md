---
title: Frühzeitige Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der nächsten Version der Campaign Web-Benutzeroberfläche
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 100%

---

# Frühzeitige Versionshinweise {#e-release}

Die Adobe Campaign Web-Benutzeroberfläche bietet kontinuierlich neue Funktionen, Verbesserungen vorhandener Funktionen und Fehlerbehebungen. Alle Änderungen werden am Ende jedes Monats in den [Versionshinweisen](release-notes.md) konsolidiert.

**Die nachfolgenden frühzeitigen Versionshinweise können ohne vorherige Ankündigung bis zum Verfügbarkeitsdatum der Version geändert werden**. Links, Bildschirme und die aktualisierte Dokumentation werden am Veröffentlichungsdatum in den [Versionshinweisen](release-notes.md) veröffentlicht.

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
<p>In der Campaign Web-Benutzeroberfläche können nun externe Sendungen und Versandvorlagen definiert werden. In diesem Modus werden Nachrichten in einer Eingabedatei zusammengefasst, die für einen externen Anbieter freigegeben werden kann. Standardmäßig wird der externe Versandmodus für den Briefpostkanal verwendet.</p>
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
<p>Sie können nun Typologien und Typologieregeln in der Adobe Campaign Web-Oberfläche erstellen. Eine Typologie ist eine Sammlung von Typologieregeln, mit denen Sie Sendungen steuern, filtern und priorisieren können. Typologien stellen sicher, dass Ihre Sendungen stets erforderliche Elemente enthalten (z. B. einen Abmelde-Link oder eine Betreffzeile) und Filterregeln anwenden, um bestimmte Gruppen aus Ihrer Zielgruppe auszuschließen (z. B. Abonnierende, Konkurrentinnen bzw. Konkurrenten oder Kundschaft, die nicht Mitglied des Treueprogramms ist).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Weitere Informationen finden Sie in der <a href="../administration/typologies.md">entsprechenden Dokumentation</a>.</p>
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

### Verbesserungen {#25-1-improvements}

* Anpassen der Anzeige benutzerdefinierter Felder in der Benutzeroberfläche:

   * Sie können nun zusätzliche benutzerdefinierte Felder auswählen, die in der Benutzeroberfläche angezeigt werden sollen.
   * Sie können nun Regeln zum Anzeigen benutzerdefinierter Felder vom Typ „Link“ festlegen, z. B. Listenwerte basierend auf der Eingabe eines anderen Felds beschränken.
   * Flexiblere Anordnung von Feldern in der Benutzeroberfläche: Felder können sich nun über eine einzelne Spalte erstrecken oder zur besseren Organisation in Unterabschnitten gruppiert werden.
   * Sie können nun bestimmte Felder als schreibgeschützt festlegen.

* Filter „Zuletzt verwendet“ und „Favoriten“: Um häufig verwendete Attribute schnell wiederzuverwenden, können Sie sie nun zu Favoriten hinzufügen. Dadurch wird sichergestellt, dass sie für zukünftige Aufgaben problemlos zugänglich sind. Zusätzlich zu den Favoriten können Sie auch die zuletzt ausgewählten Attribute anzeigen und verwenden.


