---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 6581a2d6ab44b711ed6aea6736d60f932a7ce315
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 45%

---

# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Version Juni 2026 {#26-6-release}

_16. Juni 2026_

### Verbesserungen {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* Sie können jetzt Daten aus jedem Listenbildschirm einschließlich Trackinglogs exportieren. Suchen Sie Ihre Liste und klicken Sie einfach auf die Schaltfläche Exportieren . Der Export umfasst die derzeit geladenen Zeilen und berücksichtigt die auf dem Bildschirm angezeigten Spalten sowie alle aktiven Such- oder Filtervorgänge. [Weitere Informationen](../get-started/list-filters.md)

* Die **Deduplizierung** und **End**-Workflow-Aktivitäten unterstützen jetzt mehrere eingehende Transitionen. Wenn
Mehr als eine eingehende Transition ist verfügbar. Verwenden Sie hierzu den Abschnitt **Zusammenzufügende Sätze** in der Aktivität
Eigenschaften zur Auswahl der zu verbindenden Transitionen. Weitere Informationen finden Sie auf diesen Seiten: [Deduplizierung](../workflows/activities/deduplication.md),

<!--
[End](../workflows/activities/end.md)
-->

* Erweiterte Parameter werden jetzt im Abschnitt **Anreicherungsdaten** der Workflow-Aktivitäten **Zielgruppe erstellen** (Abfragetyp) und **Anreicherung** verfügbar gemacht. Mit diesen Parametern können Sie den Aufbau von Anreicherungsdaten feinabstimmen, einschließlich Gruppierung, Deduplizierung, Verarbeitung von Primärschlüsseln und eingehenden Ereignisdaten. [Weitere Informationen](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
