---
title: Frühere Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Versionen der Campaign-Web-Benutzeroberfläche 2024
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 19a7540af7502709b7eafdace038b5958e077173
workflow-type: tm+mt
source-wordcount: '2470'
ht-degree: 100%

---

# Versionshinweise 2024 {#2024-release}

Auf dieser Seite werden alle Änderungen und Verbesserungen aufgelistet, die in **Versionen aus 2024** verfügbar sind. Die neuesten Versionshinweise finden Sie auf [dieser Seite](release-notes.md).


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


### Verbesserungen

* **Workflow-Aktivitäten**: Sie können eine Aktivität und alle untergeordneten Knoten innerhalb eines Workflows von einer Transition in eine andere verschieben. Im Bereich mit den Eigenschaften der Aktivität ist die dedizierte Schaltfläche **Verschieben** verfügbar. [Weitere Informationen](../workflows/orchestrate-activities.md#move)

* **Anreicherungsaktivität für Workflows**

   * Sie können jetzt einen Alias und ein Label definieren, wenn Sie ein neues Feld in der Aktivität **Anreicherung** erstellen. [Weitere Informationen](../workflows/activities/enrichment.md#collection-settings)
   * Sie können jetzt für jedes Profil Angebote in der Aktivität **Anreicherung** hinzufügen. [Weitere Informationen](../workflows/activities/enrichment.md##add-offers)

* **Werteverteilung**: Beim Zugriff auf die Liste der zur Personalisierung vorgesehenen Felder kann jetzt überprüft werden, wie die Werte für jedes Feld verteilt werden. Ein dediziertes Popup-Fenster zeigt die Anzahl und den Prozentsatz für jeden Wert an. [Weitere Informationen](../query/build-query.md#distribution-values-query)

* **Versions- und Systeminformationen**: Sie können jetzt sowohl für die Client-Konsole als auch für die Web-Benutzeroberfläche auf Details zu Ihren Instanzversionen zugreifen. In diesem neuen Abschnitt werden außerdem alle nativen Pakete aufgelistet, die in Ihrer Umgebung installiert sind. [Weitere Informationen](../get-started/user-interface.md#user-interface-about)

* **Listen**: Sie können die Werte einer Liste jetzt einfach neu anordnen. [Weitere Informationen](../get-started/work-with-folders.md)

* **Versand**: Auf die Variable „Versand“ kann jetzt über Personalisierungsfelder zugegriffen werden. [Weitere Informationen](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## September-Updates {#9-2024}

<table>
<thead>
<tr>
<th><strong>KI-Assistent</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nachdem Sie Ihre Nachricht erstellt und angepasst haben, entwickeln Sie sie mit dem KI-Assistenten in Adobe Campaign Web weiter. Mit diesem leistungsstarken Tool können Sie die Wirkung Ihrer Inhalte optimieren, indem Sie eine Reihe ansprechender Texte, Haupttitel und visuell überzeugender Bilder generieren.</p>
<p>Nehmen Sie an unserer <a href="https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator">Live-Funktionsvorstellung</a> teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.</a></p>
<p>Weitere Informationen finden Sie in der <a href="../email/generative-gs.md">entsprechenden Dokumentation</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Verfügbarkeitsdatum: 12. September</p>
</td>
</tr>
</tbody>
</table>

## Version August {#24-8-release}

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
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=de){target="_blank"}.-->


## Versionshinweise für Juli {#24-7-release}

**Veröffentlichungsdatum**: 30.–31. Juli 2024

Die folgenden Funktionen und Verbesserungen sind ab der Version Juli verfügbar.

### Inhaltsfragmente {#24-7-1}

Sie können jetzt Inhaltsfragmente erstellen und verwenden. Ein Inhaltsfragment ist eine wiederverwendbare Komponente, die in einer oder mehreren Nachrichten referenziert werden kann. Wenn Sie ein Fragment ändern, wird jeder Inhalt, der dieses Fragment verwendet, aktualisiert. Mit dieser Funktion können Sie mehrere benutzerdefinierte Inhaltsbausteine vorab erstellen, mit denen Marketing-Benutzende Inhalte von Nachrichten schnell in einem verbesserten Design-Prozess zusammenstellen können.

Es stehen zwei Arten von Fragmenten zur Verfügung:

* **Ausdrucksfragmente** sind vordefinierte Ausdrücke, die über einen dedizierten Eintrag im Ausdruckseditor verfügbar sind.
* **Visuelle Fragmente** sind vordefinierte visuelle Bausteine, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. [Weitere Informationen](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**Visuelle Fragmente** sind eingeschränkt verfügbar (LA, Limited Availability). Diese Funktion ist Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und kann nicht in anderen Umgebungen bereitgestellt werden.

### Trap-Gruppe {#24-7-2}

Eine **Trap-Gruppe** ist eine Liste von Testadressen. Sie wird verwendet, um bestimmte Adressen in Ihre Sendungen einzubeziehen und dann Profile auszuwählen, die nicht den definierten Zielgruppenkriterien entsprechen. Auf diese Weise können Empfängerinnen und Empfänger, die außerhalb der Versandzielgruppe liegen, die Nachricht ebenso wie jede andere Person innerhalb der Zielgruppe erhalten.  Sie können Testadressen beim Versand von Testsendungen oder zum Schutz Ihrer Mailing-Liste verwenden. [Weitere Informationen](../audience/trap-group.md)

### Vorlagen für Rich-Push-Benachrichtigungen {#24-7-3}

Sie können nun Rich-Push-Benachrichtigungen senden. Eine Rich-Push-Benachrichtigung ist eine erweiterte Form einer Mobilgeräte-Benachrichtigung, die über einfache Textnachrichten hinausgeht und Multimedia-Elemente wie Bilder, interaktive Schaltflächen oder andere Rich-Media-Inhalte enthält. Mit dieser Version sind jetzt eine Reihe von Vorlagen für Rich-Push-Benachrichtigungen für Ihre iOS- und Android-Apps verfügbar.

[Weitere Informationen](../push/rich-push.md)

>[!AVAILABILITY]
>
>Diese Funktion erfordert eine Aktualisierung auf Campaign v8.6.3 <!--or v8.7.2-->. Weitere Informationen finden Sie in den [Versionshinweisen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} zur Client-Konsole von Campaign v8.

### Verbesserungen {#improvements-24-7}

**Ordnerverwaltung**: Sie können jetzt Berechtigungen und Einschränkungen für Ordner verwalten.

## Versionshinweise für Juni {#24-6-release}

**Veröffentlichungsdatum**: 18.–19. Juni 2024

Die folgenden Funktionen und Verbesserungen stehen allen Benutzenden ab der Juni-Version zur Verfügung.

<!--### Delivery alerting {#24-6-3}

The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)-->

### Pläne und Programme {#24-6-4}

Sie können jetzt Pläne und Programme zur Organisation Ihrer Kampagnen erstellen. Durch die Definition einer Ordnerhierarchie können Sie Ihre Kampagnen in Programme und Ihre Programme in Pläne organisieren. [Weitere Informationen](../administration/plans-programs.md)

### Verbesserungen {#improvements-24-6}

* **Abstimmung in der Anreicherungsaktivität**: Die Aktivität **Anreicherung** kann jetzt verwendet werden, um Daten aus dem Campaign-Datenbankschema mit Daten aus einem anderen Schema abzustimmen oder aber mit Daten aus einem temporären Schema, z. B. mit Daten, die mithilfe der Aktivität „Datei laden“ hochgeladen wurden. Mit dieser Option können Sie zum Beispiel das Land eines Profils, das in einer hochgeladenen Datei angegeben ist, mit einem der Länder abstimmen, die in der dedizierten Tabelle der Campaign-Datenbank verfügbar sind. [Weitere Informationen](../workflows/activities/enrichment.md)

## Versionshinweise für Mai {#24-5-release}

**Veröffentlichungsdatum**: 21. Mai 2024

Die folgenden Funktionen und Verbesserungen stehen allen Benutzenden ab der Mai-Version zur Verfügung.

### Audit-Protokoll  {#24-5-1}

Die neue Funktion **Audit-Protokoll** bietet eine detaillierte, chronologische Aufzeichnung aller Aktionen und Ereignisse, die in Echtzeit an Ihrer Adobe Campaign-Instanz durchgeführt wurden. Dies bietet eine einfache Methode, um alle Änderungen an Ihren Campaign-Daten zu verfolgen und Abfragen durchzuführen, wie zum Status von Workflows, den Personen, die diese geändert haben oder den Aktivitäten, die von Benutzerinnen und Benutzern innerhalb der Instanz ausgeführt wurden. [Weitere Informationen](../reporting/audit-trail.md)

### Benutzerdefinierte Felder {#24-5-2}

**Benutzerdefinierte Felder** sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zu vorkonfigurierten Schemata hinzugefügt werden. In der Campaign Web-Benutzeroberfläche sind diese benutzerdefinierten Felder nun in verschiedenen Bildschirmen sichtbar, z. B. in den Details eines Profils oder eines Testprofils. In der Web-Benutzeroberfläche können Sie zwar keine benutzerdefinierten Felder erstellen, dafür aber ihre Anzeige ändern. [Weitere Informationen](../administration/custom-fields.md)

### Erstellen von Relationen zwischen Tabellen {#24-5-3}

Sie können jetzt in der Workflow-Aktivität **Anreicherung** Relationen mit einer anderen Tabelle erstellen. Verwenden Sie den neuen Abschnitt **Relationsdefinition** in den Aktivitätsparametern, um eine Relation zwischen den Daten der Arbeitstabelle und der Adobe Campaign-Datenbank herzustellen. Wenn Sie beispielsweise Daten aus einer Datei laden, die die Kundennummer, das Land und die E-Mail-Adresse der Empfängerinnen und Empfänger enthält, können Sie jetzt eine Relation zur Ländertabelle erzeugen, um die entsprechende Information in den Profilen zu aktualisieren. [Weitere Informationen](../workflows/activities/enrichment.md#create-links)

### Allgemeine Verbesserungen {#improvements-24-5}

* **Briefpost** – Sie können jetzt den Ausdruckseditor verwenden, um die Attribute auszuwählen, die in Briefpost-Extraktionsdateien angezeigt werden sollen. [Weitere Informationen](../direct-mail/content-direct-mail.md)

* **Ordnerverwaltung** – Sie können jetzt einen Unterordner von einem anderen Typ als den übergeordneten Ordner erstellen. [Weitere Informationen](../get-started/permissions.md#folders)

* **Globalisierung** – Im Rahmen unserer kontinuierlichen Bemühungen um ein einheitliches Benutzererlebnis harmonisieren wir die in den Adobe Experience Cloud-Produkten und -Apps verwendete Terminologie. Dies wirkt sich auf den deutschen Begriff „Titel“ aus, der in „Label“ geändert wird, wenn er sich auf den Namen eines Objekts bezieht. Die Änderungen werden schrittweise in der Benutzeroberfläche und Dokumentation eingeführt.


## Versionshinweise für April {#april-24-4-release}

**Veröffentlichungsdatum**: 2. Mai 2024

### Neue Funktionen {#new-24-4}

Die folgenden Funktionen stehen allen Benutzenden ab der April-Version zur Verfügung.

**Neue Workflow-Aktivitäten**

* **Daten-Update**: Verwenden Sie diese Aktivität, um gebündelte Aktualisierungen der Datenbankfelder durchzuführen. Die Art der Datenaktualisierung kann über verschiedene Optionen definiert werden. [Weitere Informationen](../workflows/activities/update-data.md)
* **Anmeldedienste**: Verwenden Sie diese Aktivität, um in einer einzigen Aktion mehrere Profile bei einem Dienst anzumelden oder von diesem abzumelden. [Weitere Informationen](../workflows/activities/subscription-services.md)
* **Dateiextraktion**: Verwenden Sie diese Aktivität, um Daten aus Adobe Campaign als externe Datei in ein anderes System zu exportieren. [Weitere Informationen](../workflows/activities/extract-file.md)
* **Dateiübertragung**: Verwenden Sie diese Aktivität, um Dateien zu senden oder zu empfangen, das Vorhandensein von Dateien zu prüfen oder Dateien auf einem Server aufzulisten. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein. [Weitere Informationen](../workflows/activities/transfer-file.md)
* **Test**: Verwenden Sie diese Aktivität, um Transitionen auf der Basis der angegebenen Bedingungen zu aktivieren. [Weitere Informationen](../workflows/activities/test.md)
* **JavaScript-Code**: Verwenden Sie diese Aktivität, um ein JavaScript-Code-Snippet im Kontext eines Workflows auszuführen. [Weitere Informationen](../workflows/activities/javascript-code.md)
* **Externes Signal**: Verwenden Sie diese Aktivität, um die Ausführung eines Workflows über einen anderen Workflow oder einen API-Aufruf auszulösen. [Weitere Informationen](../workflows/activities/external-signal.md)
* **Inkrementelle Abfrage**: Verwenden Sie diese Aktivität, um die Datenbank planmäßig abzufragen. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch ist es möglich, ausschließlich neue Elemente einzubeziehen. [Weitere Informationen](../workflows/activities/incremental-query.md)

**Vorlagen für Rich-Push-Benachrichtigungen**

Sie können nun Rich-Push-Benachrichtigungen über Android senden. Rich-Push-Benachrichtigungen sind eine erweiterte Form von Benachrichtigungen an Mobilgeräte, die über einfache Textnachrichten hinausgehen und Multimedia-Elemente wie Bilder, interaktive Schaltflächen oder andere Rich-Media-Inhalte enthalten. [Weitere Informationen](../push/rich-push.md)

Beachten Sie, dass diese Funktion nur **eingeschränkt verfügbar** ist.


### Neue Funktionen in eingeschränkter Verfügbarkeit {#acs-24-4}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.
>
>Weitere Informationen finden Sie auf den folgenden Seiten der Dokumentation: [Wechsel von Campaign Standard zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard-Benutzende](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de).

* **Branding**: Wenn Sie von Campaign Standard migriert sind, können Ihre technischen Admins nun eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Markenidentität auswirken, z. B. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Sie können diese Marken erstellen und mit verschiedenen Nachrichten oder Landingpages verknüpfen. Diese Konfiguration wird in Vorlagen verwaltet. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=de)

* **Rest-APIs**: Wenn Sie von Campaign Standard migriert sind, können Sie REST-APIs verwenden, um Integrationen für Adobe Campaign zu erstellen und Ihr eigenes Ökosystem zu erstellen, indem Sie Adobe Campaign mit den von Ihnen verwendeten Technologien verbinden. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=de)

* **Dynamisches Reporting**: Wenn Sie von Campaign Standard migriert sind, können Sie auf das dynamische Reporting zugreifen, das vollständig anpassbare und in Echtzeit aktualisierte Berichte zum Messen der Wirkung Ihrer Marketing-Aktivitäten bietet. Dadurch kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Stadt und Alter sowie nach Daten von E-Mail-Kampagnen wie Öffnungen und Klicks ermöglicht. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=de)

* **Landingpages**: Die folgenden Verbesserungen an Landingpages sind nur für Benutzende verfügbar, die einen Wechsel von Campaign Standard durchführen:

   * Sie können nun beim Konfigurieren eines Dienstes auf eine standardmäßige Landingpage zur An-/Abmeldung verweisen. Wenn Sie bei der Erstellung einer E-Mail einen Link zu dieser Landingpage definieren, werden die Benutzenden, die das Landingpage-Formular senden, automatisch für diesen Dienst angemeldet bzw. von ihm abgemeldet. [Weitere Informationen](../audience/manage-services.md#create-service)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht anonymen Besuchenden, auf die Landingpage zuzugreifen. Wenn Sie diese Option deaktivieren, können nur identifizierte Benutzende auf das Formular zugreifen und dieses absenden. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht, zusätzliche interne Daten bei der Landingpage-Übermittlung zu speichern. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option ermöglicht Ihnen die Verwendung einer Landingpage für mehrere Dienste, wodurch sie dynamisch wird. Wenn Sie einen Link zu einer E-Mail hinzufügen und eine dynamische Landingpage auswählen, können Sie einen beliebigen Dienst auswählen. Wenn Sie eine Landingpage auswählen, der ein bestimmter Dienst zugeordnet ist, wird dieser Dienst automatisch verwendet. Sie können keinen anderen Dienst auswählen. [Weitere Informationen](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Bedingte Inhalte werden nun auf Landingpages unterstützt. [Weitere Informationen](../landing-pages/lp-content.md)

### Allgemeine Verbesserungen {#improvements-24-4}

Die folgenden Verbesserungen stehen allen Kundinnen und Kunden ab der April-Version zur Verfügung.

* Die Aktivität **Datei laden** wurde um mehrere Abschnitte erweitert, durch die Sie eine Beispieldatei hochladen, Fehler und Zurückweisungen verwalten sowie hochgeladene Dateien nach Ausführung der Aktivität löschen können. [Weitere Informationen](../workflows/activities/load-file.md)


* Sie haben nun die Möglichkeit, **Aktivitäten in einem Workflow zu kopieren** und in einen Workflow von einer anderen Browser-Registerkarte einzufügen. [Weitere Informationen](../workflows/orchestrate-activities.md#copy-activities-copy)

* Die **Ausführungsoptionen** aller Workflow-Aktivitäten können jetzt verwaltet werden. Auf diese Weise können Sie den Ausführungsmodus und das Verhalten der Aktivität im Falle eines Fehlers definieren. [Weitere Informationen](../workflows/orchestrate-activities.md#execution-options-execution)

* Mit der Option „Transition nicht aktivieren, wenn die Population leer ist“ der **Aktivität „Aufspaltung“** können Sie festlegen, ob der Workflow bei einem leeren Segmentergebnis zur nächsten Aktivität übergehen soll. [Weitere Informationen](../workflows/activities/split.md)

## Versionshinweise für März {#24-3-release}

>[!AVAILABILITY]
>
>Diese Version steht allen Benutzenden ab [Campaign-Version (Konsole) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de) zur Verfügung. Weitere Informationen zu Versionen und Upgrades der Adobe Campaign-Client-Konsole finden Sie in der [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=de){target="_blank"}.

**Veröffentlichungsdatum**: 19.–20. März 2024

### Briefpost-Kanal {#24-3-dm}

Der **Briefpost**-Kanal ist jetzt für die Verwendung in Workflows und für eigenständige Sendungen verfügbar. Briefpost ist ein Offline-Kanal, über den Sie Extraktionsdateien erstellen, personalisieren und generieren sowie diese an Ihre Briefpost-Dienstleister weitergeben können, um Ihrer Kundschaft Post zukommen zu lassen.

### Neue Workflow-Aktivität „Datenquelle ändern“ {#24-3-change-data-source}

Mit der Targeting-Aktivität **Datenquelle ändern** können Sie die Datenquelle der von Ihrem Workflow verwendeten Arbeitstabelle ändern. Diese Aktivität bietet mehr Flexibilität, da Sie damit Daten in Ihren verschiedenen Datenbanken verwalten und die Leistung verbessern können.

### Verbesserung der Workflow-Aktivität „Aufspaltung“ {#24-3-split}

Sie können nun die Option **Alle Teilmengen in derselben Tabelle erzeugen** in der Workflow-Aktivität **Aufspaltung** verwenden, um alle Teilmengen in einer einzigen ausgehenden Transition zu gruppieren. 

### Abfrage-Modeler {#24-3-query-modeler}

* Das Abfragemodell ist jetzt im E-Mail-Designer verfügbar. Damit können Sie Bedingungen beim Erstellen bedingter Inhalte festlegen. 
* Beim Erstellen einer benutzerdefinierten Bedingung sind jetzt vordefinierte Werte für Attribute vom Typ „Datum“ verfügbar. 
* Operatoren können nicht mehr zu einer neuen Transition im Diagramm hinzugefügt werden. Sie können nur für eine vorhandene Transition hinzugefügt werden, bevor Komponenten gefiltert werden, um sie zusammen zu gruppieren. 