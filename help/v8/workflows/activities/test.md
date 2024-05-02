---
audience: end-user
title: Verwenden Sie die Workflow-Aktivität Test .
description: Erfahren Sie, wie Sie die Workflow-Aktivität Test verwenden.
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Test {#test}

Die **Test** -Aktivität **Flusssteuerung** -Aktivität. Sie ermöglicht die Aktivierung von Transitionen auf der Basis der angegebenen Bedingungen.

## Konfigurieren der Test -Aktivität {#test-configuration}

Führen Sie die folgenden Schritte aus, um die **Test** Aktivität:

1. Fügen Sie eine **Test**-Aktivität zu Ihrem Workflow hinzu.

1. Standardmäßig wird die Variable **[!UICONTROL Test]** -Aktivität stellt einen einfachen booleschen Test dar. Wenn die in der Transition &quot;True&quot; definierte Bedingung erfüllt ist, wird diese Transition aktiviert. Andernfalls wird die standardmäßige Transition &quot;False&quot;aktiviert.

1. Um die einer Transition zugeordnete Bedingung zu konfigurieren, klicken Sie auf das **[!UICONTROL Personalisierungsdialogfeld öffnen]** Symbol. Definieren Sie mithilfe des Ausdruckseditors die Regeln, die zum Aktivieren dieser Transition erforderlich sind. Sie können auch Ereignisvariablen, Bedingungen und Datums-/Uhrzeitfunktionen nutzen. [Erfahren Sie, wie Sie mit Ereignisvariablen und dem Ausdruckseditor arbeiten.](../event-variables.md)

   Darüber hinaus können Sie die **[!UICONTROL Titel]** -Feld, um den Namen der Transition auf der Arbeitsfläche des Workflows zu personalisieren.

   ![](../assets/workflow-test-default.png)

1. Sie können einer **[!UICONTROL Test]** -Aktivität. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Bedingung hinzufügen]** und konfigurieren Sie den Titel und die zugehörige Bedingung für jede Transition.

1. Während der Ausführung des Workflows wird jede Bedingung nacheinander getestet, bis eine der Bedingungen erfüllt ist. Wenn keine der Bedingungen erfüllt ist, wird der Workflow entlang des Pfads der **[!UICONTROL Standardbedingung]**. Wenn keine Standardbedingung aktiviert ist, werden die Workflows an dieser Stelle beendet.

## Beispiel {#example}

In diesem Beispiel werden je nach Anzahl der Profile, die von einer **[!UICONTROL Audience erstellen]** Aktivität:
* Bei mehr als 10.000 Zielgruppenprofilen wird eine E-Mail-Nachricht gesendet.
* Für 1.000 bis 10.000 Profile wird eine SMS gesendet.
* Wenn die Zielgruppenprofile unter 1.000 fallen, werden sie an die Transition &quot;Keine Kontakte&quot; weitergeleitet.

![](../assets/workflow-test-example.png)

Dazu muss die Variable `vars.recCount` -Ereignisvariable in den Bedingungen &quot;E-Mail&quot; und &quot;SMS&quot; verwendet wurde, um die Anzahl der Zielgruppenprofile zu zählen und die entsprechende Transition zu aktivieren.

![](../assets/workflow-test-example-config.png)
