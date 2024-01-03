---
title: Arbeiten mit Empfängerinnen bzw. Empfängern und Zielgruppen
description: Erfahren Sie, wie Sie mit Empfängern und Audiences in Campaign Web arbeiten.
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 93%

---

# Arbeiten mit Empfängerinnen bzw. Empfängern und Zielgruppen {#about-recipients}

## Empfänger und Zielgruppen {#about}

In Adobe Campaign ist die Zielpopulation eines Versands eine Zielgruppe. Eine Zielgruppe ist eine Gruppe von Personen, die ähnliche Verhaltensweisen und/oder Merkmale aufweisen. Diese Personengruppe kann entweder generiert, ausgewählt oder geladen werden [wie unten beschrieben](#audiences).

In den meisten Fällen besteht die Zielgruppe aus Profilen, die als [Empfängerinnen und Empfänger](#recipients) in Adobe Campaign gespeichert werden. Sie können auch mit anderen Zielgruppen-Mappings arbeiten, indem Sie die Dimension ändern, wie [in diesem Abschnitt](#targeting-dimensions) beschrieben.

## Zielgruppendimensionen {#targeting-dimensions}

Die Zielgruppendimension, auch bekannt als Zielgruppen-Mapping, ist der Datentyp, den ein Vorgang verarbeitet. Sie ermöglicht die Bestimmung der Zielpopulation: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw.

Die Zielgruppendimension eines Workflows wird durch die erste Aktivität **[!UICONTROL Zielgruppe erstellen]** definiert und wird bis zum Ende des Workflows für alle weiteren Aktivitäten verwendet. Wenn Sie beispielsweise eine Abfrage an die aus der Datenbank stammenden Empfängerinnen und Empfänger durchführen, enthält die ausgehende Transition Daten vom Typ Empfängerinnen und Empfänger und wird an die nächste Aktivität übermittelt.

Beachten Sie, dass Sie die Zielgruppendimension in einem Workflow mithilfe der Aktivität [Dimensionsaktivität ändern](../workflows/activities/change-dimension.md) wechseln können. Auf diese Weise können Sie beispielsweise die Datenbank in einer bestimmten Tabelle (z. B. zu Käufen oder Abonnements) abfragen und die Zielgruppendimension in Empfängerinnen und Empfänger ändern, um Sendungen an die entsprechenden Empfängerinnen und Empfänger durchzuführen.

Standardmäßig haben die E-Mail- und SMS-Versandvorlagen **[!UICONTROL Empfängerinnen und Empfänger]** als Zielgruppe. Ihr Zielgruppen-Mapping verwendet daher die Felder der Tabelle **nms:recipient**. Für Push-Benachrichtigungen ist die standardmäßige Zielgruppendimension **Abonnierte Anwendungen (nms:appSubscriptionRcp)**, das mit der Empfängertabelle verknüpft ist.

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
