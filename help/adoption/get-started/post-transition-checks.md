---
title: Prüfungen und Fehlerbehebung nach der Umstellung auf Campaign v8
description: Erfahren Sie, was zu überprüfen ist und wie Sie häufige Probleme nach der Umstellung von Campaign Standard auf Campaign v8 beheben können
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 2%
---
# Prüfungen und Fehlerbehebung nach der Umstellung {#post-transition-checks}

Nach dem Übergang von Campaign Standard zu Campaign v8 verhalten sich einige Sendungen, Workflows und Landingpages möglicherweise anders als erwartet. In der folgenden Tabelle sind die von Benutzern nach der Umstellung gemeldeten Symptome mit der Ursache und den zu ergreifenden Maßnahmen aufgeführt. Eine vollständige Liste der Unterschiede finden Sie unter [Unterschiede zwischen Campaign Standard und Campaign v8](acs-v8-differences.md).

| Symptom | Ursache und Vorgehensweise | Weitere Informationen |
|---|---|---|
| Links in einem Versand sind direkte URLs, und es werden keine Klickdaten erfasst. | Das Tracking ist für den Versand oder die Versandvorlage, auf der es basiert, deaktiviert. Überprüfen Sie, ob **Tracking aktivieren** aktiviert ist, insbesondere in den Vorlagen Ihrer wiederkehrenden Sendungen. | [Tracking-Einstellungen](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Empfänger, die sich über die „mailto“-Abmeldemethode abgemeldet haben, befinden sich nicht in Quarantäne. | Dies ist zu erwarten. Diese Empfänger werden nicht unter Quarantäne gestellt. Sie werden vom Dienst, der mit dem Versand verknüpft ist, abgemeldet oder der Blockierungsliste hinzugefügt, wenn der Versand keinen Dienst hat. Um diese Abmeldungen zu verfolgen, überprüfen Sie die Abonnements des Service oder den Abschnitt **Nicht mehr kontaktieren** des Profils. | [Quarantänen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Eine Landingpage speichert keinen Wert, der von einem Skript berechnet oder in einem ausgeblendeten Feld gespeichert wird. | In der Web-Benutzeroberfläche von Campaign erstellte Landingpages unterstützen keine ausgeblendeten Eingabefelder oder benutzerdefinierten JavaScript. Erstellen Sie das Formular stattdessen als Web-Anwendung in der Client-Konsole. | [Landingpages ](../../v8/landing-pages/get-started-lp.md) |
| **Dateiübertragung** findet die von einer Briefpost-Aktivität generierte Datei nicht. | Die ausgehende Transition einer Briefpost-Aktivität enthält die ausgewählte Population und nicht die Extraktionsdatei. Fügen Sie **Aktivität** Datenextraktion“ und dann die Aktivität **Dateiübertragung“**. | [Briefpost](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Mehrere Schübe eines Versands werden zusammen gesendet. | Die Schübe werden ab dem Kontaktdatum des Versands geplant. Wenn der Versand nach der geplanten Zeit einiger Wellen beginnt, werden diese Wellen zusammen gesendet, anstatt mit Abständen angeordnet zu werden. | [Senden mit Schüben](../../v8/advanced-settings/send-using-waves.md) |
| Eine Dateimaske mit Zeichen nach dem Sternchen findet keine Datei im Azure Blob-Speicher. | Der Azure Blob-Speicher filtert Dateien nach Namenspräfix. Es wird nur ein nachfolgendes Sternchen unterstützt. | [Externes Konto übertragen](../../v8/administration/transfer-external-account.md) |
| Ein Landingpage- oder Inhaltsbaustein, der benutzerdefinierte JavaScript verwendet, verhält sich anders. | Benutzerdefinierte JavaScript wird während der Migration transformiert, sie jedoch validieren und anpassen, insbesondere wenn sie `queryDef`, Campaign JavaScript-APIs, Sitzungsschreibvorgänge, die Handhabung von Organisationseinheiten oder die Erstellung benutzerdefinierter URLs verwendet. | [Landingpages ](../../v8/landing-pages/get-started-lp.md) |
| Ein REST-API-Aufruf gibt einen leeren Wert, einen Fehler oder eine unerwartete Antwort zurück. | Einige Datenbankfelder werden während der Migration ignoriert und geben leere Werte zurück. Ein leerer PATCH gibt 204 zurück, und ein PATCH on-Speicherort gibt 500 zurück. Ein POST mit einer verknüpften Ressource ignoriert den Link oder gibt einen Fehler zurück. Ein ungültiger PKEY gibt 404 zurück. | [REST-API-Einschränkungen](acs-v8-differences.md#rest-api-limitations) |
| Ein gespeicherter PKEY funktioniert nicht mehr in API-Aufrufen. | PKEY-Werte ändern sich nach der Migration. Nicht außerhalb von Campaign speichern. Von jedem Aufruf aus dem wird durch den vorherigen Aufruf zurückgegeben. | [Verwendung von Schlüsseln](acs-v8-differences.md#key-usage) |
| Die Zeitzone oder der `ccpaOptOut` fehlt in einer Profilantwort. | Diese Felder werden nur von `profileAndServicesExt/profile` zurückgegeben, nicht von `profileAndServices/profile`. Rufen Sie den erweiterten Endpunkt auf. | [Zeitzone des Profils und ccpaOptOut](acs-v8-differences.md#profile-timezone) |
| Ein benutzerdefinierter Filter gibt einen Fehler in einem REST-API-Aufruf zurück. | Geben Sie in Campaign v8 dem Filter im Feld **Filtername in REST-API** einen Namen und verwenden Sie diesen Namen so, wie er in der Anfrage enthalten ist, ohne das Präfix „by“. | [Filtern](acs-v8-differences.md#rest-filtering) |
| Ein Aufruf, durch den ein externes Workflow-Signal Trigger wird, kann den Anfragetext nicht erstellen. | Die Workflow-GET-API gibt die Workflow-Variablen nicht mehr zurück. Erstellen Sie die Parameter des POST-Anfragetexts aus Ihren eigenen Kenntnissen über den Workflow. | [Workflow-externe Signale](acs-v8-differences.md#workflow-signals) |
| Der Zugriff auf die Transaktions-APIs wird verweigert. | Für den Zugriff auf Transaktions-APIs über die Ausführungsinstanz ist ein neues Produktprofil erforderlich. Überprüfen Sie die Produktprofilzuordnung Ihrer technischen Konten. | [Produktprofilzuordnung](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Eine migrierte Zielgruppe zeigt nur den neuesten Wert an, oder eine Dateizielgruppe hat keine Dimensionen. | Dies ist zu erwarten. Ein vordefinierter Filter übernimmt nur den neuesten Wert nach der Zielgruppenmigration und Zielgruppen vom Typ Datei werden zu Zielgruppen vom Typ Liste ohne Dimensionen. | [Verwalten von Zielgruppen](marketers.md#acs-gs-marketers-audiences) |
| Der Verlauf der in Campaign Standard ausgeführten Workflows ist leer. | Verlaufsprotokolle der in Campaign Standard ausgeführten Workflows werden nicht migriert. In Campaign v8 ausgeführte Workflows verfügen über einen eigenen Verlauf und eigene Protokolle. | [Erstellen eines Workflows](marketers.md#acs-gs-marketers-wf) |
| Einige Benutzer können sehen oder mehr tun als zuvor. | Benutzende mit der **Datenmodell**-Rolle, aber nicht der **Administration**-Rolle erhalten **Administration**-Zugriff, und Sicherheitsgruppen mit parallelen Organisationseinheiten können über breiteren Zugriff verfügen. Überprüfen Sie die Benutzergruppen, spezifischen Berechtigungen und Ordnerberechtigungen. | [Benutzerzugriffsverwaltung](user-management-acs.md) |
| Ein als „Trap **markiertes Testprofil** nicht den endgültigen Versand. | Fügen Sie in Campaign v8 eine **Trap-Gruppe** in den Zielgruppeneinstellungen des Versands hinzu. | [Trap-Gruppe](../../v8/audience/trap-group.md) |
| Eine wiederkehrende E-Mail hat keine Option für den Aggregationszeitraum. | Diese Option ist in Campaign v8 nicht verfügbar. | [Kanalaktivitäten](../../v8/workflows/activities/channels.md) |
| Dynamische Berichte enthalten keine Daten für einen Versand. | Die dynamische Berichterstellung umfasst E-Mail-Sendungen, Kampagnen mit E-Mail-Sendungen und Transaktionsnachrichten. | [Reporting](marketers.md#acs-gs-marketers-reporting) |
