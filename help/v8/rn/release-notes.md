---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: a1b1a40be4d2004181f03bba5c43d0302d6f2c47
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 95%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## September-Updates {#9-2024}

<table>
<thead>
<tr>
<th><strong>Content Accelerator des KI-Assistenten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Nachdem Sie Ihre Nachricht erstellt und angepasst haben, stellen Sie sie mit dem AI Assistant Content Accelerator im Adobe Campaign Web auf die nächste Stufe. Mit diesem leistungsstarken Tool können Sie die Wirkung Ihrer Inhalte optimieren, indem Sie eine Reihe ansprechender Texte, Haupttitel und visuell überzeugender Bilder generieren.</p>
<p>Nehmen Sie an unserer <a href="https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator">Live-Funktionsvorstellung</a> teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.</a></p>
<p>Weitere Informationen finden Sie in der <a href="../email/generative-gs.md">entsprechenden Dokumentation</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Verfügbarkeitsdatum: 12. September</p>
</td>
</tr>
</tbody>
</table>

## Versionshinweise für August {#24-8-release}

**Veröffentlichungsdatum**: 3. September 2024

Die folgenden Funktionen und Verbesserungen sind ab der Version August verfügbar.

* **Werteverteilung**: Beim Zugriff auf die Liste der zur Personalisierung vorgesehenen Felder kann jetzt überprüft werden, wie die Werte für jedes Feld verteilt werden. Ein dediziertes Popup-Fenster zeigt die Anzahl und den Prozentsatz für jeden Wert an. [Weitere Informationen](../query/build-query.md#distribution-values-query)

* **SMTP-Parameter**: SMTP-Einstellungen sind jetzt in den E-Mail-Versandeinstellungen verfügbar. [Weitere Informationen](../advanced-settings/delivery-settings.md#smtp)

* **Globale Variablen**: Sie können jetzt globale Variablen definieren, um Werte für Ihre Sendungen zu definieren. [Weitere Informationen](../advanced-settings/delivery-settings.md#variables-delivery)

### Neue Funktionen in eingeschränkter Verfügbarkeit {#acs-24-8}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.
>
>Weitere Informationen finden Sie auf den folgenden Seiten der Dokumentation: [Wechsel von Campaign Standard zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard-Benutzende](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de){target="_blank"}.

* **Branding für Briefpost**: Technische Admins können nun eine oder mehrere Marken definieren, um die Parameter zu zentralisieren, die sich auf die Markenidentität auswirken, z. B. das Logo der Marke, die Domain der Zugangs-URL zu den Landingpages, Einstellungen zum Nachrichten-Tracking. Diese Marken können jetzt erstellt und mit verschiedenen Nachrichten oder Landingpages verknüpft werden. Diese Konfiguration wird in Vorlagen verwaltet. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/experience-cloud/campaign/branding/branding-assign)

* **Abonnements mit Landingpages**: Es ist jetzt möglich, eine Landingpage mit einem Dienst zu verknüpfen und eine Bestätigungsnachricht zu versenden, wenn Benutzende dies validieren. [Weitere Informationen](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visuelle Fragmente**: Visuelle Inhaltsfragmente können jetzt archiviert werden. [Weitere Informationen](../content/create-fragment.md#archive)

* **Captcha in Landingpages**: Sie können jetzt Captcha zum Schutz Ihrer Landingpage vor Spam und Missbrauch durch Bots hinzufügen. Dies erfordert nur wenig Einsatz aufseiten Ihrer Kundschaft, da nur eine Interaktion mit Ihrer Website erforderlich ist. [Weitere Informationen](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
