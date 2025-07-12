---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62294ce1809caee8af770b376aad97bac71c942c
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 65%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind in den [Versionshinweisen 2024](release-notes-24.md) und [Versionshinweisen 2025](release-notes-25.md) aufgeführt.

## Updates Juli &#39;25 {#25-7-updates}

>[!AVAILABILITY]
>
>Um von diesen Updates profitieren zu können, muss Ihr Server auf mindestens 8.8.1 aktualisiert werden. Siehe die Client-Konsole [Versionshinweise](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"}.

Die folgenden Funktionen, die zuvor in eingeschränkter Verfügbarkeit veröffentlicht wurden, stehen nun allen Umgebungen zur Verfügung (allgemeine Verfügbarkeit):

* **Erstellung eines mehrsprachigen Versands**: In der Adobe Campaign Web-Benutzeroberfläche ist nun die Durchführung mehrerer E-Mail-Sendungen in verschiedenen Sprachen möglich. Mit der Funktion „Mehrsprachiger Versand“ können Sie die Standardsprache Ihres Versands sowie die verschiedenen Sprachen festlegen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in einer Vorschau in den von Ihnen ausgewählten Sprachen anzeigen. [Weitere Informationen](../email/edit-content.md#multilingual-delivery)

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=de){target="_blank"}
-->

* **Versandwarnung** Die Versandwarnungsfunktion ist ein System zur Verwaltung von Versandwarnungen, mit dem Benutzende automatisch Benachrichtigungen mit Informationen zur Ausführung ihrer Sendungen erhalten können. [Weitere Informationen](../msg/delivery-alerting.md)

* **Verbesserungen bei Landingpages** - Die folgenden Verbesserungen bei Landingpages sind jetzt verfügbar:

   * Sie können nun beim Konfigurieren eines Dienstes auf eine standardmäßige Landingpage zur An-/Abmeldung verweisen. Wenn Sie bei der Erstellung einer E-Mail einen Link zu dieser Landingpage definieren, werden die Benutzenden, die das Landingpage-Formular senden, automatisch für diesen Dienst angemeldet bzw. von ihm abgemeldet. [Weitere Informationen](../audience/manage-services.md#create-service)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht anonymen Besuchenden, auf die Landingpage zuzugreifen. Wenn Sie diese Option deaktivieren, können nur identifizierte Benutzende auf das Formular zugreifen und dieses absenden. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht, zusätzliche interne Daten bei der Landingpage-Übermittlung zu speichern. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option ermöglicht Ihnen die Verwendung einer Landingpage für mehrere Dienste, wodurch sie dynamisch wird. Wenn Sie einen Link zu einer E-Mail hinzufügen und eine dynamische Landingpage auswählen, können Sie einen beliebigen Dienst auswählen. Wenn Sie eine Landingpage auswählen, der ein bestimmter Dienst zugeordnet ist, wird dieser Dienst automatisch verwendet. Sie können keinen anderen Dienst auswählen. [Weitere Informationen](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Bedingte Inhalte werden nun auf Landingpages unterstützt. [Weitere Informationen](../landing-pages/lp-content.md)
   * Sie können eine Landingpage mit einem Service verknüpfen und eine Bestätigungsnachricht senden, wenn Benutzer sie validieren. [Weitere Informationen](../landing-pages/lp-content.md#lp-message)
   * Sie können CAPTCHA hinzufügen, um Ihre Landingpage vor Spam und Missbrauch durch Bots zu schützen. Dies erfordert nur wenig Einsatz aufseiten Ihrer Kundschaft, da nur eine Interaktion mit Ihrer Website erforderlich ist. [Weitere Informationen](../landing-pages/create-lp.md#captcha)

Die folgenden Funktionen, die zuvor nur in begrenztem Umfang verfügbar waren, sind jetzt **on demand)**:

* **Dynamisches Reporting** - Sie können jetzt auf das dynamische Reporting zugreifen, das vollständig anpassbare und Echtzeitberichte zur Messung der Wirkung Ihrer Marketing-Aktivitäten bereitstellt. Dadurch kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Ort und Alter sowie nach Daten von E-Mail-Kampagnen wie Öffnungen und Klicks ermöglicht. Dynamische Berichte sind auch für mehrsprachige E-Mail-Sendungen und Transaktionsnachrichten verfügbar. [Weitere Informationen](../reporting/dynamic-reporting/get-started-reporting.md)

* **Zentrales Branding** Ihre technischen Administratoren können jetzt eine oder mehrere Marken definieren, um die Parameter, die die Identität einer Marke beeinflussen, zu zentralisieren. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Sie können diese Marken erstellen und mit verschiedenen Nachrichten oder Landingpages verknüpfen. Diese Konfiguration wird in Vorlagen verwaltet. Branding-Optionen sind für alle Kanäle verfügbar, einschließlich SMS und Briefpost. [Weitere Informationen](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Diese Funktion ist nur für neue Implementierungen verfügbar.

Zusätzlich zu den oben aufgeführten Funktionen bietet diese Version auch eine Reihe von Funktionen, die in der Client-Konsole verfügbar sind:

* [Neuer SMS-Versand-Connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=de).
* [REST-APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=de)

Siehe die Client-Konsole [Versionshinweise](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"}.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=de){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->