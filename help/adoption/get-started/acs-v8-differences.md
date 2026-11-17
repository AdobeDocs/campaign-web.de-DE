---
title: Unterschiede zwischen Campaign Standard und Campaign v8
description: Erfahren Sie, welche Änderungen sich beim Wechsel von Campaign Standard zu Campaign v8 ergeben und wo Sie die Details finden
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 64a07e65b7e6d933288b10117aae99f48d13a8d8
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 2%
---
# Unterschiede zwischen Campaign Standard und Campaign v8 {#acs-v8-differences}

Die meisten Konzepte sind in Campaign Standard und Campaign v8 identisch. Auf dieser Seite werden die Unterschiede erfasst, die sich nach der Umstellung auf Sie auswirken, sowie Links zu der jeweiligen Seite, auf der die einzelnen Unterschiede erläutert werden. Es ergänzt die Handbücher für [Marketer](marketers.md) und für [Administratoren und Entwickler](admin-developers.md).

* Informationen zu den terminologischen Änderungen finden Sie unter [Wichtige Unterschiede zwischen Campaign Standard und Campaign v8](overview.md#experiences).
* Informationen zu den auszuführenden Prüfungen und den nach einer Transition gemeldeten Problemen finden Sie unter [Prüfungen und Fehlerbehebung nach der Transition](post-transition-checks.md).
* Die Funktionen, die nur in der Client-Konsole verfügbar sind, finden Sie unter [Campaign Web- und Campaign-Client-Konsole](../../v8/get-started/capability-matrix.md).

## Kanäle und Inhalte {#channels}

Die Schritte zum Erstellen und Senden von Nachrichten sind in beiden Produkten ähnlich, wie in der [ für Marketing-Fachleute ](marketers.md). Die folgenden Unterschiede betreffen die Verfügbarkeit von Kanälen, Testsendungen, Landingpages und Briefpost-Workflows.

| Änderungen | Weitere Informationen |
|---|---|
| Der In-App-Kanal ist in Campaign v8 nicht verfügbar. | [In-App-Kanal](marketers.md#acs-gs-marketers-in-app) |
| Wenden Sie sich an Ihren Adobe Campaign Transition Manager, um bestehende Push-Workflows und -Sendungen zu übergeben. | [Push-Benachrichtigungen ](marketers.md#acs-gs-marketers-push) |
| In Campaign Standard kann ein Testprofil als „Falle **markiert werden,** den endgültigen Versand zu erhalten. Fügen Sie in Campaign v8 eine **Trap-Gruppe** in den Zielgruppeneinstellungen des Versands hinzu. | [Trap-Gruppe](../../v8/audience/trap-group.md) |
| In der Web-Benutzeroberfläche von Campaign erstellte Landingpages unterstützen keine ausgeblendeten Eingabefelder oder benutzerdefinierten JavaScript. | [Landingpages ](../../v8/landing-pages/get-started-lp.md) |
| In Campaign Standard wird die generierte Datei auch bei der ausgehenden Transition einer Briefpost-Aktivität übernommen. In Campaign v8 wird nur die Zielpopulation übermittelt. Um die Datei an einen Server zu senden, fügen Sie die Aktivität **Datenextraktion** und dann die Aktivität **Dateiübertragung** hinzu. | [Briefpost](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Audiences, Workflows und Sendungen {#data-and-workflows}

Diese Unterschiede betreffen die aus Campaign Standard migrierten Audiences und Workflows, einige Optionen für wiederkehrende Sendungen und die Aktivität **Dateiübertragung** sowie den Umfang der dynamischen Berichterstellung.

| Änderungen | Weitere Informationen |
|---|---|
| Zielgruppen werden während der Transition transformiert. Beispielsweise werden Zielgruppen, die mit der Abfrage -Aktivität erstellt werden, zu vordefinierten Filtern und Dateityp-Zielgruppen zu Listentyp-Zielgruppen ohne Dimensionen. | [Verwalten von Zielgruppen](marketers.md#acs-gs-marketers-audiences) |
| Verlaufsprotokolle der in Campaign Standard ausgeführten Workflows werden nicht migriert. | [Erstellen eines Workflows](marketers.md#acs-gs-marketers-wf) |
| In Campaign Standard können Sie den Aggregationszeitraum einer wiederkehrenden E-Mail auswählen. Diese Option ist in Campaign v8 nicht verfügbar. | [Kanalaktivitäten](../../v8/workflows/activities/channels.md) |
| Die dynamische Berichterstellung umfasst E-Mail-Sendungen, Kampagnen mit E-Mail-Sendungen und Transaktionsnachrichten. | [Reporting](marketers.md#acs-gs-marketers-reporting) |

## Zugriff und Sicherheit {#access}

Campaign Standard-Sicherheitsgruppen, -Rollen und -Organisationseinheiten sind während der Umstellung Benutzergruppen, spezifischen Berechtigungen und Ordnerberechtigungen zugeordnet. Beachten Sie die folgenden Punkte, insbesondere wenn einige Benutzer umfassendere oder engere Rechte als zuvor haben.

| Änderungen | Weitere Informationen |
|---|---|
| Sicherheitsgruppen, Rollen und Organisationseinheiten sind Benutzergruppen, spezifischen Berechtigungen und Ordnerberechtigungen zugeordnet. Benutzerdefinierte Rollen werden nicht migriert. | [Benutzerzugriffsverwaltung](user-management-acs.md) |
| Benutzende mit der Rolle **Datenmodell**, aber nicht mit der Rolle **Administration** erhalten Zugriff **Administration**. | [Benutzerzugriffsverwaltung](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Benutzende, die Sicherheitsgruppen mit parallelen Organisationseinheiten zugewiesen sind, können in Campaign v8 umfassenderen Zugriff erhalten. | [Parallele Zuweisung von Organisationseinheiten](user-management-acs.md#parallel-assignments) |
| Für den Zugriff auf Transaktions-APIs über die Ausführungsinstanz ist ein neues Produktprofil erforderlich. | [Produktprofilzuordnung](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Datenschutzanfragen können während des Zeitraums, in dem Ihre Campaign Standard-Umgebung aktiv bleibt, sowohl in Campaign Standard als auch in Campaign v8 eingehen. | [Datenschutz und Einverständnis](admin-developers.md#privacy-and-consent) |

## APIs und Integrationen {#apis-and-integrations}

Diese Unterschiede betreffen die Integrationen, die Campaign über die REST-API aufrufen, sowie die Integrationen mit anderen Adobe-Lösungen und -Tools.

| Änderungen | Weitere Informationen |
|---|---|
| PKEY-Werte ändern sich nach der Migration. Wenn Sie PKEYs außerhalb von Campaign speichern, befolgen Sie stattdessen die von der API zurückgegebenen. | [Verwendung von Schlüsseln](#key-usage) |
| Einige migrierte Profilfelder, wie Zeitzone und `ccpaOptOut`, werden nur von der `profileAndServicesExt/profile`-API zurückgegeben. | [Zeitzone des Profils](#profile-timezone) |
| Adobe migriert Ihre Adobe Analytics- und Audience Manager-Konfigurationen. Sie müssen die Trigger- und Adobe Target-Integrationen erneut einrichten. | [Verwalten von Adobe Campaign-Integrationen](admin-developers.md#acs-gs-integrations) |

## Empfehlungen und Einschränkungen der REST-API {#rest-api-limitations}

Die folgenden Empfehlungen und Einschränkungen gelten für die REST-APIs, wenn Sie von Campaign Standard zu Campaign v8 wechseln.

### Berechtigungen und Sicherheit {#permissions}

#### Zuordnung von Produktprofilen {#rest-product-profiles}

In Campaign Standard wurde Ihnen erhöhte Administratorrolle Zugriff auf APIs gewährt, unabhängig von Ihrem zugewiesenen Produktprofil. Campaign v8 führt einen anderen Satz von Produktprofilen ein, für die eine Zuordnung von Campaign Standard zu Campaign v8-Produktprofilen erforderlich ist.

Bei der Migration werden zwei Produktprofile zu Ihren vorhandenen oder vorab erstellten technischen Konten hinzugefügt: Administrator und Message Center (für den Zugriff auf Transaktions-APIs). Überprüfen Sie die Produktprofilzuordnung und weisen Sie das erforderliche Produktprofil zu, wenn Sie nicht möchten, dass das Admin-Produktprofil Ihrem technischen Konto zugeordnet wird.

#### Mandantenkennung

Nach der Migration wird für alle zukünftigen Integrationen empfohlen, Ihre **Campaign v8-Mandanten-ID** in REST-URLs zu verwenden und Ihre vorherige Campaign Standard-Mandanten-ID zu ersetzen.

#### Verwendung von Schlüsseln

Die Verwaltung der PKey-Werte unterscheidet sich zwischen Campaign Standard und Campaign v8. Wenn Sie PKeys mit Campaign Standard gespeichert haben, stellen Sie sicher, dass Ihre Implementierung nachfolgende API-Aufrufe dynamisch durch PKeys oder aus vorherigen API-Aufrufen erstellt.

### Verfügbare APIs {#available-apis}

Vorerst sind die unten aufgeführten REST-APIs zur Verwendung verfügbar:

* **Profile**
* **Services und Abonnements**
* **Benutzerdefinierte Ressourcen**
* **Workflows**
* **Transaktionsnachrichten**

>[!AVAILABILITY]
>
>Derzeit ist die REST-API **Transaktionsnachrichten** nicht verfügbar.
>
>Die unten aufgeführten REST-APIs sind veraltet und nicht mehr verfügbar:
>* Marketing-Verlauf
>* Organisationseinheiten
>* Datenschutzverwaltung

### Filterung {#rest-filtering}

* Um Ihre Filter in den REST-API-Payloads zu verwenden, müssen Sie sie in Campaign v8 bearbeiten und einen Namen angeben, der in Ihren Payloads verwendet werden soll. Greifen Sie dazu über die Registerkarte **[!UICONTROL Parameter]** auf die zusätzlichen Parameter des Filters zu und geben Sie den gewünschten Namen im Feld **[!UICONTROL Filtername in REST-API]** an.

  ![](assets/api-filtering.png)


* Das Präfix „by“, das für die Verwendung benutzerdefinierter Filter erforderlich ist, wird nicht mehr benötigt. Der Filtername sollte in Ihren Anfragen unverändert verwendet werden.

  Beispiel:

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### Abgelegte Datenbankfelder {#dropped-fields}

Einige Felder aus der Datenbank werden während der Migration gelöscht. Bei Verwendung eines abgelegten Felds geben REST-APIs leere Werte zurück. In Zukunft werden alle abgelegten Felder veraltet sein und entfernt.

### POST mit verknüpften Ressourcen {#post-linked}

Bei Verwendung des folgenden Anfragetext-Formats, wobei „vehierOwner“ den Link zu „nms“ :recipient:

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

Die Link-Informationen werden ignoriert. Daher wird unter „cusVehicle“ ein neuer Datensatz generiert, der nur die Werte „vehicleNumber“ und „vehicleName“ enthält. Der Link bleibt jedoch null, was dazu führt, dass für „VehicleOwner“ „null“ festgelegt wird.

Wenn in Campaign v8 dieselbe Anfragekörperstruktur verwendet wird und das „Fahrzeug“ mit einem Profil verknüpft ist, tritt ein Fehler auf. Dieser Fehler tritt auf, weil die Eigenschaft „firstName“ für „cusVehicle“ nicht als gültig erkannt wird. Ein Anfragetext, der nur die Attribute ohne die Relation enthält, funktioniert jedoch problemlos.

### PATCH-Vorgänge {#patch}

* Campaign v8 unterstützt PATCH nicht mit einem leeren Anfrageinhalt: Der Status „Kein Inhalt“ wird 204 zurückgegeben.
* Campaign Standard unterstützt PATCH zwar für Elemente/Attribute innerhalb eines Schemas, doch beachten Sie, dass PATCH-Vorgänge vor Ort in Campaign v8 nicht unterstützt werden. Der Versuch, einen PATCH-Speicherort zu konfigurieren, führt zu einem internen 500-Server-Fehler mit einer Fehlermeldung, die angibt, dass die Eigenschaft „zipCode“ für die Ressource „profile“ nicht gültig ist.

### REST-Antworten {#rest-responses}

Im folgenden Abschnitt werden geringfügige Unterschiede zwischen REST-Antworten von Campaign Standard und v8 aufgeführt.

* Bei einzelnen GET-Einträgen enthält die Antwort die href in der Antwort.
* Bei der Abfrage mit dem -Attribut liefert Campaign v8 Anzahl und Paginierung in der Antwort.
* Nach POST-Vorgängen werden Werte aus verknüpften Ressourcen in der Antwort zurückgegeben.

### Fehlercodes und Meldungen {#rest-errors}

Im folgenden Abschnitt werden die Unterschiede zwischen Fehler-Codes und Fehlermeldungen von Campaign Standard und Campaign v8 aufgeführt.

| Szenario | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| Ungültigen PKey im Anfragetext verwenden | 500 - Attribut &#39;O5iRp40EGA&#39; unbekannt (siehe Definition des Schemas &#39;Profiles (nms:recipient)&#39;). XTK-170036 Ausdruck &#39;@id = @O5iRp40EGA&#39; kann nicht analysiert werden. | 404 - PKey kann nicht entschlüsselt werden. (PKey=@jksad) |
| Ungültigen PKey im URI verwenden | 500 - Attribut &#39;O5iRp40EGA&#39; unbekannt (siehe Definition des Schemas &#39;Profiles (nms:recipient)&#39;). XTK-170036 Ausdruck &#39;@id = @O5iRp40EGA&#39; kann nicht analysiert werden. | 404 - PKey kann nicht entschlüsselt werden. (PKey=@jksad) Nicht unterstützter Endpunkt. (endpoint=rest/profileAndServices/profile/@jksad) |
| Verwenden zweier verschiedener roher PKey im URI und Anfragetext | 500 - RST-360011 Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. Inkonsistenter RST-360012-Vorgang für Ressource „service“ - Schlüssel „SVC3“ kann nicht auf „SVC4“ aktualisiert werden. | 500 - Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. |
| Verwenden von PKey im URI und eines anderen rohen PKey im Anfragetext | 500 - Ein &#39;Dienst&#39; mit demselben Schlüssel &#39;SVC4&#39; ist bereits vorhanden. PGS-220000 PostgreSQL-Fehler: FEHLER: Doppelter Schlüsselwert verletzt eindeutige Einschränkung „nmsservice_name“ DETAIL: Schlüssel (sname)=(SVC4) existiert bereits. | 500 - Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. |
| Verwenden einer nicht vorhandenen Roh-ID im URI | 404 - RST-360011 Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. Dokument mit dem Pfad &#39;Service&#39; kann nicht ausgehend vom Schlüssel &#39;adobe_nl:0&#39; gefunden werden (Dokument mit Schema &#39;service&#39; und Namen &#39;adobe_nl&#39;) | 404 - Dokument mit dem Pfad &#39;Service&#39; kann nicht über den Schlüssel &#39;adobe_nl&#39; gefunden werden (Dokument mit dem Schema &#39;service&#39; und dem Namen &#39;adobe_nl&#39;) |
| Verwenden einer nicht vorhandenen Raw-ID im Anfrageinhalt | 404 - RST-360011 Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. Dokument mit dem Pfad &#39;Service&#39; kann nicht ausgehend vom Schlüssel &#39;adobe_nl&#39; gefunden werden (Dokument mit Schema &#39;service&#39; und Namen &#39;adobe_nl&#39;) | 404 - Dokument mit dem Pfad &#39;Service&#39; kann nicht über den Schlüssel &#39;adobe_nl&#39; gefunden werden (Dokument mit dem Schema &#39;service&#39; und dem Namen &#39;adobe_nl&#39;) |
| - | 500 - RST-360011 Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. | 500 - Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. |
| Fügen Sie ein Profil/einen Service mit einem ungültigen Aufzählungswert für Geschlecht (oder sonstiges) ein. | 500 - RST-360011 Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. Der Wert &#39;ungültig&#39; ist für die Auflistung &#39;nms:recipient:gender&#39; des Feldes &#39;@gender&#39; ungültig | 500 - Ein Fehler ist aufgetreten - Bitte Admin kontaktieren. |

### Zeitzone des Profils {#profile-timezone}

Bei Campaign Standard wird die Zeitzone als Teil der JSON-Antwort von **profileAndServices/profile** REST-API-Aufrufen angezeigt.

In Campaign v8 wird die Zeitzone Benutzenden nur als Teil der REST-API **Aufrufe von „profileAndServicesExt/profile** angezeigt. Sie ist nicht Teil der **profileAndServices/profile** REST-API-Aufrufe, da sie in einem erweiterten Schema hinzugefügt wird.

### Externe Workflow-Signale {#workflow-signals}

Die Campaign Standard Workflow GET-API gibt Parameternamen wie die Workflow-Instanzvariablen und deren Datentypen (boolesch, Zeichenfolge usw.) zurück. Dies wird verwendet, um beim Auslösen des Signals über einen POST-API-Aufruf einen entsprechend formatierten JSON-Anfragetext zu erstellen.

Campaign v8 unterstützt keine Advertising Workflow-Instanzvariablen, erwartet jedoch, dass die Entwickler wissen, was diese sind. Daher müssen nach der Migration Parameterinformationen im POST-Anfragetext ohne Verfügbarkeit von Parameterinformationen in der GET-API-Antwort erstellt werden.
