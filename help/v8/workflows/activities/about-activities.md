---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Sie Workflow-Aktivitäten durchführen.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 100%

---

# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenbestimmungs- und Daten-Management-Aktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Aktivitäten zur Flusskontrolle](#flow-control)

![Überblick über die Workflow-Aktivitäten](../assets/workflow-activities.png)

## Zielgruppenbestimmungs-Aktivitäten {#targeting}

Diese Aktivitäten sind spezifisch für die Zielgruppenbestimmung. Sie ermöglichen es Ihnen, eine oder mehrere Zielgruppen zu erstellen, indem Sie eine Zielgruppe definieren und diese Zielgruppen mithilfe von Schnittmenge, Vereinigung oder Ausschluss aufteilen oder kombinieren.

* [Zielgruppe erstellen](build-audience.md): Mit dieser Aktivität definieren Sie Ihre Zielpopulation. Wählen Sie eine vorhandene Zielgruppe aus oder verwenden Sie den Abfrage-Modeler, um Ihre eigene Abfrage zu definieren.
* [Datenquelle ändern](change-data-source.md): Mit dieser Aktivität ändern Sie die Datenquelle für die Arbeitstabelle Ihres Workflows.
* [Dimensionsänderung](change-dimension.md): Mit dieser Aktivität ändern Sie die Zielgruppendimension, während Sie Ihren Workflow erstellen.
* [Kombinieren](combine.md): Mit dieser Aktivität segmentieren Sie Ihre eingehende Population. Verwenden Sie eine Vereinigung, eine Schnittmenge oder einen Ausschluss.
* [Deduplizierung](deduplication.md): Mit dieser Aktivität löschen Sie Duplikate in Ergebnissen aus eingehenden Aktivitäten.
* [Anreicherung](enrichment.md): Mit dieser Aktivität definieren Sie zusätzliche Daten, die in Ihrem Workflow verarbeitet werden sollen. Konfigurieren Sie die Aktivität, um die ausgehende Transition mit Zusatzdaten zu ergänzen.
* [Inkrementelle Abfrage](incremental-query.md): Mit dieser Aktivität fragen Sie die Datenbank nach einem Plan ab. Bei jeder Ausführung dieser Aktivität werden die Ergebnisse vofangehenden Ausführungen ausgeschlossen, sodass nur neue Elemente berücksichtigt werden.
* [Abstimmung](reconciliation.md): Mit dieser Aktivität definieren Sie die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle, z. B. Daten, die aus einer externen Datei geladen werden.
* [Zielgruppe speichern](save-audience.md): Mit dieser Aktivität aktualisieren Sie vorhandene Zielgruppen oder erstellen neue. Die hierfür erforderlichen Populationen werden im Vorfeld durch andere Workflow-Aktivitäten ermittelt.
* [Aufspaltung](split.md): Mit dieser Aktivität unterteilen Sie die eingehende Population in mehrere Teilmengen.

## Daten-Management-Aktivitäten {#data}

Diese Aktivitäten dienen der Manipulation und Anreicherung von Populationsdaten.

* [Dateiextraktion](extract-file.md): Mit dieser Aktivität exportieren Sie in Adobe Campaign enthaltene Daten in Form von externen Dateien.
* [Datei laden](load-file.md): Mit dieser Aktivität können Sie mit Profilen und Daten arbeiten, die in einer externen Datei gespeichert sind.
* [Datei übertragen](transfer-file.md): Mit dieser Aktivität können Sie Dateien senden oder empfangen, das Vorhandensein von Dateien prüfen oder Dateien auf einem Server auflisten. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein.
* [JavaScript-Code](javascript-code.md): Mit dieser Aktivität führen Sie ein JavaScript-Code-Snippet im Kontext eines Workflows aus.
* [Anmeldedienste](subscription-services.md): Mit dieser Aktivität können Sie in einer einzigen Aktion mehrere Profile für einen Dienst abonnieren oder von ihm abmelden.
* [Daten aktualisieren](update-data.md): Mit dieser Aktivität führen Sie eine gebündelte Aktualisierung von Datenbankfeldern durch. Die Art der Datenbankaktualisierung kann über verschiedene Optionen definiert werden.

## Kanalaktivitäten {#channel}

In Adobe Campaign Web können Sie Marketing-Kampagnen automatisieren und über mehrere Kanäle hinweg ausführen. Kombinieren Sie Kanalaktivitäten in den Arbeitsflächen, um Cross-Channel-Workflows zu erstellen, mit denen je nach Kundenverhalten Aktionen ausgelöst werden können. Es sind folgende **Kanalaktivitäten** verfügbar: E-Mail-, SMS-, Android- und iOS-Push-Benachrichtigungen. [Erfahren Sie, wie Sie einen Versand im Rahmen eines Workflows einrichten.](channels.md).

## Aktivitäten zur Flusskontrolle {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Endaktivität"
>abstract="Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional."

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Ihre Hauptaufgabe ist es, die anderen Aktivitäten zu koordinieren:

* [Und-Verknüpfung](and-join.md): Mit dieser Aktivität synchronisieren Sie mehrere Ausführungszweige eines Workflows.
* **Ende**: Mit dieser Aktivität markieren Sie grafisch das Ende eines Workflows. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional.
* [Externes Signal](external-signal.md): Mit dieser Aktivität lösen Sie die Ausführung eines Workflows über einen anderen Workflow oder einen API-Aufruf aus.
* [Verzweigung](fork.md): Mit dieser Aktivität erstellen Sie ausgehende Transitionen, um mehrere Aktivitäten gleichzeitig zu starten.
* [Planung](scheduler.md): Mit dieser Aktivität planen Sie, wann der Workflow starten soll.
* [Test](test.md): Mit dieser Aktivität aktivieren Sie Transitionen auf Grundlage der angegebenen Bedingungen.
* [Warten](wait.md): Mit dieser Aktivität halten Sie die Ausführung eines Teils eines Workflows vorübergehend an.