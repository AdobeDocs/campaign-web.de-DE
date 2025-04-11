---
audience: end-user
title: Anzeigen des Versandinhalts in einer Vorschau
description: Erfahren Sie, wie Sie mit der Campaign Web-Benutzeroberfläche den Versandinhalt in einer Vorschau anzeigen können.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 30%

---

# Vorschau des Nachrichteninhalts {#preview-content}

Verwenden Sie die Inhaltssimulationsfunktion von [!DNL Campaign], um den Nachrichteninhalt vor dem Senden in einer Vorschau anzuzeigen. Mit dieser Funktion können Sie die Personalisierung steuern und überprüfen, wie die Nachricht Ihren Empfängerinnen und Empfängern angezeigt wird.

Gehen Sie wie folgt vor, um eine Vorschau des Inhalts Ihres Versands anzuzeigen:

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ Ihres Versands und klicken Sie dann auf [E-Mail-Designer](../email/get-started-email-designer.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

   ![Bild, das die Schaltfläche „Inhalt simulieren“ zeigt](assets/simulate-button.png){zoomable="yes"}

1. Wählen Sie die Profile aus, die für die Vorschau Ihrer Inhalte verwendet werden sollen. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Testprofil(e) hinzufügen]** (für E-Mail und SMS) oder auf die Schaltfläche **[!UICONTROL Abonnenten hinzufügen]** (für Push-Benachrichtigungen).

1. Kombinieren Sie Profile und Testprofile, um Ihre E-Mail- oder SMS-Nachricht in der Vorschau anzuzeigen.

   * Die Registerkarte **[!UICONTROL Testprofile]** enthält Testprofile für zusätzliche, fiktive Empfängerinnen und Empfänger in der Datenbank. [Erfahren Sie, wie Sie mit Testprofilen arbeiten](../audience/test-profiles.md).

   * Die Registerkarte **[!UICONTROL Profile]** enthält alle in Ihrer Datenbank gespeicherten Profile. [Erfahren Sie, wie Sie mit Profilen arbeiten](../audience/about-recipients.md).

   ![Bild, das die Auswahl von Profilen zeigt](assets/simulate-select-profiles.png){zoomable="yes"}

1. Verwenden Sie beim Durchsuchen der Testprofil- oder Profillisten Filter, um die Suche zu verfeinern. Definieren Sie beispielsweise eine Regel, um alle Testprofile mit dem Status **[!UICONTROL Interessent]** zu finden. [Erfahren Sie, wie Sie Regeln mithilfe des Abfrage-Modelers hinzufügen](../query/query-modeler-overview.md).

   ![Bild mit auf Testprofile angewendeten Filtern](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Auswählen]**, um Ihre Auswahl zu bestätigen.

   Eine Vorschau des Versandinhalts wird im rechten Bereich des Bildschirms **[!UICONTROL Simulieren]** angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde.

   ![Bild mit der Vorschau des Versandinhalts](assets/simulate-preview.png){zoomable="yes"}

1. Wenn mehrere Profile hinzugefügt werden, wechseln Sie in der Liste zwischen ihnen, um eine Vorschau des entsprechenden Versandinhalts anzuzeigen. Fügen Sie weitere Testprofile hinzu oder löschen Sie Ihre Auswahl mithilfe der entsprechenden Schaltflächen im linken Bereich.

1. Passen Sie bei E-Mail **[!UICONTROL Sendungen den Zoom-Faktor]** und zeigen Sie Ihre Inhalte mit dem entsprechenden Symbol oben rechts auf einem Desktop oder Mobilgerät in der Vorschau an.

1. Auf dem Bildschirm **[!UICONTROL Simulieren]** haben Sie außerdem folgende Möglichkeiten:
   * Durchführen eines Testversands an bestimmte Empfängerinnen und Empfänger zu Validierungszwecken: [Weitere Informationen](test-deliveries.md).
   * Zugreifen auf die Protokolle der durchgeführten Testsendungen: [Weitere Informationen](test-deliveries.md#access-test-deliveries).
   * (Nur für E-Mails) Überprüfen des Renderings des Nachrichteninhalts in gängigen E-Mail-Clients: [Weitere Informationen](email-rendering.md).