---
audience: end-user
title: Anzeigen des Versandinhalts in einer Vorschau
description: Erfahren Sie, wie Sie mit der Campaign Web-Benutzeroberfläche den Versandinhalt in einer Vorschau anzeigen können.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 100%

---


# Vorschau des Nachrichteninhalts {#preview-content}

Verwenden Sie die Inhaltssimulationsfunktion von [!DNL Campaign], um den Nachrichteninhalt vor dem Senden in einer Vorschau anzuzeigen. Auf diese Weise können Sie die Personalisierung steuern und überprüfen, wie sie Ihren Empfängerinnen und Empfängern angezeigt wird.

Gehen Sie wie folgt vor, um den Versandinhalt in einer Vorschau anzuzeigen.

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ Ihres Versands und klicken Sie dann auf [E-Mail-Designer](../email/get-started-email-designer.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

   ![](assets/simulate-button.png){zoomable=&quot;yes&quot;}

1. Wählen Sie die Profile aus, die für die Vorschau des Inhalts verwendet werden sollen. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Hinzufügen von Testprofilen]** (für E-Mail und SMS) oder auf die Schaltfläche **[!UICONTROL Abonnenten hinzufügen]** (für Push-Benachrichtigungen).

1. Sie können Profile und Testprofile miteinander kombinieren, um Ihre E-Mail- oder SMS-Nachricht in einer Vorschau anzuzeigen.

   * Die Registerkarte **[!UICONTROL Testprofile]** enthält Testprofile für zusätzliche, fiktive Empfängerinnen und Empfänger in der Datenbank. [Erfahren Sie, wie Sie mit Testprofilen arbeiten](../audience/test-profiles.md)

   * Die Registerkarte **[!UICONTROL Profile]** enthält alle in Ihrer Datenbank gespeicherten Profile. [Erfahren Sie, wie Sie mit Profilen arbeiten](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable=&quot;yes&quot;}

1. Beim Durchsuchen der Testprofile oder Profillisten können Sie Filter verwenden, um Ihre Suche zu verfeinern. Sie können beispielsweise eine Regel definieren, um nach allen Testprofilen mit dem Status **[!UICONTROL Interessent]** zu suchen. [Erfahren Sie, wie Sie Regeln mithilfe des Abfrage-Modelers hinzufügen](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Klicken Sie auf **[!UICONTROL Auswählen]**, um Ihre Auswahl zu bestätigen.

   Eine Vorschau des Versandinhalts wird im rechten Bereich des Bildschirms **[!UICONTROL Simulieren]** angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde.

   ![](assets/simulate-preview.png){zoomable=&quot;yes&quot;}

1. Wenn mehrere Profile hinzugefügt wurden, können Sie in der Liste zwischen diesen wechseln, um eine Vorschau des entsprechenden Versandinhalts anzuzeigen. Sie können auch weitere Testprofile hinzufügen und Ihre Auswahl mithilfe der entsprechenden Schaltflächen im linken Bereich löschen.

1. Beim Versand von E-Mails können Sie den **[!UICONTROL Zoom-Faktor]** einstellen und den Inhalt über das entsprechende Symbol oben rechts auf dem Desktop oder einem Mobilgerät in einer Vorschau anzeigen.

1. Auf dem Bildschirm **[!UICONTROL Simulieren]** können Sie auch folgende Aktionen durchführen:
   * Durchführen von Testsendungen zur Validierung an bestimmte Empfangende: [Weitere Informationen](test-deliveries.md)
   * Zugreifen auf die Protokolle der durchgeführten Testsendungen: [Weitere Informationen](test-deliveries.md#access-test-deliveries)
   * (Nur für E-Mails) Überprüfen des Renderings des Nachrichteninhalts in gängigen E-Mail-Clients: [Weitere Informationen](email-rendering.md)



