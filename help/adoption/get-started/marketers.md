---
title: Erste Schritte mit Adobe Campaign v8 für Marketing-Fachleute
description: Entdecken Sie die wichtigsten Funktionen von Campaign v8. Es richtet sich an Marketing-Fachleute, die von Campaign Standard zu Campaign v8 migrieren.
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 22cea48ecdf1233dbbc1dc679ad6fcb2cf18bd2d
workflow-type: ht
source-wordcount: '2453'
ht-degree: 100%

---

# Erste Schritte für Marketing-Fachleute {#acs-gs-marketers}

Dieses Handbuch bietet Marketing-Fachleuten, die von Campaign Standard zu Campaign v8 wechseln, einen Überblick über die wichtigsten Funktionen von Campaign v8.

Sie können über die Client-Konsole oder die Web-Benutzeroberfläche auf Adobe Campaign v8 zugreifen. Über die Web-Benutzeroberfläche können Sie wichtige Marketing-Aktionen erstellen, verwalten und ausführen. Die neue Oberfläche von Adobe Campaign Web bietet ein modernes und intuitives Anwendererlebnis, das die Gestaltung und den Versand von Marketing-Kampagnen vereinfacht. [Weitere Informationen](../../v8/get-started/user-interface.md).

Durch die Migration werden all Ihre Daten aus Campaign Standard in Campaign v8 importiert. Dadurch wird ein reibungsloser Übergang bei minimaler Störung der laufenden Vorgänge sichergestellt.

Sie können Ihre vorhandenen Anmeldedaten weiterhin verwenden, um sich bei Ihrer neuen Adobe Campaign v8-Instanz anzumelden und eine Verbindung zu ihr herzustellen. Nach der Anmeldung können Sie alle Ihre Profile und Workflows finden, die migriert werden, sodass Sie weiterhin an Ihren Kampagnen arbeiten können.

Der Hauptunterschied liegt in der Benutzeroberfläche. Nachfolgend finden Sie einen Vergleich desselben Workflows in den beiden Benutzeroberflächen:

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Die Versionen der Adobe Campaign-Web-Benutzeroberfläche werden kontinuierlich bereitgestellt, was einen besser skalierbaren, schrittweisen Ansatz für die Bereitstellung von Funktionen ermöglicht. In den [Versionshinweisen](../../v8/rn/release-notes.md) finden Sie regelmäßig die neuesten Aktualisierungen.

## Entdecken der Campaign Web-Benutzeroberfläche {#acs-gs-marketers-ui}

Im folgenden Video erfahren Sie, wie Sie auf die Campaign Web-Benutzeroberfläche zugreifen, darin navigieren und Bestandslisten anpassen können.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie in der nachstehenden Dokumentation:

1. [Entdecken der Campaign Web-Benutzeroberfläche](../../v8/get-started/user-interface.md)

1. [Durchsuchen und Filtern von Listen](../../v8/get-started/list-filters.md)


## Erstellen und Verwalten von Profilen und Zielgruppen {#acs-gs-marketers-profiles-and-audiences}

Das allgemeine Konzept zum Erstellen und Verwalten von Profilen und Zielgruppen in Campaign v8 ist dasselbe wie in Adobe Campaign Standard. In [diesem Abschnitt](../../v8/audience/gs-audiences-recipients.md) erfahren Sie mehr über die ersten Schritte mit Profilen und Zielgruppen.

Nachstehend finden Sie einige nützliche Links für den Beginn.

### Verwalten von Profilen {#acs-gs-marketers-profiles}

In Adobe Campaign ist ein Profil ein in der Datenbank gespeicherter Eintrag, der als Schlüsselkomponente dient, um Zielgruppen für Sendungen zu erstellen und Personalisierungsdaten zu Ihrem Inhalt hinzuzufügen.

1. In diesem Video erfahren Sie, wie Sie mit der Campaign Web-Benutzeroberfläche auf Profile zugreifen, diese verwalten und erkunden:

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   Weitere Informationen finden Sie unter [Erste Schritte mit Profilen](../../v8/audience/about-recipients.md).

1. Erfahren Sie, wie Sie in Campaign v8 [Testprofile erstellen und verwalten](../../v8/audience/test-profiles.md).

### Verwalten von Zielgruppen {#acs-gs-marketers-audiences}

Zielgruppen sind Gruppen von Profilen mit ähnlichen Verhaltensweisen und/oder Merkmalen. Diese Sammlung von Personen kann entweder erstellt, ausgewählt oder geladen werden. Einmal erstellt, können Zielgruppen als Zielgruppe für Ihre Sendungen genutzt werden.

In diesem Video erfahren Sie, wie Sie Zielgruppen erstellen und verwalten, Zielgruppen für einen Versand auswählen und Kontrollgruppen definieren:

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie unter [Erste Schritte mit Zielgruppen](../../v8/audience/manage-audience.md){target="_blank"}.

Wie im Campaign Standard können Sie Ihrem Versand eine Kontrollgruppe hinzufügen. Sie können eine Kontrollgruppe definieren, um zu verhindern, dass Nachrichten an einen Teil Ihrer Zielgruppe gesendet werden, und das Verhalten nach dem Versand mit der Hauptzielgruppe vergleichen. Mit dieser Option können Sie die Wirkung Ihrer Kampagne messen.
Erfahren Sie, wie Sie eine [Kontrollgruppe festlegen](../../v8/audience/control-group.md){target="_blank"}.

>[!AVAILABILITY]
>
>* Alle mit der Campaign Standard-Aktivität „Abfrage“ erstellten Zielgruppen werden während des Wechsels in Campaign v8 in einen vordefinierten Filter umgewandelt. Campaign v8 unterstützt auch die Abfrageaktivität.
>
>* „Zielgruppe lesen“ wird mit [Vordefinierter Filter](../../v8/query/build-query.md) in eine Abfrageaktivität umgewandelt.
>
>* „Vordefinierter Filter“ verwendet nur den neuesten Wert im Anschluss an die Zielgruppenmigration nach Campaign v8.
>
>* Dateityp-Zielgruppen in Campaign Standard werden als Listentyp ohne Dimensionen migriert.

### Verwalten von Abonnements {#acs-gs-marketers-sub}

Sie können Ihre Dienste, z. B. Newsletter, verwalten und erstellen sowie Anmeldungen und Abmeldungen für diese Dienste überprüfen. Die wichtigsten Schritte stimmen allgemein mit denen in Campaign Standard überein. Weitere Informationen finden Sie auf den nachfolgenden Seiten:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="Gelegentlich" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>Erstellen von Anmeldediensten</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="Gelegentlich" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>Verwalten von Abonnentinnen und Abonnenten<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="Validierung" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/send-to-subscribers"><strong>Senden von Nachrichten an die Abonnentinnen und Abonnenten eines Dienstes</strong></a>
</div>
<p>
</td>
</tr>
</table>

## Verwenden von Plänen, Programmen und Kampagnen {#acs-gs-marketers-plans}

Adobe Campaign v8 ermöglicht es Ihnen, Ihre Ordnerhierarchie für Marketing-Pläne und -Programme zu konfigurieren. Die Funktionen für Pläne, Programme und Kampagnen sind in Campaign Standard und Campaign v8 ähnlich.

Weitere Informationen finden Sie in der [Dokumentation zu Plänen und Programmen](../../v8/administration/plans-programs.md).

Nachstehend finden Sie nützliche Links für den Beginn. Änderungen, die sich auf Ihr Anwendererlebnis auswirken können, werden in den Verfügbarkeitshinweisen beschrieben.


### Erstellen einer Kampagne {#acs-gs-marketers-campaign}

Mit Adobe Campaign können Sie Ihre zielgerichteten Marketing-Initiativen mithilfe der integrierten Kampagnenverwaltungsfunktion einfach orchestrieren. Mit der Fähigkeit, einen Zeitplan zu definieren, können Sie die Dauer und den Zeitpunkt Ihrer Kampagnen so planen, dass sie mit strategischen Zielen übereinstimmen und die Interaktion der Zielgruppe maximieren.

![Kampagnenfluss](assets/campaign-flow.png)

Weitere Informationen über Kampagnen finden Sie in der folgenden Dokumentation:

1. [Erste Schritte mit Kampagnen](../../v8/campaigns/gs-campaigns.md)
1. [Zugreifen auf und Verwalten von Kampagnen](../../v8/campaigns/manage-campaigns.md)
1. [Erste Kampagne erstellen](../../v8/campaigns/create-campaigns.md)


### Erstellen eines Workflows {#acs-gs-marketers-wf}

Die Workflow-Benutzeroberfläche wurde in der Campaign Web-Benutzeroberfläche völlig neu gestaltet, um die Verwendung, Konfiguration, Ausführung und Fehlerbehebung zu erleichtern. So wie aus Campaign Standard bekannt, können Sie mithilfe von Workflows das gesamte Spektrum an Prozessen und Aufgaben orchestrieren und die Geschwindigkeit und Skalierung aller Aspekte Ihrer Marketing-Kampagnen verbessern, angefangen bei der Segmenterstellung über die Vorbereitung von Nachrichten bis hin zum Versand. Außerdem können Sie Ihre Kanäle mit einer einzigen, benutzerfreundlichen Benutzeroberfläche für die Kampagnen-Orchestrierung synchronisieren.

In diesem Video erfahren Sie, wie Workflows funktionieren und wie Sie einen Zielgruppen-Workflow erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie in der [Workflow-Dokumentation](../../v8/workflows/gs-workflows.md).

Die Adobe Campaign Web-Benutzeroberfläche verfügt über einen Abfrage-Modeler in Workflows, der das Filtern von Datenbanken anhand verschiedener Kriterien vereinfacht. [Weitere Informationen über den Abfrage-Modeler](../../v8/query/query-modeler-overview.md)

Um den Zweck und die Funktionalität jeder Aktivität innerhalb Ihres Workflows zu verstehen, lesen Sie die detaillierten Informationen zu den [Workflow-Aktivitäten](../../v8/workflows/activities/about-activities.md).

Informationen zum Maximieren der Effizienz Ihres Workflows finden Sie unter [Schutzmechanismen und Einschränkungen für Workflows](../../v8/get-started/guardrails.md).

>[!AVAILABILITY]
>
>* [Verlauf und Protokolle](../../v8/workflows/start-monitor-workflows.md#logs-tasks) zur Workflow-Ausführung sind in Adobe Campaign v8 verfügbar.
>
>* Historische Protokolle für in Ihrer Campaign Standard-Instanz ausgeführte Workflows werden nicht nach Campaign v8 migriert.
>
>* Organisationseinheiten unterliegen dem Ordnerkonzept zum Zuordnen und Sicherstellen einer ähnlichen Zugriffskontrolle.
>

## Erstellen und Verwalten von Sendungen {#acs-gs-marketers-deliveries}

Mit der Campaign Web-Benutzeroberfläche können Marketing-Fachleute eigenständige Sendungen über das Menü **Sendungen** auf der linken Seite bzw. Sendungen im Kontext eines Workflows erstellen, ob nun in einer Kampagne enthalten oder nicht. Die wichtigsten Schritte entsprechen Ihrem bisherigen Erlebnis in Campaign Standard. Informationen zum Erstellen eines Versands finden Sie in der [Dokumentation zur Erstellung und Verwaltung von Sendungen](../../v8/msg/gs-deliveries.md).

Nützliche Links:

* **Versandvorlagen**: Um den Design-Prozess zu beschleunigen und zu verbessern, können Sie Versandvorlagen erstellen und so benutzerdefinierte Inhalte und Einstellungen in Ihren Kampagnen einfach wiederverwenden. Diese Funktion ermöglicht es Ihnen, das kreative Look-and-Feel zu standardisieren, um Kampagnen schneller durchführen und starten zu können. Weitere Informationen finden Sie auf der Seite zu [Versandvorlagen](../../v8/msg/delivery-template.md).

* **Versandeinstellungen**: Bei den Versandeinstellungen handelt es sich um technische Versandparameter, die in der Versandvorlage definiert sind. Sie können bei jedem Versand überschrieben werden.  Diese Einstellungen sind über die Schaltfläche „Einstellungen“ verfügbar, wenn ein Versand oder eine Versandvorlage bearbeitet wird. Weitere Informationen finden Sie im Abschnitt [Versandeinstellungen](../../v8/advanced-settings/delivery-settings.md).

* **Dynamische Inhalte**: Mit den Funktionen für dynamische Inhalte von Adobe Campaign Web können Sie Ihre Inhalte auf der Grundlage der Informationen, die Sie über Ihre Empfängerinnen und Empfänger gesammelt haben, anpassen. Durch die Verwendung dynamischer Inhalte stellen Sie sicher, dass Ihre Marketing-Bemühungen relevanter sind, indem Sie die Vermarktung unerwünschter oder unnötiger Produkte oder Dienstleistungen vermeiden. Weitere Informationen finden Sie im Abschnitt [Dynamische Inhalte](../../v8/personalization/gs-personalization.md).

* **Tests und Testversand**: Sobald der Versandinhalt definiert ist, können Sie ihn vor dem Senden der Nachricht mithilfe von Profilen und Testprofilen in einer Vorschau anzeigen und testen. Dies ist ein entscheidender Schritt, um sicherzustellen, dass er präzise, aber auch frei von Fehlern ist, sowohl in den Inhalts- als auch in den Personalisierungseinstellungen. Siehe [Über die Vorschau und Tests](../../v8/preview-test/preview-test.md).

* **Planung**: Sie können Datum und Uhrzeit für den Versand Ihrer Nachrichten festlegen. Die Auswahl des günstigsten Zeitpunkts für die Werbenachricht führt zur Maximierung der Öffnungsraten.

   * Erfahren Sie, wie Sie einen [eigenständigen Versand planen](../../v8/msg/gs-deliveries.md#gs-schedule).
   * Erfahren Sie, wie Sie den [Versand in einem Workflow planen](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow).

* **Angebote hinzufügen**: Sie können Ihren Sendungen über die Adobe Campaign Web-Benutzeroberfläche Angebote hinzufügen. Diese Angebote sind über das Menü „Angebote“ auf der linken Seite verfügbar. So können Sie auf die Liste der Angebote zugreifen. Erfahren Sie, wie Sie [Angebote zu Ihren Nachrichten hinzufügen](../../v8/msg/offers.md).

>[!AVAILABILITY]
>
>* Sendungen mit dem Status „Entwurf“ oder „Fertig“ wurden migriert.
>
>* Sendungen, die einen der folgenden Status aufweisen, wurden nach Adobe Campaign v8 migriert, müssen jedoch erneut vorbereitet werden: „In Transit“, „In Bearbeitung“, „Abgebrochen“, „Erneuter Versuch läuft“, „Vorbereitungsfehler“.
>
>* Sendungen mit einem der folgenden Status wurden als abgebrochene Sendungen migriert: „Für abgebrochen“ und „Erneuter Versuch läuft“.
>
>* Trackinglinks, Mirror-Seiten-URL-Links, Anmelde-/Abmelde-Links funktionieren wie in Campaign Standard.
>
>Weitere Informationen finden Sie zudem in den Abschnitten [Tracking und Monitoring](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/analytics/tracking){target="_blank"} sowie [Branding](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} in Adobe Campaign.

### E-Mail-Versand {#acs-gs-marketers-email}

In diesem Video erfahren Sie, wie Sie einen neuen E-Mail-Versand erstellen, die Zielgruppe definieren, den Inhalt gestalten, eine Vorschau simulieren und einen Testversand durchführen:

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Informationen zum Erstellen Ihrer ersten Targeting-E-Mail finden Sie in der [Dokumentation zum Erstellen der ersten E-Mail](../../v8/email/create-email.md)

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Durchführen eines E-Mail-Versands denen in Campaign Standard.

1. **Entwerfen und Definieren von Inhalten**

   Der E-Mail-Designer von Campaign v8 ähnelt dem in Campaign Standard. Zur Erinnerung: Die Unterstützung für den [alten E-Mail-Editor von Campaign Standard wurde vor einigen Jahren eingestellt](https://experienceleague.adobe.com/de/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}. Sie sollten bereits zum E-Mail-Designer von Campaign gewechselt sein, um E-Mail-Inhalte zu erstellen und zu personalisieren.

   Hier erfahren Sie, wie Sie im E-Mail-Designer navigieren. Im folgenden Video erfahren Sie, wie Sie eine E-Mail neu strukturieren und entwerfen und wie Sie Ihre E-Mail personalisieren und testen:

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   Mit dem E-Mail-Designer können Sie über eine intuitive Drag-and-Drop-Oberfläche überzeugende, individuell zugeschnittene E-Mails erstellen. Weitere Informationen finden Sie in der [Dokumentation zum E-Mail-Designer](../../v8/email/get-started-email-designer.md).

   In diesem Video erfahren Sie, wie Sie eine E-Mail durch Hochladen von HTML erstellen, mit dem E-Mail-Designer kompatibel machen und in eine Vorlage umwandeln:

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   Ein Inhaltsfragment ist eine wiederverwendbare Komponente, die in einer oder mehreren Nachrichten referenziert werden kann. Erfahren Sie mehr über [Inhaltsfragmente](../../v8/content/fragments.md), um die Erstellung Ihres E-Mail-Versands zu vereinfachen.

   Um den Design-Prozess zu beschleunigen und zu verbessern, können Sie eigenständige E-Mail-Vorlagen erstellen und so benutzerdefinierte Inhalte in Adobe Campaign einfach wiederverwenden. Siehe [Erstellen von E-Mail-Vorlagen](../../v8/email/create-email-templates.md).

1. **Vorschau und Test**

   In diesem Video erfahren Sie, wie Sie sich eine Vorschau des Inhalts und der Personalisierung von E-Mail-Nachrichten anzeigen, Testsendungen durchführen und das E-Mail-Rendering in gängigen Desktop-, Mobile- und Web-basierten Clients überprüfen:

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Senden von E-Mails und Prüfen von Protokollen**

   Wenn Sie Inhalt, Zielgruppe und Zeitplan definiert haben, können Sie den E-Mail-Versand vorbereiten. Weitere Informationen finden Sie in den folgenden Abschnitten:

   * [Vorbereiten und Senden einer E-Mail](../../v8/monitor/prepare-send.md)
   * [Überwachen von Versandlogs](../../v8/monitor/delivery-logs.md)


### SMS-Versand {#acs-gs-marketers-sms}

SMS-Sendungen bieten eine praktische und effiziente Möglichkeit, Textnachrichten an die Mobilgeräte Ihrer Kundinnen und Kunden zu senden. Mit dieser Funktion können Sie textbasierte Nachrichten erstellen, personalisieren und in der Vorschau anzeigen, um eine effektive Kommunikation zu gewährleisten.

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Durchführen eines SMS-Versands denen in Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="Lead" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/sms/create-sms"><strong>Erstellen eines SMS-Versands</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="Gelegentlich" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/sms/content-sms"><strong>Gestalten eines SMS-Versands<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="Validierung" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/sms/send-sms"><strong>Vorschau und Senden eines SMS-Versands</strong></a>
</div>
<p>
</td>
</tr></table>

### Push-Benachrichtigungen {#acs-gs-marketers-push}

Push-Benachrichtigungen sind unverzichtbar, um die Benutzenden Ihrer App zu erreichen, auch wenn sie die App nicht aktiv nutzen. Sie dienen verschiedenen Zwecken, z. B. der Bereitstellung von Aktualisierungen, der Durchführung spezifischer Aktionen und der Benachrichtigung über Angebote.

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Durchführen eines Push-Versands denen in Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/push/create-push">
<img alt="Lead" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/push/create-push"><strong>Erstellen eines Push-Versands</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/push/content-push">
<img alt="Gelegentlich" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/push/content-push"><strong>Entwerfen eines Push-Versands<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/push/send-push">
<img alt="Validierung" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/msg/push/send-push"><strong>Vorschau und Senden eines Push-Versands</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8 unterstützt sowohl den Android- als auch den iOS-Push-Kanal. Für die Transition bestehender Workflows und Sendungen, die den Push-Kanal nutzen, wenden Sie sich an Ihr Adobe Campaign Transition Team. Weitere Informationen finden Sie unter [Kanaleinrichtung](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* Beachten Sie, dass die SDK V4-Unterstützung für Apps vor einigen Jahren [in Campaign Standard eingestellt](https://experienceleague.adobe.com/de/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} wurde. Sie sollten bereits zum Adobe Experience Platform SDK gewechselt sein, das auch in Campaign v8 verwendet wird.
> 

### Briefpost {#acs-gs-marketers-direct-mail}

Briefpost ist ein Offline-Kanal, über den Sie Dateien erstellen können, um Ihrer Kundschaft personalisierte Sendungen wie Postkarten, Flyer oder Kataloge in großem Umfang zukommen zu lassen. Bei der Erstellung eines Briefpostversands generiert Adobe Campaign automatisch eine Extraktionsdatei, die alle Zielgruppenprofile und ausgewählten Daten wie Postanschriften und Profilattribute enthält.

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Durchführen eines Briefpostversands denen in Campaign Standard.


1. [Erstellen eines Briefpostversands](../../v8/direct-mail/create-direct-mail.md)
1. [Definieren der Extraktionsdatei](../../v8/direct-mail/content-direct-mail.md)
1. [Vorschau und Senden](../../v8/direct-mail/send-direct-mail.md)

### In-App-Kanal {#acs-gs-marketers-in-app}

Beachten Sie, dass der In-App-Kanal in Campaign v8 nicht verfügbar ist. Wenn Sie In-App-Benachrichtigungen senden müssen, wenden Sie sich an den Adobe-Support.

## Erstellen und Verwalten von Landingpages {#acs-gs-marketers-lp}

Die Web-Benutzeroberfläche von Adobe Campaign v8 bietet ein neu gestaltetes Anwendererlebnis für Landingpages. Mit Campaign können Sie Landingpages erstellen, entwerfen und freigeben. Durch Landingpages können Sie Benutzende zu Online-Formularen leiten, auf denen sie ihre Daten aktualisieren, sich für den Erhalt Ihrer Nachrichten anmelden bzw. davon abmelden oder einen bestimmten Dienst wie einen Newsletter abonnieren können.

Wenn Sie von Campaign Standard zu Campaign v8 wechseln, wurden Ihre vorhandenen Landingpages in die Campaign Web-Benutzeroberfläche migriert. Sie haben Zugriff auf dieselbe Bandbreite an Funktionen.

Weitere Informationen über Landingpages finden Sie in den folgenden Abschnitten:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="Lead" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/landing-pages/create-lp"><strong>Erstellen von Landingpages</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="Validierung" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/landing-pages/lp-content"><strong>Entwerfen von Landingpages</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="Validierung" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/landing-pages/lp-templates"><strong>Arbeiten mit Landingpage-Vorlagen</strong></a>
</div>
<p>
</td>
</tr></table>


## Reporting {#acs-gs-marketers-reporting}

Adobe Campaign bietet verschiedene [Reporting-Tools](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. Als Admin können Sie Berichte erstellen und konfigurieren, um sie für andere Campaign-Benutzer freizugeben.

Die umfassende Suite an Reporting-Tools von Adobe Campaign liefert wertvolle Erkenntnisse zur Effektivität Ihrer Marketing-Maßnahmen, sodass Sie Ihre Kampagnen für eine maximale Wirkung optimieren können. Weitere Informationen finden Sie in der [Dokumentation zum Reporting](../../v8/reporting/gs-reports.md).

Zusätzlich stehen Ihnen in Campaign v8 entsprechend dem Adobe Campaign Standard-Erlebnis dynamische Berichte für Ihre E-Mail-Sendungen zur Verfügung. Sie erhalten vollständig anpassbare und in Echtzeit aktualisierte Berichte, um die Wirkung Ihrer Marketing-Aktivitäten zu messen. Dadurch kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Ort und Alter sowie nach Daten von E-Mail-Kampagnen wie Öffnungen und Klicks ermöglicht. Weitere Informationen finden Sie in der [Dokumentation zu dynamischen Berichten](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}.

>[!AVAILABILITY]
>
>* Die Funktion für [dynamische Berichte](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} kann zum Reporting von E-Mail-Sendungen, Kampagnen mit E-Mail-Sendungen und Transaktionsnachrichten verwendet werden. Eine demografische Analyse nach Profildimension ist ebenfalls verfügbar.
>
> * Die [Reporting-Funktion der Adobe Campaign Web-Benutzeroberfläche](../../v8/reporting/campaign-reports.md) ist auch für alle Benutzenden verfügbar, die von Adobe Campaign Standard zu Adobe Campaign v8 wechseln.

Adobe Campaign bietet drei unterschiedliche Berichte:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="Validierung" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>Kampagnenberichte</strong></a>
</div>
<p>
<div>
<p>Stellen detaillierte Informationen zur Leistung, Effektivität und zu den Ergebnissen Ihrer einzelnen Sendungen bereit und bieten Ihnen so einen umfassenden Überblick.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="Lead" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>Versandberichte</strong>
</div>
<p>
<div>
<p>Bieten Ihnen eine gründliche Analyse der Leistung jedes einzelnen Versands, aufgeschlüsselt nach Kanal: Erfolgsraten, Interaktion der Zielgruppe und andere wichtige Metriken. Sie ermöglichen es Ihnen, die Effektivität und Wirkung Ihrer Kampagne insgesamt zu bewerten.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="Allgemeine Berichte" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/de/docs/campaign-web/v8/reports/global-report/global-reports"><strong> Allgemeine Berichte</strong></a>
</div>
<p>
<div>
<p>Bieten Ihnen eine konsolidierte Gesamtübersicht über die Traffic- und Interaktionsmetriken für jeden Kanal innerhalb Ihrer Campaign-Instanz. Diese Berichte bestehen aus verschiedenen Widgets, von denen jedes einen bestimmten Blickwinkel auf Ihre Kampagnen- oder Versandleistung bietet.</p>
</div>
<p>
</td>
</tr>
</table>
