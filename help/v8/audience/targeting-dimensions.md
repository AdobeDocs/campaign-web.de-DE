---
title: Zielgruppendimensionen
description: Erfahren Sie mehr über Zielgruppendimensionen in Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 25%

---

# Zielgruppendimensionen {#targeting-dimensions}

>[!CONTEXTUALHELP]
>
Die Zielgruppendimension, auch als Zielgruppen-Mapping bezeichnet, ist der Datentyp, den ein Vorgang verarbeitet. Sie definiert die Zielpopulation, z. B. Profile, Vertragsbegünstigte, Benutzer oder Abonnenten.

## Zielgruppendimensionen von Workflows {#workflow}

Die Zielgruppendimension eines Workflows wird durch die erste Aktivität **[!UICONTROL Zielgruppe aufbauen]** definiert und für alle nachfolgenden Aktivitäten bis zum Ende des Workflows verwendet. Wenn Sie beispielsweise Profile aus der Datenbank abfragen, enthält die ausgehende Transition Daten vom Typ „Empfänger“, die an die nächste Aktivität übertragen werden.

Wechseln Sie die Zielgruppendimension in einem Workflow mithilfe einer Aktivität vom Typ [Dimensionsänderung](../workflows/activities/change-dimension.md). Dies ermöglicht die Abfrage der Datenbank für eine bestimmte Tabelle, z. B. Käufe oder Abonnements, und das anschließende Ändern der Zielgruppendimension auf Empfänger , um Sendungen an die entsprechenden Profile zu senden.

Bei der Auswahl einer Zielgruppendimension (in den Workflow-Einstellungen oder in Aktivitäten wie **Zielgruppe erstellen**, **Abstimmung** oder **Dimensionsänderung** wird standardmäßig eine Liste der häufig verwendeten Schemata angezeigt. Um alle verfügbaren Schemata anzuzeigen, schalten Sie die Schaltfläche **[!UICONTROL Alle Schemata anzeigen]** um. Die Optionsauswahl wird für jeden Benutzer bzw. jede Benutzerin gespeichert.

![Screenshot der Oberfläche der Zielgruppendimension mit aktivierter Schaltfläche „Alle Schemata anzeigen“.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Zielgruppendimensionen {#list}

Standardmäßig haben die E-Mail- und SMS-Versandvorlagen Profile als Zielgruppe. Ihre Zieldimension verwendet die Felder der Tabelle **nms:recipient**. Für Push-Benachrichtigungen ist die standardmäßige Zielgruppendimension **Abonnierte Anwendungen (nms:appSubscriptionRcp)**, das mit der Empfängertabelle verknüpft ist.

Verwenden Sie andere integrierte Zielgruppen-Mappings in Workflows und Sendungen, wie unten aufgeführt:

| Name | Für Versand an verwenden | Schema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Empfängerinnen und Empfänger | Profile/Empfänger (integrierte Empfängertabelle) | nms:recipient |
| Besucher | Besucherinnen und Besucher, deren Profile über eine Empfehlung erfasst wurden (z. B. Viral Marketing) | mns:visitor |
| Abonnements  | Profile, die einen Informationsdienst wie einen Newsletter abonniert haben | nms:subscription |
| Besucher-Abonnements | Besucherinnen und Besucher haben einen Informationsdienst abonniert | nms:visitorSub |
| Operatoren | Adobe Campaign-Benutzer | nms:operator |
| Externe Datei | Versand über eine Datei mit allen erforderlichen Informationen | Ohne Schema oder Zielgruppe |
| Abonnierte Anwendungen | An eine Anwendung abonnierte Profile | nms:appSubscriptionRcp |

Erstellen Sie außerdem neue Zielgruppen-Mappings basierend auf bestimmten Anforderungen. Führen Sie diesen Vorgang nur über die Client-Konsole aus. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=de#new-mapping){target="_blank"}.