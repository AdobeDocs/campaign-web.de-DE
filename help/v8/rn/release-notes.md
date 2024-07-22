---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5b6843e57ac4160d943aac5aca5d86a9b4fa7783
workflow-type: ht
source-wordcount: '1623'
ht-degree: 100%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Versionshinweise für Juni {#24-6-release}

**Veröffentlichungsdatum**: 18.–19. Juni 2024

Die folgenden Funktionen und Verbesserungen stehen allen Benutzenden ab der Juni-Version zur Verfügung.

### Versandwarnung {#24-6-3}

Bei der Funktion „Versandwarnungen“ handelt es sich um ein System zum Warnungs-Management, über das eine Benutzergruppe automatisch Benachrichtigungen zu ihren Sendungen erhält.  [Weitere Informationen](../msg/delivery-alerting.md)

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
