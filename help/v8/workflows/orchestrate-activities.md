---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 51%

---

# Orchestrieren von Aktivitäten {#orchestrate}

Sobald Sie [einen Workflow erstellt haben](create-workflow.md) ob im Workflow-Menü oder innerhalb einer Kampagne, können Sie mit der Orchestrierung der verschiedenen Aufgaben beginnen, die er ausführt. Zu diesem Zweck wird eine visuelle Arbeitsfläche bereitgestellt, über die Sie ein Workflow-Diagramm erstellen können. Innerhalb dieses Diagramms können Sie verschiedene Aktivitäten hinzufügen und sie in einer sequentiellen Reihenfolge miteinander verbinden.

## Hinzufügen von Aktivitäten {#add}

In diesem Schritt der Konfiguration wird das Diagramm mit einem Startsymbol angezeigt, das den Anfang Ihres Workflows darstellt. Um Ihre erste Aktivität hinzuzufügen, klicken Sie auf die Schaltfläche **+**, die mit dem Startsymbol verbunden ist.

Es erscheint eine Liste von Aktivitäten, die dem Diagramm hinzugefügt werden können. Die verfügbaren Aktivitäten hängen von Ihrer Position im Workflow-Diagramm ab. Wenn Sie Ihre erste Aktivität hinzufügen, können Sie Ihren Workflow starten, indem Sie beispielsweise eine Zielgruppe ansprechen, den Workflow-Pfad aufteilen oder eine **Warte-Aktivität** festlegen, um die Ausführung des Workflows zu verzögern. Nach der Aktivität **Zielgruppe aufbauen** können Sie Ihre Zielgruppe mit Zielgruppenbestimmungsaktivitäten verfeinern, einen Versand an Ihre Zielgruppe mit Kanalaktivitäten durchführen oder den Workflow-Prozess mit Flusssteuerungsaktivitäten organisieren.

![Workflow-Startsymbol und Aktivitätsoptionen](assets/workflow-start.png){zoomable="yes"}

Nachdem eine Aktivität zum Diagramm hinzugefügt wurde, wird ein rechter Bereich angezeigt, in dem Sie die neu hinzugefügte Aktivität mit bestimmten Einstellungen konfigurieren können. Detaillierte Informationen über die Konfiguration jeder Aktivität finden Sie in [diesem Abschnitt](activities/about-activities.md).

![Konfigurationsbereich für Aktivitäten](assets/workflow-configure-activities.png){zoomable="yes"}

Wiederholen Sie diesen Vorgang, um je nach den Aufgaben, die Ihr Workflow ausführt, so viele Aktivitäten wie nötig hinzuzufügen. Sie können auch eine neue Aktivität zwischen zwei Aktivitäten einfügen. Klicken Sie dazu auf die Schaltfläche **+** auf der Transition zwischen den Aktivitäten, wählen Sie die gewünschte Aktivität aus und konfigurieren Sie sie im rechten Bereich.

Um eine Aktivität zu entfernen, wählen Sie sie auf der Arbeitsfläche aus und klicken in den Eigenschaften der Aktivität auf das Symbol **Löschen**.

>[!TIP]
>
>Sie können den Namen der Transitionen zwischen den einzelnen Aktivitäten personalisieren. Wählen Sie dazu die Transition aus und ändern Sie die Bezeichnung im rechten Bereich.

## Die Symbolleiste {#toolbar}

Die Symbolleiste oben rechts auf der Arbeitsfläche bietet Optionen zur einfachen Bearbeitung der Aktivitäten und zur Navigation auf der Arbeitsfläche:

* **Mehrfachauswahl-Modus**: Wählen Sie mehrere Aktivitäten aus, um sie alle gleichzeitig zu löschen oder zu kopieren/einzufügen. Weitere Informationen finden Sie [in diesem Abschnitt](#copy).
* **Drehen**: Dreht die Arbeitsfläche vertikal.
* **An Bildschirm anpassen**: Passt die Vergrößerung der Arbeitsfläche an Ihren Bildschirm an.
* **Verkleinern**/**Vergrößern**: Verkleinert bzw. vergrößert die Arbeitsfläche.
* **Karte anzeigen**: Öffnet einen Schnappschuss der Arbeitsfläche, der Ihren Standort anzeigt.

![Symbolleistenoptionen für die Workflow-Arbeitsfläche](assets/workflow-toolbar.png){zoomable="yes"}{width="50%"}

## Verwalten von Aktivitäten {#manage}

Beim Hinzufügen von Aktivitäten sind im Bereich mit den Eigenschaften Aktionsschaltflächen verfügbar, mit denen Sie mehrere Vorgänge ausführen können. 

![Aktivitätsaktionsschaltflächen](assets/activity-action.png){zoomable="yes"}

Sie haben folgende Möglichkeiten:

* **Löschen** der Aktivität von der Arbeitsfläche aus.
* **Deaktivieren/Aktivieren** der Aktivität. Wenn der Workflow ausgeführt wird, werden deaktivierte Aktivitäten und die folgenden Aktivitäten im selben Pfad nicht ausgeführt und der Workflow wird angehalten.
* **Anhalten/Fortsetzen** der Aktivität. Wenn der Workflow ausgeführt wird, wird er bei der angehaltenen Aktivität angehalten. Die entsprechende Aufgabe sowie alle Aufgaben, die ihr im selben Pfad folgen, werden nicht ausgeführt.
* **Kopieren** der Aktivität. Weitere Informationen finden Sie in diesem [Abschnitt](#copy).
* **Verschieben** Sie eine Aktivität und alle untergeordneten Knoten in eine andere Transition. Weitere Informationen finden Sie [in diesem Abschnitt](#move).
* Rufen Sie die **Ausführungsoptionen** der Aktivität auf.
* Zugreifen auf die **Protokolle und Aufgaben** der Aktivität.

Verschiedene **Targeting**-Aktivitäten wie **Kombinieren** oder **Deduplizierung** ermöglichen es Ihnen, die verbleibende Population zu verarbeiten und in eine zusätzliche ausgehende Transition einzuschließen. Wenn Sie beispielsweise die Aktivität **Aufspaltung** verwenden, besteht das Komplement aus der Population, die keiner der zuvor definierten Teilmengen entsprochen hat. Um diese Funktion zu verwenden, aktivieren Sie die Option **Komplement erzeugen**.

![Aktivität mit Komplement aufteilen](assets/workflow-split-complement.png)

## Verschieben oder Kopieren von Aktivitäten {#move-copy}

### Kopieren und Einfügen von Aktivitäten {#copy}

Sie können Workflow-Aktivitäten kopieren und in einen beliebigen Workflow einfügen. Der Ziel-Workflow kann sich auf einer anderen Browser-Registerkarte befinden.

Zum Kopieren von Aktivitäten haben Sie zwei Möglichkeiten:

* Kopieren Sie eine Aktivität mithilfe der Aktionsschaltfläche.

  ![Schaltfläche „Einzelne Aktivität kopieren“](assets/workflow-copy.png){zoomable="yes"}{width="70%"}

* Kopieren Sie mehrere Aktivitäten mithilfe der Symbolleistenschaltfläche.

  ![Schaltfläche „Mehrere Aktivitäten kopieren“](assets/workflow-copy-2.png){zoomable="yes"}{width="70%"}

Um die kopierten Aktivitäten einzufügen, klicken Sie auf die Schaltfläche **+** auf einer Transition und wählen Sie „Aktivität X einfügen“.

![Option „Kopierte Aktivitäten einfügen“](assets/workflow-copy-3.png){zoomable="yes"}{width="50%"}

### Verschieben von Aktivitäten und ihren untergeordneten Knoten {#move}

Mit Journey Optimizer können Sie eine Aktivität zusammen mit dem gesamten Inhalt ihrer untergeordneten Knoten (einschließlich aller darin enthaltenen Transitionen und Aktivitäten) an das Ende einer anderen Transition innerhalb desselben Workflows verschieben.

Dieser Prozess trennt die Aktivität und alles, was sich in ihrer ausgehenden Transition befindet, vom ursprünglichen Speicherort und verschiebt sie zur neuen Zieltransition.

So verschieben Sie eine Aktivität:

1. Wählen Sie die Aktivität aus, die Sie verschieben möchten.
1. Klicken Sie im Bereich mit den Eigenschaften der Aktivität auf die Schaltfläche **Verschieben**.
1. Wählen Sie die Transition, in der die Aktivität platziert werden soll, und die ausgehende Transition aus, und bestätigen Sie dann die Auswahl.

![Aktivität und untergeordnete Knoten verschieben](assets/activity-move.png)

## Ausführungsoptionen {#execution}

Sie können die Ausführungsoptionen aller Aktivitäten verwalten.  Wählen Sie eine Aktivität aus und klicken Sie auf **Schaltfläche „Ausführungsoptionen**. Auf diese Weise können Sie den Ausführungsmodus und das Verhalten der Aktivität im Falle eines Fehlers definieren.

![Bedienfeld „Ausführungsoptionen“](assets/workflow-execution-options.png){zoomable="yes"}{width="70%"}

### Eigenschaften

Im Feld **Ausführung** können Sie die Aktion definieren, die beim Start der Aufgabe ausgeführt werden soll.

Im Feld **Maximale Ausführungsdauer** können Sie eine Dauer wie „30s“ oder „1h“ angeben. Wenn die Aktivität nach der angegebenen Dauer nicht beendet wird, wird ein Warnhinweis ausgelöst. Die Workflow-Ausführung wird hiervon jedoch nicht beeinflusst.

Im Feld **Zeitzone** können Sie der Aktivität eine bestimmte Zeitzone zuweisen. Adobe Campaign verwaltet Zeitunterschiede zwischen mehreren Ländern auf derselben Instanz. Die entsprechenden Einstellungen werden bei der Instanzerstellung vorgenommen.

Das Feld **Affinität** bietet die Möglichkeit, die Ausführung eines Workflows oder einer Workflow-Aktivität an eine bestimmte Engine zu binden. Geben Sie dazu eine oder mehrere Affinitäten für den betreffenden Workflow oder die betreffende Aktivität an.

Im Feld **Verhalten** können Sie das Verhalten des Workflows im Fall von asynchronen Aufgaben bestimmen.

### Umgang mit Fehlern

Im Feld **Im Fehlerfall** können Sie die Aktion angeben, die ausgeführt werden soll, wenn bei der Aktivität ein Fehler auftritt.

### Initialisierungsskript

Mit dem **Initialisierungsskript** können Sie Variablen initialisieren oder Aktivitätseigenschaften ändern. Klicken Sie auf die Schaltfläche **Code bearbeiten** und geben Sie das auszuführende Code-Fragment ein. Das Skript wird aufgerufen, wenn die Aktivität ausgeführt wird. Weitere Informationen finden Sie im Abschnitt zu den [Ereignisvariablen](../workflows/event-variables.md).

## Beispiel {#example}

Hier ist ein Beispiel für einen Workflow, der eine E-Mail an alle Kundinnen und Kunden (außer VIP) sendet, die an Kaffeemaschinen interessiert sind.

![Workflow-Beispieldiagramm](assets/workflow-example.png){zoomable="yes"}

Um dies zu erreichen, wurden die folgenden Aktivitäten hinzugefügt:

* Eine Aktivität **[!UICONTROL Verzweigung]** die den Workflow in drei Pfade unterteilt (einen für jede Kundengruppe),
* Aktivitäten **[!UICONTROL Zielgruppe aufbauen]**, um die drei Kundengruppen anzusprechen:
   * Kundinnen und Kunden mit einer E-Mail-Adresse,
   * Kunden, die zur bereits bestehenden Zielgruppe „Interessiert an Kaffeemaschinen“ gehören,
   * Kunden, die zur bereits bestehenden Zielgruppe &quot;VIP zur Belohnung“ gehören.
* Eine Aktivität **[!UICONTROL Kombinieren]**, die Kundinnen und Kunden mit einer E-Mail-Adresse und solche, die sich für Kaffeemaschinen interessieren, zusammenfasst,
* Eine Aktivität **[!UICONTROL Kombinieren]**, die VIP-Kundinnen und -Kunden ausschließt,
* Eine Aktivität **[!UICONTROL E-Mail-Versand]**, die eine E-Mail an die resultierenden Kundinnen und Kunden sendet.

Fügen Sie nach Abschluss des Workflows **[!UICONTROL Aktivität]** Ende“ am Ende des Diagramms hinzu. Diese Aktivität markiert visuell das Ende eines Workflows und hat keine funktionalen Auswirkungen.

Nachdem Sie das Workflow-Diagramm erfolgreich entworfen haben, führen Sie den Workflow aus und verfolgen Sie den Fortschritt der verschiedenen Aufgaben. [Erfahren Sie, wie Sie einen Workflow starten und dessen Ausführung überwachen](start-monitor-workflows.md).