---
audience: end-user
title: Workflow-Aktivität Dimensionsänderung verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Dimensionsänderung verwenden
badge: label="Beta"
source-git-commit: 9bb80d10f20bb36162b74982d51ed67c1600f831
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 9%

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

Die **Dimensionsänderung** -Aktivität **Targeting** -Aktivität. Mithilfe dieser Aktivität können Sie die Zielgruppendimension bei der Workflow-Erstellung ändern.
Diese Aktivität verschiebt die Achse je nach Datenvorlage und der eingegebenen Dimension.

Sie können beispielsweise die Zielgruppendimension eines Workflows von &quot;Empfänger&quot;in &quot;Abonnentenanwendung&quot;ändern, um Push-Benachrichtigungen an die Zielempfänger zu senden.

## Konfigurieren der Aktivität Dimensionsänderung {#configure}

Führen Sie die folgenden Schritte aus, um die **Dimensionsänderung** Aktivität:

1. Hinzufügen einer **Dimensionsänderung** -Aktivität zu Ihrem Workflow hinzu.

   ![](../assets/workflow-change-dimension.png)

1. Definieren Sie die **Neue Zieldimension**. Bei Dimensionsänderung werden alle Datensätze beibehalten. Andere Optionen sind noch nicht verfügbar.

1. Führen Sie den Workflow aus, um das Ergebnis anzuzeigen. Vergleichen Sie die Daten in den Tabellen vor und nach der Dimensionsänderung-Aktivität und vergleichen Sie die Struktur der Workflow-Tabellen.

## Beispiel {#example}

In diesem Beispiel möchten wir einen SMS-Versand an alle Profile senden, die einen Kauf getätigt haben. Dazu verwenden wir zunächst eine **[!UICONTROL Audience erstellen]** Aktivität, die mit einer benutzerdefinierten Zielgruppendimension &quot;Kauf&quot;verknüpft ist, um alle erfolgten Käufe auszuwählen.

Wir verwenden dann eine **[!UICONTROL Dimensionsänderung]** -Aktivität, um die Zielgruppendimension des Workflows in &quot;Empfänger&quot;zu ändern. Auf diese Weise können wir die Empfänger ansprechen, die der Abfrage entsprechen.

![](../assets/workflow-change-dimension-example.png)

