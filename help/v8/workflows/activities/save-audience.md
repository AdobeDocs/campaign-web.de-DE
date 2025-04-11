---
audience: end-user
title: Verwenden der Workflow-Aktivität „Zielgruppe speichern“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Verzweigung“ verwenden.
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 44%

---

# Zielgruppe speichern {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Speichern einer Zielgruppe"
>abstract="Mit dieser Aktivität können Sie eine vorhandene Zielgruppe aktualisieren oder eine neue Zielgruppe aus der Population erstellen, die im Vorfeld durch andere Workflow-Aktivitäten ermittelt wurde. Die Zielgruppen werden zur bereits bestehenden Zielgruppenliste hinzugefügt und sind über das Menü **Zielgruppen** zugänglich."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Ausgehende Transition erzeugen"
>abstract="Verwenden Sie diese Option, wenn Sie nach der Aktivität **Zielgruppe speichern** eine Transition hinzufügen möchten."

Die Aktivität **Zielgruppe speichern** ist eine Aktivität zur **Zielgruppenbestimmung**. Mit dieser Aktivität können Sie eine vorhandene Zielgruppe aktualisieren oder eine neue Zielgruppe aus der Population erstellen, die im Vorfeld durch andere Workflow-Aktivitäten ermittelt wurde. Die Zielgruppen werden zur bereits bestehenden Zielgruppenliste in Adobe Campaign hinzugefügt und sind über das Menü **Zielgruppen** zugänglich.

Diese Aktivität wird in erster Linie verwendet, um im selben Workflow berechnete Populationen beizubehalten, indem sie in wiederverwendbare Zielgruppen konvertiert werden. Verbinden Sie sie mit anderen Zielgruppenbestimmungsaktivitäten, wie etwa den Aktivitäten **Zielgruppe aufbauen** oder **Kombinieren**.

## Konfigurieren der Aktivität „Zielgruppe speichern“ {#save-audience-configuration}

Führen Sie die folgenden Schritte aus, um die Aktivität **Zielgruppe aufbauen** zu konfigurieren:

![Beschreibung: Workflow-Konfiguration für die Aktivität „Zielgruppe speichern“](../assets/workflow-save-audience.png)

1. Fügen Sie die Aktivität **Zielgruppe speichern** zum Workflow hinzu.

1. Wählen Sie in **Dropdown** Modus die Aktion aus, die Sie ausführen möchten:

   * **Vorhandene Zielgruppe erstellen oder aktualisieren**: Definieren Sie eine **Zielgruppentitel**. Wenn die Zielgruppe bereits vorhanden ist, wird sie aktualisiert. Andernfalls wird eine neue Zielgruppe erstellt.

   * **Vorhandene Zielgruppe aktualisieren**: Wählen Sie die **Zielgruppe** aus, die Sie in der Liste der vorhandenen Zielgruppen aktualisieren möchten.

1. Wählen Sie den **Aktualisierungsmodus** der für bestehende Zielgruppen gilt:

   * **Zielgruppeninhalt durch neue Daten ersetzen**: Alle Zielgruppeninhalte werden ersetzt und alte Daten gehen verloren. Nur die Daten aus der eingehenden Transition der Aktivität **Zielgruppe speichern** werden beibehalten. Bei dieser Option werden Zielgruppendimension und -typ der aktualisierten Zielgruppe gelöscht.

   * **Audience mit neuen Daten abschließen**: Der alte Audience-Inhalt wird beibehalten, und die Daten aus der eingehenden Transition der Aktivität **Audience speichern** werden ihr hinzugefügt.

1. Aktivieren Sie die **Ausgehende Transition erzeugen**, wenn Sie nach der Aktivität **Zielgruppe speichern** eine Transition hinzufügen möchten.

Der Inhalt der gespeicherten Zielgruppe ist anschließend in der Detailansicht der Zielgruppe verfügbar, auf die Sie im Menü **Zielgruppen** zugreifen können. Die in dieser Ansicht verfügbaren Spalten entsprechen den Spalten der eingehenden Transition der Aktivität „Zielgruppe **&quot;** Workflows.

## Beispiel {#save-audience-example}

Im folgenden Beispiel wird eine einfache Zielgruppenaktualisierung von der Zielgruppenbestimmung aus gezeigt. Eine Planung führt den Workflow einmal monatlich aus. Mit einer Abfrage werden alle Profile abgerufen, die für die verschiedenen verfügbaren Programme abonniert wurden. Die Aktivität **Zielgruppe speichern** aktualisiert die Zielgruppe, indem sie Profile entfernt, die sich seit der letzten Ausführung des Workflows vom Service abgemeldet haben, und neu abonnierte Profile hinzufügt.