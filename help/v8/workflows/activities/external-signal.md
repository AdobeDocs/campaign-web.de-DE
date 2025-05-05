---
audience: end-user
title: Verwenden der Aktivität „Externes Signal“
description: Informationen dazu, wie Sie die Workflow-Aktivität „Externes Signal“ verwenden
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 36%

---

# Externes Signal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Externes Signal"
>abstract="Mit der Aktivität **Externes Signal** können Sie die Ausführung eines Workflows über einen anderen Workflow oder einen API-Aufruf auslösen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Parameter von externen Signalen"
>abstract="Parameter von externen Signalen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Trigger für Ende"
>abstract="Trigger für Ende"

Die Aktivität **Externes Signal** ist eine Aktivität zur **Flusskontrolle**. Damit können Sie die Ausführung eines Workflows von einem anderen Workflow oder einem API-Aufruf aus Trigger herstellen.

>[!NOTE]
>
>Auf dieser Seite werden die wichtigsten Schritte zum Konfigurieren **[!UICONTROL Aktivität „Externes Signal]** in der Web-Benutzeroberfläche von Campaign und zum Trigger aus einem anderen Workflow oder API-Aufruf beschrieben. Ausführliche Informationen zum Trigger eines Workflows, zu Best Practices und zur Arbeit mit Campaign-APIs finden Sie in der Dokumentation [Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/de/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example).

Führen Sie die folgenden Schritte aus, um die Aktivität **Externes Signal** zu konfigurieren und deren Ausführung auszulösen:

1. Fügen Sie die Aktivität **Externes Signal** in Ihren Workflow ein.

1. Schließen Sie die Konfiguration Ihres Workflows ab und starten Sie seine Ausführung. Die **[!UICONTROL Externes Signal]**-Aktivität wird als „Ausstehend“ angezeigt, die darauf wartet, ausgelöst zu werden.

   ![Der Screenshot zeigt die Aktivität Externes Signal in einem ausstehenden Status.](../assets/external-signal-pending.png)

1. Rufen Sie die folgenden Informationen ab:

   * Den **internen Namen des Workflows**, der neben dem Titel angezeigt wird.

     +++Beispiel anzeigen

     ![Der Screenshot zeigt den internen Namen des Workflows neben seiner Beschriftung.](../assets/external-signal-workflow-name.png)

     +++

   * Den **Namen der Aktivität „Externes Signal“**, der in den **[!UICONTROL Ausführungsoptionen]** des Workflows angezeigt wird.

     +++Beispiel anzeigen

     ![Der Screenshot zeigt den Namen der Aktivität „Externes Signal“ in den Ausführungsoptionen.](../assets/external-signal-name.png)

     +++

1. Führen Sie zum Trigger des Workflows die `PostEvent` JavaScript-Funktion aus. Mit dieser Funktion können Sie Variablen mit den Werten Ihrer Wahl übergeben und im ausgelösten Workflow verwenden.

   Die `PostEvent` kann entweder von einem anderen Workflow oder von einem API-Aufruf aus ausgeführt werden.

   * Trigger Um eine Aktivität vom Typ **[!UICONTROL Externes Signal]** aus einem Workflow auszuführen, führen Sie die Funktion PostEvent im Bereich **[!UICONTROL Initialisierungsskript]** aus, auf den über die Ausführungsoptionen **[!UICONTROL Aktivität zugegriffen werden kann]**. Führen Sie für die **[!UICONTROL JavaScript-Code]**-Aktivität die Funktion aus dem Skript der Aktivität aus.

     Die Syntax sieht folgendermaßen aus:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Beispiel anzeigen

   In diesem Beispiel wird die externe Signalaktivität „signal1“ ausgelöst. Sie wurde dem Workflow hinzugefügt, dessen interner Name „WKF12345 lautet. Eine Variable namens „customID“ wird mit dem Wert „123456“ übergeben.

   ![Der Screenshot zeigt ein Beispiel für das Auslösen der Aktivität „Externes Signal“ mithilfe der PostEvent-Funktion.](../assets/external-signal-sample.png)

   +++

   * Um die Aktivität **[!UICONTROL Externes Signal]** über einen API-Aufruf auszuführen, befolgen Sie die in der Dokumentation zu Campaign-APIs beschriebenen Schritte. [Erfahren Sie, wie Sie die statische `PostEvent` verwenden](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=de).