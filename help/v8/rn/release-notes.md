---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 23%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Version Juli &#39;26 {#26-7-release}

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
<p>Sie können jetzt Angebote durchgängig direkt über die Web-Benutzeroberfläche von Campaign verwalten. Konfigurieren Sie Angebotsumgebungen und Platzierungen, erstellen Sie Ihren Angebotskatalog und Ihre Kategorien, erstellen Sie Angebote mit Eignungsregeln und Prioritätsgewichten und genehmigen und stellen Sie sie für Ihre Sendungen bereit. Erweiterte Konfigurationen sind weiterhin in der Client-Konsole verfügbar.</p>
<p>Weitere Informationen finden Sie im <a href="../offers/gs-offer-management.md">entsprechenden Handbuch</a>.</p>
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
<p>Technische Administratoren können jetzt Marken direkt über die Web-Benutzeroberfläche von Campaign erstellen und konfigurieren, ohne die Client-Konsole zu verwenden. Alle Markeneinstellungen, einschließlich Identität, Subdomain und Protokolle, E-Mail-Header-Parameter und URL-Tracking-Parameter, sind jetzt in der Web-Benutzeroberfläche verfügbar.</p>
<p>Weitere Informationen finden Sie im <a href="../administration/branding/branding-configure.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Öffentliche Ressourcen in der E-Mail-Designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Beim Hinzufügen von Bildern zu Ihren E-Mails können Sie jetzt "<strong> Ressourcen“ </strong>. Auf diese Weise können Sie ein Bild auswählen, das bereits in Ihrer Adobe Campaign-Instanz verfügbar ist, z. B. eine zuvor in die E-Mail-Designer importierte Datei oder eine öffentliche Ressource, die über die Client-Konsole hochgeladen wurde.</p>
<p>Weitere Informationen finden Sie im <a href="../email/content-components.md#image">entsprechenden Handbuch</a>.</p>
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
<p>Die Aktivität <strong>Laden (RDBMS</strong> ist jetzt in der Web-Benutzeroberfläche von Campaign verfügbar. Verwenden Sie diese Aktivität, um Daten direkt aus einer externen relationalen Datenbank in Ihren Workflow zu laden. Die extrahierten Daten stehen während des gesamten Workflows zur Verfügung und können für die Zielgruppenbestimmung, Anreicherung oder weitere Datenverarbeitung verwendet werden.</p>
<p>Weitere Informationen finden Sie im <a href="../workflows/activities/data-loading-rdbms.md">entsprechenden Handbuch</a>.</p>
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
<p>Mit Dynamic JavaScript Pages (JSSP) können Sie Server-seitige Seiten erstellen, die dynamische Inhalte generieren, wenn über eine URL zugegriffen wird, z. B. benutzerdefinierte APIs, Exporte oder Web-Anwendungslogik. Sie können diese Seiten jetzt direkt in der Web-Benutzeroberfläche von Campaign erstellen, ändern, duplizieren und löschen.</p>
<p>Weitere Informationen finden Sie im <a href="../administration/dynamic-javascript-pages.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-7-improvements}

* Die folgenden Verbesserungen wurden an der **benutzerdefinierten Schemakonfiguration“**:
  * Der neue **Aktionsdaten**-Abschnitt ermöglicht es Ihnen, die für die Datensätze eines benutzerdefinierten Schemas verfügbaren Aktionen zu beschränken, unabhängig von den für einzelne Ordner konfigurierten Sicherheitsregeln. [Weitere Informationen](../administration/schemas-action-data.md)
  * **Benutzerdefinierte Filter** wurden im Abschnitt **Konfiguration der Inventarliste“**. Damit können Sie auswählen, welche Attribute als Schnellzugriffsfelder im Filterbereich der Listenansicht angezeigt werden sollen. [Weitere Informationen](../administration/schemas-custom-filters.md)

* Die folgenden Verbesserungen wurden an (**)**:
  * Das Löschen einer Workflow-Aktivität ist jetzt flexibler: Wenn eine Aktivität nachfolgende Aktivitäten aufweist, können Sie diese entweder alle löschen, nur die ausgewählte Aktivität löschen oder sie löschen, während ihre nachfolgenden Aktivitäten in einer neuen Verzweigung verbleiben. [Weitere Informationen](../workflows/orchestrate-activities.md#delete-activity)
  * Sie können jetzt eine Transition zwischen zwei Workflow-Aktivitäten trennen, ohne eine der Workflow-Aktivitäten zu löschen. Auf diese Weise können Sie ein Workflow-Diagramm neu organisieren, z. B. um eine Gruppe von Aktivitäten, die Sie beibehalten möchten, vorübergehend beiseite zu legen, ohne sie löschen und neu erstellen zu müssen. [Weitere Informationen](../workflows/orchestrate-activities.md#disconnect-transition)
  * Horizontale und vertikale Bildlaufleisten werden jetzt auf der Workflow-Arbeitsfläche angezeigt, sodass Sie durch Ziehen direkt in den Bereich, den Sie anzeigen möchten, in großen Workflows navigieren können. [Weitere Informationen](../workflows/orchestrate-activities.md)
  * Beim Speichern oder Starten/Neustarten eines Workflows wird jetzt eine Warnung angezeigt, wenn ein anderer Benutzer den Workflow in der Web-Benutzeroberfläche oder der Client-Konsole geändert hat, seit Sie ihn geöffnet haben. Sie können die anderen Änderungen mit Ihren überschreiben, den Workflow neu laden, um die neueste Version zu erhalten, oder abbrechen.

* **Absender-E** Mail-Adresse: Sie können jetzt das Feld **Von E-Mail** Ihrer Sendungen mithilfe der Option **NmsDelivery_senderAddressMask** auf eine vordefinierte Liste von Adressen beschränken. [Weitere Informationen](../administration/options.md#restrict-sender-address)
* **Login-Fehlermeldungen** wurden verbessert: Wenn ein Anmeldeversuch fehlschlägt, zeigt die Web-Benutzeroberfläche jetzt eine spezifischere Fehlermeldung für mehrere Szenarien an (z. B. wenn dem Benutzer keine Sicherheitszone zugewiesen ist oder seine IP-Adresse eingeschränkt ist).
