---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Oktober-Version {#24-10-release}

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
<p>Sie können jetzt Transaktionsnachrichten in der Campaign-Web-Benutzeroberfläche erstellen und überwachen. Transaktionsnachrichten sind ein spezielles Modul in Adobe Campaign, das für die Verarbeitung ausgelöster Nachrichten entwickelt wurde. Diese Nachrichten werden automatisch als Reaktion auf Ereignisse aus Informationssystemen generiert. Häufige Beispiele für solche Ereignisse sind das Klicken auf Schaltflächen oder Links, das Abbrechen des Warenkorbs, das Anfordern von Warnungen zur Produktverfügbarkeit, das Erstellen oder Ändern von Konten usw.</p>
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


## September-Updates {#9-2024}

<table>
<thead>
<tr>
<th><strong>Content Accelerator des KI-Assistenten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nachdem Sie Ihre Nachricht erstellt und angepasst haben, stellen Sie sie mit dem AI Assistant Content Accelerator im Adobe Campaign Web auf die nächste Stufe. Mit diesem leistungsstarken Tool können Sie die Wirkung Ihrer Inhalte optimieren, indem Sie eine Reihe ansprechender Texte, Haupttitel und visuell überzeugender Bilder generieren.</p>
<p>Nehmen Sie an unserer <a href="https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator">Live-Funktionsvorstellung</a> teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.</a></p>
<p>Weitere Informationen finden Sie in der <a href="../email/generative-gs.md">entsprechenden Dokumentation</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Verfügbarkeitsdatum: 12. September</p>
</td>
</tr>
</tbody>
</table>

## August-Version {#24-8-release}

**Veröffentlichungsdatum**: 3. September 2024

Die folgenden Funktionen und Verbesserungen sind ab der Version August verfügbar.

* **SMTP-Parameter**: SMTP-Einstellungen sind jetzt in den E-Mail-Versandeinstellungen verfügbar. [Weitere Informationen](../advanced-settings/delivery-settings.md#smtp)

* **Globale Variablen**: Sie können jetzt globale Variablen definieren, um Werte für Ihre Sendungen zu definieren. [Weitere Informationen](../advanced-settings/delivery-settings.md#variables-delivery)

### Neue Funktionen in eingeschränkter Verfügbarkeit {#acs-24-8}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.
>
>Weitere Informationen finden Sie auf den folgenden Seiten der Dokumentation: [Wechsel von Campaign Standard zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard-Benutzende](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de){target="_blank"}.

* **Branding für Briefpost**: Technische Admins können nun eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Markenidentität auswirken, z. B. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Diese Marken können jetzt erstellt und mit verschiedenen Nachrichten oder Landingpages verknüpft werden. Diese Konfiguration wird in Vorlagen verwaltet. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/branding/branding-assign)

* **Abonnements mit Landingpages**: Es ist jetzt möglich, eine Landingpage mit einem Dienst zu verknüpfen und eine Bestätigungsnachricht zu versenden, wenn Benutzende dies validieren. [Weitere Informationen](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visuelle Fragmente**: Visuelle Inhaltsfragmente können jetzt archiviert werden. [Weitere Informationen](../content/create-fragment.md#archive)

* **Captcha in Landingpages**: Sie können jetzt Captcha zum Schutz Ihrer Landingpage vor Spam und Missbrauch durch Bots hinzufügen. Dies erfordert nur wenig Einsatz aufseiten Ihrer Kundschaft, da nur eine Interaktion mit Ihrer Website erforderlich ist. [Weitere Informationen](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
