---
audience: end-user
title: Verwenden der Workflow-Aktivität „Daten-Update“
description: Informationen dazu, wie Sie die Workflow-Aktivität „Daten-Update“ verwenden
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 33%

---

# Daten-Update {#update-data}

Die Aktivität **Daten-Update** ist eine **Daten-Management**-Aktivität. Dies ermöglicht eine gebündelte Aktualisierung von Datenbankfeldern. Mehrere Optionen ermöglichen es Ihnen, die Datenaktualisierung anzupassen.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update it if it has already been added. You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely.

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or directly use reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section lets you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.
-->

## Konfigurieren der Aktivität „Daten-Update“ {#update-data-configuration}

Um die Aktivität **Daten aktualisieren** zu konfigurieren, fügen Sie die Aktivität zu Ihrem Workflow hinzu und definieren Sie einen Titel.

![Aktivität „Workflow-Daten-Update“](../assets/workflow-update-data.png)

### Aktionstyp

Geben Sie im Feld **Aktionstyp** an, auf welche Weise die Daten aktualisiert werden sollen:

* **Einfügen oder Aktualisieren**: Fügt Daten ein oder aktualisiert sie, wenn die Datensätze bereits in der Datenbank vorhanden sind.
* **Einfügen**: Nur Daten einfügen. Bereits vorhandene Datensätze werden nicht aktualisiert. Wenn Abstimmkriterien definiert wurden, werden nur nicht abgestimmte Datensätze hinzugefügt.
* **Aktualisieren**: Aktualisieren Sie nur die Daten der Datensätze, die bereits in der Datenbank vorhanden sind.
* **Löschen**: Daten löschen.

Im Feld **Aktualisierungsgröße** wird bestimmt, wie viele Elemente der eingehenden Transition aktualisiert werden. Wenn Sie beispielsweise 500 angeben, werden die ersten 500 verarbeiteten Datensätze aktualisiert.

### Identifizierung von Einträgen

In diesem Abschnitt können Sie angeben, auf welche Weise die Einträge der Datenbank erkannt werden:

* Wenn sich Dateneinträge auf eine vorhandene Zielgruppendimension beziehen, wählen Sie die Option **Verwenden der Zielgruppendimension** und wählen Sie sie im Feld **Zu aktualisierende Zielgruppendimension** aus.
* Sie können auch **Benutzerdefinierte Links verwenden** auswählen und einen oder mehrere Links angeben, die die Identifizierung der Daten in der Datenbank ermöglichen.
* Wenn für den ausgewählten Vorgangstyp eine Aktualisierung erforderlich ist, verwenden Sie die Option **Abstimmregeln verwenden**.

### Zu aktualisierende Felder

Fügen Sie im **Zu aktualisierende Felder** die Felder hinzu, auf die die Aktualisierung angewendet wird. Fügen Sie bei Bedarf Bedingungen hinzu, damit diese Aktualisierung durchgeführt wird. Verwenden Sie das Feld **Berücksichtigt wenn**, um Bedingungen zu definieren. Bedingungen werden sequenziell in der Listenreihenfolge angewendet. Die Reihenfolge kann mithilfe der Pfeile rechts der Tabelle angepasst werden. Es ist möglich, mehrmals dasselbe Zielfeld zu verwenden.

Verknüpfen Sie Felder automatisch über die Schaltfläche **Automatische Zuordnung**. Die Funktion des automatischen Verbindens erkennt Felder gleichen Namens.

Wählen **bei einem Vorgangstyp** Einfügen oder Aktualisieren“ einzeln den Vorgang aus, der für jedes Feld angewendet werden soll. Geben Sie **gewünschten Wert im Feld** Vorgangstyp“ an.

### Erweiterte Optionen

Im Abschnitt **Erweiterte Optionen** können Sie zusätzliche Optionen zum Aktualisieren von Daten und Verwalten von Duplikaten angeben.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Mit diesen beiden letzten Optionen können Sie bestimmte Aktionen ausführen:

* **Ausgehende Transition erzeugen**: Erstellt eine ausgehende Transition, die am Ende der Ausführung aktiviert wird. Die Aktualisierung signalisiert in der Regel das Ende eines Workflows zur Zielgruppenbestimmung. Daher ist diese Option standardmäßig nicht aktiviert.

* **Ausgehende Transition für die Zurückweisungen erzeugen**: Erstellt eine ausgehende Transition, die Datensätze enthält, die nach der Aktualisierung nicht korrekt verarbeitet wurden (z. B. wenn ein Duplikat vorliegt). Die Aktualisierung markiert im Allgemeinen das Ende eines Zielgruppen-Workflows, und die Option ist nicht standardmäßig aktiviert.