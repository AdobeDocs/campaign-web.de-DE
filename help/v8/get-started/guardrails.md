---
title: Limits und Einschränkungen in der Web-Benutzeroberfläche von Campaign
description: Limits und Einschränkungen in der Web-Benutzeroberfläche von Campaign
badge: label="Beta"
source-git-commit: 86d87e9a3ac9028634a08c2c0969cd232dff15f5
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 6%

---


# Schutzmechanismen und Begrenzungen {#guardrails-limitations}

Bei der Arbeit mit in der Campaign-Webbenutzeroberfläche erstellten oder geänderten Komponenten in der Campaign-Clientkonsole gelten die unten aufgeführten Limits und Einschränkungen.

## Workflows {#wf-guardrails-limitations}

**Activities**

* Workflow-Aktivitäten, die noch nicht in der Web-Benutzeroberfläche unterstützt werden, sind schreibgeschützt. Sie können weiterhin den Workflow ausführen, Nachrichten senden, die Protokolle überprüfen usw. Workflow-Aktivitäten, die sowohl in der Web-Benutzeroberfläche als auch in der Client-Konsole verfügbar sind, können bearbeitet werden.

| Konsole | Web-Benutzeroberfläche |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="50%" align="left" zoomable="yes"} |

**Arbeitsfläche**

* Beim Erstellen eines neuen Workflows in der Web-Benutzeroberfläche unterstützt die Arbeitsfläche nur einen Einstiegspunkt. Wenn Sie jedoch einen Workflow in der Konsole mit mehreren Einstiegspunkten erstellt haben,

Selbst wenn Ihr Workflow auf der Arbeitsfläche der Clientkonsole mit mehreren Einstiegspunkten erstellt wurde, kann er auch in der Web-Benutzeroberfläche bearbeitet werden. Sie können weiterhin öffnen und bearbeiten



Erstellen Sie dazu einen Workflow aus der Clientkonsole mit mehreren Einstiegspunkten und öffnen Sie ihn über die Web-Benutzeroberfläche, um das Ergebnis anzuzeigen.



Natürlich können Sie die Aktivitäten bearbeiten und den Workflow wie gewohnt starten und ausführen.



**Aktivitätspositionierung**

* Die Positionierung der Knoten wird nur dann neu berechnet (die anfängliche Positionierung der Aktivitäten wird daher geändert), wenn eine Aktivität hinzugefügt oder entfernt wurde (nicht immer).

**Nicht verfügbare Optionen**

* Nicht kompatible Optionen werden nicht in der Web-Benutzeroberfläche angezeigt.

**Schleifen**

* Schleifen sind in der Web-Benutzeroberfläche noch nicht verfügbar. Wenn Sie einen Workflow mit einer Schleife mithilfe der Konsole erstellt haben, können Sie nicht über die Web-Benutzeroberfläche darauf zugreifen. Eine Fehlermeldung wird angezeigt.

| Konsole | Web-Benutzeroberfläche |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="50%" align="left" zoomable="yes"} |

**Abstimmung und Anreicherung**

In der Campaign-Clientkonsole wird die **Anreicherung** -Aktivität kann sowohl Abstimmung als auch Anreicherung durchführen. In der Campaign-Web-Benutzeroberfläche sind die Abstimmungsfunktionen noch nicht verfügbar. Wenn Sie die Abstimmung in der Konsolenaktivität festgelegt haben, wird diese als nicht kompatible Aktivität in der Web-Benutzeroberfläche angezeigt.

* Wenn die Variable **Anreicherung** -Aktivität in der Konsole nur eine Anreicherung durchführt, wird die **Anreicherung** -Aktivität im Web angezeigt.
* Wenn die Variable **Anreicherung** -Aktivität in der Konsole führt nur eine Abstimmung durch. Es wird eine inkompatible Aktivität angezeigt.

## Vordefinierte Filter {#filters-guardrails-limitations}

In dieser Produktversion, bei der Auswahl der Zielgruppe eines Versands oder beim Erstellen einer Zielgruppe in einem Workflow stehen in der Benutzeroberfläche keine vordefinierten Filter zur Verfügung.

Eine spezifische Fehlermeldung wird angezeigt. Auch wenn Sie die grafische Darstellung der Abfrage im Regel-Builder nicht anzeigen und den Filter nicht bearbeiten können, können Sie ihn dennoch verwenden und die Filterbedingungen sowie die Ergebnisse anzeigen. Sie können auch auf die SQL-Abfrage zugreifen, um die genauen Einstellungen zu überprüfen.

![](assets/filter-unavailable.png){width="70%" align="left"}

Beachten Sie, dass beim Erstellen eines Filters in der Web-Oberfläche und dessen Änderung in der Konsole mit nicht unterstützten Attributen die grafische Darstellung nicht mehr in der Web-Oberfläche verfügbar sein kann. In jedem Fall können Sie den Filter weiterhin verwenden.

Ununterstützte Attribute sind unten aufgeführt.

### Nicht unterstützte Datentypen {#unsupported-data-type}

Die folgenden in der Clientkonsole verfügbaren Datentypen werden beim Anzeigen eines Filters oder einer Regel in der Webschnittstelle nicht unterstützt:

* datetime
* Zeit
* timespan
* double
* float

### Nicht unterstützte Filterfunktionen {#unsupported-filtering-capabilities}

Wenn ein Filter mit komplexen Ausdrücken und Funktionen in der Clientkonsole erstellt wurde, kann er nicht in der Webschnittstelle bearbeitet werden.

Darüber hinaus werden die folgenden Operatoren nicht unterstützt:

* Numerischer Typ
   * ist enthalten in
   * nein

* String type
   * größer als
   * kleiner als
   * größer als oder gleich
   * kleiner oder gleich
   * ist wie
   * ist nicht wie

* Datum Typ
   * später als
   * früher als
   * ist nicht gleich
   * ist leer
   * ist nicht leer
   * ist enthalten in
   * ist nicht enthalten in
   * letzten

* 1:N-Links
   * COUNT, SUM, AVG, MIN, MAX