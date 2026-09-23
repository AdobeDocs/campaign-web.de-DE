---
title: Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der neuesten Version der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 73553f19c6e88256f0e9f38479bdfc292a3221f8
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# Versionshinweise {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Versionshinweise"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden die Versionshinweise zu Campaign mehrmals im Monat mit den neuesten Funktionen, Verbesserungen und Fehlerbehebungen aktualisiert. Wir empfehlen Ihnen, sich diese regelmäßig anzusehen."

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

## Version September &#39;26 {#26-9-release}

_22. September 2026_

### Neue Funktionen {#26-9-features}

<table>
<thead>
<tr>
<th><strong>LINE-Kanal</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign unterstützt jetzt den <strong>LINE</strong>-Kanal, eine beliebte Instant Messaging-Anwendung. Erstellen und senden Sie LINE-Nachrichten mithilfe von Text-, Bild- oder Videoinhalten in eigenständigen Sendungen oder in Workflows neben Ihren anderen Kanälen. <a href="../line/get-started-line.md">Mehr dazu</a></p>
</td>
</tr>
</tbody>
</table>

### Verbesserungen {#26-9-improvements}

* **Seitennavigationszugriff**: Administratoren können jetzt bestimmte Menüeinträge in der Seitennavigation ausblenden. [Weitere Informationen](../administration/schemas-browse-access.md#screen-def)
* **Zusätzliche Validierungstypen**: Sie können jetzt neben Inhalts- und Zielgruppengenehmigungen auch Budget- und Versandstart-Genehmigungen für Campaign-Sendungen verlangen. [Weitere Informationen](../campaigns/campaign-approvals.md#configure-approvals)
* **Besucherbasiertes SMS-Targeting**: Das Besucher-Zielgruppen-Mapping ist jetzt für SMS-Sendungen verfügbar. [Weitere Informationen](../sms/create-sms.md)
* **Schaltfläche zum Abbrechen des Workflows**: Mit der neuen Schaltfläche **Abbrechen** können Sie nicht gespeicherte Änderungen in einem Workflow rückgängig machen. [Weitere Informationen](../workflows/orchestrate-activities.md#save-cancel)
* **Deduplizierung mit mehreren Werten**: Die Option **Nach einer Liste von Werten** unterstützt jetzt mehrere Attribute. [Weitere Informationen](../workflows/activities/deduplication.md#deduplication-configuration)
* **Mobile-Zielgruppen-Mapping**: Sie können jetzt Zielgruppen-Mappings für Mobile-App-Ziele erstellen. [Weitere Informationen](../administration/target-mappings.md#create-mapping)
* **Anreicherung externer Datenbanken**: Sie können jetzt Daten aus einer externen Datenbank in der Aktivität **Anreicherung** oder **Zielgruppe erstellen** anreichern. [Weitere Informationen](../workflows/activities/enrichment.md#external-data)
* **Abstimmung der Dateizielgruppe**: Sie können jetzt konfigurieren, ob Empfängerinnen und Empfänger in die Datenbank importiert werden sollen, wenn die Zielgruppe aus einer Datei ausgewählt wird. [Weitere Informationen](../audience/file-audience.md#upload)
* **Direkte Joins für Sammlungen**: Wenn Sie ein Attribut direkt aus einer Sammlung auswählen, können Sie jetzt auswählen, wie die Bedingung erstellt wird: mithilfe der empfohlenen Standardoption, einer Aggregatfunktion oder einer erweiterten direkten Join. [Weitere Informationen](../query/build-query.md#links)

