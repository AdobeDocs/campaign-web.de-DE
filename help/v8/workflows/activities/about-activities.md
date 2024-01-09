---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Sie Workflow-Aktivitäten durchführen.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: a0611ac41957b4bd7796c4c42c40232fba1dfc2b
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 39%

---


# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppen- und Datenverwaltungsaktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Aktivitäten zur Flusskontrolle](#flow-control)

![](../assets/workflow-activities.png)

## Zielgruppen- und Datenverwaltungsaktivitäten {#targeting}

Diese Aktivitäten dienen der Zielgruppenbestimmung, Manipulation und Anreicherung von Populationsdaten. Sie ermöglichen es Ihnen, ein oder mehrere Ziele zu erstellen, indem Sie eine Zielgruppe definieren und diese Zielgruppen mithilfe von Schnittmenge, Vereinigung oder Ausschluss aufteilen oder kombinieren.

* Verwenden Sie die [Audience-Speicherung](save-audience.md) -Aktivität, um eine existierende Audience zu aktualisieren oder eine neue Audience aus der zuvor durch einen Workflow berechneten Population zu erstellen.
* Verwenden Sie die [Audience erstellen](build-audience.md) Aktivität zur Bestimmung der Zielpopulation. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Regel-Builder verwenden, um Ihre eigene Abfrage zu definieren.
* Verwenden Sie die [Kombinieren](combine.md) -Aktivität zur Segmentierung Ihrer eingehenden Population. Sie können eine Vereinigung, eine Schnittmenge oder einen Ausschluss verwenden.
* Verwenden Sie die [Aufspaltung](split.md) Aktivität zur Segmentierung der eingehenden Population in mehrere Teilmengen.
* Verwenden Sie die [Abstimmung](reconciliation.md) -Aktivität, um die Relation zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle zu definieren, z. B. Daten, die aus einer externen Datei geladen werden.
* Verwenden Sie die [Anreicherung](enrichment.md) -Aktivität, um zusätzliche Daten zu definieren, die in Ihrem Workflow verarbeitet werden sollen. Mit dieser Aktivität können Sie die eingehende Transition nutzen und entsprechend der Konfiguration der Aktivität die ausgehende Transition mit Zusatzdaten ergänzen.
* Verwenden Sie die [Deduplizierung](deduplication.md) Aktivität zum Löschen von Dubletten in den Ergebnissen der eingehenden Aktivitäten.
* Verwenden Sie die [Dimensionsänderung](change-dimension.md) Aktivität , um die Zielgruppendimension während der Workflow-Erstellung zu ändern.
* Verwenden Sie die [Datei laden](load-file.md) -Aktivität verwenden, um mit Profilen und Daten zu arbeiten, die in einer externen Datei gespeichert sind.


## Kanalaktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketingkampagnen über mehrere Kanäle hinweg automatisieren und ausführen. Sie können Kanalaktivitäten in der Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen Trigger-Aktionen basierend auf dem Kundenverhalten durchgeführt werden können. Die folgenden **Kanal** sind verfügbar: E-Mail-, SMS-, Android- und iOS-Push-Benachrichtigungen. [Erfahren Sie, wie Sie einen Versand im Rahmen eines Workflows einrichten.](channels.md).

## Aktivitäten zur Flusskontrolle {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Endaktivität"
>abstract="Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional."

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Ihre Hauptaufgabe ist es, die anderen Aktivitäten zu koordinieren:

* Verwenden Sie die [Planung](scheduler.md) -Aktivität, um zu planen, wann der Workflow gestartet wird.
* Verwenden Sie die [Und-Verknüpfung](and-join.md) -Aktivität zum Synchronisieren mehrerer Ausführungszweige eines Workflows.
* Hinzufügen einer **Ende** -Aktivität, um das Ende eines Workflows grafisch zu markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional.
* Verwenden Sie die [Verzweigung](fork.md) -Aktivität, um ausgehende Transitionen zu erstellen und mehrere Aktivitäten gleichzeitig zu starten.
* Hinzufügen einer [Warten](wait.md) -Aktivität die Ausführung eines Teils eines Workflows vorübergehend anhalten.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

