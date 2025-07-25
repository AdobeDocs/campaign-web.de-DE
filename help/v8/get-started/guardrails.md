---
title: Schutzmechanismen und Begrenzungen in den Campaign Web-Benutzeroberflächen-Workflows
description: Schutzmechanismen und Begrenzungen bei der Arbeit mit Workflows auf der Campaign Web-Benutzeroberfläche
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 100%

---

# Schutzmechanismen und Begrenzungen für Workflows {#guardrails-limitations}

Wenn Sie in der Campaign Web-Benutzeroberfläche mit Workflows arbeiten, die in der Campaign-Client-Konsole erstellt oder geändert wurden, gelten die unten aufgeführten Schutzmechanismen und Begrenzungen.

Beachten Sie, dass auf dieser Seite zwar wichtige Aspekte bei der Arbeit mit Workflows in der Konsole und der Web-Benutzeroberfläche aufgeführt werden, jedoch nicht alle möglichen Inkompatibilitäten zwischen den beiden Oberflächen abgedeckt werden.

## Workflow-Aktivitäten {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Aktivität nicht bearbeitbar"
>abstract="Wenn eine **Abfrageaktivität** oder eine **Anreicherungsaktivität** mit zusätzlichen Daten in der Konsole konfiguriert ist, werden die Anreicherungsdaten in Campaign Web berücksichtigt und an die ausgehende Transition übergeben. Sie können jedoch nicht bearbeitet werden."

Workflow-Aktivitäten, die noch nicht in der Campaign Web-Benutzeroberfläche unterstützt werden, sind schreibgeschützt und werden als inkompatible Aktivitäten angezeigt. Sie können weiterhin den Workflow ausführen, Nachrichten senden, Logs überprüfen und weitere Aufgaben erledigen. Workflow-Aktivitäten, die sowohl in der Campaign Web-Benutzeroberfläche als auch in der Campaign-Client-Konsole verfügbar sind, können bearbeitet werden.

| Konsole | Web |
| --- | --- |
| ![Screenshot zu Einschränkungen von Aktivitäten in der Konsole](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Screenshot zu Einschränkungen von Aktivitäten in der Web-Benutzeroberfläche](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Wenn eine **Abfrageaktivität** oder **Anreicherungsaktivität** mit zusätzlichen Daten in der Konsole konfiguriert ist, werden die Anreicherungsdaten im Campaign Web berücksichtigt und an die ausgehende Transition übergeben. Sie können jedoch nicht bearbeitet werden.

| Konsole | Web |
| --- | --- |
| ![Screenshot zu Einschränkungen von Optionen in der Konsole](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Screenshot zu Einschränkungen von Optionen in der Web-Benutzeroberfläche](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

In der Konsole kann die Aktivität **Anreicherung** sowohl Abstimmungen als auch Anreicherungen durchführen. Wenn Sie in der Client-Konsole Abstimmungseinstellungen in der Aktivität **Anreicherung** definiert haben, wird diese in der Campaign Web-Benutzeroberfläche als Aktivität **Abstimmung** angezeigt.

| Konsole | Web |
| --- | --- |
| ![Screenshot der Aktivität „Anreicherung“ in der Konsole](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Screenshot der Aktivität „Anreicherung“ in der Web-Benutzeroberfläche](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Workflow-Arbeitsfläche {#wkf-canvas}

Beim Erstellen eines neuen Workflows in der Campaign Web-Benutzeroberfläche unterstützt die Arbeitsfläche nur einen Einstiegspunkt. Wenn Sie jedoch in der Konsole einen Workflow mit mehreren Einstiegspunkten erstellt haben, können Sie ihn in der Campaign Web-Benutzeroberfläche öffnen und bearbeiten.

| Konsole | Web |
| --- | --- |
| ![Screenshot mit mehreren Einstiegspunkten in der Konsole](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Screenshot mit mehreren Einstiegspunkten in der Web-Benutzeroberfläche](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Die Positionierung der Knoten wird bei jedem Hinzufügen oder Entfernen einer Aktivität aktualisiert. Wenn Sie einen Workflow in der Konsole erstellen, ihn über die Campaign Web-Benutzeroberfläche ändern und dann in der Konsole erneut öffnen, treten möglicherweise kleinere Ungenauigkeiten bei der Positionierung auf. Dies hat keine Auswirkungen auf die Prozesse und Aufgaben des Workflows.

| Anfangs-Workflow | Positionsänderung |
| --- | --- |
| ![Screenshot zur ersten Workflow-Positionierung](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Screenshot mit im Anschluss von Änderungen durchgeführten Positionsänderungen](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |