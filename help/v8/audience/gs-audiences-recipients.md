---
title: Erste Schritte mit Profilen und Audiences
description: Erfahren Sie, wie Sie mit Profilen und Audiences in Campaign Web arbeiten.
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 9e6f0a5894ae0b31d275f978553d7fc73ba9c2eb
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 65%

---

# Erste Schritte mit Profilen und Audiences {#about-profiles}

## Profile &amp; Audiences {#about}

In Adobe Campaign ist die Zielpopulation eines Versands eine Zielgruppe. Eine Zielgruppe ist eine Gruppe von Profilen, die ähnliche Verhaltensweisen und/oder Merkmale aufweisen. Diese Personengruppe kann entweder generiert, ausgewählt oder geladen werden [wie unten beschrieben](#audiences).

## Zielgruppendimensionen {#targeting-dimensions}

Die Zielgruppendimension, auch bekannt als Zielgruppen-Mapping, ist der Datentyp, den ein Vorgang verarbeitet. Sie ermöglicht die Bestimmung der Zielpopulation: Profile, Vertragsempfänger, Benutzer, Abonnenten etc.

Die Zielgruppendimension eines Workflows wird durch die erste Aktivität **[!UICONTROL Zielgruppe erstellen]** definiert und wird bis zum Ende des Workflows für alle weiteren Aktivitäten verwendet. Wenn Sie beispielsweise eine Abfrage bezüglich der Profile aus der Datenbank durchführen, enthält die ausgehende Transition Daten vom Typ &#39;recipient&#39; und wird an die nächste Aktivität übermittelt.

Beachten Sie, dass Sie die Zielgruppendimension in einem Workflow mithilfe der Aktivität [Dimensionsaktivität ändern](../workflows/activities/change-dimension.md) wechseln können. Auf diese Weise können Sie beispielsweise die Datenbank in einer bestimmten Tabelle (z. B. bei Käufen oder Abonnements) abfragen und dann die Zielgruppendimension in Empfänger ändern, um Sendungen an die entsprechenden Profile durchzuführen.

Standardmäßig sind die Zielprofile für E-Mail- und SMS-Versandvorlagen ausgewählt. Ihr Zielgruppen-Mapping verwendet daher die Felder der Tabelle **nms:recipient**. Für Push-Benachrichtigungen ist die standardmäßige Zielgruppendimension **Abonnierte Anwendungen (nms:appSubscriptionRcp)**, das mit der Empfängertabelle verknüpft ist.

Sie können auch andere integrierte Zielgruppen-Mappings in Ihren Workflows und Sendungen verwenden, die unten aufgeführt sind:

| Name | Verwendungszweck | Schema |
|---|---|---|
| Empfängerinnen und Empfänger | Versand an Empfänger (integrierte Empfängertabelle) | nms:recipient |
| Besucher | Versand an Besucher, deren Profile beispielsweise über Empfehlungen (Viral Marketing) erfasst wurden. | mns:visitor |
| Abonnements  | Versand richtet sich an Abonnenten eines Informationsdienstes wie z. B. einen Newsletter | nms:subscription |
| Besucher-Abonnements | Versand richtet sich an Besucher, die einen Informationsdienst beziehen | nms:visitorSub |
| Benutzer | Versand richtet sich an Adobe-Campaign-Benutzer | nms:operator |
| Externe Datei | Versand basiert auf einer Datei, die alle notwendigen Informationen enthält | Ohne Schema oder Zielgruppe |
| Abonnierte Anwendungen | Versand an Empfängerinnen und Empfänger, die eine Anwendung abonniert haben | nms:appSubscriptionRcp |

Zusätzlich können Sie je nach Bedarf ein neues Zielgruppen-Mapping erstellen. Dies erfolgt über die Client-Konsole. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=de#new-mapping){target="_blank"}.
