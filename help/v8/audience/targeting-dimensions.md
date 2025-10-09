---
title: Zielgruppen- und Filterdimensionen
description: Erfahren Sie mehr über Zielgruppen- und Filterdimensionen in der Adobe Campaign Web-Benutzeroberfläche
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 100%

---

# Zielgruppen- und Filterdimensionen {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Auswählen der Zielgruppendimension"
>abstract="Die Zielgruppendimension ermöglicht die Bestimmung der vom Vorgang betroffenen Population: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw. Standardmäßig wird die Zielgruppe für E-Mails und SMS in der integrierten Tabelle der Empfängerinnen und Empfänger ausgewählt. Bei Push-Benachrichtigungen ist die Standard-Zielgruppendimension „Abonnierte Anwendungen“."

Bei der Zielgruppendimension, auch als Zielgruppen-Mapping bezeichnet, handelt es sich um den Datentyp, den ein Vorgang verarbeitet. Sie definiert die Zielpopulation, z. B. Profile, Vertragsbegünstigte, Benutzende oder Abonnierende. Mit der Filterdimension können Sie Filter auf die Zielpopulation anwenden, indem Sie auf zugehörige Kriterien verweisen, ohne die Hauptzielgruppendimension zu ändern.

## Zielgruppendimensionen {#targeting}

Die Zielgruppendimension eines Workflows wird durch die erste Aktivität **[!UICONTROL Zielgruppe erstellen]** definiert und wird bis zum Ende des Workflows für alle nachfolgenden Aktivitäten verwendet. Wenn Sie beispielsweise Profile aus der Datenbank abfragen, enthält die ausgehende Transition Daten vom Typ „Empfänger“, die an die nächste Aktivität übertragen werden.

Wechseln Sie die Zielgruppendimension in einem Workflow mithilfe der Aktivität [Dimensionsänderung](../workflows/activities/change-dimension.md). Auf diese Weise können Sie die Datenbank im Hinblick auf eine bestimmte Tabelle (z. B. zu Käufen oder Abonnements) abfragen und die Zielgruppendimension in „Empfänger“ ändern, um Sendungen an die entsprechenden Profile durchzuführen.

Bei der Auswahl einer Zielgruppendimension (in den Workflow-Einstellungen oder in Aktivitäten wie **Zielgruppe erstellen**, **Abstimmung** oder **Dimensionsänderung**) wird standardmäßig eine Liste häufig verwendeter Schemata angezeigt. Um alle verfügbaren Schemata anzuzeigen, aktivieren Sie die Schaltfläche **[!UICONTROL Alle Schemata anzeigen]**. Die Optionsauswahl wird für jeden Benutzer bzw. jede Benutzerin gespeichert.

![Screenshot der Zielgruppendimension-Benutzeroberfläche mit aktivierter Schaltfläche „Alle Schemata anzeigen“](assets/targeting-dimension-show-all.png){zoomable="yes"}

Standardmäßig haben die E-Mail- und SMS-Versandvorlagen Profile als Ziel. Ihre Zielgruppendimension verwendet daher die Felder der Tabelle **nms:recipient**. Für Push-Benachrichtigungen ist die standardmäßige Zielgruppendimension **Abonnierte Anwendungen (nms):appSubscriptionRcp**, die mit der Empfängertabelle verknüpft ist.

Verwenden Sie andere integrierte Zielgruppen-Mappings in Workflows und Sendungen, wie unten aufgeführt:

| Name | Für den Versand an | Schema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Empfängerinnen und Empfänger | Profile/Empfängerinnen und Empfänger (integrierte Empfängertabelle) | nms:recipient |
| Besuchende | Besuchende, deren Profile beispielsweise über Empfehlungen (z. B. Viral Marketing) erfasst wurden | mns:visitor |
| Abonnements     | Profile, die einen Informationsdienst abonniert haben, z. B. einen Newsletter | nms:subscription |
| Besucher-Abonnements | Besuchende, die einen Informationsdienst abonniert haben | nms:visitorSub |
| Operatoren | Adobe Campaign-Benutzende | nms:operator |
| Externe Datei | Versand über eine Datei mit allen erforderlichen Informationen | Ohne Schema oder Zielgruppe |
| Abonnierte Anwendungen | Profile, die eine Anwendung abonniert haben | nms:appSubscriptionRcp |

Erstellen Sie außerdem neue Zielgruppen-Mappings basierend auf bestimmten Anforderungen. Führen Sie diesen Vorgang nur über die Client-Konsole aus. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=de#new-mapping){target="_blank"}.

## Filterdimensionen {#filtering}

Die Zielgruppendimension ermöglicht die Bestimmung der vom Vorgang betroffenen Population: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw. Mit der Filterdimension können Sie Filter auf diese Population anwenden, indem Sie auf zugehörige Daten verweisen, ohne die Hauptzielgruppendimension zu ändern. Sie können beispielsweise die Population anhand bestimmter Kriterien wie Vertragsinhabende oder Newsletter-Abonnierende auswählen.

Filterdimensionen sind nur in der Aktivität **Zielgruppe erstellen** verfügbar.

Um Kundinnen und Kunden auszuwählen, die seit mehr als 5 Jahren über eine Lebensversicherung verfügen, wählen Sie Folgendes aus:

* Zielgruppendimension: **Kundinnen und Kunden**
* Filterdimension: **Vertragsinhabende**.

Anschließend können Sie die Filterbedingungen in der Aktivität **Zielgruppe erstellen** definieren. Mehr dazu erfahren Sie auf [dieser Seite](../workflows/activities/build-audience.md).

Nach Auswahl einer Zielgruppendimension stehen nur die kompatiblen Filterdimensionen auf der Benutzeroberfläche zur Verfügung. Diese zwei Dimensionen müssen miteinander in Zusammenhang stehen. Der Inhalt der Liste der Filterdimensionen hängt somit von der im ersten Feld ausgewählten Zielgruppendimension ab.
