---
audience: end-user
title: Verwenden der Workflow-Aktivität Audience erstellen
description: Erfahren Sie, wie Sie die Workflow-Aktivität Audience erstellen verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 4c0157c0457d1d6fa3194463adef8572017af8f0
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 10%

---


# Zielgruppe aufbauen {#build-audience}

Mithilfe dieser Aktivität können Sie eine Audience definieren. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Regel-Builder verwenden, um Ihre eigene Abfrage zu definieren.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

Führen Sie die folgenden Schritte aus, um die **Audience erstellen** Aktivität:

1. Fügen Sie die Aktivität Audience erstellen hinzu.
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
