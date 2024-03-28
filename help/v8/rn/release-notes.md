---
title: Neueste Versionshinweise
description: Entdecken Sie neue Funktionen in der Campaign Web-Benutzeroberfläche.
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 99%

---

# Versionshinweise {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Neue Funktionen"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Versandmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Die Versionshinweise werden daher mehrmals im Monat aktualisiert. **Die Version vom März ist jetzt live** und umfasst den Briefpost-Kanal, die neue Workflow-Aktivität „Datenquelle ändern“ sowie weitere Verbesserungen."


<!--Last update: **March 19, 2024**-->

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Versandmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.

>[!AVAILABILITY]
>
>Diese Version steht allen Benutzenden ab [Campaign-Version (Konsole) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de) zur Verfügung. Weitere Informationen zu Versionen und Upgrades der Adobe Campaign-Client-Konsole finden Sie in der [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=de){target="_blank"}.

## März - Versionshinweise {#24-3-release}

**Veröffentlichungsdatum**: 19.–20. März 2024

### Briefpost-Kanal {#24-3-dm}

Der **Briefpost**-Kanal ist jetzt für die Verwendung in Workflows und für eigenständige Sendungen verfügbar. Briefpost ist ein Offline-Kanal, über den Sie Extraktionsdateien erstellen, personalisieren und generieren sowie diese an Ihre Briefpost-Dienstleister weitergeben können, um Ihrer Kundschaft Post zukommen zu lassen. [Weitere Informationen](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Neue Workflow-Aktivität „Datenquelle ändern“ {#24-3-change-data-source}

Mit der Targeting-Aktivität **Datenquelle ändern** können Sie die Datenquelle der von Ihrem Workflow verwendeten Arbeitstabelle ändern. Diese Aktivität bietet mehr Flexibilität, da Sie damit Daten in Ihren verschiedenen Datenbanken verwalten und die Leistung verbessern können. [Weitere Informationen](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Verbesserung der Workflow-Aktivität „Aufspaltung“ {#24-3-split}

Sie können jetzt die Option **Alle Teilmengen in derselben Tabelle erzeugen** in der Workflow-Aktivität **Aufspaltung** verwenden, um alle Teilmengen in einer einzigen ausgehenden Transition zu gruppieren. [Weitere Informationen](../workflows/activities/split.md)

### Abfrage-Modeler {#24-3-query-modeler}

* Das Abfragemodell ist jetzt im E-Mail-Designer verfügbar. Damit können Sie Bedingungen beim Erstellen bedingter Inhalte festlegen. [Weitere Informationen](../personalization/conditions.md)
* Beim Erstellen einer benutzerdefinierten Bedingung sind jetzt vordefinierte Werte für Attribute vom Typ „Datum“ verfügbar. [Weitere Informationen](../query/build-query.md)
* Operatoren können nicht mehr zu einer neuen Transition im Diagramm hinzugefügt werden. Sie können nur für eine vorhandene Transition hinzugefügt werden, bevor Komponenten gefiltert werden, um sie zu gruppieren. [Weitere Informationen](../query/build-query.md)
