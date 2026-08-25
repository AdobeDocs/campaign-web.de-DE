---
audience: end-user
title: Erstellen von Workflows mit Adobe Campaign Web
description: Erfahren Sie, wie Sie Workflows mit Adobe Campaign Web erstellen
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
TQID: https://experienceleague.adobe.com/D9lkZe8AvBCas-wt-Fe6GLaAoBR-JJNfAHSrRrpkP-w
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
source-git-commit: 6e68cd4e3741b480dc04d8a86d0cf6cb07835811
workflow-type: ht
source-wordcount: 1720
ht-degree: 100%

---

# Orchestrieren von Aktivitäten {#orchestrate}

Sobald Sie einen [Workflow erstellt](create-workflow.md) haben, sei es über das Workflow-Menü oder innerhalb einer Kampagne, können Sie mit der Orchestrierung der verschiedenen Aufgaben beginnen, die er ausführen soll. Zu diesem Zweck wird eine visuelle Arbeitsfläche bereitgestellt, über die Sie ein Workflow-Diagramm erstellen können. Innerhalb dieses Diagramms können Sie verschiedene Aktivitäten hinzufügen und sie in einer sequentiellen Reihenfolge miteinander verbinden. Auf der Arbeitsfläche werden horizontale und vertikale Bildlaufleisten angezeigt, mit denen Sie in großen Workflows durch Ziehen direkt zu dem Bereich navigieren können, den Sie anzeigen möchten.

## Hinzufügen von Aktivitäten {#add}

In diesem Schritt der Konfiguration wird das Diagramm mit einem Startsymbol angezeigt, das den Anfang Ihres Workflows darstellt. Um Ihre erste Aktivität hinzuzufügen, klicken Sie auf die Schaltfläche **+**, die mit dem Startsymbol verbunden ist.

Es erscheint eine Liste von Aktivitäten, die dem Diagramm hinzugefügt werden können. Die verfügbaren Aktivitäten hängen von Ihrer Position im Workflow-Diagramm ab. Wenn Sie Ihre erste Aktivität hinzufügen, können Sie Ihren Workflow starten, indem Sie beispielsweise eine Zielgruppe ansprechen, den Workflow-Pfad aufteilen oder eine **Warte-Aktivität** festlegen, um die Ausführung des Workflows zu verzögern. Nach einer Aktivität **Zielgruppe erstellen** können Sie Ihre Zielgruppe mit Zielgruppenbestimmungsaktivitäten verfeinern, einen Versand an Ihre Zielgruppe mit Kanalaktivitäten durchführen oder den Workflow-Prozess mit Flusskontrollaktivitäten organisieren.

![Workflow-Startsymbol und Aktivitätsoptionen](assets/workflow-start.png){zoomable="yes"}

Sobald eine Aktivität zum Diagramm hinzugefügt wurde, wird rechts ein Bereich angezeigt, in dem Sie die neu hinzugefügte Aktivität mit spezifischen Einstellungen konfigurieren können. Detaillierte Informationen über die Konfiguration jeder Aktivität finden Sie in [diesem Abschnitt](activities/about-activities.md).

![Panel zur Konfiguration von Aktivitäten](assets/workflow-configure-activities.png){zoomable="yes"}

Wiederholen Sie diesen Vorgang, um je nach den Aufgaben, die Ihr Workflow ausführt, so viele Aktivitäten wie nötig hinzuzufügen. Sie können auch eine neue Aktivität zwischen zwei Aktivitäten einfügen. Klicken Sie dazu auf die Schaltfläche **+** in der Transition zwischen den Aktivitäten, wählen Sie die gewünschte Aktivität aus und konfigurieren Sie sie im rechten Bereich.

Um eine Aktivität zu entfernen, wählen Sie sie auf der Arbeitsfläche aus und klicken in den Eigenschaften der Aktivität auf das Symbol **Löschen**. Unter [Löschen und Trennen von Aktivitäten](#delete) finden Sie die verfügbaren Optionen.

>[!TIP]
>
>Sie können den Namen der Transitionen zwischen den einzelnen Aktivitäten personalisieren. Wählen Sie dazu die Transition aus und ändern Sie das Label im rechten Bereich.

## Die Symbolleiste {#toolbar}

Die Symbolleiste, die sich in der oberen rechten Ecke der Arbeitsfläche befindet, bietet Optionen, um die Aktivitäten einfach zu bearbeiten und in der Arbeitsfläche zu navigieren.

* **Mehrfachauswahl-Modus**: Wählen Sie mehrere Aktivitäten aus, um sie alle gleichzeitig zu löschen oder zu kopieren/einzufügen. Siehe [diesen Abschnitt](#copy).
* **Verzweigung hinzufügen**: Klicken Sie in der Symbolleiste auf die Schaltfläche **+**, um eine separate Ausführungsverzweigung auf der Arbeitsfläche zu erstellen. Das Ergebnis entspricht der Verwendung einer [Verzweigung](activities/fork.md) für parallele Pfade, das Diagramm ist jedoch grafisch klarer.
* **Drehen**: Dreht die Arbeitsfläche vertikal.
* **An Bildschirm anpassen**: Passt die Vergrößerung der Arbeitsfläche an Ihren Bildschirm an.
* **Verkleinern**/**Vergrößern**: Verkleinert bzw. vergrößert die Arbeitsfläche.
* **Karte anzeigen**: Öffnet einen Snapshot der Arbeitsfläche mit Ihrer aktuellen Position.

![Symbolleistenoptionen für die Workflow-Arbeitsfläche](assets/workflow-toolbar.png){zoomable="yes"}{width="50%"}

## Verwalten von Aktivitäten {#manage}

Beim Hinzufügen von Aktivitäten sind im Bereich mit den Eigenschaften Aktionsschaltflächen verfügbar, mit denen Sie mehrere Vorgänge ausführen können.

![Aktionsschaltflächen für Aktivitäten](assets/activity-action.png){zoomable="yes"}

Sie haben folgende Möglichkeiten:

* **Löschen** der Aktivität von der Arbeitsfläche aus. Siehe [diesen Abschnitt](#delete-activity).
* **Deaktivieren/Aktivieren** der Aktivität. Wenn der Workflow ausgeführt wird, werden deaktivierte Aktivitäten und auf demselben Pfad folgende Aktivitäten nicht ausgeführt und der Workflow wird angehalten.
* **Anhalten/Fortsetzen** der Aktivität. Wenn der Workflow ausgeführt wird, wird er bei der angehaltenen Aktivität angehalten. Die entsprechende Aufgabe sowie alle auf demselben Pfad folgenden Aufgaben werden nicht ausgeführt.
* **Kopieren** der Aktivität. Siehe [diesen Abschnitt](#copy).
* **Verschieben** Sie eine Aktivität und alle untergeordneten Knoten in eine andere Transition. Siehe [diesen Abschnitt](#move).
* Rufen Sie die **Ausführungsoptionen** der Aktivität auf.
* Zugreifen auf die **Protokolle und Aufgaben** der Aktivität.

Bei mehreren **Zielgruppenbestimmungsaktivitäten**, z. B. **Kombinieren** oder **Deduplizierung**, können Sie die verbleibende Population verarbeiten und in eine zusätzliche ausgehende Transition einschließen. Wenn Sie beispielsweise die Aktivität **Aufspaltung** verwenden, besteht das Komplement aus der Population, die keiner der zuvor definierten Teilmengen entsprochen hat. Um diese Funktion zu verwenden, aktivieren Sie die Option **Komplement erzeugen**.

![Aktivität „Aufspaltung“ mit Komplement-Option](assets/workflow-split-complement.png)

## Verschieben oder Kopieren von Aktivitäten {#move-copy}

### Kopieren und Einfügen von Aktivitäten {#copy}

Sie können Workflow-Aktivitäten kopieren und in einen beliebigen Workflow einfügen. Der Ziel-Workflow kann sich auf einer anderen Browser-Registerkarte befinden.

Zum Kopieren von Aktivitäten haben Sie zwei Möglichkeiten:

* Kopieren Sie eine Aktivität mithilfe der Aktionsschaltfläche.

  ![Schaltfläche zum Kopieren einer einzelnen Aktivität](assets/workflow-copy.png){zoomable="yes"}{width="70%"}

* Kopieren Sie mehrere Aktivitäten mithilfe der Symbolleistenschaltfläche.

  ![Schaltfläche zum Kopieren mehrerer Aktivitäten](assets/workflow-copy-2.png){zoomable="yes"}{width="70%"}

Um die kopierten Aktivitäten einzufügen, klicken Sie auf die Schaltfläche **+** in einer Transition und wählen Sie „Aktivität X einfügen“ aus.

![Option zum Einfügen kopierter Aktivitäten](assets/workflow-copy-3.png){zoomable="yes"}{width="50%"}

### Verschieben von Aktivitäten und ihren untergeordneten Knoten {#move}

Mit Journey Optimizer können Sie eine Aktivität zusammen mit dem gesamten Inhalt ihrer untergeordneten Knoten (einschließlich aller darin enthaltenen Transitionen und Aktivitäten) an das Ende einer anderen Transition innerhalb desselben Workflows verschieben.

Dieser Prozess trennt die Aktivität und alles, was sich in ihrer ausgehenden Transition befindet, vom ursprünglichen Speicherort und verschiebt sie zur neuen Zieltransition.

So verschieben Sie eine Aktivität:

1. Wählen Sie die Aktivität aus, die verschoben werden soll.
1. Klicken Sie im Bereich mit den Eigenschaften der Aktivität auf die Schaltfläche **Verschieben**.
1. Wählen Sie die Transition, in der die Aktivität platziert werden soll, und die ausgehende Transition aus, und bestätigen Sie dann die Auswahl.

![Verschieben der Aktivität und untergeordneter Knoten](assets/activity-move.png)

## Löschen und Trennen von Aktivitäten {#delete}

### Löschen einer Aktivität {#delete-activity}

Um eine Aktivität zu löschen, wählen Sie sie auf der Arbeitsfläche aus und klicken Sie in den Eigenschaften der Aktivität auf das Symbol **Löschen**. Ein Bestätigungsdialogfeld wird angezeigt.

* Wenn die Aktivität nicht mit einer anderen Aktivität verbunden ist, bestätigen Sie, dass Sie sie löschen möchten.

  ![Einfaches Löschen einer Aktivität](assets/workflow-delete.png)

* Wenn die Aktivität mit einer oder mehreren nachfolgenden Aktivitäten verbunden ist, wählen Sie aus, wie mit diesen umgegangen werden soll:

  ![Löschen mehrerer Aktivitäten](assets/workflow-delete2.png)

  * **Alle nachfolgenden Aktivitäten löschen**: Entfernt die Aktivität und alle Aktivitäten, die ihr auf demselben Pfad folgen.
  * **Nur diese Aktivität löschen**: Entfernt nur die ausgewählte Aktivität und stellt die Verbindung zum verbleibenden Pfad wieder her. Diese Option steht nur dann zur Verfügung, wenn die Aktivität genau einen Nachfolger hat.
  * **Löschen und neue Verzweigung erstellen**: Entfernt die ausgewählte Aktivität, behält jedoch ihre nachfolgenden Aktivitäten bei und verschiebt sie in eine neue, separate Verzweigung.

Klicken Sie auf **Löschen**, um Ihre Auswahl zu bestätigen, oder auf **Abbrechen**, um das Dialogfeld zu schließen, ohne etwas zu löschen.

### Trennen einer Transition {#disconnect-transition}

Sie können zwei Aktivitäten trennen, ohne eine davon zu löschen. Die Aktivitäten, die nach der getrennten Transition platziert wurden, werden nicht gelöscht: Sie werden in eine neue, separate Verzweigung des Workflows verschoben.

Auf diese Weise können Sie ein Workflow-Diagramm neu organisieren, z. B. um eine Gruppe von Aktivitäten, die Sie beibehalten möchten, vorübergehend beiseite zu legen, ohne sie löschen und neu erstellen zu müssen.

Dies kann in einer einzigen Transition erfolgen:

1. Wählen Sie die Transition aus, die Sie trennen möchten.

1. Klicken Sie in den Eigenschaften der Transition auf das Symbol **Trennen**.

   ![Symbol „Trennen“ im Eigenschaftenbereichs der Transition](assets/workflow-transition.png)

   Dieses Symbol ist nur verfügbar, wenn die Transition zu einer nachgelagerten Aktivität führt. Ein Bestätigungsdialogfeld wird angezeigt.

1. Klicken Sie zum Bestätigen auf **Trennen** oder auf **Abbrechen**, um das Dialogfeld zu schließen, ohne etwas zu trennen.

   ![Bestätigungsdialogfeld zum Trennen einer Transition](assets/workflow-transition2.png)

Wenn die Quellaktivität mehrere ausgehende Transitionen aufweist (z. B. eine Aktivität des Typs **Aufspaltung** mit mehreren Ergebnisverzweigungen oder eine Aktivität des Typs **Verzweigung**), können Sie jede dieser Transitionen einzeln aus dem Eigenschaftsbereich der Aktivität entfernen:

1. Wählen Sie die Aktivität aus und suchen Sie dann im Abschnitt **Segment** nach der Transition, die Sie entfernen möchten.

1. Klicken Sie auf das Papierkorbsymbol neben dieser Transition. Ein Bestätigungsdialogfeld wird angezeigt.

   ![Papierkorbsymbol neben einem Segmentergebnis](assets/workflow-transition3.png)

1. Klicken Sie zum Bestätigen auf **Entfernen** oder auf **Abbrechen**, um das Dialogfeld zu schließen, ohne etwas zu entfernen.

   ![Bestätigungsdialogfeld zum Entfernen einer Transition](assets/workflow-transition4.png)

## Ausführungsoptionen {#execution}

Sie können die Ausführungsoptionen aller Aktivitäten verwalten. Wählen Sie eine Aktivität aus und klicken Sie auf die Schaltfläche **Ausführungsoptionen**. Auf diese Weise können Sie den Ausführungsmodus und das Verhalten der Aktivität im Falle eines Fehlers definieren.

![Panel „Ausführungsoptionen“](assets/workflow-execution-options.png){zoomable="yes"}{width="70%"}

### Eigenschaften {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_activity_execution_options_properties"
>title="Aktivitätseigenschaften"
>abstract="In diesem Abschnitt können Sie die Ausführungseinstellungen für eine Aktivität konfigurieren, einschließlich der auszuführenden Aktion, der maximalen Dauer, der Zeitzone, der Maschinenaffinität und des asynchronen Verhaltens."

Im Feld **Ausführung** können Sie die Aktion definieren, die beim Starten der Aufgabe ausgelöst werden soll.

Im Feld **Maximale Ausführungsdauer** können Sie eine maximale Dauer festlegen, z. B. „30s“ oder „1h“. Wenn eine Aktivität die angegebene Dauer überschreitet, wird ein Warnhinweis ausgelöst. Die Workflow-Ausführung wird hiervon jedoch nicht beeinflusst.

Im Feld **Zeitzone** können Sie der Aktivität eine bestimmte Zeitzone zuweisen. Adobe Campaign kann verschiedene Zeitzonen innerhalb einer Instanz verwalten. Die entsprechenden Einstellungen werden bei der Instanzerstellung vorgenommen.

Das Feld **Affinität** bietet die Möglichkeit, die Ausführung eines Workflows oder einer Workflow-Aktivität an eine bestimmte Engine zu binden. Definieren Sie hierzu eine oder mehrere Affinitäten auf Workflow- oder Aktivitätsebene.

Im Feld **Verhalten** können Sie das Verhalten des Workflows im Fall von asynchronen Aufgaben bestimmen.

### Umgang mit Fehlern {#execution-options}

>[!CONTEXTUALHELP]
>id="acw_workflow_activity_execution_options_error"
>title="Initialisierungsskript"
>abstract="In diesem Abschnitt können Sie festlegen, was geschieht, wenn eine Aktivität fehlschlägt. Sie können Aktionen wie das Stoppen des Workflows, das Wechseln zur nächsten Aktivität oder das Auslösen eines benutzerdefinierten Fehlerbehandlungsprozesses auswählen."

Im Feld **Bei Fehler** können Sie die Aktion festlegen, die ausgeführt werden soll, wenn bei der Aktivität ein Fehler auftritt. Weitere Informationen finden Sie in diesem [Abschnitt](workflow-settings.md#error-settings).

### Initialisierungsskript {#initialization-options}

>[!CONTEXTUALHELP]
>id="acw_workflow_activity_execution_options_initialization"
>title="Initialisierungsskript"
>abstract="In diesem Abschnitt können Sie JavaScript hinzufügen, das ausgeführt wird, wenn die Aktivität beginnt. Verwenden Sie es, um Variablen zu initialisieren, Parameter festzulegen oder Daten speziell für die Ausführung dieser Aktivität vorzubereiten."

Mit dem **Initialisierungsskript** können Sie Variablen initialisieren oder Aktivitätseigenschaften ändern. Klicken Sie auf die Schaltfläche **Code bearbeiten** und geben Sie das auszuführende Code-Fragment ein. Das Skript wird aufgerufen, wenn die Aktivität ausgeführt wird. Weitere Informationen finden Sie im Abschnitt zu den [Ereignisvariablen](../workflows/event-variables.md).

## Beispiel {#example}

Hier ist ein Beispiel für einen Workflow, der eine E-Mail an alle Kundinnen und Kunden (außer VIP) sendet, die an Kaffeemaschinen interessiert sind.

![Beispielhaftes Workflow-Diagramm](assets/workflow-example.png){zoomable="yes"}

Um dies zu bewerkstelligen, wurden die folgenden Aktivitäten hinzugefügt:

* eine Aktivität **[!UICONTROL Verzweigung]**, die den Workflow in drei Pfade unterteilt (einen für jede Kundengruppe),
* Aktivitäten **[!UICONTROL Zielgruppe aufbauen]**, um die drei Kundengruppen anzusprechen:
  * Kundinnen und Kunden mit einer E-Mail-Adresse,
  * Kundinnen und Kunden, die zu der bereits bestehenden Zielgruppe „Interessiert an Kaffeemaschinen“ gehören,
  * Kundinnen und Kunden, die zur bereits bestehenden Zielgruppe „Zu belohnende VIP“ gehören.
* Eine Aktivität **[!UICONTROL Kombinieren]**, die Kundinnen und Kunden mit einer E-Mail-Adresse und solche, die sich für Kaffeemaschinen interessieren, zusammenfasst,
* Eine Aktivität **[!UICONTROL Kombinieren]**, die VIP-Kundinnen und -Kunden ausschließt,
* Eine Aktivität **[!UICONTROL E-Mail-Versand]**, die eine E-Mail an die resultierenden Kundinnen und Kunden sendet.

Wenn Sie den Workflow abgeschlossen haben, fügen Sie am Ende des Diagramms die Aktivität **[!UICONTROL Ende]** hinzu. Diese Aktivität ermöglicht es, das Ende eines Workflows visuell zu markieren, und hat keine funktionalen Auswirkungen.

Nachdem Sie das Workflow-Diagramm erfolgreich entworfen haben, führen Sie den Workflow aus und verfolgen Sie den Fortschritt der verschiedenen Aufgaben. [Erfahren Sie, wie Sie einen Workflow starten und dessen Ausführung überwachen](start-monitor-workflows.md).