---
audience: end-user
title: Filterlisten
description: Erfahren Sie, wie Sie Adobe Campaign-Weblisten mithilfe integrierter und benutzerdefinierter Filter filtern.
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 7f4d8a2c2b0592515c25628f35234311dc61b4fd
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---


# Filterlisten {#filter-lists}

Adobe Campaign Web bietet Filter in jeder Objektliste, mit denen Sie Informationen nach bestimmten Kontextkriterien filtern können. Sie können beispielsweise Sendungen nach Status, Kanal, Kontaktdatum oder Ordner filtern. Sie können auch Tests ausblenden.

## Filter anwenden{#apply}

Um Filter auf eine Liste anzuwenden, klicken Sie auf die Schaltfläche **[!UICONTROL Filter anzeigen]** -Schaltfläche in der linken oberen Ecke der Liste neben der Suchleiste.

Der Filterbereich wird geöffnet und zeigt verfügbare Filter für die ausgewählte Liste an. Sie können beispielsweise Kampagnen nach Status, Start- und Enddatum oder Speicherordner filtern, während die Liste der Abonnementdienste nach Kanal und Speicherordner gefiltert werden kann.

![](assets/filters-pane.png){width="70%" align="left" zoomable="yes"}

Um eine Liste nach Ihren eigenen Kriterien zu filtern, erstellen Sie einen benutzerdefinierten Filter. Navigieren Sie dazu zum unteren Bereich des Filterbereichs und klicken Sie auf die Schaltfläche **Regeln hinzufügen** Schaltfläche. [Erfahren Sie, wie Sie benutzerdefinierte Filter erstellen](#custom)

Nach dem Anwenden auf eine Liste werden Filter unter der Suchleiste angezeigt. Sie können einen einzelnen Filter jederzeit entfernen oder alle Filter entfernen, indem Sie auf die **Alle löschen** Schaltfläche.

## Benutzerdefinierte Filter erstellen {#custom}

Mit benutzerdefinierten Filtern können Sie Listen anhand Ihrer eigenen spezifischen Kriterien verfeinern. Sie werden mithilfe des Campaign-Abfragemodells entwickelt. Gehen Sie wie folgt vor, um einen benutzerdefinierten Filter zu erstellen:

1. Öffnen Sie den Filterbereich und klicken Sie auf die Schaltfläche **Regeln hinzufügen** -Schaltfläche am unteren Rand des Bereichs.
1. Das Abfragemodell wird geöffnet. Definieren und kombinieren Sie Ihre Filterkriterien entsprechend Ihren Anforderungen. Detaillierte Informationen zur Verwendung des Abfragemodells finden Sie unter [diesem Abschnitt](../query/query-modeler-overview.md).

   Das folgende Beispiel zeigt einen benutzerdefinierten Filter, der dazu bestimmt ist, in der Kampagnenliste SMS-Kampagnen anzuzeigen, die von Benutzern der Abteilungen &quot;Ausführen&quot;oder &quot;Yoga&quot;ausgeführt werden.

   ![](assets/filters-sample.png){width="70%" align="left" zoomable="yes"}

1. Sobald Ihr benutzerdefinierter Filter konfiguriert ist, klicken Sie auf **[!UICONTROL Bestätigen]** , um sie auf die Liste anzuwenden.
