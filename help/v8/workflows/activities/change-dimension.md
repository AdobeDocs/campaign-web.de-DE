---
audience: end-user
title: Workflow-Aktivität Dimensionsänderung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Dimensionsänderung verwenden
badge: label="Beta"
source-git-commit: 9b945dcd4151e536e8a8be904100730c86e483b7
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 13%

---


# Ändern der Dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Komplement erzeugen"
>abstract="Sie können eine zusätzliche ausgehende Transition mit der verbleibenden Population generieren, die als Duplikat ausgeschlossen wurde. Schalten Sie dazu die Option **Komplement erzeugen** ein"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Dimensionsaktivität ändern"
>abstract="Mithilfe dieser Aktivität können Sie die Zielgruppendimension beim Erstellen einer Audience ändern. Die Achse wird entsprechend der Datenvorlage und der Eingabedimension verschoben. Sie können beispielsweise von der Dimension &quot;Verträge&quot;zur Dimension &quot;Kunden&quot;wechseln."

Die **Dimensionsänderung** -Aktivität **Targeting** -Aktivität. Mithilfe dieser Aktivität können Sie die Zielgruppendimension beim Erstellen einer Audience ändern. Diese Aktivität verschiebt die Achse je nach Datenvorlage und der eingegebenen Dimension. Sie können beispielsweise von der Dimension &quot;Verträge&quot;zur Dimension &quot;Kunden&quot;wechseln.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Dimensionsänderung** Aktivität:

1. Hinzufügen einer **Dimensionsänderung** -Aktivität zu Ihrem Workflow hinzu.

   ![](../assets/workflow-change-dimension.png)

1. Definieren Sie die **Neue Zieldimension**. Bei Dimensionsänderung werden alle Datensätze beibehalten. Andere Optionen sind noch nicht verfügbar.

1. Führen Sie den Workflow aus, um das Ergebnis anzuzeigen. Vergleichen Sie die Daten in den Tabellen vor und nach der Dimensionsänderung-Aktivität und vergleichen Sie die Struktur der Workflow-Tabellen.



