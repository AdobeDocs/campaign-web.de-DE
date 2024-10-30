---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 42%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind auf dieser Seite ](release-notes-24.md) [aufgeführt.

## Version Oktober 24 {#24-10-release}

**Veröffentlichungsdatum**: 29. Oktober 2024

Die folgenden Funktionen und Verbesserungen sind ab der Oktober-Version verfügbar.

### Funktionen

<table>
<thead>
<tr>
<th><strong>Externe Konten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können jetzt externe Konten direkt über die Adobe Campaign-Webbenutzeroberfläche einrichten und verwalten. Diese neue Funktion vereinfacht die Konfiguration verschiedener Typen von externen Konten, wie z. B. Bounce-E-Mails (POP3) oder Ausführungsinstanzen.</p>
<p>Weitere Informationen finden Sie in der <a href="../administration/external-account.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transaktionsnachrichtenversand</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transaktionsnachrichten (Message Center) sind jetzt in der Web-Benutzeroberfläche von Campaign verfügbar. Dieses Add-on wurde entwickelt, um Nachrichten auszulösen, die aus Ereignissen generiert wurden, die von Informationssystemen ausgelöst wurden. Es kann sich dabei um Rechnungen, Bestellbestätigungen, Versandbestätigungen, Kennwortänderungen, Benachrichtigungen über die Nichtverfügbarkeit von Produkten, Kontoauszüge, die Erstellung von Website-Konten usw. handeln.</p>
<p>Weitere Informationen finden Sie in der <a href="../transactional-messaging/transactional.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Verbesserungen

* **Workflow-Aktivitäten** - Sie können eine Aktivität und alle ihre untergeordneten Knoten innerhalb eines Workflows von einer Transition in eine andere verschieben. Eine dedizierte Schaltfläche **Verschieben** ist im Eigenschaftenbereich der Aktivität verfügbar, um dies durchzuführen. [Weitere Informationen](../workflows/orchestrate-activities.md#move)

* **Workflow-Anreicherungsaktivität**

   * Sie können jetzt einen Alias und einen Titel definieren, wenn Sie ein neues Feld in der Aktivität **Anreicherung** erstellen. [Weitere Informationen](../workflows/activities/enrichment.md#collection-settings)
   * Sie können jetzt für jedes Profil in der Aktivität **Anreicherung** Angebote hinzufügen. [Weitere Informationen](../workflows/activities/enrichment.md##add-offers)

* **Werteverteilung**: Beim Zugriff auf die Liste der zur Personalisierung vorgesehenen Felder kann jetzt überprüft werden, wie die Werte für jedes Feld verteilt werden. Ein dediziertes Popup-Fenster zeigt die Anzahl und den Prozentsatz für jeden Wert an. [Weitere Informationen](../query/build-query.md#distribution-values-query)

* **Version und Systeminformationen** - Sie können jetzt auf Details zu Ihren Instanzversionen zugreifen, sowohl für die Client-Konsole als auch für die Web-Benutzeroberfläche. In diesem neuen Abschnitt werden auch alle nativen Pakete aufgelistet, die in Ihrer Umgebung installiert sind. [Weitere Informationen](../get-started/user-interface.md#user-interface-about)

* **Listen** - Sie können die Werte einer Liste jetzt einfach neu anordnen. [Weitere Informationen](../get-started/work-with-folders.md)

* **Versand** - Auf die Variable &quot;Versand&quot;kann jetzt über Personalisierungsfelder zugegriffen werden. [Weitere Informationen](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)