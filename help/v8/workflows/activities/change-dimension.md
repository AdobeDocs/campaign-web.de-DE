---
audience: end-user
title: Workflow-Aktivität Dimensionsänderung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Dimensionsänderung verwenden
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 24%

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

Sie können diese Aktivität auch verwenden, um die zusätzlichen Spalten der neuen Zielgruppe und Kriterien zur Datendeduplizierung zu definieren.

## Konfiguration

Führen Sie die folgenden Schritte aus, um die **Dimensionsänderung** Aktivität:

1. Hinzufügen einer **Dimensionsänderung** -Aktivität zu Ihrem Workflow hinzu.

   ![](../assets/workflow-change-dimension.png)

1. Definieren Sie die **Neue Zieldimension**.

Bei Dimensionsänderung werden alle Datensätze beibehalten.