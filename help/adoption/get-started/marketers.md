---
title: Erste Schritte mit Adobe Campaign v8 für Marketing-Fachleute
description: Entdecken Sie die wichtigsten Funktionen von Campaign v8. Es richtet sich an Marketing-Fachleute, die von Campaign Standard zu Campaign v8 migrieren.
role: User
level: Beginner, Experienced
source-git-commit: e68ad7ca3368165feb534363c36b03b510291e8a
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 22%

---


# Erste Schritte für Marketing-Fachleute {#acs-gs-marketers}

Dieses Handbuch bietet einen Überblick über die wichtigsten Funktionen von Campaign v8 für Marketingexperten, die von Campaign Standard auf Campaign v8 umsteigen.

Der Zugriff auf Adobe Campaign v8 erfolgt über die Clientkonsole oder die Web-Benutzeroberfläche. Über die Web-Oberfläche können Sie wichtige Marketing-Aktionen erstellen, verwalten und ausführen. Die neue Oberfläche von Adobe Campaign Web bietet ein modernes und intuitives Anwendererlebnis, das die Gestaltung und den Versand von Marketing-Kampagnen vereinfacht. [Weitere Informationen](../../v8/get-started/user-interface.md).

Durch die Migration werden all Ihre Daten aus Campaign Standard in Campaign v8 importiert, wodurch ein reibungsloser Übergang bei minimaler Unterbrechung Ihrer laufenden Vorgänge gewährleistet wird.

Sie können Ihre vorhandenen Anmeldedaten weiterhin verwenden, um sich bei Ihrer neuen Adobe Campaign v8-Instanz anzumelden und eine Verbindung mit ihr herzustellen. Nach der Anmeldung können Sie alle Ihre Profile und Workflows finden, die migriert werden, sodass Sie weiterhin an Ihren Kampagnen arbeiten können.

Der Hauptunterschied liegt in der Benutzeroberfläche. Nachfolgend finden Sie einen Vergleich desselben Workflows mit den beiden Benutzeroberflächen:

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Die Versionen der Adobe Campaign-Web-Benutzeroberfläche werden kontinuierlich bereitgestellt, was einen besser skalierbaren, schrittweisen Ansatz für die Bereitstellung von Funktionen ermöglicht. In den [Versionshinweisen](../../v8/rn/release-notes.md) finden Sie regelmäßig die neuesten Aktualisierungen.

## Entdecken Sie die Campaign-Webbenutzeroberfläche {#acs-gs-marketers-ui}

Im folgenden Video erfahren Sie, wie Sie auf die Web-Benutzeroberfläche von Campaign zugreifen und darin navigieren und wie Sie die Inventarlisten anpassen können.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie in der folgenden Dokumentation:

1. [Benutzeroberfläche des Campaign-Webs](../../v8/get-started/user-interface.md)

1. [Listen durchsuchen und filtern](../../v8/get-started/list-filters.md)


## Erstellen und Verwalten von Profilen und Zielgruppen {#acs-gs-marketers-profiles-and-audiences}

Die allgemeinen Konzepte zum Erstellen und Verwalten von Profilen und Audiences in Campaign v8 sind mit denen in Adobe Campaign Standard identisch. In [diesem Abschnitt](../../v8/audience/gs-audiences-recipients.md) erfahren Sie, wie Sie mit Profilen und Zielgruppen beginnen.

Unten finden Sie einige nützliche Links, mit denen Sie beginnen können.

### Verwalten von Profilen {#acs-gs-marketers-profiles}

In Adobe Campaign ist ein Profil ein in der Datenbank gespeicherter Datensatz, der als Schlüsselkomponente dient, um Zielgruppen für Sendungen zu erstellen und Ihrem Inhalt Personalisierungsdaten hinzuzufügen.

1. In diesem Video erfahren Sie, wie Sie über die Campaign-Web-Benutzeroberfläche auf Profile zugreifen, diese verwalten und untersuchen können:

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   Weitere Informationen finden Sie in der Dokumentation [Erste Schritte mit Profilen](../../v8/audience/about-recipients.md) .

1. Erfahren Sie, wie Sie in Campaign v8 [Testprofile erstellen und verwalten](../../v8/audience/test-profiles.md).

### Verwalten von Zielgruppen {#acs-gs-marketers-audiences}

Zielgruppen sind Gruppen von Profilen, die ähnliche Verhaltensweisen und/oder Merkmale aufweisen. Diese Sammlung von Personen kann entweder erstellt, ausgewählt oder geladen werden. Einmal erstellt, können Zielgruppen als Zielgruppe für Ihre Sendungen genutzt werden.

In diesem Video erfahren Sie, wie Sie Audiences erstellen und verwalten, Audiences für einen Versand auswählen und Kontrollgruppen definieren:

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Weitere Informationen finden Sie unter [Erste Schritte mit Zielgruppen](../../v8/audience/manage-audience.md){target="_blank"} .

Wie im Campaign Standard können Sie Ihrem Versand eine Kontrollgruppe hinzufügen. Sie können eine Kontrollgruppe definieren, um zu verhindern, dass Nachrichten an einen Teil Ihrer Zielgruppe gesendet werden, und das Verhalten nach dem Versand mit der Hauptzielgruppe vergleichen. Mit dieser Option können Sie die Wirkung Ihrer Kampagne messen.
Erfahren Sie, wie Sie [eine Kontrollgruppe ](../../v8/audience/control-group.md){target="_blank"} festlegen.

>[!AVAILABILITY]
>
>* Alle mit der Aktivität Abfrage des Campaign Standards erstellten Audiences werden in Campaign v8 während der Transition in einen vordefinierten Filter umgewandelt. Campaign v8 unterstützt auch die Aktivität Abfrage .
>
>* Audience lesen wird mit [vordefiniertem Filter](../../v8/query/build-query.md) in Abfrageaktivität umgewandelt
>
>* Vordefinierter Filter verwendet nur den neuesten Wert nach der Zielgruppenmigration nach Campaign v8.
>
>* Dateityp-Zielgruppen in Campaign Standard werden als Listentyp ohne Dimensionen migriert.

### Verwalten von Abonnements {#acs-gs-marketers-sub}

Sie können Ihre Dienste wie z. B. Newsletter verwalten und erstellen und die An- und Abmeldungen dieser Dienste überprüfen. Die wichtigsten Schritte sind global dieselben wie in Campaign Standard. Weitere Informationen finden Sie auf den folgenden Seiten:

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

Mit Adobe Campaign v8 können Sie Ihre Ordnerhierarchie für Marketingpläne und -programme konfigurieren. Die Funktionen für Pläne, Programme und Kampagnen sind mit Campaign Standard und Campaign v8 vergleichbar.

Weitere Informationen finden Sie in der Dokumentation zu [Plänen und Programmen](../../v8/administration/plans-programs.md).

Nachstehend finden Sie nützliche Links, mit denen Sie beginnen können. Änderungen, die sich auf Ihr Benutzererlebnis auswirken können, werden in den Versionshinweisen hervorgehoben.


### Erstellen einer Kampagne {#acs-gs-marketers-campaign}

Mit Adobe Campaign können Sie Ihre zielgerichteten Marketinginitiativen mithilfe der integrierten Kampagnenverwaltungsfunktion einfach koordinieren. Mit der Fähigkeit, einen Zeitplan zu definieren, können Sie die Dauer und den Zeitpunkt Ihrer Kampagnen so planen, dass sie mit strategischen Zielen übereinstimmen und die Interaktion der Zielgruppe maximieren.

![Kampagnenfluss](assets/campaign-flow.png)

Weitere Informationen zu Kampagnen finden Sie in der folgenden Dokumentation:

1. [Erste Schritte mit Kampagnen](../../v8/campaigns/gs-campaigns.md)
1. [Zugreifen auf und Verwalten von Kampagnen](../../v8/campaigns/manage-campaigns.md)
1. [Erste Kampagne erstellen](../../v8/campaigns/create-campaigns.md)


### Erstellen eines Workflows {#acs-gs-marketers-wf}

Die Benutzeroberfläche des Workflows wurde in der Campaign-Webbenutzeroberfläche vollständig neu gestaltet, um die Verwendung, Konfiguration, Ausführung und Fehlerbehebung zu erleichtern. Wie Sie bereits im Campaign Standard erfahren haben, können Sie mit Workflows das gesamte Spektrum an Prozessen und Aufgaben koordinieren, die Geschwindigkeit und Skalierung Ihrer Marketingkampagnen verbessern, von der Erstellung von Segmenten über die Vorbereitung von Nachrichten bis hin zum Versand. Außerdem können Sie Ihre Kanäle mit einer einzigen, benutzerfreundlichen Benutzeroberfläche für die Kampagnenorchestrierung synchronisieren.

In diesem Video erfahren Sie, wie Workflows funktionieren und wie Sie einen Zielgruppen-Workflow erstellen:

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Erhalten Sie weitere Details mit der [Workflow-Dokumentation](../../v8/workflows/gs-workflows.md).

Die Web-Benutzeroberfläche von Adobe Campaign bietet in Workflows einen Abfragemodellierer, der die Filterung der Datenbank anhand verschiedener Kriterien vereinfacht. [Weitere Informationen zum Abfragemodell](../../v8/query/query-modeler-overview.md)

Um den Zweck und die Funktionalität jeder Aktivität innerhalb Ihres Workflows zu verstehen, lesen Sie die detaillierten Informationen zu den [Workflow-Aktivitäten](../../v8/workflows/activities/about-activities.md) .

Maximieren Sie die Effizienz Ihres Workflows, indem Sie die [Limits und Einschränkungen für Workflows](../../v8/get-started/guardrails.md) überprüfen.

>[!AVAILABILITY]
>
>* Workflow-Ausführungsverlauf [und -protokolle](../../v8/workflows/start-monitor-workflows.md#logs-tasks) sind in Adobe Campaign v8 verfügbar.
>
>* Historische Protokolle für Workflows, die in Ihrer Campaign Standard-Instanz ausgeführt werden, werden nicht nach Campaign v8 migriert.
>
>* Organisationseinheiten werden zum Zuordnen und Sicherstellen einer ähnlichen Zugriffskontrolle dem Ordnerkonzept zugeordnet.
>

## Erstellen und Verwalten von Sendungen {#acs-gs-marketers-deliveries}

Über die Campaign-Webbenutzeroberfläche können Sie als Marketing-Experte eigenständige Sendungen aus dem linken Menü **Sendungen** erstellen oder Sendungen im Kontext eines Workflows erstellen, der in einer Kampagne enthalten ist oder nicht. Die wichtigsten Schritte sind an Ihrem bisherigen Erlebnis in Campaign Standard ausgerichtet. Erfahren Sie im folgenden Abschnitt, wie Sie einen Versand erstellen: [Dokumentation zur Erstellung und Verwaltung von Sendungen](../../v8/msg/gs-deliveries.md).

Nützliche Links:

* **Versandvorlagen** - Für einen beschleunigten und verbesserten Designprozess können Sie Versandvorlagen erstellen, um benutzerdefinierte Inhalte und Einstellungen in allen Ihren Kampagnen wiederzuverwenden. Mit dieser Funktion können Sie das kreative Erscheinungsbild standardisieren, um Kampagnen schneller ausführen und starten zu können. Weitere Informationen finden Sie auf der Seite [Versandvorlage](../../v8/msg/delivery-template.md) .

* **Versandeinstellungen** - Versandeinstellungen sind technische Versandparameter, die in der Versandvorlage definiert sind. Sie können bei jedem Versand überschrieben werden.  Diese Einstellungen sind über die Schaltfläche Einstellungen verfügbar, die beim Bearbeiten eines Versands oder einer Versandvorlage verfügbar ist. Weitere Informationen finden Sie im Abschnitt [Versandeinstellungen](../../v8/advanced-settings/delivery-settings.md) .

* **Dynamischer Inhalt** - Mit den Funktionen für dynamische Inhalte im Adobe Campaign-Web können Sie Ihren Inhalt auf der Grundlage der Informationen anpassen, die Sie über Ihre Empfänger erfasst haben. Durch die Verwendung dynamischer Inhalte stellen Sie sicher, dass Ihre Marketing-Bemühungen relevanter sind, indem Sie die Vermarktung unerwünschter oder unnötiger Produkte oder Dienstleistungen vermeiden. Weitere Informationen finden Sie im Abschnitt [Dynamischer Inhalt](../../v8/personalization/gs-personalization.md) .

* **Test und Testsendungen** - Sobald Ihr Versandinhalt definiert wurde, können Sie Profile und Testprofile verwenden, um eine Vorschau anzuzeigen und zu testen, bevor Sie die Nachricht senden. Dieser Schritt ist entscheidend, um sicherzustellen, dass er korrekt, aber auch fehlerfrei ist, sowohl in den Inhalts- als auch in den Personalisierungseinstellungen. Siehe [Vorschau und Test](../../v8/preview-test/preview-test.md).

* **Planung** - Sie können das Datum und die genaue Uhrzeit für den Versand Ihrer Nachrichten festlegen. Die Auswahl des günstigsten Zeitpunkts für die Werbenachricht führt zur Maximierung der Öffnungsraten.

   * Erfahren Sie, wie Sie [einen eigenständigen Versand planen](../../v8/msg/gs-deliveries.md#gs-schedule)
   * Erfahren Sie, wie Sie einen Versand in einem Workflow planen ](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)[

* **Angebote hinzufügen** - Sie können Ihren Sendungen Angebote in der Adobe Campaign-Web-Benutzeroberfläche hinzufügen. Diese Angebote sind über das Menü Angebote verfügbar, über das Sie auf die Liste der Angebote zugreifen können.  Erfahren Sie, wie Sie Ihren Nachrichten [Angebote hinzufügen](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* Sendungen mit Entwurfsstatus oder Fertigstellung wurden migriert.
>
>* Sendungen, die einen der folgenden Status aufweisen, wurden auf Adobe Campaign v8 migriert, müssen jedoch erneut vorbereitet werden: Verlaufs/Gestartet/Abgebrochen/Erneuter Versuch läuft/Vorbereitungsfehler.
>
>* Sendungen mit einem der folgenden Status wurden als abgebrochene Sendungen migriert: Für Abgebrochen/Erneuter Versuch läuft.
>
>* Tracking-Links, Mirrorseiten-URL-Links, Anmelde-/Abmelde-Links funktionieren wie in Campaign Standard.
>
>Siehe auch die folgenden Abschnitte: [Tracking und Monitoring](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Branding](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} in Adobe Campaign.

### E-Mail-Versand {#acs-gs-marketers-email}

In diesem Video erfahren Sie, wie Sie einen neuen E-Mail-Versand erstellen, die Zielgruppe definieren, den Inhalt entwerfen, eine Vorschau simulieren und einen Testversand durchführen:

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Erfahren Sie, wie Sie Ihre erste Targeting-E-Mail erstellen, in der [Erstellen der ersten E-Mail-Dokumentation](../../v8/email/create-email.md)

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Senden eines E-Mail-Versands dem Campaign Standard.

1. **Entwerfen und Definieren von Inhalten**

   Email Designer von Campaign v8 ähnelt dem in Campaign Standard verfügbaren Designer. Zur Erinnerung: Der alte E-Mail-Editor von Campaign Standard[wurde vor einigen Jahren als veraltet eingestuft](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"}. Sie sollten bereits zu Campaign Email Designer übergegangen sein, um E-Mail-Inhalte zu erstellen und zu personalisieren.

   Hier erfahren Sie, wie Sie im E-Mail-Designer navigieren. Im folgenden Video erfahren Sie, wie Sie eine E-Mail neu strukturieren und entwerfen, wie Sie Ihre E-Mail personalisieren und testen können:

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   Mit dem E-Mail-Designer können Sie über eine intuitive Drag-and-Drop-Oberfläche überzeugende, individuell zugeschnittene E-Mails erstellen. Weitere Informationen finden Sie in der Dokumentation zu [E-Mail-Designer](../../v8/email/get-started-email-designer.md)

   In diesem Video erfahren Sie, wie Sie eine E-Mail durch Hochladen von HTML erstellen, wie Sie sie mit E-Mail-Designer kompatibel machen und wie Sie sie in eine Vorlage konvertieren können:

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   Ein Inhaltsfragment ist eine wiederverwendbare Komponente, die in einer oder mehreren Nachrichten referenziert werden kann. Erfahren Sie mehr über [Inhaltsfragmente](../../v8/content/fragments.md) , um die Erstellung Ihres E-Mail-Versands zu vereinfachen.

   Für einen beschleunigten und verbesserten Designprozess können Sie eigenständige Vorlagen erstellen, um benutzerdefinierte Inhalte in Adobe Campaign einfach wiederzuverwenden. Siehe [E-Mail-Vorlagen erstellen](../../v8/email/create-email-templates.md)

1. **Vorschau und Test**

   In diesem Video erfahren Sie, wie Sie eine Vorschau des Inhalts und der Personalisierung von E-Mail-Nachrichten anzeigen, Testsendungen (Testsendungen) durchführen und das E-Mail-Rendering in bevorzugten Desktop-, Mobile- und Web-basierten Clients überprüfen können:

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Senden von E-Mails und Prüfen von Protokollen**

   Wenn Sie Inhalt, Zielgruppe und Zeitplan definiert haben, können Sie Ihren E-Mail-Versand vorbereiten. Weitere Informationen finden Sie in den folgenden Abschnitten:

   * [Vorbereiten und Senden einer E-Mail](../../v8/monitor/prepare-send.md)
   * [Überwachen von Versandlogs](../../v8/monitor/delivery-logs.md)


### SMS-Versand {#acs-gs-marketers-sms}

SMS-Sendungen bieten eine praktische und effiziente Möglichkeit, Textnachrichten an die Mobilgeräte Ihrer Kundinnen und Kunden zu senden. Mit dieser Funktion können Sie textbasierte Nachrichten erstellen, personalisieren und in der Vorschau anzeigen, um eine effektive Kommunikation zu gewährleisten.

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Senden eines SMS-Versands dem Campaign Standard.


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

### Push-Benachrichtigungen  {#acs-gs-marketers-push}

Push-Benachrichtigungen sind für die Kontaktaufnahme mit Ihren Mobile-App-Benutzern unerlässlich, auch wenn diese Ihre App nicht aktiv verwenden. Sie dienen verschiedenen Zwecken, z. B. der Bereitstellung von Aktualisierungen, der Durchführung spezifischer Aktionen und der Benachrichtigung über Angebote.

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Senden eines Push-Benachrichtigungsversands dem Campaign Standard.


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
>* Adobe Campaign v8 unterstützt sowohl Android als auch iOS Push Channel. Stellen Sie für die Transition vorhandener Workflows und Sendungen mithilfe des Push-Kanals eine Verbindung zu Ihrem Adobe Campaign Transition Manager her. Weitere Informationen finden Sie unter [Einrichten des Kanals](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* Beachten Sie, dass das SDK V4 für Mobile Apps vor einigen Jahren in Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} nicht mehr unterstützt wurde. [ Sie sollten bereits zum Adobe Experience Platform SDK übergegangen sein, das auch in Campaign v8 verwendet wird.
> 

### Briefpost {#acs-gs-marketers-direct-mail}

Briefpost ist ein Offline-Kanal, über den Sie Dateien erstellen können, um Ihren Kunden personalisierte Briefe wie Postkarten, Flyer oder Kataloge in großem Umfang zukommen zu lassen. Bei der Erstellung eines Briefpost-Versands generiert Adobe Campaign automatisch eine Extraktionsdatei, die alle Zielgruppenprofile und ausgewählten Daten wie Postanschriften und Profilattribute enthält.

In Campaign v8 ähneln die detaillierten Schritte zum Erstellen, Testen und Senden eines Briefpost-Versands dem Campaign Standard.


1. [Briefpost-Versand erstellen](../../v8/direct-mail/create-direct-mail.md)
1. [Definieren Sie die Extraktionsdatei](../../v8/direct-mail/content-direct-mail.md)
1. [Vorschau erstellen und senden](../../v8/direct-mail/send-direct-mail.md)

### In-App-Kanal {#acs-gs-marketers-in-app}

Beachten Sie, dass der In-App-Kanal in Campaign v8 nicht verfügbar ist. Wenn Sie In-App-Benachrichtigungen senden müssen, wenden Sie sich an Ihren Adobe-Support-Mitarbeiter.

## Erstellen und Verwalten von Landingpages {#acs-gs-marketers-lp}

Die Web-Benutzeroberfläche von Adobe Campaign v8 verfügt über ein neu gestaltetes Benutzererlebnis für Landingpages. Mit Campaign können Sie Landingpages erstellen, entwerfen und freigeben. Durch Landingpages können Sie Benutzende zu Online-Formularen leiten, auf denen sie ihre Daten aktualisieren, sich für den Erhalt Ihrer Nachrichten anmelden bzw. davon abmelden oder einen bestimmten Dienst wie einen Newsletter abonnieren können.

Als Campaign Standard, der zu Campaign v8 wechselt, wurden Ihre Landingpages auf die Campaign-Webbenutzeroberfläche migriert. Sie können auf dieselbe Bandbreite an Funktionen zugreifen.

Weitere Informationen zu Landingpages finden Sie in den folgenden Abschnitten:

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

Adobe Campaign bietet eine Reihe von [Reporting-Tools](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. Als Administrator können Sie Berichte erstellen und konfigurieren, um sie für andere Campaign-Benutzer freizugeben.

Die Adobe Campaign-Suite mit Reporting-Tools bietet wertvolle Einblicke in die Effektivität Ihrer Marketing-Maßnahmen, sodass Sie Ihre Kampagnen für maximale Wirkung optimieren können. Weitere Informationen finden Sie in der [Dokumentation zur Berichterstellung](../../v8/reporting/gs-reports.md).

Zusätzlich steht Ihnen in Campaign v8 entsprechend dem Adobe Campaign Standard-Erlebnis die dynamische Berichterstellung für Ihre E-Mail-Sendungen zur Verfügung. Es bietet vollständig anpassbare und in Echtzeit aktualisierte Berichte, um die Wirkung Ihrer Marketing-Aktivitäten zu messen. Dadurch kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Stadt und Alter sowie nach Daten von E-Mail-Kampagnen wie Öffnungen und Klicks ermöglicht. Weitere Informationen finden Sie in der Dokumentation zu [dynamischen Berichten](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} .

>[!AVAILABILITY]
>
>* [Dynamische Berichterstellung](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} kann für die Berichterstellung von E-Mail-Sendungen, Kampagnen mit E-Mail-Sendungen und Transaktionsnachrichten verwendet werden. Die demografische Analyse nach Profil -Dimension ist ebenfalls verfügbar.
>
> * Die Berichterstellung für die Adobe Campaign-Webbenutzeroberfläche](../../v8/reporting/campaign-reports.md) ist auch für alle Benutzer verfügbar, die von Adobe Campaign Standard auf Adobe Campaign v8 wechseln.[

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
<p>Geben Sie detaillierte Informationen zu Leistung, Effektivität und Ergebnis Ihrer Sendungen an und erhalten Sie einen umfassenden Überblick.</p>
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
<p>Bieten Sie eine gründliche Analyse der Leistung jedes Versands pro Kanal an: Erfolgsraten, Zielgruppeninteraktion und andere wichtige Metriken. Sie ermöglichen es Ihnen, die Effektivität und Wirkung Ihrer Kampagne insgesamt zu bewerten.</p>
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
<p>Bieten Sie eine konsolidierte Zusammenfassung der Traffic- und Interaktionsmetriken für jeden Kanal in Ihrer Campaign-Instanz an. Diese Berichte bestehen aus verschiedenen Widgets, von denen jedes einen bestimmten Blickwinkel auf Ihre Kampagnen- oder Versandleistung bietet.</p>
</div>
<p>
</td>
</tr>
</table>
