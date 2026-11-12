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
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '878'
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
| In Campaign Standard kann ein Testprofil als „Falle **markiert werden,** den endgültigen Versand zu erhalten. Aktivieren Sie in Campaign v8 die Option, um Testprofile in die Hauptzielgruppe des Versands aufzunehmen. | [Sendungen testen](../../v8/preview-test/test-deliveries.md) |
| In der Web-Benutzeroberfläche von Campaign erstellte Landingpages unterstützen keine ausgeblendeten Eingabefelder oder benutzerdefinierten JavaScript. | [Landingpages ](../../v8/landing-pages/get-started-lp.md) |
| In Campaign Standard wird die generierte Datei auch bei der ausgehenden Transition einer Briefpost-Aktivität übernommen. In Campaign v8 wird nur die Zielpopulation übermittelt. Um die Datei an einen Server zu senden, fügen Sie die Aktivität **Datenextraktion** und dann die Aktivität **Dateiübertragung** hinzu. | [Briefpost](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Audiences, Workflows und Sendungen {#data-and-workflows}

Diese Unterschiede betreffen die aus Campaign Standard migrierten Audiences und Workflows, einige Optionen für wiederkehrende Sendungen und die Aktivität **Dateiübertragung** sowie den Umfang der dynamischen Berichterstellung.

| Änderungen | Weitere Informationen |
|---|---|
| Zielgruppen werden während der Transition transformiert. Beispielsweise werden Zielgruppen, die mit der Abfrage -Aktivität erstellt werden, zu vordefinierten Filtern und Dateityp-Zielgruppen zu Listentyp-Zielgruppen ohne Dimensionen. | [Verwalten von Zielgruppen](marketers.md#acs-gs-marketers-audiences) |
| Verlaufsprotokolle der in Campaign Standard ausgeführten Workflows werden nicht migriert. | [Erstellen eines Workflows](marketers.md#acs-gs-marketers-wf) |
| In Campaign Standard können Sie den Aggregationszeitraum einer wiederkehrenden E-Mail auswählen. Diese Option ist in Campaign v8 nicht verfügbar. | [Kanalaktivitäten](../../v8/workflows/activities/channels.md) |
| In Campaign Standard konnte die Aktivität **Dateiübertragung** Dateien alphanumerisch sortieren. Diese Option ist in Campaign v8 nicht verfügbar. | [Datei übertragen](../../v8/workflows/activities/transfer-file.md) |
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

## Verwaltung, Tracking und Mirrorseiten {#admin-tracking}

Diese Unterschiede betreffen Sendungen aus Campaign Standard vor der Umstellung sowie administrative Informationen, die nicht auf Campaign v8 übertragen werden.

| Änderungen | Weitere Informationen |
|---|---|
| Mirrorseiten von Sendungen, die von Campaign Standard vor der Umstellung gesendet wurden, sind nicht verfügbar. Mirrorseiten der von Campaign v8 gesendeten Sendungen funktionieren wie gewohnt. | [Mirrorseiten](../../v8/email/mirror-page.md) |
| Tracking-Daten von Echtzeit-Transaktionssendungen, die von Campaign Standard vor der Umstellung gesendet wurden, werden in Campaign v8 nicht erfasst. Die Links dieser Nachrichten werden weiterhin umgeleitet. | [Transaktionsnachrichten überwachen](../../v8/transactional-messaging/monitor-transactional.md) |
| Die Einstellungen für getrackte URLs von Versandentwürfen werden nicht beibehalten. Nach der Umstellung folgen Tracking-, Mirrorseiten- und Abonnement-Links dem Campaign v8-Standard. Links werden standardmäßig verfolgt. | [Links hinzufügen und Nachrichten verfolgen](../../v8/email/message-tracking.md) |
| Geografische Einheiten sind nicht verfügbar. Die Zugriffskontrolle mithilfe geografischer Einheiten geht verloren. | [Zugriffssteuerung](../../v8/get-started/connect-to-campaign.md#access-control) |
| Die **Erstellt von** und **Geändert von** von Entitäten sind nach der Transition nicht mehr verfügbar. | [Audit-Protokoll](admin-developers.md#acs-gs-admin-audit-trail) |
| Die URLs von Branding-Subdomains werden an den Campaign v8-Standard angepasst. Nicht standardmäßige Branding-Konfigurationen werden nicht migriert und über die Standardmarke bereitgestellt. | [Branding](../../v8/administration/branding/branding-gs.md) |

## APIs und Integrationen {#apis-and-integrations}

Diese Unterschiede betreffen die Integrationen, die Campaign über die REST-API aufrufen, sowie die Integrationen mit anderen Adobe-Lösungen und -Tools.

| Änderungen | Weitere Informationen |
|---|---|
| PKEY-Werte ändern sich nach der Migration. Wenn Sie PKEYs außerhalb von Campaign speichern, befolgen Sie stattdessen die von der API zurückgegebenen. | [REST-APIs](admin-developers.md#acs-gs-admin-apis) |
| Einige migrierte Profilfelder, wie Zeitzone und `ccpaOptOut`, werden nur von der `profileAndServicesExt/profile`-API zurückgegeben. | [REST-APIs](admin-developers.md#acs-gs-admin-apis) |
| Die Dreamweaver- und Adobe Experience Platform Data Connector-Integrationen von Campaign Standard sind in Campaign v8 nicht verfügbar. | [Arbeiten mit Campaign und anderen Adobe-Lösungen](../../v8/integrations/integration.md) |
| Adobe migriert Ihre Adobe Analytics- und Audience Manager-Konfigurationen. Sie müssen die Trigger- und Adobe Target-Integrationen erneut einrichten. | [Verwalten von Adobe Campaign-Integrationen](admin-developers.md#acs-gs-integrations) |
