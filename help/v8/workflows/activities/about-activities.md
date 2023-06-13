---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Workflow-Aktivitäten ausgeführt werden
badge: label="Alpha"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: b66afeedbfcb342102c833899756afc35de9d504
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 25%

---


# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenaktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Flusssteuerungsaktivitäten](#flow-control)

![](../assets/workflow-activities.png)

## Zielgruppenbestimmungsaktivitäten {#targeting}

Diese Aktivitäten dienen der Zielgruppenbestimmung, Manipulation und Anreicherung von Populationsdaten. Damit können Sie eine oder mehrere Zielgruppen erstellen, indem Sie eine Zielgruppe definieren und diese mithilfe von Schnittmengen-, Vereinigungs- oder Ausschlussvorgängen teilen oder kombinieren.

* Die [Audience erstellen](build-audience.md) ermöglicht die Bestimmung der Zielpopulation. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Regel-Builder verwenden, um Ihre eigene Abfrage zu definieren.
* Die [Kombinieren](combine.md) -Aktivität ermöglicht die Segmentierung Ihrer eingehenden Population. Sie können eine Vereinigung, eine Schnittmenge oder einen Ausschluss verwenden.
* Die [Anreicherung](enrichment.md) -Aktivität können Sie zusätzliche Daten definieren, die in Ihrem Workflow verarbeitet werden sollen. Mit dieser Aktivität können Sie die eingehende Transition nutzen und die Aktivität so konfigurieren, dass die ausgehende Transition mit zusätzlichen Daten ergänzt wird.

## Kanalaktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketingkampagnen über mehrere Kanäle hinweg automatisieren und ausführen, z. B. E-Mail, SMS oder Push-Benachrichtigungen. Sie können Kanalaktivitäten in der Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen Trigger-Aktionen basierend auf dem Kundenverhalten durchgeführt werden können.

Folgendes **Kanal** sind verfügbar:

* E-Mail
* Push-Benachrichtigung
* SMS

Näheres dazu finden Sie in [diesem Abschnitt](enrichment.md).

## Flusssteuerungsaktivitäten {#flow-control}

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Sie ermöglichen die Koordinierung der anderen Aktivitäten:

* Die [Und-Verknüpfung](and-join.md) ermöglicht die Synchronisation mehrerer Ausführungszweige eines Workflows.
* Die **Ende** -Aktivität können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional.
* Eine [Verzweigung](fork.md) erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten.
* Die [Warten](wait.md)-Aktivität ermöglicht das zeitweise Aussetzen der Ausführung eines Teils eines Workflows.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

