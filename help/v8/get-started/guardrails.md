---
title: Limits und Einschränkungen in Workflows der Campaign-Webbenutzeroberfläche
description: Limits und Einschränkungen bei der Arbeit mit Workflows in der Campaign-Webbenutzeroberfläche
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 19864179f02d39583cc90d42bf6ab677f4841600
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 19%

---

# Limits und Einschränkungen für Workflows {#guardrails-limitations}

Bei der Arbeit mit in der Campaign-Webbenutzeroberfläche erstellten oder geänderten Workflows in der Campaign-Clientkonsole gelten die unten aufgeführten Limits und Einschränkungen.

Beachten Sie, dass auf dieser Seite zwar wichtige Aspekte bei der Arbeit mit Workflows in der Konsole und der Web-Benutzeroberfläche aufgeführt werden, jedoch nicht alle möglichen Inkompatibilitäten zwischen den beiden Oberflächen erfasst werden.

## Workflow-Aktivitäten {#wkf-activities}

Workflow-Aktivitäten, die noch nicht im Campaign-Web unterstützt werden, sind schreibgeschützt und werden als inkompatible Aktivitäten angezeigt. Sie können weiterhin den Workflow ausführen, Nachrichten senden, die Protokolle überprüfen usw. Workflow-Aktivitäten, die sowohl im Campaign-Web als auch in der Client-Konsole verfügbar sind, können bearbeitet werden.

Workflow-Aktivitäten, die noch nicht in der Campaign-Webbenutzeroberfläche unterstützt werden, sind schreibgeschützt und werden als inkompatible Aktivitäten angezeigt. Sie können weiterhin den Workflow ausführen, Nachrichten senden, die Protokolle überprüfen usw. Workflow-Aktivitäten, die sowohl in der Campaign-Webbenutzeroberfläche als auch in der Campaign-Clientkonsole verfügbar sind, können bearbeitet werden.

| Konsole | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Wenn eine **Abfrage** oder **Anreicherung** -Aktivität mit zusätzlichen Daten in der Konsole konfiguriert ist, werden die Anreicherungsdaten im Campaign Web berücksichtigt und an die ausgehende Transition übergeben. Sie können jedoch nicht bearbeitet werden.

| Konsole | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

In der Konsole kann die **Anreicherungsaktivität** sowohl Abstimmungen als auch Anreicherungen durchführen. Wenn Sie in der Clientkonsole Abstimmungseinstellungen im **Anreicherung** -Aktivität, wird sie als **Abstimmung** Aktivität in der Campaign-Web-Benutzeroberfläche.

| Konsole | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

## Arbeitsfläche {#wkf-canvas}

Beim Erstellen eines neuen Workflows in der Campaign-Webbenutzeroberfläche unterstützt die Arbeitsfläche nur einen Einstiegspunkt. Wenn Sie jedoch einen Workflow in der Konsole mit mehreren Einstiegspunkten erstellt haben, können Sie ihn in der Web-Benutzeroberfläche von Campaign öffnen und bearbeiten.

| Konsole | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Die Positionierung der Knoten wird bei jedem Hinzufügen oder Entfernen einer Aktivität aktualisiert. Wenn Sie einen Workflow in der Konsole erstellen, ihn über die Campaign-Webbenutzeroberfläche ändern und in der Konsole erneut öffnen, treten möglicherweise kleinere Positionierungsfehler auf. Dies hat keine Auswirkungen auf die Prozesse und Aufgaben des Workflows.

| Anfangs-Workflow | Positionsänderung |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |
