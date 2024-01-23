---
audience: end-user
title: Filtern von Listen
description: Erfahren Sie, wie Sie in Adobe Campaign Web-Listen mithilfe integrierter und benutzerdefinierter Filter filtern.
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 7f4d8a2c2b0592515c25628f35234311dc61b4fd
workflow-type: ht
source-wordcount: '308'
ht-degree: 100%

---


# Filtern von Listen {#filter-lists}

Adobe Campaign Web bietet Filter in jeder Objektliste, mit denen Sie Informationen nach bestimmten Kontextkriterien filtern können. Sie können beispielsweise Sendungen nach Status, Kanal, Kontaktdatum oder Ordner filtern. Sie können auch Tests ausblenden.

## Anwenden von Filtern{#apply}

Um Filter auf eine Liste anzuwenden, klicken Sie auf **[!UICONTROL Filter anzeigen]** links oben in der Liste neben der Suchleiste.

Der Filterbereich wird geöffnet und zeigt die für die ausgewählte Liste verfügbaren Filter an. Sie können beispielsweise Kampagnen nach Status, Start- und Enddatum oder Speicherordner filtern, während die Liste der Abonnementdienste nach Kanal und Speicherordner gefiltert werden kann.

![](assets/filters-pane.png){width="70%" align="left" zoomable="yes"}

Um eine Liste nach Ihren eigenen Kriterien zu filtern, können Sie einen benutzerdefinierten Filter erstellen. Navigieren Sie dazu zum unteren Ende des Filterbereichs und klicken Sie auf **Regeln hinzufügen**. [Erfahren Sie, wie Sie vordefinierte Filter erstellen](#custom)

Nachdem Sie Filter auf eine Liste angewendet haben, werden sie unter der Suchleiste angezeigt. Sie können einen jederzeit einzelne Filter entfernen oder auch alle, indem Sie auf **Alle löschen** klicken.

## Erstellen benutzerdefinierter Filter {#custom}

Mit benutzerdefinierten Filtern können Sie Listen anhand Ihrer eigenen spezifischen Kriterien verfeinern. Sie werden mithilfe des Abfrage-Modelers in Campaign entwickelt. Gehen Sie wie folgt vor, um einen benutzerdefinierten Filter zu erstellen:

1. Öffnen Sie das Filterfenster und klicken Sie auf **Regeln hinzufügen** unten im Fenster.
1. Es öffnet sich der Abfrage-Modeler. Definieren und kombinieren Sie Ihre Filterkriterien entsprechend Ihren Anforderungen. Detaillierte Informationen über die Verwendung des Abfrage-Modelers finden Sie in [diesem Abschnitt](../query/query-modeler-overview.md).

   Das folgende Beispiel zeigt einen benutzerdefinierten Filter, der dazu bestimmt ist, in der Kampagnenliste SMS-Kampagnen anzuzeigen, die von Benutzenden der Abteilungen „Laufen“ oder „Yoga“ ausgeführt werden.

   ![](assets/filters-sample.png){width="70%" align="left" zoomable="yes"}

1. Sobald Ihr benutzerdefinierter Filter konfiguriert ist, klicken Sie auf **[!UICONTROL Bestätigen]**, um ihn auf die Liste anzuwenden.
