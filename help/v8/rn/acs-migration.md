---
audience: end-user
title: Wechsel von Campaign Standard zu Adobe Campaign Web
description: Funktionsweise der Campaign Web-Benutzeroberfläche
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 99%

---

# Wechsel von Campaign Standard zu Campaign v8 {#acs-to-ac}

Benutzende von Adobe Campaign Standard sind nun berechtigt, zu Adobe Campaign Managed Cloud Services v8 zu wechseln. Dieser Wechsel bietet zahlreiche Vorteile:

* **Robuste IT-Infrastruktur**: Managed Cloud Services v8 bietet eine robustere IT-Infrastruktur, die eine höhere Performance, Zuverlässigkeit und Skalierbarkeit von Kampagnen gewährleistet.
* **Verbesserter Support**: Das Managed Cloud Services-Team bietet erstklassige Unterstützung und stellt so einen reibungslosen Wechsel sowie fortlaufendes Monitoring Ihrer Plattform sicher. Der Support umfasst Fehlerbehebung und proaktive Wartung.
* **Integration mit Adobe Experience Platform**: Managed Cloud Services v8 verbindet sich nahtlos mit Adobe Experience Platform, sodass Benutzende ihre Daten vollständig nutzen und kanalübergreifend personalisierte, wirkungsvolle Kampagnen senden können.
* **Konsistente Benutzeroberfläche und Erlebnisse**: Der Wechsel zu Managed Cloud Services v8 führt zu keinerlei Unterbrechung von Workflows. Benutzeroberfläche und Benutzererlebnisse sind vertraut und können wie gewohnt genutzt werden, was eine minimale Lernkurve für Teams sicherstellt.

**Wenn Sie von Campaign Standard zu Campaign v8 wechseln, finden Sie [in diesem Dokument](../../adoption/home.md) Informationen zu den ersten Schritten.**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Wichtigste Funktionen {#key-features}

Benutzende von Campaign v8 haben Zugriff auf die neue Campaign Web-Benutzeroberfläche und die v8-Konsole. Daten und Einstellungen werden zwischen Umgebungen synchronisiert. Alle Daten und Einstellungen, die in der Client-Konsole verfügbar sind, sind in der Campaign Web-Benutzeroberfläche im linken Navigationsbereich des Explorers sichtbar. [Weitere Informationen](../get-started/user-interface.md#user-interface-explorer)

Die Campaign Web-Benutzeroberfläche wurde für Marketing-Fachleute entwickelt, damit diese Kampagnen einfach erstellen und koordinieren können. Die wichtigsten Funktionen der Web-Benutzeroberfläche von Campaign v8 umfassen:

* **Modernes, intuitives und einheitliches Erlebnis** [Weitere Informationen](../get-started/connect-to-campaign.md).
* **Neue leistungsstarke Funktionen und nahtlose Prozesse** [Weitere Informationen](../get-started/user-interface.md).
* **Vereinfachter und intuitiver Abfrage-Modeler** [Weitere Informationen](../query/query-modeler-overview.md).
* **Integrierte Funktionen zum Cross-Channel-Kampagnen-Management** [Weitere Informationen](../msg/gs-messages.md).
* **Neu gestaltete Kampagnen-Workflow-Aktivitäten** [Weitere Informationen](../workflows/gs-workflows.md).
* **Einfache Erstellung und Verwaltung von Profilen** [Weitere Informationen](../audience/about-recipients.md).
* **Vordefinierte Filter** [Weitere Informationen](../get-started/predefined-filters.md).
* **HTML-Konvertierer für E-Mail-Design** [Weitere Informationen](../email/existing-content.md).
* **SMS mit Angeboten** [Weitere Informationen](../msg/offers.md).

Die Campaign-Client-Konsole ist für Admins sowie für Entwicklerinnen und Entwickler vorgesehen, damit diese ihre Umgebung konfigurieren und anpassen können. Die wichtigsten in der Campaign-Client-Konsole verfügbaren Funktionen werden in dieser [Dokumentation](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/new/whats-new){target="_blank"} beschrieben.

>[!NOTE]
>
>[Auf dieser Seite](../get-started/capability-matrix.md) erfahren Sie mehr über unterstützte und nicht unterstützte Funktionen sowie über die Interoperabilität zwischen der Campaign Web-Benutzeroberfläche und der Campaign-Client-Konsole.

## Terminologie {#terminology}

Die meisten Konzepte in Campaign v8 und Campaign Standard sind sich ähnlich. Es gibt jedoch einige Unterschiede bezüglich der Terminologie. Beispiele hierfür sind:

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

Um einen reibungslosen Wechsel zu Campaign v8 gewährleisten zu können, wurden wichtige Funktionen von Campaign Standard in Campaign v8 aufgenommen. Diese Funktionen werden in [dieser Dokumentation](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de){target=_blank} beschrieben und stehen nur Benutzenden zur Verfügung, die einen Wechsel von Campaign Standard durchführen.

* **Dynamisches Reporting**: Das dynamische Reporting ermöglicht anpassbare und in Echtzeit aktualisierte Berichte, um die Wirkung von Marketing-Aktivitäten zu messen. Es umfasst den Zugriff auf Profildaten für die demografische Analyse nach Profildimensionen wie Geschlecht, Ort und Alter sowie nach funktionalen Daten von E-Mail-Kampagnen wie Öffnungen und Klicks. [Weitere Informationen](../reporting/dynamic-reporting/get-started-reporting.md).

* **Zentrales Branding**: Adobe Campaign ermöglicht Unternehmen das Festlegen von Richtlinien bezüglich der optischen Darstellung und technischen Charakteristika ihrer Marken. Benutzende können Kundinnen und Kunden ihre Marke einheitlich präsentieren, von Logos bis hin zu technischen Aspekten wie E-Mail-Absender, URL oder Domains. [Weitere Informationen](../administration/branding/branding-gs.md).

* **REST-APIs**: Von Campaign Standard migrierte Benutzende können REST-APIs verwenden, um Integrationen für Adobe Campaign und Ökosysteme zu erstellen, indem sie Adobe Campaign mit anderen Technologien verbinden. [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=de){target="_blank"}.

* **Landingpages**: Die Landingpages von Campaign v8 umfassen Verbesserungen zur Gewährleistung der Vergleichbarkeit der Funktionen mit denen von Campaign Standard. Weitere Informationen finden Sie in den [Versionshinweisen](../rn/release-notes.md#new-24-4) und in der [Dokumentation](../landing-pages/get-started-lp.md) zu Landingpages.

* **Visuelle Fragmente**: Visuelle Fragmente sind wiederverwendbare visuelle Komponenten, die in einer oder mehreren E-Mail-Sendungen oder in Inhaltsvorlagen referenziert werden. Wird ein Fragment geändert, wird jeder Inhalt, der es verwendet, aktualisiert. Diese Funktionalität ermöglicht es Benutzenden aus dem Bereich Marketing, mehrere benutzerdefinierte Inhaltsbausteine vorab zu erstellen, um Nachrichten in einem verbesserten Design-Prozess schnell zusammenzustellen. [Weitere Informationen](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->