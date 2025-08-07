---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: ht
source-wordcount: '900'
ht-degree: 100%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind auf den Seiten für [2024](release-notes-24.md) und [2025](release-notes-25.md) aufgeführt.

## Version Juli 2025 {#25-7-release}

### Neue Funktionen {#25-7-features}

Die folgenden Funktionen sind ab der Version Juli verfügbar.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Unterstützung von benutzerdefiniertem CSS im E-Mail-Designer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Beim Erstellen Ihrer E-Mails können Sie nun Ihr eigenes benutzerdefiniertes CSS direkt im E-Mail-Designer hinzufügen. Mit dieser Funktion können Sie erweiterte und spezifische Stile anwenden, um die Flexibilität und Kontrolle über das Erscheinungsbild Ihrer Inhalte zu erhöhen.</p>
<p>Weitere Informationen finden Sie in der <a href="../email/custom-css.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Marken</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können nun Ihre eigenen Marken erstellen und anpassen, um Ihre visuelle und verbale Identität in der gesamten Kommunikation klar zu definieren. Über den Markenausrichtungswert erhalten Sie Echtzeit-Feedback dazu, wie gut Ihr Inhalt den Ton, den Stil und die Richtlinien Ihrer Marke widerspiegelt. So können Sie sicherstellen, dass jede gesendete Nachricht markenkonform ist.
</p>
<p>Weitere Informationen finden Sie in der <a href="../content/brands.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Versandwarnung</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Bei der Funktion „Versandwarnungen“ handelt es sich um ein System zum Warnungs-Management, über das eine Benutzergruppe automatisch Benachrichtigungen zu ihren Sendungen erhält. </p>
<p>Weitere Informationen finden Sie in der <a href="../msg/delivery-alerting.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Dynamisches Reporting</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Sie können nun auf dynamisches Reporting zugreifen, das vollständig anpassbare Berichte und Echtzeitberichte zum Messen der Wirkung Ihrer Marketing-Aktivitäten bietet. Dadurch kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Ort und Alter ermöglicht, zusätzlich zur Analyse basierend auf Daten von E-Mail-Kampagnen wie Öffnungen und Klicks. Dynamische Berichte sind auch für mehrsprachige E-Mail-Sendungen und Transaktionsnachrichten verfügbar.</p>
<p>Diese Funktion ist nur auf Anfrage verfügbar. Wenden Sie sich für Zugriff an den Adobe-Support. Ihr Server muss mindestens auf 8.8.1 aktualisiert sein. Weitere Informationen finden Sie in den <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de" target="_blank">Versionshinweisen</a> zur Client-Konsole.
<p>Weitere Informationen finden Sie in der <a href="../reporting/dynamic-reporting/get-started-reporting.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Zentralisiertes Branding</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ihre technischen Admins können nun eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Markenidentität auswirken. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Sie können diese Marken erstellen und mit verschiedenen Nachrichten oder Landingpages verknüpfen. Diese Konfiguration wird in Vorlagen verwaltet. Branding-Optionen sind für alle Kanäle verfügbar, einschließlich SMS und Briefpost.</p>
<p>Diese Funktion ist nur auf Anfrage und nur für neue Implementierungen verfügbar. Wenden Sie sich für Zugriff an den Adobe-Support. Ihr Server muss mindestens auf 8.8.1 aktualisiert sein. Weitere Informationen finden Sie in den <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de" target="_blank">Versionshinweisen</a> zur Client-Konsole.
<p>Weitere Informationen finden Sie in der <a href="../administration/branding/branding-gs.md">entsprechenden Dokumentation</a>.</p>
</td>
</tr>
</tbody>
</table>

Zusätzlich zu den oben aufgeführten Funktionen bietet diese Version auch eine Reihe von Funktionen, die in der Client-Konsole verfügbar sind:

* [Neuer Connector für den SMS-Versand](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=de) (FDA-Umgebungen)
* [Rest-APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=de) (nach Bedarf, FDA-Umgebungen)

Weitere Informationen finden Sie in den [Versionshinweisen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"} zur Client-Konsole.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=de){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=de) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=de) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"}.

-->

### Verbesserungen {#25-7-improvements}

* Sie können jetzt die Zielpopulation direkt für jede Bedingung und Gruppe im Regel-Builder berechnen. Klicken Sie auf die Ergebnisnummer, um die detaillierte Liste der Einträge anzuzeigen. [Weitere Informationen](../query/build-query.md#validate-query)

* Sie können jetzt einen vordefinierten Filter direkt im Regel-Builder bearbeiten oder löschen. [Weitere Informationen](../get-started/predefined-filters.md#manage-predefined-filter)

* Beim Konfigurieren eines SMS-Versands haben Sie jetzt im Abschnitt **SMS** Zugriff auf die **optionalen SMPP-Parameter (TLV)**. Dieser Parameter entspricht dem Parameter in der Client-Konsole. [Weitere Informationen](../advanced-settings/delivery-settings.md#sms-tab)

* Sie können jetzt Hintergrundbenachrichtigungen für iOS mit der neuen Option **Inhalt verfügbar** aktivieren, die im Abschnitt **Erweiterte Einstellungen** des Bildschirms zur iOS-Inhaltsbearbeitung verfügbar ist. Dadurch wird die Markierung `content-available:1` in der `aps`-Payload hinzugefügt. Weitere Informationen finden Sie [auf dieser Seite](../push/content-push.md). Siehe auch [diese Seite](../push/rich-push-ios.md)

* Die folgenden Verbesserungen für Landingpages sind jetzt verfügbar:

   * Sie können nun beim Konfigurieren eines Dienstes auf eine standardmäßige Landingpage zur An-/Abmeldung verweisen. Wenn Sie bei der Erstellung einer E-Mail einen Link zu dieser Landingpage definieren, werden die Benutzenden, die das Landingpage-Formular senden, automatisch für diesen Dienst angemeldet bzw. von ihm abgemeldet. [Weitere Informationen](../audience/manage-services.md#create-service)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht anonymen Besuchenden, auf die Landingpage zuzugreifen. Wenn Sie diese Option deaktivieren, können nur identifizierte Benutzende auf das Formular zugreifen und dieses absenden. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht, zusätzliche interne Daten bei der Landingpage-Übermittlung zu speichern. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option ermöglicht Ihnen die Verwendung einer Landingpage für mehrere Dienste, wodurch sie dynamisch wird. Wenn Sie einen Link zu einer E-Mail hinzufügen und eine dynamische Landingpage auswählen, können Sie einen beliebigen Dienst auswählen. Wenn Sie eine Landingpage auswählen, der ein bestimmter Dienst zugeordnet ist, wird dieser Dienst automatisch verwendet. Sie können keinen anderen Dienst auswählen. [Weitere Informationen](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Bedingte Inhalte werden nun auf Landingpages unterstützt. [Weitere Informationen](../landing-pages/lp-content.md)
   * Es ist jetzt möglich, eine Landingpage mit einem Dienst zu verknüpfen und eine Bestätigungsnachricht zu versenden, wenn Benutzende dies validieren. [Weitere Informationen](../landing-pages/lp-content.md#lp-message)
   * Sie können Captcha zum Schutz Ihrer Landingpage vor Spam und Missbrauch durch Bots hinzufügen. Dies erfordert nur wenig Einsatz aufseiten Ihrer Kundschaft, da nur eine Interaktion mit Ihrer Website erforderlich ist. [Weitere Informationen](../landing-pages/create-lp.md#captcha)
