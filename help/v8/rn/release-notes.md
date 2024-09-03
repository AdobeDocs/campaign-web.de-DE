---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## August - Versionshinweise {#24-8-release}

**Veröffentlichungsdatum**: 3. September 2024

Die folgenden Funktionen und Verbesserungen sind ab der August-Version verfügbar.

* **Werteverteilung** - Beim Zugriff auf die Liste der zur Personalisierung vorgesehenen Felder können Sie jetzt überprüfen, wie die Werte für jedes Feld verteilt werden. Ein dediziertes Popup-Fenster zeigt die Anzahl und den Prozentsatz für jeden Wert an. [Weitere Informationen](../query/build-query.md#distribution-values-query)

* **SMTP-Parameter** - SMTP-Einstellungen sind jetzt in den E-Mail-Versandeinstellungen verfügbar. [Weitere Informationen](../advanced-settings/delivery-settings.md#smtp)

* **Globale Variablen** - Sie können jetzt globale Variablen definieren, um Werte für Ihre Sendungen zu definieren. [Weitere Informationen](../advanced-settings/delivery-settings.md#variables-delivery)

### Neue Funktionen in eingeschränkter Verfügbarkeit {#acs-24-8}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.
>
>Weitere Informationen finden Sie auf den folgenden Dokumentationsseiten: [Campaign Standard Übergang zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de){target="_blank"}.

* **Branding für Briefpost** - Technische Administratoren können jetzt eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Identität einer Marke auswirken. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Sie können diese Marken jetzt erstellen und mit Nachrichten oder Landingpages verknüpfen. Diese Konfiguration wird in Vorlagen verwaltet. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Abonnements mit Landingpages** - Jetzt können Sie eine Landingpage mit einem Dienst verknüpfen und eine Bestätigungsnachricht senden, wenn Benutzer sie validieren. [Weitere Informationen](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visuelle Fragmente** - Sie können jetzt visuelle Inhaltsfragmente archivieren. [Weitere Informationen](../content/create-fragment.md#archive)

* **Captcha in Landingpages** - Sie können jetzt Captcha hinzufügen, um Ihre Landingpage vor Spam und Missbrauch durch Bots zu schützen. Dies erfordert nur wenig Einsatz aufseiten Ihrer Kunden, da nur eine Interaktion mit Ihrer Website erforderlich ist. [Weitere Informationen](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
