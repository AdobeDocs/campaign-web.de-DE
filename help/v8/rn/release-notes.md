---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 98%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

Änderungen und Verbesserungen, die in früheren Versionen verfügbar sind, sind in den [Versionshinweisen 2024](release-notes-24.md) und [Versionshinweisen 2025](release-notes-25.md) aufgeführt.

## Aktualisierungen von Juli 2025 {#25-7-updates}

>[!AVAILABILITY]
>
>Damit Sie von diesen Aktualisierungen profitieren können, muss Ihr Server mindestens auf 8.8.1 aktualisiert sein. Weitere Informationen finden Sie in den [Versionshinweisen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"} zur Client-Konsole.

Die folgenden Funktionen, die zuvor in eingeschränkter Verfügbarkeit veröffentlicht waren, stehen nun allen Umgebungen zur Verfügung (allgemeine Verfügbarkeit):

* **Erstellung eines mehrsprachigen Versands**: In der Adobe Campaign Web-Benutzeroberfläche ist nun die Durchführung mehrerer E-Mail-Sendungen in verschiedenen Sprachen möglich. Mit der Funktion „Mehrsprachiger Versand“ können Sie die Standardsprache Ihres Versands sowie die verschiedenen Sprachen festlegen, in denen der Versand durchgeführt werden kann. Sie können diese Sendungen auch in einer Vorschau in den von Ihnen ausgewählten Sprachen anzeigen. [Weitere Informationen](../email/edit-content.md#multilingual-delivery)

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=de){target="_blank"}
-->

* **Versandwarnung**: Bei der Funktion „Versandwarnung“ handelt es sich um ein System zur Verwaltung von Warnungen, über das eine Benutzergruppe automatisch Benachrichtigungen mit Informationen zur Ausführung ihrer Sendungen erhält. [Weitere Informationen](../msg/delivery-alerting.md)

* **Verbesserungen für Landingpages**: Die folgenden Verbesserungen für Landingpages sind jetzt verfügbar:

   * Sie können nun beim Konfigurieren eines Dienstes auf eine standardmäßige Landingpage zur An-/Abmeldung verweisen. Wenn Sie bei der Erstellung einer E-Mail einen Link zu dieser Landingpage definieren, werden die Benutzenden, die das Landingpage-Formular senden, automatisch für diesen Dienst angemeldet bzw. von ihm abgemeldet. [Weitere Informationen](../audience/manage-services.md#create-service)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht anonymen Besuchenden, auf die Landingpage zuzugreifen. Wenn Sie diese Option deaktivieren, können nur identifizierte Benutzende auf das Formular zugreifen und dieses absenden. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option in der Landingpage-Konfiguration ermöglicht, zusätzliche interne Daten bei der Landingpage-Übermittlung zu speichern. [Weitere Informationen](../landing-pages/create-lp.md#create-landing-page)
   * Eine neue Option ermöglicht Ihnen die Verwendung einer Landingpage für mehrere Dienste, wodurch sie dynamisch wird. Wenn Sie einen Link zu einer E-Mail hinzufügen und eine dynamische Landingpage auswählen, können Sie einen beliebigen Dienst auswählen. Wenn Sie eine Landingpage auswählen, der ein bestimmter Dienst zugeordnet ist, wird dieser Dienst automatisch verwendet. Sie können keinen anderen Dienst auswählen. [Weitere Informationen](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Bedingte Inhalte werden nun auf Landingpages unterstützt. [Weitere Informationen](../landing-pages/lp-content.md)
   * Es ist jetzt möglich, eine Landingpage mit einem Dienst zu verknüpfen und eine Bestätigungsnachricht zu versenden, wenn Benutzende dies validieren. [Weitere Informationen](../landing-pages/lp-content.md#lp-message)
   * Sie können Captcha zum Schutz Ihrer Landingpage vor Spam und Missbrauch durch Bots hinzufügen. Dies erfordert nur wenig Einsatz aufseiten Ihrer Kundschaft, da nur eine Interaktion mit Ihrer Website erforderlich ist. [Weitere Informationen](../landing-pages/create-lp.md#captcha)

Die folgenden Funktionen, die zuvor in eingeschränkter Verfügbarkeit veröffentlicht waren, sind jetzt **auf Anfrage** verfügbar:

* **Dynamische Berichte**: Sie können nun auf dynamische Berichte zugreifen, die vollständig anpassbare Berichte und Echtzeitberichte zum Messen der Wirkung Ihrer Marketing-Aktivitäten bieten. Dadurch kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Ort und Alter ermöglicht, zusätzlich zur Analyse basierend auf Daten von E-Mail-Kampagnen wie Öffnungen und Klicks. Dynamische Berichte sind auch für mehrsprachige E-Mail-Sendungen und Transaktionsnachrichten verfügbar. [Weitere Informationen](../reporting/dynamic-reporting/get-started-reporting.md)

* **Zentralisiertes Branding**: Ihre technischen Admins können nun eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Markenidentität auswirken. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Sie können diese Marken erstellen und mit verschiedenen Nachrichten oder Landingpages verknüpfen. Diese Konfiguration wird in Vorlagen verwaltet. Branding-Optionen sind für alle Kanäle verfügbar, einschließlich SMS und Briefpost. [Weitere Informationen](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Diese Funktion ist nur für neue Implementierungen verfügbar.

Zusätzlich zu den oben aufgeführten Funktionen bietet diese Version auch eine Reihe von Funktionen, die in der Client-Konsole verfügbar sind:

* [Neuer SMS-Versand-Connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=de). (FDA-Umgebungen)
* [Rest-APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=de) (On-Demand, FDA-Umgebungen)

Weitere Informationen finden Sie in den [Versionshinweisen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de){target="_blank"} zur Client-Konsole.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=de){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->