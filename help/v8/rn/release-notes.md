---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 78%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Version August 2026 {#26-8-release}

_18. August 2026_

### Neue Funktionen {#26-8-features}

<table>
<thead>
<tr>
<th><strong>Workflow-Aktivität „Validierung“</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die Workflow-Aktivität <strong>Validierung</strong>, die zuvor nur in der Client-Konsole verfügbar war, ist jetzt in der Web-Benutzeroberfläche von Campaign verfügbar. Weisen Sie die Aufgabe einer Gruppe oder einer einzelnen Benutzerin bzw. einem einzelnen Benutzer zu, passen Sie den Benachrichtigungstitel und die Nachricht an und definieren Sie die möglichen Antworten (z. B. Ja/Nein) als Ausgabeverzweigungen.</p>
<p>Weitere Informationen finden Sie im <a href="../workflows/activities/approval.md">entsprechenden Handbuch</a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-8-improvements}

* **Öffnungs-Tracking**: Sie können jetzt das Öffnungs-Tracking direkt über die Web-Benutzeroberfläche von Campaign aktivieren oder deaktivieren. Dies hilft Ihnen bei der Einhaltung der Datenschutzbestimmungen. [Weitere Informationen](../advanced-settings/delivery-settings.md#tracking-tab)
* **Programmlistenansicht**: Programme werden jetzt in einer dedizierten Ansicht aufgelistet, ähnlich wie bei Kampagnen, Sendungen und Workflows. Sie können von dieser Ansicht aus bestehende Programme durchsuchen und neue erstellen. [Weitere Informationen](../administration/plans-programs.md#create-program)
* **Konfiguration benutzerdefinierter Schema**: Im Abschnitt **Aktionsdaten** können Sie jetzt die Aktion **Duplizieren** für die Einträge eines benutzerdefinierten Schemas deaktivieren. [Weitere Informationen](../administration/schemas-action-data.md#action-data)
* **Benutzerdefinierte Filter**: Im Schema-Editor können Sie jetzt die Werte, die in der Auswahl für einen benutzerdefinierten Filter des Typs Link verfügbar sind, mithilfe des neuen Dialogfelds **Link-Einstellungen** einschränken. [Weitere Informationen](../administration/schemas-custom-filters.md#settings)
* **Schemavalidierung**: Sie können jetzt die Struktur eines Schemas direkt im Schema-Editor mithilfe der neuen Schaltfläche **Überprüfen** validieren. [Weitere Informationen](../administration/schemas-create-publish.md#create-new)
* **Ordnersicherheit**: Aktionen, die für einen Ordner verfügbar sind, werden nun durchgängig durch die Benutzerrechte geregelt, was dem Verhalten der Client-Konsole entspricht. [Weitere Informationen](../get-started/work-with-folders.md#about-folders).
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->

