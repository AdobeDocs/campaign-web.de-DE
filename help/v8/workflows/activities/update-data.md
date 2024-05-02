---
audience: end-user
title: Verwenden der Workflow-Aktivität Daten-Update
description: Erfahren Sie, wie Sie die Workflow-Aktivität Daten-Update verwenden.
source-git-commit: 347f8f84a8eda60538366eb3dc49f8d7e06379c3
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 31%

---

# Daten-Update {#update-data}

Die **Daten aktualisieren** -Aktivität **Data Management** -Aktivität. Damit können Sie Felder in der Datenbank gebündelt aktualisieren. Mit verschiedenen Optionen können Sie die Datenaktualisierung personalisieren.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## Konfigurieren der Aktivität Daten-Update{#update-data-configuration}

So konfigurieren Sie die **Daten aktualisieren** Aktivität erstellen, fügen Sie die Aktivität Ihrem Workflow hinzu und definieren Sie einen Titel.

![](../assets/workflow-update-data.png)

### Aktionstyp

Geben Sie im Feld **Aktionstyp** an, auf welche Weise die Daten aktualisiert werden sollen:

* **Einfügen oder Aktualisieren**: fügt neue Daten hinzu oder aktualisiert existierende Datensätze.
* **Einfügen**: fügt nur Daten ein. existierende Datensätze werden nicht verändert. Wenn Abstimmkriterien definiert wurden, werden nur nicht abgestimmte Datensätze hinzugefügt.
* **Aktualisieren** – aktualisiert Daten existierender Datensätze, fügt keine neuen Datensätze hinzu.
* **Löschen** – löscht in der Datenbank existierende Daten.

Im Feld **Aktualisierungsgröße** wird bestimmt, wie viele Elemente der eingehenden Transition aktualisiert werden. Bei Angabe von 500 beispielsweise werden die 500 ersten Datensätze aktualisiert.

### Datensatz-Identifizierung

In diesem Abschnitt können Sie angeben, wie die Datensätze der Datenbank identifiziert werden können:

* Wenn sich Dateneinträge auf eine existierende Zielgruppendimension beziehen, wählen Sie die **Zielgruppendimension verwenden** und wählen Sie sie aus dem **Zu aktualisierende Zielgruppendimension** -Feld.
* Sie können auch die **Verwenden benutzerdefinierter Links** und eine oder mehrere Relationen angeben, die die Identifizierung der Daten in der Datenbank ermöglichen
* Wenn der ausgewählte Vorgangstyp eine Aktualisierung erfordert, müssen Sie die **Abstimmungsregeln verwenden** -Option.

### Zu aktualisierende Felder

Im **Zu aktualisierende Felder** die Felder hinzufügen, auf die sich die Aktualisierung beziehen soll, und bei Bedarf Bedingungen für diese Aktualisierung hinzufügen. Verwenden Sie dazu die **Wird berücksichtigt, wenn** -Feld. Die Bedingungen werden nacheinander, in Reihenfolge der Liste geprüft. Die Reihenfolge kann mithilfe der Pfeile rechts der Tabelle angepasst werden. Es ist möglich, mehrmals dasselbe Zielfeld zu verwenden.

Sie können Felder automatisch über die **Automatische Zuordnung** Schaltfläche. Die Funktion erkennt Felder gleichen Namens.

Während **Einfügen oder Aktualisieren** -Aktionstyp, können Sie für jedes Feld individuell den anzuwendenden Vorgang auswählen. Wählen Sie dazu den gewünschten Wert im **Aktionstyp** -Feld.

### Erweiterte Optionen

Die **Erweiterte Optionen** ermöglicht die Angabe zusätzlicher Optionen für die Aktualisierung von Daten sowie die Verwaltung von Duplikaten.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Mit den letzten beiden Optionen können Sie bestimmte Aktionen ausführen:

* **Ausgehende Transition erzeugen**: erstellt eine ausgehende Transition, die am Ende der Ausführung aktiviert wird. Die Aktualisierung signalisiert in der Regel das Ende eines Zielgruppen-Workflows und ist daher nicht standardmäßig aktiviert.

* **Ausgehende Transition für die Zurückweisungen erzeugen**: erstellt eine ausgehende Transition mit Datensätzen, die nach der Aktualisierung nicht korrekt verarbeitet wurden (z. B. bei Duplikaten). Die Aktualisierung markiert in der Regel das Ende eines Zielgruppenbestimmungs-Workflows. Daher ist die Option standardmäßig nicht aktiviert.
