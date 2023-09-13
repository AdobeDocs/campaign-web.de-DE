---
audience: end-user
title: Verwenden der Workflow-Aktivität Planung
description: Erfahren Sie, wie Sie die Workflow-Aktivität Planung verwenden.
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 62%

---


# Planung {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Planungsaktivität"
>abstract="Die Aktivität Planung ..."

Die Planungsaktivität ermöglicht die Festlegung des Starts eines Workflows oder einer Aktivität auf einen bestimmten Zeitpunkt.

Eine Planung entspricht einem programmierten Start, Diese Aktivität kann nur als erste Aktivität des Workflows verwendet werden.

## Best Practices

* Es wird empfohlen, Workflows nicht öfter als alle 15 Minuten auszuführen, da die Gesamtleistung des Systems beeinträchtigt werden kann und Blöcke in der Datenbank entstehen können.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Planung** Aktivität:

1. Hinzufügen einer **Planung** -Aktivität zu Ihrem Workflow hinzu.

1. Konfigurieren Sie die **Ausführungsfrequenz**:

   * Einmal - der Workflow wird nur einmal ausgeführt.

   * Täglich - der Workflow wird jeden Tag einmal zu einem bestimmten Zeitpunkt ausgeführt.

   * Mehrmals pro Tag - der Workflow wird wiederholt zu bestimmten Zeiten am Tag ausgeführt. Sie können Ausführungen zu bestimmten Zeiten oder in regelmäßigen Abständen einrichten.

   * Wöchentlich - der Workflow wird wiederholt zu bestimmten Zeiten in der Woche ausgeführt.

   * Monatlich - der Workflow wird wiederholt zu bestimmten Zeiten im Monat ausgeführt. Sie können die Monate auswählen, in denen der Workflow ausgeführt werden soll. Sie können für die Ausführung von Workflows auch bestimmte Wochentage des Monats auswählen, z. B. am zweiten Dienstag des Monats.
1. Definieren Sie die Ausführungsdetails. Je nach gewählter Frequenz sind verschiedene Parameter (Uhrzeit, Ausführungsintervall, bestimmte Tage etc.) zu konfigurieren.

1. Klicks **Vorschau der Startzeiten anzeigen** um den Zeitplan der nächsten zehn Ausführungen Ihres Workflows zu überprüfen.

1. Definieren Sie den Gültigkeitszeitraum der Planung:

   * Dauerhaft (nie abläuft): Der Workflow wird in den angegebenen Intervallen ausgeführt, ohne dass Zeitrahmen oder Anzahl der Ausführungen überschritten wird.

   * Gültigkeitszeitraum: Der Workflow wird in den festgelegten Intervallen bis zu einem bestimmten Datum ausgeführt. bis das im Feld „Bis zum“ angegebene Datum erreicht ist.

## Beispiel


