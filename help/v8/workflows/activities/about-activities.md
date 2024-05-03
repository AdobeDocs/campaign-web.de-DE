---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Sie Workflow-Aktivitäten durchführen.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 5947d7f6b2fd39ede6322273e7497744f9aff953
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 38%

---


# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenbestimmungs- und Daten-Management-Aktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Aktivitäten zur Flusskontrolle](#flow-control)

![](../assets/workflow-activities.png)

## Zielgruppenbestimmungs-Aktivitäten {#targeting}

Diese Aktivitäten sind spezifisch für die Zielgruppenbestimmung. Sie ermöglichen es Ihnen, ein oder mehrere Ziele zu erstellen, indem Sie eine Zielgruppe definieren und diese Zielgruppen mithilfe von Schnittmenge, Vereinigung oder Ausschluss aufteilen oder kombinieren.

* [Audience erstellen](build-audience.md): Definieren Sie Ihre Zielpopulation. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Abfrage-Modeler verwenden, um Ihre eigene Abfrage zu definieren.
* [Datenquelle ändern](change-data-source.md): Ändern Sie die Datenquelle für die Arbeitstabelle Ihres Workflows.&quot;
* [Dimensionsänderung](change-dimension.md): Ändern Sie die Zielgruppendimension während der Workflow-Erstellung.
* [Kombinieren](combine.md): Führen Sie eine Segmentierung für Ihre Eingangspopulation durch. Sie können eine Vereinigung, eine Schnittmenge oder einen Ausschluss verwenden.
* [Deduplizierung](deduplication.md): Löschen Sie Dubletten in den Ergebnissen der eingehenden Aktivitäten.
* [Anreicherung](enrichment.md): Definieren Sie zusätzliche Daten, die in Ihrem Workflow verarbeitet werden sollen. Mit dieser Aktivität können Sie die eingehende Transition nutzen und entsprechend der Konfiguration der Aktivität die ausgehende Transition mit Zusatzdaten ergänzen.
* [Inkrementelle Abfrage](incremental-query.md): Abfrage der Datenbank auf geplanter Basis. Bei jeder neuen Ausführung dieser Aktivität werden die Ergebnisse der vorangehenden Ausführungen ausgeschlossen. Dadurch lassen sich ausschließlich neue Elemente abrufen.
* [Abstimmung](reconciliation.md): Definieren Sie die Relation zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle, z. B. aus einer externen Datei geladenen Daten.
* [Audience-Speicherung](save-audience.md): Aktualisieren Sie eine existierende Audience oder erstellen Sie eine neue Audience aus der zuvor in einem Workflow berechneten Population.
* [Aufspaltung](split.md): Segmentieren Sie eingehende Population in mehrere Teilmengen.

## Daten-Management-Aktivitäten {#data}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Aktivitäten &quot;Extrahieren&quot;und &quot;Datei laden&quot;"
>abstract="In Workflows stehen neue Datenverwaltungsaktivitäten zur Verfügung. Verwenden Sie die Aktivität Dateiextraktion , um Daten aus Adobe Campaign als externe Datei in ein anderes System zu exportieren. Verwenden Sie die Aktivität Datei laden , um mit Profilen und Daten zu arbeiten, die in einer externen Datei gespeichert sind."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

Diese Aktivitäten dienen der Verarbeitung und Anreicherung von Populationsdaten.

* [Dateiextraktion](extract-file.md): Exportieren Sie Daten von Adobe Campaign in ein anderes System als externe Datei.
* [Datei laden](load-file.md): Arbeiten Sie mit Profilen und Daten, die in einer externen Datei gespeichert sind.
* [Dateiübertragung](transfer-file.md): Empfangen oder Senden von Dateien, Testen auf Existenz von Dateien oder Auflisten von Dateien auf einem Server. Das verwendete Protokoll kann entweder ein Server-zu-Server-Protokoll oder ein HTTP-Protokoll sein.
* [JavaScript-Code](javascript-code.md): Führen Sie ein JavaScript-Codefragment im Kontext eines Workflows aus.
* [Abonnementdienste](subscription-services.md): In einer einzigen Aktion können Sie mehrere Profile für/von einem Dienst anmelden oder abmelden.
* [Daten aktualisieren](update-data.md): Führen Sie Massenaktualisierungen für Felder in der Datenbank durch. Mit verschiedenen Optionen können Sie die Datenaktualisierung personalisieren.

## Kanalaktivitäten {#channel}

In Adobe Campaign Web können Sie Marketing-Kampagnen automatisieren und über mehrere Kanäle hinweg ausführen. Sie können Kanalaktivitäten in den Arbeitsflächen kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen je nach Kundenverhalten Aktionen ausgelöst werden können. Es sind folgende **Kanalaktivitäten** verfügbar: E-Mail-, SMS-, Android- und iOS-Push-Benachrichtigungen. [Erfahren Sie, wie Sie einen Versand im Rahmen eines Workflows einrichten.](channels.md).

## Aktivitäten zur Flusskontrolle {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Erweiterte Workflow-Aktivitäten"
>abstract="Sie können jetzt die Aktivitäten Test, JavaScript-Code und Externes Signal in einem Workflow konfigurieren. Verwenden Sie die Test -Aktivität, um Workflow-Transitionen auf der Basis von Bedingungen zu aktivieren. Fügen Sie die Aktivität JavaScript-Code hinzu, um im Kontext Ihres Workflows ein JS-Codefragment auszuführen. Konfigurieren Sie die Aktivität Externes Signal , um die Ausführung Ihres Workflows über eine API oder einen anderen Workflow Trigger."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"



>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Endaktivität"
>abstract="Mit der Aktivität **Ende** können Sie das Ende eines Workflows grafisch markieren. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional."

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Ihre Hauptaufgabe ist es, die anderen Aktivitäten zu koordinieren:

* [Und-Verknüpfung](and-join.md): Synchronisieren Sie mehrere Ausführungszweige eines Workflows.
* **Ende**: Markieren Sie grafisch das Ende eines Workflows. Diese Aktivität hat keine funktionalen Auswirkungen und ist daher optional
* [Externes Signal](external-signal.md): Trigger der Ausführung eines Workflows über einen anderen Workflow oder einen API-Aufruf.
* [Verzweigung](fork.md): Erstellen Sie ausgehende Transitionen, um mehrere Aktivitäten gleichzeitig zu starten.
* [Planung](scheduler.md): Planen Sie den Beginn des Workflows ein.
* [Test](test.md): Aktivieren Sie Transitionen auf der Basis der angegebenen Bedingungen.
* [Warten](wait.md): Halten Sie die Ausführung eines Teils eines Workflows vorübergehend an.
