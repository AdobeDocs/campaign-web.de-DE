---
audience: end-user
title: Wechsel von Campaign Standard zu Adobe Campaign Web
description: Funktionsweise der Campaign Web-Benutzeroberfläche
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# Wechsel von Campaign Standard zu Campaign v8 {#acs-to-ac}

Adobe Campaign Standard-Benutzende sind jetzt berechtigt, auf Adobe Campaign Managed Cloud Services v8 zu wechseln. Dieser Übergang bietet mehrere Vorteile:

* **Robuste IT-Infrastruktur**: Managed Cloud Services v8 bietet eine robustere IT-Infrastruktur und stellt so eine verbesserte Leistung, Zuverlässigkeit und Skalierbarkeit für Kampagnen sicher.
* **Verbesserter Support**: Das Managed Cloud Services-Team bietet erstklassige Unterstützung, um einen reibungslosen Übergang und eine kontinuierliche Plattformüberwachung sicherzustellen. Der Support umfasst Fehlerbehebung und proaktive Wartung.
* **Integration mit Adobe Experience Platform**: Managed Cloud Services v8 ist nahtlos mit Adobe Experience Platform verbunden, sodass Benutzende ihre Daten vollständig nutzen und kanalübergreifend personalisierte, wirkungsvolle Kampagnen durchführen können.
* **Konsistente Benutzeroberfläche und Erlebnis**: Die Umstellung auf Managed Cloud Services v8 unterbricht keine Workflows. Benutzer genießen weiterhin die vertraute Benutzeroberfläche und das vertraute Erlebnis, wodurch die Lernkurve für Teams minimiert wird.

**Wenn Sie von Campaign Standard zu Campaign v8 wechseln, finden Sie [in diesem Dokument](../../adoption/home.md) Informationen zu den ersten Schritten.**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Wichtigste Funktionen {#key-features}

Campaign v8-Benutzer haben Zugriff auf die neue Campaign Web-Benutzeroberfläche und die v8-Konsole. Daten und Einstellungen werden zwischen Umgebungen synchronisiert. Alle in der Client-Konsole verfügbaren Daten und Einstellungen sind in der Benutzeroberfläche von Campaign Web sichtbar, auf die über den linken Navigationsbereich des Explorers zugegriffen werden kann. [Weitere Informationen](../get-started/user-interface.md#user-interface-explorer)

Die Web-Benutzeroberfläche von Campaign wurde für Marketing-Experten entwickelt, um einfach Kampagnen zu erstellen und zu orchestrieren. Zu den wichtigsten Funktionen der Web-Benutzeroberfläche von Campaign v8 gehören:

* **Moderne, freundliche und einheitliche Erfahrung**. [Weitere Informationen](../get-started/connect-to-campaign.md).
* **Neue leistungsstarke Funktionen und nahtlose**. [Weitere Informationen](../get-started/user-interface.md).
* **Vereinfachter und intuitiver Abfrage-Modellierer**. [Weitere Informationen](../query/query-modeler-overview.md).
* **Integrierte kanalübergreifende Kampagnen-Management-Funktionen**. [Weitere Informationen](../msg/gs-messages.md).
* **Neu gestaltete Kampagnen-Workflow-Aktivitäten**. [Weitere Informationen](../workflows/gs-workflows.md).
* **Einfache Profilerstellung und -verwaltung**. [Weitere Informationen](../audience/about-recipients.md).
* **Vordefinierte Filter**. [Weitere Informationen](../get-started/predefined-filters.md).
* **HTML Converter für E-Mail-Design**. [Weitere Informationen](../email/existing-content.md).
* **SMS mit Angeboten** [Weitere Informationen](../msg/offers.md).

Die Campaign-Client-Konsole ist für Administratoren und Entwickler konzipiert, um ihre Umgebung zu konfigurieren und anzupassen. Die wichtigsten in der Campaign-Client-Konsole verfügbaren Funktionen werden im Detail in [dieser Dokumentation](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/new/whats-new){target="_blank"} beschrieben.

>[!NOTE]
>
>Erfahren Sie mehr über unterstützte und nicht unterstützte Funktionen und die Interoperabilität zwischen der Web-Benutzeroberfläche von Campaign und der Campaign-Client-Konsole [auf dieser Seite](../get-started/capability-matrix.md).

## Terminologie {#terminology}

Die meisten Konzepte in Campaign v8 und Campaign Standard sind sich ähnlich. Es gibt jedoch einige terminologische Unterschiede. Beispiele:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Spezifische Funktionen {#new-features}

Um einen reibungslosen Übergang zu Campaign v8 zu gewährleisten, wurden wichtige Campaign Standard-Funktionen zu Campaign v8 hinzugefügt. Diese Funktionen werden in [dieser Dokumentation) beschrieben ](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de){target="_blank} sind nur für Benutzer verfügbar, die von Campaign Standard wechseln.

* **Dynamisches Reporting**: Dynamische Berichte bieten anpassbare Echtzeitberichte, um die Wirkung von Marketing-Aktivitäten zu messen. Dazu gehört der Zugriff auf Profildaten für demografische Analysen nach Dimensionen wie Geschlecht, Stadt und Alter sowie auf funktionale E-Mail-Kampagnendaten wie Öffnungen und Klicks. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=de){target="_blank"}.

* **Zentrales Branding**: Mit Adobe Campaign können Unternehmen visuelle und technische Richtlinien für Marken definieren. Benutzer können Kunden eine konsistente Marke präsentieren, von Logos bis hin zu technischen Aspekten wie E-Mail-Absender, URL oder Domains. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=de).

* **REST-APIs**: Migrierte Campaign Standard-Benutzende können REST-APIs verwenden, um Integrationen für Adobe Campaign zu erstellen und Ökosysteme zu erstellen, indem sie Adobe Campaign mit anderen Technologien verbinden. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=de){target="_blank"}.

* **Landingpages**: Die Landingpages von Campaign v8 enthalten Verbesserungen, um die Funktionsgleichheit mit Campaign Standard sicherzustellen. Weitere Informationen finden Sie in den [Versionshinweisen](../rn/release-notes.md#new-24-4) und in der [Dokumentation](../landing-pages/get-started-lp.md) zu Landingpages.

* **Visuelle Fragmente**: Visuelle Fragmente sind wiederverwendbare visuelle Komponenten, auf die in einem oder mehreren E-Mail-Sendungen oder Inhaltsvorlagen verwiesen wird. Beim Ändern eines Fragments werden alle Inhalte aktualisiert, die es verwenden. Mit dieser Funktion können Marketing-Benutzer in einem verbesserten Design-Prozess mehrere benutzerdefinierte Inhaltsbausteine für die Schnellzusammenstellung von Nachrichten vorab erstellen. [Weitere Informationen](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->