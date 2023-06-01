---
audience: end-user
title: Workflow-Aktivität "Und-Verknüpfung" verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Und-Verknüpfung verwenden.
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 27%

---


# Und-Verknüpfung {#join}

Die **Und-Verknüpfung** ermöglicht die Synchronisation mehrerer Ausführungszweige eines Workflows.

Bei einer Und-Verknüpfung wird die ausgehende Transition erst aktiviert, wenn alle eingehenden Transitionen aktiviert wurden, d. h. wenn alle vorangehenden Aktivitäten beendet sind.

Führen Sie die folgenden Schritte aus, um die **Und-Verknüpfung** Aktivität:

1. Hinzufügen mehrerer Aktivitäten wie **Kombinieren** Aktivitäten, um mindestens zwei verschiedene Ausführungszweige zu bilden.
1. Hinzufügen einer **Und-Verknüpfung** -Aktivität zu einem der Zweige.
1. Im **Zusammenführungsoptionen** alle vorherigen Aktivitäten, denen Sie beitreten möchten.
1. Wählen Sie die **Primärer Satz** in der ausgehenden Transition beibehalten werden.
