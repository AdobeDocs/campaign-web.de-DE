---
audience: end-user
title: Verwenden der Workflow-Aktivität Audience erstellen
description: Erfahren Sie, wie Sie die Workflow-Aktivität Audience erstellen verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 07da5f804e25382c6202b7438e15dafaee413f27
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 7%

---


# Zielgruppe aufbauen {#build-audience}

Die **Audience erstellen** -Aktivität **Targeting** Aktivität. Diese Aktivität ermöglicht die Bestimmung der Audience, die in den Workflow eintreten soll. Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Nachrichtenzielgruppe nicht in der Kanalaktivität, sondern im **Audience erstellen** Aktivität.

Zur Definition der Audience-Population haben Sie folgende Möglichkeiten:

* Wählen Sie eine vorhandene Zielgruppe aus, die als Liste in der Client-Konsole erstellt wurde.
* Wählen Sie eine Adobe Experience Platform-Zielgruppe aus.
* Erstellen Sie mit dem Regel-Builder eine neue Zielgruppe, indem Sie Filterkriterien definieren und kombinieren.

>[!NOTE]
>
>In diesem Zusammenhang können Sie keine Audience aus einer Datei laden. Dazu müssen Sie einen eigenständigen Versand erstellen. [Weitere Informationen](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Audience erstellen** Aktivität:

1. Hinzufügen einer **Audience erstellen** Aktivität.
1. Titel definieren.
1. Definieren Sie den Audience-Typ: **Erstellen eigener** oder **Audience lesen**.

Gehen Sie wie folgt vor, um eine eigene Abfrage zu erstellen:

1. Auswählen **Erstellen Sie Ihre eigene (Abfrage)**.
1. Wählen Sie die **Zielgruppendimension**. Die Zielgruppendimension ermöglicht die Bestimmung der vom Vorgang betroffenen Population: Empfänger, Empfänger, Betreiber, Abonnenten usw. Standardmäßig wird die Zielgruppe aus den Empfängern ausgewählt. Siehe Abschnitt [v8-Dokumentation](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Bestätigen Sie die Angaben mit der Schaltfläche **Fortfahren**.
1. Verwenden Sie den Regel-Builder, um Ihre Abfrage zu definieren, genauso wie Sie eine Zielgruppe beim Erstellen einer neuen E-Mail erstellen. Näheres dazu finden Sie in [diesem Abschnitt](../../audience/segment-builder.md).

Gehen Sie wie folgt vor, um eine vorhandene Zielgruppe auszuwählen:

1. Auswählen **Audience lesen**.
1. Bestätigen Sie die Angaben mit der Schaltfläche **Fortfahren**.
1. Wählen Sie Ihre Audience auf die gleiche Weise aus wie eine Audience beim Entwerfen einer neuen E-Mail. Näheres dazu finden Sie in [diesem Abschnitt](../../audience/add-audience.md).

## Beispiel

Hier ist ein Beispiel für einen Workflow mit zwei **Audience erstellen** Aktivitäten. Die erste Version richtet sich an die Pokerspieler-Audience, gefolgt von einem E-Mail-Versand. Die zweite Zielgruppe ist die Zielgruppe der VIP, gefolgt von einem SMS-Versand.

![](../assets/workflow-audience-example.png)