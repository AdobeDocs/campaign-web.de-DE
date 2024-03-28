---
title: Neueste Versionshinweise
description: Entdecken Sie neue Funktionen in der Campaign Web-Benutzeroberfläche
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 30%

---

# Versionshinweise {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Neue Funktionen"
>abstract="Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem Modell der kontinuierlichen Bereitstellung, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Die Versionshinweise werden daher mehrmals im Monat aktualisiert. **Die Version vom März ist jetzt live** und umfasst unter anderem den Briefpost-Kanal, die neue Workflow-Aktivität „Datenquelle ändern“ und weitere Verbesserungen."


<!--Last update: **March 19, 2024**-->

Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem Modell der kontinuierlichen Bereitstellung, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Bitte überprüfen Sie sie regelmäßig.

>[!AVAILABILITY]
>
>Diese Version steht allen Benutzern zur Verfügung, die [Campaign (Konsole) Version 8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=de). Weitere Informationen zu den Versionen und Upgrades der Adobe Campaign-Clientkonsole finden Sie unter [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=de){target="_blank"}.

## März - Versionshinweise {#24-3-release}

**Veröffentlichungsdatum**: 19.-20. März 2024

### Briefpost-Kanal {#24-3-dm}

**Briefpost** -Kanal ist jetzt für die Verwendung in Workflows und als eigenständige Sendungen verfügbar. Briefpost ist ein Offline-Kanal, über den Sie Extraktionsdateien erstellen, personalisieren und generieren sowie diese an Ihre Briefpost-Dienstleister weitergeben können, um E-Mails an Ihre Kunden zu senden. [Weitere Informationen](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Neue Workflow-Aktivität &quot;Datenquelle ändern&quot; {#24-3-change-data-source}

Die **Datenquelle ändern** Die Zielgruppenbestimmungsaktivität ermöglicht die Änderung der Datenquelle, die von der Arbeitstabelle Ihres Workflows verwendet wird. Diese Aktivität bietet mehr Flexibilität, da Sie Daten in Ihren verschiedenen Datenbanken verwalten und die Leistung verbessern können. [Weitere Informationen](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Verbesserung der Aufspaltungs-Workflow-Aktivität {#24-3-split}

Sie können jetzt die **Alle Teilmengen in derselben Tabelle generieren** in der **Aufspaltung** Workflow-Aktivität, um alle Teilmengen in einer ausgehenden Transition zusammenzufassen. [Weitere Informationen](../workflows/activities/split.md)

### Abfrage-Modeler {#24-3-query-modeler}

* Das Abfragemodell ist jetzt in Email Designer verfügbar. Damit können Sie Bedingungen beim Erstellen bedingter Inhalte erstellen. [Weitere Informationen](../personalization/conditions.md)
* Beim Erstellen einer benutzerdefinierten Bedingung sind jetzt vordefinierte Werte für Attribute vom Typ Datum verfügbar. [Weitere Informationen](../query/build-query.md)
* Benutzer können nicht mehr zu einer neuen Transition im Diagramm hinzugefügt werden. Sie können nur für eine bestehende Transition hinzugefügt werden, bevor Komponenten gefiltert werden, um sie zu gruppieren. [Weitere Informationen](../query/build-query.md)
