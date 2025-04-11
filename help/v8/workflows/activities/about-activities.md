---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Sie Workflow-Aktivitäten durchführen.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 54%

---

# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenbestimmungs- und Daten-Management-Aktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Aktivitäten zur Flusskontrolle](#flow-control)

![Workflow-Aktivitäten - Übersicht](../assets/workflow-activities.png)

## Zielgruppenbestimmungs-Aktivitäten {#targeting}

Diese Aktivitäten sind spezifisch für die Zielgruppenbestimmung. Sie ermöglichen es Ihnen, eine oder mehrere Zielgruppen zu erstellen, indem Sie eine Zielgruppe definieren und diese Zielgruppen mithilfe von Schnittmengen-, Vereinigungs- oder Ausschlussvorgängen aufteilen oder kombinieren.

* [Zielgruppe erstellen](build-audience.md): Mit dieser Aktivität definieren Sie Ihre Zielpopulation. Wählen Sie eine vorhandene Audience aus oder verwenden Sie den Abfrage-Modellierer, um Ihre eigene Abfrage zu definieren.
* [Datenquelle ändern](change-data-source.md): Ändern Sie die Datenquelle für die Arbeitstabelle Ihres Workflows.
* [Dimensionsänderung](change-dimension.md): Ändern der Zielgruppendimension beim Erstellen des Workflows.
* [Kombinieren](combine.md): Mit dieser Aktivität segmentieren Sie Ihre eingehende Population. Verwenden Sie eine Vereinigung, eine Schnittmenge oder einen Ausschluss.
* [Deduplizierung](deduplication.md): Entfernen Sie Duplikate in den Ergebnissen eingehender Aktivitäten.
* [Anreicherung](enrichment.md): Mit dieser Aktivität definieren Sie zusätzliche Daten, die in Ihrem Workflow verarbeitet werden sollen. Konfigurieren Sie die Aktivität so, dass die ausgehende Transition mit zusätzlichen Daten durchgeführt wird.
* [Inkrementelle Abfrage](incremental-query.md): Mit dieser Aktivität fragen Sie die Datenbank nach einem Plan ab. Bei jeder Ausführung dieser Aktivität werden die Ergebnisse früherer Ausführungen ausgeschlossen, sodass nur neue Elemente berücksichtigt werden.
* [Abstimmung](reconciliation.md): Definieren Sie die Relation zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle, z. B. Daten aus einer externen Datei.
* [Zielgruppe speichern](save-audience.md): Mit dieser Aktivität aktualisieren Sie vorhandene Zielgruppen oder erstellen neue. Die hierfür erforderlichen Populationen werden im Vorfeld durch andere Workflow-Aktivitäten ermittelt.
* [Aufspaltung](split.md): Segmentiert die eingehende Population in mehrere Teilmengen.

## Daten-Management-Aktivitäten {#data}

Diese Aktivitäten dienen der Manipulation und Anreicherung von Populationsdaten.

* [Dateiextraktion](extract-file.md): Mit dieser Aktivität exportieren Sie in Adobe Campaign enthaltene Daten in Form von externen Dateien.
* [Datei laden](load-file.md): Mit dieser Aktivität können Sie mit Profilen und Daten arbeiten, die in einer externen Datei gespeichert sind.
* [Datei übertragen](transfer-file.md): Mit dieser Aktivität können Sie Dateien senden oder empfangen, das Vorhandensein von Dateien prüfen oder Dateien auf einem Server auflisten. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein.
* [JavaScript-Code](javascript-code.md): Führen Sie ein JavaScript-Codefragment im Kontext eines Workflows aus.
* [Anmeldedienste](subscription-services.md): Mit einer einzigen Aktion können Sie mehrere Profile für einen Dienst an- oder abmelden.
* [Daten aktualisieren](update-data.md): Mit dieser Aktivität führen Sie eine gebündelte Aktualisierung von Datenbankfeldern durch. Die Art der Datenbankaktualisierung kann über verschiedene Optionen definiert werden.

## Kanalaktivitäten {#channel}

In Adobe Campaign Web können Sie Marketing-Kampagnen automatisieren und über mehrere Kanäle hinweg ausführen. Kombinieren Sie Kanalaktivitäten in der Arbeitsfläche, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf dem Kundenverhalten Trigger für Aktionen erstellt wird. Die folgenden **Kanal**-Aktivitäten sind verfügbar: E-Mail-, SMS-, Android- und iOS-Push-Benachrichtigungen. [Erfahren Sie, wie Sie einen Versand im Rahmen eines Workflows einrichten.](channels.md).

## Aktivitäten zur Flusskontrolle {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Endaktivität"
>abstract="Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional."

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Ihre Hauptaufgabe ist es, die anderen Aktivitäten zu koordinieren:

* [Und-Verknüpfung](and-join.md): Mit dieser Aktivität synchronisieren Sie mehrere Ausführungszweige eines Workflows.
* **Ende**: Mit dieser Aktivität markieren Sie grafisch das Ende eines Workflows. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional.
* [Externes Signal](external-signal.md): Trigger bei der Ausführung eines Workflows aus einem anderen Workflow oder einem API-Aufruf.
* [Verzweigung](fork.md): Erstellen Sie ausgehende Transitionen, um mehrere Aktivitäten gleichzeitig zu starten.
* [Planung](scheduler.md): Planung des Starts des Workflows.
* [Test](test.md): Mit dieser Aktivität aktivieren Sie Transitionen auf Grundlage der angegebenen Bedingungen.
* [Warten](wait.md): Hält die Ausführung eines Teils eines Workflows vorübergehend an.