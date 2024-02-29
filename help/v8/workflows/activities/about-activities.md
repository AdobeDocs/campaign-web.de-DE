---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Sie Workflow-Aktivitäten durchführen.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 100%

---


# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenbestimmungs- und Daten-Management-Aktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Aktivitäten zur Flusskontrolle](#flow-control)

![](../assets/workflow-activities.png)

## Zielgruppenbestimmungs- und Daten-Management-Aktivitäten {#targeting}

Diese Aktivitäten dienen der Zielgruppenbestimmung, Manipulation und Anreicherung von Populationsdaten. Sie ermöglichen es Ihnen, ein oder mehrere Ziele zu erstellen, indem Sie eine Zielgruppe definieren und diese Zielgruppen mithilfe von Schnittmenge, Vereinigung oder Ausschluss aufteilen oder kombinieren.

* Mithilfe der Aktivität [Zielgruppe speichern](save-audience.md) können vorhandene Zielgruppen aktualisiert oder neue erstellt werden. Die hierfür erforderlichen Populationen werden im Vorfeld durch andere Workflow-Aktivitäten ermittelt.
* Mit der Aktivität [Zielgruppe erstellen](build-audience.md) können Sie Ihre Zielgruppenpopulation definieren. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Abfrage-Modeler verwenden, um Ihre eigene Abfrage zu definieren.
* Mit der Aktivität [Kombinieren](combine.md) können Sie Ihre eingehende Population segmentieren. Sie können eine Vereinigung, eine Schnittmenge oder einen Ausschluss verwenden.
* Mit der Aktivität [Aufteilen](split.md) können Sie die eingehende Population in mehrere Teilmengen unterteilen.
* Verwenden Sie die Aktivität [Abstimmung](reconciliation.md), um die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle zu definieren, z. B. Daten, die aus einer externen Datei geladen werden.
* Mit der Aktivität [Anreicherung](enrichment.md) können Sie zusätzliche Daten definieren, die in Ihrem Workflow verarbeitet werden sollen. Mit dieser Aktivität können Sie die eingehende Transition nutzen und entsprechend der Konfiguration der Aktivität die ausgehende Transition mit Zusatzdaten ergänzen.
* Mithilfe der Aktivität [Deduplizierung](deduplication.md) lassen sich Dubletten in Ergebnissen aus eingehenden Aktivitäten löschen.
* Mit der Aktivität [Dimensionsänderung](change-dimension.md) können Sie die Zielgruppendimension ändern, während Sie Ihren Workflow erstellen.
* Mit der Aktivität [Datei laden](load-file.md) können Sie mit Profilen und Daten arbeiten, die in einer externen Datei gespeichert sind.

## Kanalaktivitäten {#channel}

In Adobe Campaign Web können Sie Marketing-Kampagnen automatisieren und über mehrere Kanäle hinweg ausführen. Sie können Kanalaktivitäten in den Arbeitsflächen kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen je nach Kundenverhalten Aktionen ausgelöst werden können. Es sind folgende **Kanalaktivitäten** verfügbar: E-Mail-, SMS-, Android- und iOS-Push-Benachrichtigungen. [Erfahren Sie, wie Sie einen Versand im Rahmen eines Workflows einrichten.](channels.md).

## Aktivitäten zur Flusskontrolle {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Endaktivität"
>abstract="Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional."

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Ihre Hauptaufgabe ist es, die anderen Aktivitäten zu koordinieren:

* Mit der Aktivität [Planung](scheduler.md) können Sie planen, wann der Workflow gestartet werden soll.
* Mit der Aktivität [Und-Verknüpfung](and-join.md) können Sie die Ausführung verschiedener Workflow-Verzweigungen synchronisieren.
* Fügen Sie eine **End**-Aktivität hinzu, um das Ende eines Workflows grafisch zu markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional.
* Die Aktivität [Verzweigung](fork.md) erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten.
* Fügen Sie eine Aktivität [Warten](wait.md) hinzu, um die Ausführung eines Teils eines Workflows vorübergehend anzuhalten.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

