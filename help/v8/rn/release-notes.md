---
title: Neueste Versionshinweise
description: Entdecken Sie neue Funktionen in der Campaign Web-Benutzeroberfläche.
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e98a1cf9bcda2183dbfa2c607b53f0aa2f70a998
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 27%

---

# Versionshinweise {#latest-release}

<!--Last update: **March 19, 2024**-->

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Versandmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## April - Versionshinweise {#april-24-4-release}

**Veröffentlichungsdatum**: 30. April 2024

### Neue Funktionen {#new-24-4}

Die folgenden Funktionen stehen allen Benutzern ab der April-Version zur Verfügung.

**Neue Workflow-Aktivitäten**

* **Daten aktualisieren** - Verwenden Sie diese Aktivität, um gebündelte Aktualisierungen der Datenbankfelder durchzuführen. Mit verschiedenen Optionen können Sie die Datenaktualisierung personalisieren. [Weitere Informationen](../workflows/activities/update-data.md)
* **Abonnementdienste** - Verwenden Sie diese Aktivität, um mehrere Profile für/von einem Dienst in einer einzigen Aktion anzumelden oder abzumelden. [Weitere Informationen](../workflows/activities/subscription-services.md)
* **Dateiextraktion** - Verwenden Sie diese Aktivität, um Daten aus Adobe Campaign als externe Datei in ein anderes System zu exportieren. [Weitere Informationen](../workflows/activities/extract-file.md)
* **Dateiübertragung** - Verwenden Sie diese Aktivität, um Dateien zu empfangen oder zu senden, auf Existenz von Dateien zu testen oder Dateien auf einem Server aufzulisten. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein. [Weitere Informationen](../workflows/activities/transfer-file.md)
* **Test** - Verwenden Sie diese Aktivität, um Transitionen auf der Basis der angegebenen Bedingungen zu aktivieren. [Weitere Informationen](../workflows/activities/test.md)
* **JavaScript-Code** - Verwenden Sie diese Aktivität, um ein JavaScript-Codefragment im Kontext eines Workflows auszuführen. [Weitere Informationen](../workflows/activities/javascript-code.md)
* **Externes Signal** - Verwenden Sie diese Aktivität, um die Ausführung eines Workflows aus einem anderen Workflow oder einem API-Aufruf Trigger. [Weitere Informationen](../workflows/activities/external-signal.md)
* **Inkrementelle Abfrage** - Verwenden Sie diese Aktivität, um die Datenbank auf geplanter Basis abzufragen. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Auf diese Weise können Sie nur neue Elemente ansprechen. [Weitere Informationen](../workflows/activities/incremental-query.md)

**Vorlagen für Rich-Push-Benachrichtigungen**

Sie können jetzt Rich-Push-Benachrichtigungen über Android senden. Rich-Push-Benachrichtigungen sind eine erweiterte Form von Mobile-Benachrichtigungen, die über einfache Textnachrichten hinausgehen und Multimedia-Elemente wie Bilder, interaktive Schaltflächen oder andere Rich-Media-Inhalte enthalten. [Weitere Informationen](../push/rich-push.md)

Beachten Sie, dass diese Funktion **Eingeschränkte Verfügbarkeit** (LA).

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### Neue Funktionen in begrenzter Verfügbarkeit {#acs-24-4}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind in der eingeschränkten Verfügbarkeit (LA) verfügbar. Sie sind auf Kunden beschränkt, die migrieren **von Adobe Campaign Standard nach Adobe Campaign v8** und können nicht in einer anderen Umgebung bereitgestellt werden.
>
>Weitere Informationen finden Sie auf den folgenden Dokumentationsseiten: [Umstellung der Campaign Standard auf Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Branding** - Als Campaign Standard migrierte Benutzer können Ihre technischen Administratoren jetzt eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Markenidentität auswirken. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Sie können diese Marken erstellen und mit Nachrichten oder Landingpages verknüpfen. Diese Konfiguration wird in Vorlagen verwaltet. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest-APIs** - Als Campaign Standard migrierter Benutzer können Sie REST-APIs verwenden, um Integrationen für Adobe Campaign zu erstellen und Ihr eigenes Ökosystem zu erstellen, indem Sie Adobe Campaign mit dem von Ihnen verwendeten Technologiebereich verbinden. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Dynamische Berichterstellung** - Als Campaign Standard migrierter Benutzer können Sie auf die dynamische Berichterstellung zugreifen, die vollständig anpassbare und in Echtzeit aktualisierte Berichte zur Messung der Wirkung Ihrer Marketingaktivitäten bietet. Durch sie kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Stadt und Alter sowie nach Daten von E-Mail-Kampagnen wie Öffnungen und Klicks ermöglicht. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Verbesserung der Aktivität &quot;Datei laden&quot;** - die **Datei laden** Die -Aktivität wurde um mehrere Abschnitte erweitert, in denen Sie eine Beispieldatei hochladen, Fehler und Zurückweisungen verwalten sowie hochgeladene Dateien nach der Ausführung der Aktivität löschen können. [Weitere Informationen](../workflows/activities/load-file.md)

* **Landing Pages** - Die folgenden Verbesserungen an Landingpages sind nur für Benutzer verfügbar, die von Campaign Standard aus wechseln:

   * Sie können jetzt beim Konfigurieren eines Dienstes auf eine standardmäßige Anmelde-/Abmelde-Landingpage verweisen. Wenn Sie bei der Erstellung einer E-Mail einen Link zu dieser Landingpage definieren, werden die Benutzer, die das Landingpage-Formular senden, automatisch für diesen Dienst angemeldet oder von ihm abgemeldet. [Weitere Informationen](../audience/manage-services.md#create-service)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht anonymen Besuchern den Zugriff auf die Landingpage. Wenn Sie diese Option deaktivieren, können nur identifizierte Benutzer auf das Formular zugreifen und es senden. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht die Speicherung zusätzlicher interner Daten beim Senden der Landingpage. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option ermöglicht die Verwendung einer Landingpage für mehrere Dienste, wodurch sie dynamisch wird. Wenn Sie einen Link zu einer E-Mail hinzufügen und eine dynamische Landingpage auswählen, können Sie einen beliebigen Dienst auswählen. Wenn Sie eine Landingpage auswählen, der ein bestimmter Dienst zugeordnet ist, wird dieser Dienst automatisch verwendet (Sie können keinen anderen Dienst auswählen). [Weitere Informationen](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Bedingte Inhalte werden jetzt auf Landingpages unterstützt. [Weitere Informationen](../landing-pages/lp-content.md)

### Allgemeine Verbesserungen {#improvements-24-4}

Die folgenden Verbesserungen stehen allen Kunden ab der April-Version zur Verfügung.
<!--**Workflow - Copy/Paste into another tab**: -->

* Jetzt können Sie Aktivitäten von einem Workflow in einen anderen Workflow über eine andere Browser-Registerkarte kopieren/einfügen. [Weitere Informationen](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Alle Workflow-Aktivitäten können jetzt ihre Ausführungsoptionen verwalten. Auf diese Weise können Sie den Ausführungsmodus und das Verhalten der Aktivität im Fall von Fehlern definieren. [Weitere Informationen](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* Die Option &quot;Bei leerer Population die Transition nicht aktivieren&quot; im **Aufspaltung** Sie können auswählen, ob der Workflow zur nächsten Aktivität übergehen soll, wenn das Segmentergebnis leer ist. [Weitere Informationen](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* Benutzerdefinierte Felder sind zusätzliche Attribute, die den nativen Schemas über die Adobe Campaign-Konsole hinzugefügt werden. In der Web-Benutzeroberfläche von Campaign sind diese benutzerdefinierten Felder jetzt in verschiedenen Bildschirmen sichtbar, z. B. in den Details eines Profils oder eines Testprofils. In der Web-Benutzeroberfläche können Sie keine benutzerdefinierten Felder erstellen, aber jetzt können Sie die Anzeige ändern. [Weitere Informationen](../administration/custom-fields.md)


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

Sie können jetzt die **Alle Teilmengen in derselben Tabelle generieren** in der **Aufspaltung** Workflow-Aktivität, um alle Teilmengen in einer ausgehenden Transition zusammenzufassen.

### Abfrage-Modeler {#24-3-query-modeler}

* Das Abfragemodell ist jetzt im E-Mail-Designer verfügbar. Damit können Sie Bedingungen beim Erstellen bedingter Inhalte erstellen.
* Beim Erstellen einer benutzerdefinierten Bedingung sind jetzt vordefinierte Werte für Attribute vom Typ Datum verfügbar.
* Operatoren können nicht mehr zu einer neuen Transition im Diagramm hinzugefügt werden. Sie können nur für eine bestehende Transition hinzugefügt werden, bevor Komponenten gefiltert werden, um sie zu gruppieren.
