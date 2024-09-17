---
title: Erste Schritte mit Adobe Campaign v8 für Admins und Entwicklerinnen und Entwickler.
description: Dieses Tutorial bietet einen Überblick über die wichtigsten Verwaltungs- und Daten-Management-Funktionen von Campaign v8. Es richtet sich an Admins und technische Marketing-Fachleute, die von Campaign Standard zu Campaign v8 migrieren.
role: Admin, Developer
level: Beginner, Experienced
source-git-commit: 271fb8805e046c20fad824ba37b84be43638011a
workflow-type: tm+mt
source-wordcount: '2666'
ht-degree: 16%

---


# Erste Schritte für Admin und Entwickler {#acs-gs-admin}

Auf dieser Seite erhalten Sie einen Überblick über die wichtigsten Verwaltungs- und Datenverwaltungsfunktionen von Campaign v8. Es richtet sich an Administratoren und technische Marketingexperten, die von Campaign Standard auf Campaign v8 umsteigen.

Die wichtigste Änderung für Sie ist die Einführung der Clientkonsole, der nativen Anwendung, die mit dem Adobe Campaign-Anwendungsserver kommuniziert.

Die Campaign-Client-Konsole zentralisiert alle Funktionen und Einstellungen. Sie wird mit der Campaign-Webbenutzeroberfläche synchronisiert, um eine konsistente Darstellung in beiden Umgebungen zu gewährleisten.

![](assets/client_console.png){zoomable="yes"}

[Erfahren Sie mehr über die Clientkonsole-Benutzeroberfläche von Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"} .

## Architektur von Campaign v8 {#acs-gs-admi-archi}

Die Kampagnenarchitektur wird im Handbuch von Campaign v8 (Konsole) beschrieben. Grundlegende Informationen finden Sie auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"} .

Nützlicher Link zum Starten:

* Adobe Campaign-Komponenten und die globale Architektur werden auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"} beschrieben.

* Unter [Erste Schritte mit der Campaign-Architektur](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} finden Sie Informationen zur Campaign-Architektur, bevor Sie mit der Strukturierung Ihrer Instanz beginnen.

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* Transaktionsnachrichten (Message Center) ist das Campaign v8-Modul zur Verwaltung ausgelöster Nachrichten. Sie beruht auf einem bestimmten Architekturmodell, das in [diesem Abschnitt](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"} beschrieben wird.

## Campaign-Clientkonsole {#acs-gs-console}

### Installieren der Client-Konsole {#acs-gs-admin-console}

Administrations- und Konfigurationsaufgaben werden in der Clientkonsole ausgeführt. Der erste Schritt besteht darin, Ihre Umgebung einzurichten.

Die Campaign-Clientkonsole ist eine native Anwendung, die über standardmäßige Internetprotokolle wie SOAP und HTTP mit dem Adobe Campaign-Anwendungsserver kommuniziert. In der Campaign Client-Konsole sind alle Funktionen und Einstellungen verfügbar. Sie erfordert eine minimale Bandbreite, da sie auf einem lokalen Cache beruht. Die Campaign-Clientkonsole wurde für eine einfache Bereitstellung konzipiert und kann über einen Internetbrowser bereitgestellt werden. Sie wird automatisch aktualisiert und erfordert keine spezielle Netzwerkkonfiguration, da sie nur HTTP(S)-Traffic generiert.

Das folgende Video erklärt, wie Sie die Adobe Campaign-Client-Konsole herunterladen und installieren und wie Sie die Verbindung zu Ihrer Instanz verwalten.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie unter [Herstellen einer Verbindung mit Campaign über die Client-Konsole](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/new/connect){target="_blank"}.

Beachten Sie, dass die Client-Konsole in einer unterstützten Umgebung installiert werden muss. Weitere Informationen finden Sie in der Kompatibilitätsmatrix ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"} der Campaign v8 (Konsole).[

### Entdecken Sie die Benutzeroberfläche der Clientkonsole  {#acs-gs-ui}

In diesem Tutorial-Video erfahren Sie über die Benutzeroberfläche von Adobe Campaign V8 und wie Sie in den Hauptfunktionen navigieren.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie unter [Arbeiten mit der Clientkonsole](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} .

## Umgebung verwalten {#acs-gs-admin-env}

Nachdem die Client-Konsole installiert wurde, führen Sie die Schritte in dieser Dokumentation aus, um die Verbindung zum Anwendungsserver herzustellen: [Verbindung zur Dokumentation zum Anwendungsserver](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}.

Sicherheitspraktiken sind tief in unsere internen Softwareentwicklungs- und Betriebsprozesse und -werkzeuge eingebunden und werden von unseren funktionsübergreifenden Teams streng befolgt, um Vorfälle auf angemessene Weise zu verhindern, zu erkennen und darauf zu reagieren. Weitere Informationen finden Sie unter [Best Practices für die Sicherheit von Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

### Zugriffsberechtigungen und Berechtigungen {#acs-gs-admin-rights}

Mit Adobe Campaign können Sie die den Benutzern zugewiesenen Rechte definieren und verwalten. Diese Berechtigungen werden durch die Kombination von Benutzergruppenberechtigungen, spezifischen Berechtigungen und Berechtigungen für Ordner definiert.

Wenn ein Campaign Standard zu Campaign v8 wechselt, bleiben Ihre Berechtigungen und Zugriffsberechtigungen gleich. Sicherheitsgruppen wurden durch Adobe in die Benutzergruppen von Campaign v8 verschoben, und Ihre Berechtigungen für Organisationseinheiten wurden auf Ordnerberechtigungen umgestellt. Campaign-Benutzer   Verwenden Sie ihre Adobe ID, um eine Verbindung zu Campaign v8 herzustellen, und können dann dieselben Anmelde- und Kennwortdaten wie in Campaign Standard verwenden.

Campaign [folders](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} sind Knoten im Explorer-Baum der Clientkonsole. Je nach Typ enthalten sie bestimmte Datentypen. Programme werden durch Ordner in Campaign v8 materialisiert. Sie können Ordner erstellen und Berechtigungen für sie verwalten, um den Zugriff zu beschränken. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Weitere Informationen finden Sie in der Dokumentation zu [Benutzerberechtigungen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"} .


### Campaign Control Panel {#acs-gs-admin-cp}

Campaign Standard: Sie können das Control Panel verwenden, um Ihre Umgebung zu verwalten. Beachten Sie, dass das Control Panel für v8 zusätzliche Funktionen bietet.

Das Campaign Control Panel ermöglicht Produktadministratoren von Adobe Campaign effizienteres Arbeiten. Sie können damit die Einstellungen aller Instanzen verwalten und deren Nutzung erfassen. Dank der intuitiven Benutzeroberfläche können die Nutzung wichtiger Assets überwacht und administrative Aufgaben einfach durchgeführt werden. So können beispielsweise IP-Adressen auf die Zulassungsliste gesetzt, der Speicher von SFTP-Servern überwacht und die Schlüssel verwaltet werden.

Weitere Informationen finden Sie in den [Tutorials zum Control Panel](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} und in der [Dokumentation zum Control Panel](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=de){target="_blank"}.

* **IP-Adressen hinzufügen** - Mit dem Campaign Control Panel können Sie neue Verbindungen zu Ihren Instanzen einrichten, indem Sie IP-Adressbereiche zur Zulassungsliste hinzufügen. Weitere Informationen finden Sie in der Dokumentation zur [IP-Zulassungsauflistung](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"} .

* **Subdomain-Konfiguration** - Sie können einen Unterabschnitt Ihrer Domäne (technisch eine &quot;DNS-Zone&quot;) für die Verwendung mit Adobe Campaign konfigurieren.
Weitere Informationen finden Sie in der Dokumentation zur [Subdomain-Zuweisung](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"} .

* **SFTP-Server verwalten** - Im Control Panel können Sie mit allen SFTP-Servern interagieren, die mit Campaign-Instanzen verbunden sind, auf die Sie Zugriff haben. Weitere Informationen finden Sie in der [Dokumentation zur SFTP-Verwaltung](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Audit-Protokoll {#acs-gs-admin-audit-trail}

Wie bereits in Campaign Standard verfügbar, kann das Audit-Protokoll in Campaign v8 verwendet werden, um auf den vollständigen Verlauf der in Ihrer Instanz vorgenommenen Änderungen zuzugreifen.

In der Adobe Campaign-Webbenutzeroberfläche bietet die Funktion &quot;Audit-Protokoll&quot;den Benutzern vollständige Einsicht in alle Änderungen, die an wichtigen Entitäten in Ihrer Instanz vorgenommen wurden. Dies sind in der Regel Änderungen, die einen reibungslosen Betrieb der Instanz erheblich beeinträchtigen. Weitere Informationen finden Sie in der Dokumentation zum [Audit-Protokoll](../../v8/reporting/audit-trail.md) .

### Daten-Packages {#acs-gs-admin-audit-packages}

Ähnlich wie in Campaign Standard können Administratoren Pakete definieren, um Ressourcen zwischen verschiedenen Adobe Campaign-Instanzen über strukturierte XML-Dateien auszutauschen. Packages können Konfigurationsparameter oder Daten enthalten.

Sie können Daten-Packages verwenden, um benutzerdefinierte Plattformeinstellungen und -daten zu exportieren und zu importieren. Ein Paket kann verschiedene Arten von Konfigurationen und Komponenten enthalten, gefiltert oder nicht. In [dieser Dokumentation](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/developer/packages){target="_blank"} erfahren Sie, wie Sie mit Datenpackages in Campaign v8 arbeiten.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### Benutzeroberfläche personalisieren {#acs-gs-admin-ui}

Es stehen verschiedene Optionen zum Anpassen der Benutzeroberfläche in der Clientkonsole zur Verfügung, z. B.:

* **Listen- und Datenanzeige** - Richtlinien zum Verwalten von Benutzeroberflächeneinstellungen wie Listen, Einheiten oder Datenanzeige finden Sie in diesem Dokument: [Dokumentation zu Benutzeroberflächeneinstellungen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **Ordnerverwaltung** - Ordner sind Objekte in Adobe Campaign, mit denen Sie Ihre Komponenten und Daten organisieren können. Sie werden auch zur Verwaltung von Berechtigungen verwendet. Erfahren Sie, wie Sie [mit Ordnern arbeiten](../../v8/get-started/work-with-folders.md).

* **Benutzerdefinierte Felder** - Benutzerdefinierte Felder sind zusätzliche Attribute, die den nativen Schemas über die Adobe Campaign-Konsole hinzugefügt werden. Diese benutzerdefinierten Felder werden in verschiedenen Bildschirmen angezeigt, beispielsweise in den Details eines Profils oder eines Testprofils. Weitere Informationen finden Sie in der Dokumentation zur Konfiguration von [benutzerdefinierten Feldern](../../v8/administration/custom-fields.md).

## Branding konfigurieren {#acs-gs-admin-branding}

Jedes Unternehmen verfügt über Markenrichtlinien, die sowohl visuelle Elemente als auch technische Details definieren. Was Adobe Campaign Standard angeht, hilft Ihnen Adobe Campaign v8 bei der zentralen Verwaltung dieser Richtlinien, sodass Sie Ihren Kunden ein konsistentes Markenbild präsentieren können - von Logos in E-Mails bis hin zu den URLs und Domänen, die in Ihren Kampagnen verwendet werden. Als technischer Administrator können Sie mehrere Marken in Adobe Campaign erstellen und verwalten.

Weitere Informationen finden Sie in der [Branding-Dokumentation](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} .

## Grundlagen zur Erstellung von Datenmodellen {#acs-gs-admin-data-model-creation}

Ähnlich wie Campaign Standard enthält Adobe Campaign v8 das vordefinierte Datenmodell. Adobe Campaign stützt sich auf eine Cloud-Datenbank mit Tabellen, die verknüpft sind. Weitere Informationen finden Sie in der [Dokumentation zum Datenmodell](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"} .

Ein Schema ist ein mit einer Datenbanktabelle verknüpftes XML-Dokument. Es definiert die Datenstruktur und beschreibt die SQL-Definition der Tabelle. Weitere Informationen finden Sie in der Dokumentation zur Erstellung von [Schemas](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

In diesem Video erfahren Sie, wie Sie ein Schema erstellen und ein vorhandenes Schema in Campaign v8 erweitern:

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Ähnlich wie bei den in Campaign Standard verfügbaren Funktionen können Sie auch benutzerdefinierte Ressourcen erstellen. In Campaign v8 sind benutzerdefinierte Ressourcen benutzerdefinierte oder erweiterte **Schemas**.

* Erfahren Sie, wie Sie mit Schema in [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"} arbeiten.

* Erfahren Sie, wie Sie ein vorhandenes Schema auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"} erweitern.

* Erfahren Sie, wie Sie auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"} ein neues Schema erstellen.

* Wenn Sie ein Schema erstellen oder erweitern, müssen Sie die zugehörigen Eingabeformulare erstellen oder ändern, damit diese Änderungen für Endbenutzer sichtbar sind. Mit einem Formular können Sie eine Instanz, die mit einem Datenschema verknüpft ist, über die Adobe Campaign-Client-Konsole bearbeiten. Das Formular wird anhand seines Namens und Namespace identifiziert. Weitere Informationen finden Sie in der Dokumentation zur Erstellung von [Eingabeformularen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Workflows und Datenverwaltung {#acs-gs-admin-data-management}

Wie bei Adobe Campaign Standard umfasst Adobe Campaign v8 ein Workflow-Modul, mit dem Sie das gesamte Spektrum an Prozessen und Aufgaben auf den verschiedenen Modulen des Anwendungsservers koordinieren können. In dieser vielseitigen grafischen Umgebung können Sie Prozesse erstellen, wie etwa die Segmentierung, die Kampagnenausführung, die Dateiverarbeitung und den Eingriff durch Personen. Die Workflow-Engine führt diese Prozesse aus und verfolgt sie. Erfahren Sie in [dieser Dokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"} , wie Sie mit Workflows in Campaign v8 beginnen.

Siehe Links zu anderen nützlichen Ressourcen unten:

* In diesem Video erfahren Sie, was Zielgruppendimensionen und Arbeitstabellen sind und wie Adobe Campaign Daten aus verschiedenen Datenquellen verwaltet:

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Mit Campaign können Sie der Cloud-Datenbank Kontakte hinzufügen. Sie können eine Datei laden, mehrere Kontaktaktualisierungen planen und automatisieren, Daten im Web erfassen oder Profilinformationen direkt in die Empfängertabelle eingeben.  Weitere Informationen finden Sie in der Dokumentation zum [Importieren von Daten (Konsole)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}.

* Sie können Ihre verschiedenen Berichte einfach in das PDF- oder CSV-Format exportieren, sodass Sie sie freigeben, bearbeiten oder drucken können. Weitere Informationen finden Sie in der [Dokumentation zum Exportieren von Daten](../../v8/reporting/export-reports.md).

## REST APIs {#acs-gs-admin-apis}

Mit Campaign REST-APIs können Sie Integrationen für Adobe Campaign erstellen und Ihr eigenes Ökosystem einrichten, indem Sie Adobe Campaign mit den von Ihnen verwendeten Technologien verbinden.

Als Campaign Standard, der zu Campaign v8 wechselt, stehen Ihnen REST-APIs zur Verfügung.

Weitere Informationen finden Sie in der Dokumentation zur REST-API](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"} .[

Beachten Sie, dass bei der Umstellung von Campaign Standard auf Campaign v8 einige Empfehlungen und Einschränkungen für REST-APIs gelten. Sie werden auf [dieser Seite](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"} aufgelistet. Für die Umstellung auf Campaign v8 gelten spezifische Einschränkungen, wie im unten stehenden Hinweis zur Verfügbarkeit aufgeführt:

>[!AVAILABILITY]
>
>* Die PKEYs-Werte ändern sich zwischen der vorhandenen Campaign Standard-Instanz und der migrierten Campaign v8-Instanz. Falls PKEYs in einer externen Datenbank gespeichert werden, muss sich die Implementierung so ändern, dass sie die Adobe Campaign v8-Haupt-APIs aufrufen müssen, die Pkeys/href-Links mit PKEYs und nachfolgenden API-Aufrufen bereitstellen, indem die Pkeys /href aus vorherigen API-Aufrufen dynamisch gebildet werden &#x200B;
>
>* In Campaign v8 ist die Eigenschaft firstName für denselben Hauptteil, für den das Fahrzeug mit einem Profil verknüpft ist, &#x200B; eine Fehlereigenschaft firstName für `cusVehicle` nicht gültig, aber ein Anfragetext mit nur den Attributen ohne Link funktioniert einwandfrei. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* Die Zeitzone wird dem Benutzer im Rahmen des REST-API-Aufrufs `profileAndServicesExt/profile` und nicht des Aufrufs der REST-API `profileAndServices/profile` angezeigt, da sie im Rahmen der Datenmigration in einem erweiterten Schema hinzugefügt wird&#x200B;
>
>* Der `ccpaOptOut` wird dem Benutzer nur im Rahmen des `profileAndServicesExt/profile` REST-API-Aufrufs und nicht im `profileAndServices/profile` REST-API-Aufruf angezeigt, da er im Rahmen der Datenmigration in einem erweiterten Schema hinzugefügt wird.
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## Anmeldedienste {#acs-gs-admin-sub}

Wie in Campaign Standard können Sie als Administrator Abonnementdienste erstellen und Marketing-Experten können Nachrichten an ihre Abonnenten senden. Die wichtigsten Konzepte und Implementierungsschritte sind mit dem Campaign Standard abgestimmt. Unten finden Sie nützliche Links und Videos.

Erfahren Sie, wie Sie Anmeldungen und Abonnements einrichten und verwalten und Zielgruppen adressieren.

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* Weitere Informationen finden Sie in der Dokumentation zur Web-Benutzeroberfläche für Abonnements [1](../../v8/audience/manage-subscribers.md).

* Weitere Informationen finden Sie in der Dokumentation zum Einrichten von Abonnementdiensten in der Clientkonsole in [diesem Abschnitt](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"} .

## Nachrichten und Sendungen{#acs-gs-msg}

### Konfigurieren von Versandkanälen {#acs-gs-admin-channels}

Als Campaign Standard unterstützt Adobe Campaign v8 den Versand kanalübergreifender Kampagnen, einschließlich E-Mails, SMS, Push-Benachrichtigungen und Briefpost, sowie die Messung ihrer Effektivität mithilfe diverser Berichte. Diese Nachrichten werden mittels Sendungen entworfen und gesendet und können für jede Empfängerin und jeden Empfänger personalisiert werden. Zu den Kernfunktionen zählen Zielgruppenbestimmung, Definition und Personalisierung von Nachrichten, Ausführung der Kommunikation und die damit verbundenen operativen Berichte. Der wichtigste funktionale Zugangspunkt ist der Versandassistent. Dieser Zugriffspunkt führt zu mehreren Funktionen, die von Adobe Campaign abgedeckt werden.

Als Administrator müssen Sie Ihre Kanalkonfigurationen definieren. Weitere Informationen finden Sie unter den unten stehenden Links.

* **E-Mail** - Die E-Mail-Einstellungen werden alle auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"} beschrieben.
* **SMS** - Erfahren Sie in [dieser Dokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}, wie Sie Ihren SMS-Kanal konfigurieren.
* **Push-Benachrichtigungen** - Die Schritte zum Konfigurieren des Push-Benachrichtigungskanals werden [in diesem Abschnitt](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"} beschrieben.
* **Transaktionsnachrichten** - Schritte zum Konfigurieren von [Transaktionsnachrichten](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} in Campaign v8 werden in diesem Abschnitt [beschrieben.](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### Externe Konten {#acs-gs-ext-accounts}

Als Administrator sind Sie für die Konfiguration und Verwaltung externer Campaign-Konten verantwortlich. Wie im Campaign Standard werden externe Konten von technischen Prozessen wie technischen Workflows oder Kampagnen-Workflows verwendet.

Der Übergangsprozess zu Campaign v8 übernimmt die von Ihnen existierenden externen Campaign Standard-Konten. Diese sind jetzt in der Clientkonsole verfügbar.

Erfahren Sie mehr über die Konfiguration des [externen Kontos](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/config/configuration/external-accounts){target="_blank"}.


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### Dynamischer Inhalt {#acs-gs-dyn-content}

Verwenden Sie Campaign, um dynamische Inhalte zu erstellen und personalisierte Nachrichten zu versenden. Personalisierungsfunktionen können kombiniert werden, um Ihre Nachrichten zu verbessern und ein individuelles Benutzererlebnis zu schaffen.

Mit Campaign v8 können Sie als Administrator in diesem Video dynamische Inhaltsbausteine definieren und festlegen, wie diese zur Personalisierung des Inhalts Ihres E-Mail-Versands verwendet werden können:

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

Nützliche Links:

* [Erste Schritte mit der Personalisierung](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [Verwenden Sie Gestaltungsbausteine](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [Bedingten Inhalt erstellen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [Personalization-Datenquellen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### Versandvorlagen {#acs-gs-templates}

Die Verwendung von Versandvorlagen ist in Campaign v8 wie in Campaign Standard eine Voraussetzung.

Erstellen Sie Versandvorlagen, um Ihren Entwurf zu beschleunigen und zu verbessern, damit Sie benutzerdefinierte Inhalte und Einstellungen in allen Ihren Kampagnen einfach wiederverwenden können. Mit dieser Funktion können Sie das kreative Erscheinungsbild standardisieren, um Kampagnen schneller ausführen und starten zu können. Erfahren Sie, wie Sie in der Campaign-Web-Benutzeroberfläche ](../../v8/msg/delivery-template.md) Versandvorlagen erstellen. [ Siehe auch Erstellen von Versandvorlagen in der Clientkonsole in [diesem Abschnitt](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/create-templates){target="_blank"}.

### Typologieregeln {#acs-gs-admin-rules}

Als Administrator sind Sie für die Erstellung und Verwaltung von Typologieregeln für Ihre Sendungen verantwortlich. Wie in Adobe Campaign Standard sind Typologieregeln in Campaign v8 Geschäftsregeln, mit denen Sie vor dem Versand eine Prüfung und Filterung Ihrer Nachricht durchführen können.

Beim Übergang von einer Campaign Standard-Umgebung zu Campaign v8 werden Ihre Typologieregeln nach Campaign v8 verschoben.

In Campaign v8 verfügen Typologieregeln über einen speziellen Kampagnenoptimierungs-Modus. Dieses Modul ermöglicht die Kontrolle, Filterung und Überwachung des Versands von Sendungen. Um Konflikte zwischen Kampagnen zu vermeiden, kann Adobe Campaign verschiedene Kombinationen durch Anwendung spezifischer Beschränkungsregeln testen. Dadurch wird sichergestellt, dass die gesendeten Nachrichten den Anforderungen und Erwartungen der Kunden und den Kommunikationspolitiken des Unternehmens entsprechen. Weitere Informationen finden Sie in der Dokumentation zu [Typologieregeln](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"} .

### Quarantäneverwaltung {#acs-gs-admin-quarantine}

Alle unter Quarantäne gestellten Adressen und Quarantäneregeln wurden von Ihrer Campaign Standard-Umgebung auf Campaign v8 migriert. Für die Quarantäneverwaltung ist keine spezifische Aktion erforderlich.

Als Administrator sollten Sie sich mit der Quarantäneverwaltung in Campaign v8 vertraut machen, beginnend mit [dieser Seite](../../v8/audience/quarantine.md). Weitere Informationen zur Quarantäneverwaltung finden Sie in der ausführlichen Dokumentation der Clientkonsole in [diesem Abschnitt](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"} .


## Verwalten von Adobe Campaign-Integrationen {#acs-gs-integrations}

Sie können Ihre Campaign-Instanz mit Adobe Experience Cloud-Lösungen verbinden, um Funktionen zu kombinieren. Adobe Campaign verfügt über mehrere Connectoren, über die Sie mit externen Programmen kommunizieren, eine Verbindung zu Datenbank-Engines herstellen sowie Daten freigeben und synchronisieren können. Erfahren Sie, wie Sie Ihre Lösungen in [dieser Dokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"} kombinieren.

Als Campaign Standard, der zu Campaign v8 migriert, gilt Folgendes:

* Wenn Sie diese Integrationen mit Campaign Standard verwendet haben, wurden Ihre **Adobe Analytics** - und **Audience Manager** -Konfigurationen und -Daten vom Adobe migriert.
* Wenn Ihre Campaign Standard-Umgebung in **Adobe Experience Manager** integriert wurde, empfiehlt Adobe, zu **Adobe Experience Manager as a Cloud Service** zu wechseln, damit Sie diese Funktion beim Erstellen von E-Mails in der Campaign-Webbenutzeroberfläche verwenden und die optimierte Verwaltung von E-Mail-Versandinhalten und -Formularen direkt in Ihrer Adobe Experience Manager-Umgebung erleichtern können. Weitere Informationen finden Sie auf [dieser Seite](../../v8/integrations/aem-content.md).
Beachten Sie, dass Campaign auch in Adobe Experience Manager 6.5 integriert werden kann. Informationen zum Konfigurieren dieser Integration finden Sie in [dieser Dokumentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}.
* Wenn Ihre Campaign Standard-Umgebung in **Trigger** integriert wurde, müssen Sie diese Integration in Campaign v8 einrichten und konfigurieren, wie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"} beschrieben.
* Wenn Ihre Campaign Standard-Umgebung in **Adobe Target** integriert wurde, müssen Sie diese Integration in Campaign v8 einrichten und konfigurieren, wie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/connect/ac-at){target="_blank"} beschrieben.

