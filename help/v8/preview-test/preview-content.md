---
audience: end-user
title: Anzeigen des Versandinhalts in einer Vorschau
description: Erfahren Sie, wie Sie mit der Campaign Web-Benutzeroberfläche den Versandinhalt in einer Vorschau anzeigen können.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '363'
ht-degree: 100%

---

# Vorschau des Nachrichteninhalts {#preview-content}

Verwenden Sie die Inhaltssimulationsfunktion von [!DNL Campaign], um den Nachrichteninhalt vor dem Senden in einer Vorschau anzuzeigen. Mit dieser Funktion können Sie die Personalisierung steuern und überprüfen, wie die Nachricht Ihren Empfängerinnen und Empfängern angezeigt wird.

Gehen Sie wie folgt vor, um eine Vorschau des Inhalts Ihres Versands anzuzeigen:

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ Ihres Versands und klicken Sie dann auf [E-Mail-Designer](../email/get-started-email-designer.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

   ![Bild, das die Schaltfläche „Inhalte simulieren“ zeigt](assets/simulate-button.png){zoomable="yes"}

1. Wählen Sie die Profile aus, die für die Vorschau des Inhalts verwendet werden sollen. Klicken Sie zum Ausführen dieser Aktion auf die Schaltfläche **[!UICONTROL Testprofil(e) hinzufügen]** (für E-Mail und SMS) oder auf die Schaltfläche **[!UICONTROL Abonnierende hinzufügen]** (für Push-Benachrichtigungen).

1. Kombinieren Sie Profile und Testprofile miteinander, um Ihre E-Mail- oder SMS-Nachricht in einer Vorschau anzuzeigen.

   * Die Registerkarte **[!UICONTROL Testprofile]** enthält Testprofile für zusätzliche, fiktive Empfängerinnen und Empfänger in der Datenbank. [Erfahren Sie, wie Sie mit Testprofilen arbeiten](../audience/test-profiles.md).

   * Die Registerkarte **[!UICONTROL Profile]** enthält alle in Ihrer Datenbank gespeicherten Profile. [Erfahren Sie, wie Sie mit Profilen arbeiten](../audience/about-recipients.md).

   ![Bild, das die Auswahl von Profilen zeigt](assets/simulate-select-profiles.png){zoomable="yes"}

1. Verwenden Sie Filter beim Durchsuchen der Testprofile oder Profillisten, um Ihre Suche zu präzisieren. Sie können beispielsweise eine Regel definieren, um nach allen Testprofilen mit dem Status **[!UICONTROL potenzieller Kunde]** zu suchen. [Erfahren Sie, wie Sie Regeln mithilfe des Abfrage-Modelers hinzufügen](../query/query-modeler-overview.md).

   ![Bild, das auf Testprofile angewendete Filter zeigt](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Auswählen]**, um Ihre Auswahl zu bestätigen.

   Eine Vorschau des Versandinhalts wird im rechten Bereich des Bildschirms **[!UICONTROL Simulieren]** angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde.

   ![Bild, das die Vorschau des Versandinhalts zeigt](assets/simulate-preview.png){zoomable="yes"}

1. Wenn mehrere Profile hinzugefügt wurden, können Sie in der Liste zwischen diesen wechseln, um eine Vorschau des entsprechenden Versandinhalts anzuzeigen. Fügen Sie weitere Testprofile hinzu oder löschen Sie Ihre Auswahl mithilfe der entsprechenden Schaltflächen im linken Bereich.

1. Stellen Sie bei E-Mail-Sendungen den **[!UICONTROL Zoomfaktor]** ein und zeigen Sie den Inhalt über das entsprechende Symbol oben rechts auf dem Desktop oder einem Mobilgerät in einer Vorschau an.

1. Auf dem Bildschirm **[!UICONTROL Simulieren]** können Sie auch folgende Aktionen durchführen:
   * Durchführen von Testsendungen zur Validierung an bestimmte Empfangende: [Weitere Informationen](test-deliveries.md).
   * Zugreifen auf die Protokolle der durchgeführten Testsendungen: [Weitere Informationen](test-deliveries.md#access-test-deliveries).
   * (Nur für E-Mails) Überprüfen des Renderings des Nachrichteninhalts in gängigen E-Mail-Clients: [Weitere Informationen](email-rendering.md).