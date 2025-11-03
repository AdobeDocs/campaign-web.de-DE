---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 64%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind auf den Seiten für [2024](release-notes-24.md) und [2025](release-notes-25.md) aufgeführt.

## Version Oktober &#39;25 {#25-10-updates}

_28. Okt. 2025_

<table>
<thead>
<tr>
<th><strong>Mehrsprachige Funktionen für Transaktionsnachrichten, Push-Benachrichtigungen und SMS (eingeschränkte Verfügbarkeit)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können über die Adobe Campaign Web-Benutzeroberfläche jetzt mehrere Transaktionsnachrichten, Push-Benachrichtigungen und SMS-Nachrichten in verschiedenen Sprachen versenden. Mit der Funktion „Mehrsprachiger Versand“ können Sie die Standardsprache Ihres Versands sowie die verschiedenen Sprachen festlegen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in einer Vorschau in den von Ihnen ausgewählten Sprachen anzeigen.</p>
<p>Hinweis: Diese Funktion ist nur für eine bestimmte Gruppe von Unternehmen verfügbar (eingeschränkte Verfügbarkeit) und wird in einer zukünftigen Version global eingeführt.</p>
<p>Weitere Informationen finden Sie in der <a href="../msg/multilingual.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>Profilanreicherung in Transaktionsnachrichten (eingeschränkte Verfügbarkeit)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Mit dieser Funktion können Sie Transaktionsnachrichten personalisieren, indem Sie Adobe Campaign-Datenbankfelder mit dem Nachrichteninhalt verknüpfen. Sie können Zielgruppen-Mappings, Anreicherungsspalten und einen Abstimmschlüssel auswählen, um präzise Echtzeit-Personalisierung unter Einhaltung der Leistungsschwellen sicherzustellen.</p>
<p>Hinweis: Diese Funktion ist nur für eine bestimmte Gruppe von Unternehmen verfügbar (eingeschränkte Verfügbarkeit) und wird in einer zukünftigen Version global eingeführt. Diese Funktion ist derzeit nur für E-Mails verfügbar.</p>
<p>Weitere Informationen finden Sie in der <a href="../transactional-messaging/profile-enrichment.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integration mit Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Um die Marketing-Effizienz zu steigern und die Markenkonsistenz zu gewährleisten, können GenStudio for Performance Marketing-Erlebnisse jetzt nahtlos in Campaign integriert werden. Auf diese Weise können Sie die KI-gestützte Inhaltserstellung von GenStudio zusammen mit den erweiterten Orchestrierungsfunktionen von Campaign nutzen.<p>
<p>Weitere Informationen finden Sie in der <a href="../integrations/genstudio.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Unterstützung des Dunkelmodus in Email Designer</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Die E-Mail-Designer bietet jetzt die Möglichkeit, in die Dunkelmodusansicht zu wechseln, in der Sie zusätzlich bestimmte benutzerdefinierte Einstellungen definieren können. Beachten Sie, dass das endgültige Rendering vom E-Mail-Client des Empfängers abhängt. Nicht alle E-Mail-Clients unterstützen den Dunkelmodus.</p>
<p>Weitere Informationen finden Sie in der <a href="../email/accessible-content.md#dark-mode">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Verbesserungen {#25-10-improvements}

* In Sendungen, die in der Client-Konsole erstellt wurden, zeigt der Abschnitt **Zielgruppe** jetzt an, ob eine dynamische Bedingung für Testversand-Ziele definiert wurde. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Beim Einrichten einer Bedingung mit der Funktion für bedingte Inhalte von Email Designer können Sie jetzt zwischen dem neuen und dem alten Regel-Builder wechseln. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Sie können jetzt in der Bildschirmdefinition des Empfängerschemas Sammlungs-Links wie Käufe auswählen. Dadurch werden die zugehörigen Daten auf Profilbildschirmen über eine dedizierte Registerkarte angezeigt. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Als Campaign-Administrator können Sie jetzt Verbindungen zu Salesforce CRM und Microsoft Dynamics einrichten.
  [Weitere Informationen](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

