---
audience: end-user
title: Verwenden der Workflow-Aktivität JavaScript-Code
description: Erfahren Sie, wie Sie die Workflow-Aktivität JavaScript-Code verwenden
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 9%

---

# JavaScript-Code {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript-Code"
>abstract="Die **JavaScript-Code** -Aktivität ermöglicht die Ausführung eines JavaScript-Skripts im Kontext eines Workflows. Auf diese Weise können Sie Aktionen durchführen oder Informationen aus der Datenbank sammeln. Verwendung **Einfach** JavaScript-Code-Aktivitäten, um bei der Ausführung des Workflows einen Codeausschnitt auszuführen. **Erweitert** Mit JavaScript-Code-Aktivitäten können Sie komplexere Vorgänge durchführen, indem Sie zwei verschiedene Code-Snippets in einer sequenziellen Reihenfolge ausführen. Beim ersten Start des Workflows wird der erste Aufruf ausgeführt. Jedes Mal, wenn der Workflow erneut ausgeführt wird, wird der im zweiten Aufruf definierte Code ausgeführt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript-Snippet"
>abstract="Definieren Sie das Skript, das beim Ausführen der Aktivität ausgeführt werden soll. Wenn Sie eine **Erweitert** Für die JavaScript-Aktivität müssen Sie zwei Code-Snippets bearbeiten: den ersten Aufrufcode, der bei der ersten Ausführung des Workflows ausgeführt wird, und den nächsten Aufrufcode, der bei den nächsten Aufrufen des Workflows ausgeführt wird."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript-Ausführung"
>abstract="Konfigurieren Sie die Ausführungsverzögerung so, dass sie die Aktivität nach einer bestimmten Zeit der Ausführung stoppt. Standardmäßig darf die Ausführungsphase nicht länger als eine Stunde dauern. Nach dieser Verzögerung wird der Vorgang mit einer Fehlermeldung abgebrochen und die Ausführung der Aktivität schlägt fehl. Um diese Begrenzung zu ignorieren, setzen Sie den Wert auf 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript-Übergang"
>abstract="Wenn Sie mehrere ausgehende Transitionen hinzufügen möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Transitionen hinzufügen]** Schaltfläche. Dies ermöglicht beispielsweise den Trigger einer bestimmten Transition ausgehend von einer in der JavaScript-Code -Aktivität definierten Bedingung. Diese Option steht für **Erweitert** Nur JavaScript-Code-Aktivitäten."

Die **JavaScript-Code** -Aktivität **Data Management** -Aktivität. Verwenden Sie diese Aktivität, um ein JavaScript-Skript im Kontext eines Workflows auszuführen. Auf diese Weise können Sie Informationen aus der Datenbank erfassen oder andere komplexe Vorgänge durchführen.

## JavaScript-Code-Aktivität konfigurieren {#javascript-code-configuration}

Führen Sie die folgenden Schritte aus, um die **JavaScript-Code** Aktivität:

1. Hinzufügen einer **JavaScript-Code** in Ihren Workflow ein.

1. Wählen Sie den zu erstellenden Aktivitätstyp aus:

   * **Einfach**: Führen Sie ein Codefragment aus.
   * **Erweitert**: Mit dieser Option können Sie erweiterte Vorgänge ausführen, indem Sie zwei verschiedene Codefragmente ausführen. [Erfahren Sie, wie Sie eine erweiterte JavaScript-Aktivität konfigurieren](#advanced)

   >[!NOTE]
   >
   >Mit der Campaign-Webbenutzeroberfläche haben wir zwei Aktivitäten zu einer zusammengefasst, indem wir beide zusammenführen **Einfach** und **Erweitert** JavaScript-Code-Funktionen. Diese Konsolidierung wirkt sich in keiner Weise auf die Funktionalität der Aktivität aus.

1. Klicken Sie dann auf die Schaltfläche **[!UICONTROL Code bearbeiten]** -Schaltfläche, um den Ausdruckseditor zu öffnen. Der linke Seitenbereich enthält vordefinierte Syntaxen, die Sie zur Erstellung Ihres Codes verwenden können, einschließlich Ereignisvariablen. [Erfahren Sie, wie Sie mit Ereignisvariablen und dem Ausdruckseditor arbeiten.](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. Im **[!UICONTROL Ausführung]** konfigurieren Sie die Verzögerung so, dass die Aktivität nach einer bestimmten Ausführungsdauer beendet wird. Standardmäßig darf die Ausführungsphase nicht länger als eine Stunde dauern. Nach dieser Verzögerung wird der Vorgang mit einer Fehlermeldung abgebrochen und die Ausführung der Aktivität schlägt fehl. Um diese Begrenzung zu ignorieren, setzen Sie den Wert auf 0.

   ![](../assets/javascript-config.png)

1. Ein-/Ausschalten der **[!UICONTROL Fehler verarbeiten]** -Option, um während der Skriptausführung auftretende Fehler in einer zusätzlichen ausgehenden Transition zu speichern.

## Erweiterte JavaScript-Code-Aktivitäten {#advanced}

Erweiterte JavaScript-Aktivitäten ermöglichen komplexe Vorgänge. Damit können Sie:

* Führen Sie zwei verschiedene Codefragmente aus. Das erste Codefragment wird ausgeführt, wenn der Workflow zum ersten Mal gestartet wird. Jedes Mal, wenn der Workflow erneut ausgeführt wird, wird das im zweiten Aufruf definierte Codefragment ausgeführt.
* Fügen Sie mehrere ausgehende Transitionen hinzu, mit denen Sie mithilfe eines Skripts dynamisch interagieren können.

Gehen Sie wie folgt vor, um eine erweiterte JavaScript-Code -Aktivität zu konfigurieren:

1. Wählen Sie die **Erweitert** eingeben und konfigurieren Sie dann die auszuführenden Codefragmente:

   * Klicks **[!UICONTROL Erstaufrufcode bearbeiten]** , um das Skript zu definieren, das beim ersten Aufruf ausgeführt werden soll.
   * Klicks **[!UICONTROL Nächsten Anrufcode bearbeiten]** , um das Skript zu definieren, das bei den nächsten Aufrufen des Workflows ausgeführt werden soll. (optional)

1. Um eine oder mehrere ausgehende Transitionen hinzuzufügen, klicken Sie auf die Schaltfläche **[!UICONTROL Transitionen hinzufügen]** und geben Sie für jede Transition einen Titel und einen internen Namen an.

   In diesem Beispiel haben wir zwei Transitionen konfiguriert, die vom Skript im Code-Snippet basierend auf bestimmten Bedingungen aktiviert werden.

   ![](../assets/javascript-transitions.png)

1. Schließen Sie die Konfiguration der Aktivität ab und starten Sie den Workflow.

## Beispiel {#javascript-code-example}

### Initialisieren von Variablen basierend auf der eingehenden Population {#example1}

In diesem Beispiel wird gezeigt, wie eine Variable basierend auf der Anzahl der Profile initialisiert wird, die in einem Workflow angesprochen werden.

![](../assets/javascript-example1.png)

Im vorliegenden Beispiel werden VIP Profile aus unserer Datenbank angesprochen. Wir möchten eine Variable mit dem Namen &quot;channel&quot;mit einem Wert erstellen, der von der Anzahl der Profile abhängt, auf die die Aktivität Audience erstellen abzielt:

* Wenn mehr als 1000 Profile angesprochen werden, initialisieren Sie die Variable mit dem Wert &quot;email&quot;.
* Initialisieren Sie andernfalls den Wert &quot;sms&quot;.

Gehen Sie dazu wie folgt vor:

1. Hinzufügen einer **JavaScript-Code** Aktivität mit dem Typ **Einfach** hinter dem **Audience erstellen** -Aktivität.

1. Klicks **Code bearbeiten** und konfigurieren Sie das Code-Snippet wie folgt:

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. Starten Sie den Workflow. Die Variable &quot;channel&quot; wird je nach Anzahl der Profile, die in der Zielgruppe der Variablen enthalten sind, mit dem Wert &quot;email&quot; oder &quot;sms&quot; erstellt **Audience erstellen** -Aktivität.

### Trigger-Transitionen basierend auf dem Wert einer Variablen {#example2}

In diesem Beispiel wird gezeigt, wie eine Transition basierend auf dem Wert einer Variablen Trigger wird.

![](../assets/javascript-example2-transitions.png)

Im vorliegenden Beispiel beginnt der Workflow mit einer **Externes Signal** -Aktivität, in die eine Variable (`interest`) von einem anderen Workflow übergeben wird. Der Wert der Variablen ist je nach den im ersten Workflow durchgeführten Filtervorgängen entweder &quot;Wird ausgeführt&quot; oder &quot;Yoga&quot;.

Wir möchten verschiedene Transitionen im Workflow basierend auf dem Wert der Variablen Trigger haben.

Gehen Sie dazu wie folgt vor:

1. Hinzufügen einer **JavaScript-Code** Aktivität nach der Aktivität Externes Signal mit dem Typ **Erweitert**.

1. Fügen Sie zwei Transitionen hinzu: eine für jeden möglichen Variablenwert (&quot;running&quot;, &quot;yoga&quot;).

1. Klicks **Erstaufrufcode bearbeiten** und konfigurieren Sie das Code-Snippet wie folgt:

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Schließen Sie die Konfiguration jeder Transition an Ihre Anforderungen an und starten Sie dann den Workflow. Eine der beiden ausgehenden Transitionen wird je nach Wert der `interest` -Variable, die über die **Externes Signal** -Aktivität.
