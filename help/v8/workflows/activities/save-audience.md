---
audience: end-user
title: Verwenden der Workflow-Aktivität „Zielgruppe speichern“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Verzweigung“ verwenden.
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 100%

---

# Zielgruppe speichern {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Speichern einer Zielgruppe"
>abstract="Mit dieser Aktivität können Sie eine vorhandene Zielgruppe aktualisieren oder eine neue Zielgruppe aus der Population erstellen, die im Vorfeld durch andere Workflow-Aktivitäten ermittelt wurde. Die Zielgruppen werden zur bereits bestehenden Zielgruppenliste hinzugefügt und sind über das Menü **Zielgruppen** zugänglich."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Ausgehende Transition erzeugen"
>abstract="Verwenden Sie diese Option, wenn Sie eine Transition nach der Aktivität **Zielgruppe speichern** hinzufügen möchten."

Die Aktivität **Zielgruppe speichern** ist eine Aktivität zur **Zielgruppenbestimmung**. Mit dieser Aktivität können Sie eine vorhandene Zielgruppe aktualisieren oder eine neue Zielgruppe aus der Population erstellen, die im Vorfeld durch andere Workflow-Aktivitäten ermittelt wurde. Die Zielgruppen werden zur bereits bestehenden Zielgruppenliste in Adobe Campaign hinzugefügt und sind über das Menü **Zielgruppen** zugänglich.

Die Aktivität wird hauptsächlich verwendet, um Populationsgruppen beizubehalten, die im selben Workflow ermittelt wurden, indem sie in wiederverwendbare Zielgruppen umgewandelt werden. Verbinden Sie sie mit anderen Zielgruppenbestimmungsaktivitäten, wie etwa den Aktivitäten **Zielgruppe aufbauen** oder **Kombinieren**.

## Konfigurieren der Aktivität „Zielgruppe speichern“ {#save-audience-configuration}

Führen Sie die folgenden Schritte aus, um die Aktivität **Zielgruppe aufbauen** zu konfigurieren:

![Beschreibung: Workflow-Konfiguration für die Aktivität „Zielgruppe speichern“](../assets/workflow-save-audience.png)

1. Fügen Sie die Aktivität **Zielgruppe speichern** zum Workflow hinzu.

1. Wählen Sie im Dropdown **Modus** die Aktion aus, die ausgeführt werden soll:

   * **Zielgruppe erstellen oder aktualisieren**: Definieren Sie ein **Zielgruppen-Label**. Wenn die Zielgruppe bereits existiert, wird sie aktualisiert. Andernfalls wird eine neue Zielgruppe erstellt.

   * **Existierende Zielgruppe aktualisieren**: Wählen Sie die zu aktualisierende **Zielgruppe** in der Liste der vorhandenen Zielgruppen aus.

1. Wählen Sie die **Update-Methode** aus, der für vorhandene Zielgruppen gelten soll:

   * **Zielgruppen-Inhalt durch die neuen Daten ersetzen**: Alle Zielgruppeninhalte werden ersetzt und alte Daten gehen verloren. Nur die in der eingehenden Transition der Aktivität **Zielgruppe speichern** übermittelten Daten werden beibehalten. Bei dieser Option werden Zielgruppendimension und -typ der aktualisierten Zielgruppe gelöscht.

   * **Zielgruppen-Inhalt mit den neuen Daten ergänzen**: Der alte Zielgruppeninhalt wird beibehalten und die Daten der eingehenden Transition der Aktivität **Zielgruppe speichern** werden hinzugefügt.

1. Aktivieren Sie die Option **Ausgehende Transition erzeugen**, wenn Sie eine Transition nach der Aktivität **Zielgruppe speichern** hinzufügen möchten.

Der Inhalt der gespeicherten Zielgruppe ist anschließend in der Detailansicht der Zielgruppe verfügbar, auf die Sie im Menü **Zielgruppen** zugreifen können. Die in dieser Ansicht verfügbaren Spalten entsprechen den Spalten in der eingehenden Transition der Aktivität **Zielgruppe speichern** des Workflows.

## Beispiel {#save-audience-example}

Im folgenden Beispiel wird eine einfache Zielgruppenaktualisierung von der Zielgruppenbestimmung aus gezeigt. Der Workflow wird im Rahmen eines Planungsvorgangs einmal monatlich ausgeführt. Eine Abfrage ruft alle Profile ab, die für die verschiedenen verfügbaren Anwendungen angemeldet sind. Die Aktivität **Zielgruppe speichern** aktualisiert in diesem Fall die angegebene Zielgruppe, indem die Profile, die seit der letzten Ausführung des Workflows den Informationsdienst abbestellt haben, entfernt und neu angemeldete Profile hinzugefügt werden.