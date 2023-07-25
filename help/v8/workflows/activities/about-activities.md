---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Sie Workflow-Aktivitäten durchführen.
badge: label="Alpha"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 96%

---


# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenbestimmungs-Aktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Flusskontroll-Aktivitäten](#flow-control)

![](../assets/workflow-activities.png)

## Zielgruppenbestimmungs-Aktivitäten {#targeting}

Diese Aktivitäten dienen der Zielgruppenbestimmung, Manipulation und Anreicherung von Populationsdaten. Sie ermöglichen es Ihnen, ein oder mehrere Ziele zu erstellen, indem Sie eine Zielgruppe definieren und diese Zielgruppen mithilfe von Schnittmenge, Vereinigung oder Ausschluss aufteilen oder kombinieren.

* Mit der Aktivität [Zielgruppe erstellen](build-audience.md) können Sie Ihre Zielgruppenpopulation definieren. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Regel-Builder verwenden, um Ihre eigene Abfrage zu definieren.
* Die Aktivität [Kombinieren](combine.md) ermöglicht die Segmentierung Ihrer eingehenden Population. Sie können eine Vereinigung, eine Schnittmenge oder einen Ausschluss verwenden.
* Mit der Aktivität [Anreicherung](enrichment.md) können Sie zusätzliche Daten definieren, die in Ihrem Workflow verarbeitet werden sollen. Mit dieser Aktivität können Sie die eingehende Transition nutzen und entsprechend der Konfiguration der Aktivität die ausgehende Transition mit Zusatzdaten ergänzen.
* Die [Aufspaltung](split.md) ermöglicht die Segmentierung der eingehenden Population in mehrere Teilmengen.

## Kanalaktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketing-Kampagnen über mehrere Kanäle wie E-Mail, SMS oder Push automatisieren und durchführen. Sie können Kanalaktivitäten in der Arbeitsfläche kombinieren, um Cross-Channel-Workflows zu erstellen, mit denen basierend auf dem Kundenverhalten Aktionen ausgelöst werden können.

Die folgenden **Kanalaktivitäten** sind verfügbar:

* E-Mail
* Push
* SMS

Näheres dazu finden Sie in [diesem Abschnitt](enrichment.md).

## Flussskontroll-Aktivitäten {#flow-control}

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Ihre Hauptaufgabe ist es, die anderen Aktivitäten zu koordinieren:

* Die Aktivität [Und-Verknüpfung](and-join.md) ermöglicht es, die Ausführung verschiedener Workflow-Verzweigungen zu synchronisieren.
* Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional.
* Eine [Verzweigung](fork.md) erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten.
* Die Aktivität [Warten](wait.md) unterbricht vorübergehend die Ausführung eines Teils eines Workflows.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

