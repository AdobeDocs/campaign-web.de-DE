---
audience: end-user
title: Workflow-Aktivität "Datei laden"verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Datei laden verwenden
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: f88c3cd200aa92f4db7a2ab36c85d778a07a4dc3
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 31%

---

# Datei laden  {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Aktivität „Datei laden“"
>abstract="Die **Datei laden** -Aktivität **Data Management** -Aktivität. Verwenden Sie diese Aktivität, um mit Daten zu arbeiten, die in einer externen Datei gespeichert sind."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Beispieldatei"
>abstract="Beispieldatei"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Name der Datei"
>abstract="Name der Datei"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Zieldatenbank"
>abstract="Zieldatenbank"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Zurückweisungsverwaltung für die Aktivität „Datei laden“"
>abstract="Zurückweisungsverwaltung für die Aktivität „Datei laden“"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Ausgehende Transition von der Zurückweisungsverwaltung"
>abstract="Ausgehende Transition von der Zurückweisungsverwaltung"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Ausgehende Transition für Zurückweisungen der Zurückweisungsverwaltung"
>abstract="Ausgehende Transition für Zurückweisungen der Zurückweisungsverwaltung"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formatierung der Aktivität „Datei laden“"
>abstract="Formatierung der Aktivität „Datei laden“"

Die **Datei laden** -Aktivität **Data Management** -Aktivität. Verwenden Sie diese Aktivität, um mit Profilen und Daten zu arbeiten, die in einer externen Datei gespeichert sind. Profile und Daten werden nicht zur Datenbank hinzugefügt, aber alle Felder in der Eingabedatei sind verfügbar für [Personalisierung](../../personalization/gs-personalization.md)oder um Profile oder andere Tabellen zu aktualisieren.

>[!NOTE]
>Unterstützte Dateiformate sind: Text (TXT) und kommagetrennte Werte (CSV).

Diese Aktivität kann mit einer [Abstimmung](reconciliation.md) -Aktivität zum Verknüpfen nicht identifizierter Daten mit vorhandenen Ressourcen. Beispiel: die **Datei laden** -Aktivität platziert werden, bevor eine **Abstimmung** Aktivität , wenn Sie nicht standardmäßige Daten in die Datenbank importieren.

## Konfigurieren der Aktivität Datei laden {#load-configuration}

Führen Sie die folgenden Schritte aus, um die **Datei laden** Aktivität:

1. Ziehen und Ablegen eines **Datei laden** in Ihren Workflow ein. Klicken Sie auf **Aus Datei auswählen** Schaltfläche.

1. Wählen Sie die zu verwendende lokale Datei aus. Das Format muss mit diesem [Beispieldatei](../../audience/file-audience.md#sample-file).

1. Im mittleren Abschnitt des Bildschirms können Sie eine Vorschau der Datenzuordnung anzeigen, um sie zu überprüfen.

   ![](../assets/load-file.png)

1. Verwenden Sie die **Spalten** im linken Bereich, um den Datentyp und die Breite für jede Spalte anzupassen.

1. Im **Formatierung** Geben Sie im Bereich unter der Spaltenkonfiguration an, wie die externe Datei formatiert wird, um sicherzustellen, dass die Daten korrekt importiert werden.

1. Klicken Sie auf **Bestätigen**, wenn die Einstellungen korrekt sind.

## Beispiel{#load-example}

Beispiel für ein Laden einer externen Datei, das mit der Variablen **Abstimmung** ist verfügbar unter [diesem Abschnitt](reconciliation.md#example).