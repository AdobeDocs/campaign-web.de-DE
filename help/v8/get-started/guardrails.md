---
title: Limits und Einschränkungen in der Web-Benutzeroberfläche von Campaign
description: Limits und Einschränkungen in der Web-Benutzeroberfläche von Campaign
badge: label="Beta"
source-git-commit: ff95b563784ae507245e6690feedda33ea6a111b
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

---


# Schutzmechanismen und Begrenzungen {#guardrails-limitations}

Bei der Arbeit mit in der Campaign-Webbenutzeroberfläche erstellten oder geänderten Komponenten in der Campaign-Clientkonsole gelten die unten aufgeführten Limits und Einschränkungen.

## Workflows {#wf-guardrails-limitations}

Auf denselben Workflow kann sowohl in der Konsole als auch in der Web-Benutzeroberfläche zugegriffen werden. Beachten Sie jedoch, dass bestimmte Einschränkungen gelten.

**Activity Edition**

* Beim Zugriff auf einen Konsolen-Workflow in der Web-Benutzeroberfläche können Sie nur kompatible Aktivitäten ändern.

**Leinwandbearbeitung**

* Wenn ein Konsolen-Workflow über mehrere Startknoten/Zweige oder schwebende Aktivitäten verfügt, müssen Sie eine Startaktivität und eine Abspaltung hinzufügen, um Startknoten mit dem Hauptknoten zu verbinden. Sie müssen auch schwebende Aktivitäten entfernen.

**Aktivitätspositionierung**

* Die Positionierung der Knoten wird nur dann neu berechnet (die anfängliche Positionierung der Aktivitäten wird daher geändert), wenn eine Aktivität hinzugefügt oder entfernt wurde (nicht immer).

**Nicht verfügbare Optionen**

* Nicht kompatible Optionen werden nicht in der Web-Benutzeroberfläche angezeigt.

**Schleifen**

* Workflows einschließlich Schleifen werden nicht in der Web-Benutzeroberfläche angezeigt. Eine Fehlermeldung wird angezeigt.

**Abstimmung und Anreicherung**

In der Campaign-Clientkonsole wird die **Anreicherung** -Aktivität kann sowohl Abstimmung als auch Anreicherung durchführen. In der Campaign-Web-Benutzeroberfläche sind die Abstimmungsfunktionen noch nicht verfügbar. Wenn Sie die Abstimmung in der Konsolenaktivität festgelegt haben, wird diese als nicht kompatible Aktivität in der Web-Benutzeroberfläche angezeigt.

* Wenn die Variable **Anreicherung** -Aktivität in der Konsole nur eine Anreicherung durchführt, wird die **Anreicherung** -Aktivität im Web angezeigt.
* Wenn die Variable **Anreicherung** -Aktivität in der Konsole führt nur eine Abstimmung durch. Es wird eine inkompatible Aktivität angezeigt.

## Vordefinierte Filter {#filters-guardrails-limitations}


Bei der Auswahl der Audience eines Versands oder beim Erstellen einer Audience in einem Workflow stehen einige vordefinierte Filter nicht zur Verfügung. Eine spezifische Fehlermeldung wird angezeigt. Sie können weiterhin die Abfrage und die Anzeige verwenden: die Filterbedingung und die Ergebnisse, aber Sie können die genaue Abfrage nicht im Regel-Builder anzeigen und den Filter nicht bearbeiten.

![](assets/filter-unavailable.png)
