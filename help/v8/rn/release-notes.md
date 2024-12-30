---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 100%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind [auf dieser Seite](release-notes-24.md) aufgeführt.

## Version Oktober 2024 {#24-10-release}

**Veröffentlichungsdatum**: 29. Oktober 2024

Die folgenden Funktionen und Verbesserungen sind ab der Version Oktober verfügbar.

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
<p>Sie können externe Konten jetzt direkt über die Web-Benutzeroberfläche in Adobe Campaign einrichten und verwalten. Diese neue Funktion vereinfacht die Konfiguration verschiedener Typen von externen Konten, wie z. B. Bounce-E-Mails (POP3) oder Ausführungsinstanzen.</p>
<p>Weitere Informationen finden Sie in der <a href="../administration/external-account.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transaktionsnachrichten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>„Transaktionsnachricht (Message Center)“ ist jetzt in der Campaign Web-Benutzeroberfläche verfügbar.  Dieses Add-on dient dem Auslösen von Nachrichten, die durch Ereignisse erzeugt werden, die von Informationssystemen ausgelöst werden. Hierzu zählen u. a.: Rechnungen, Bestellbestätigungen, Lieferbestätigungen, Passwortänderungen, Benachrichtigungen über die Nicht-Verfügbarkeit eines Produkts, Kontostandsinformationen oder die Erstellung eines Website-Kontos.</p>
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

* **Workflow-Aktivitäten**: Sie können eine Aktivität und alle untergeordneten Knoten innerhalb eines Workflows von einer Transition in eine andere verschieben. Im Bereich mit den Eigenschaften der Aktivität ist die dedizierte Schaltfläche **Verschieben** verfügbar. [Weitere Informationen](../workflows/orchestrate-activities.md#move)

* **Anreicherungsaktivität für Workflows**

   * Sie können jetzt einen Alias und ein Label definieren, wenn Sie ein neues Feld in der Aktivität **Anreicherung** erstellen. [Weitere Informationen](../workflows/activities/enrichment.md#collection-settings)
   * Sie können jetzt für jedes Profil Angebote in der Aktivität **Anreicherung** hinzufügen. [Weitere Informationen](../workflows/activities/enrichment.md##add-offers)

* **Werteverteilung**: Beim Zugriff auf die Liste der zur Personalisierung vorgesehenen Felder kann jetzt überprüft werden, wie die Werte für jedes Feld verteilt werden. Ein dediziertes Popup-Fenster zeigt die Anzahl und den Prozentsatz für jeden Wert an. [Weitere Informationen](../query/build-query.md#distribution-values-query)

* **Versions- und Systeminformationen**: Sie können jetzt sowohl für die Client-Konsole als auch für die Web-Benutzeroberfläche auf Details zu Ihren Instanzversionen zugreifen. In diesem neuen Abschnitt werden außerdem alle nativen Pakete aufgelistet, die in Ihrer Umgebung installiert sind. [Weitere Informationen](../get-started/user-interface.md#user-interface-about)

* **Listen**: Sie können die Werte einer Liste jetzt einfach neu anordnen. [Weitere Informationen](../get-started/work-with-folders.md)

* **Versand**: Auf die Variable „Versand“ kann jetzt über Personalisierungsfelder zugegriffen werden. [Weitere Informationen](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)