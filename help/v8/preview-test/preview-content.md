---
audience: end-user
title: Anzeigen des Versandinhalts in einer Vorschau
description: Erfahren Sie, wie Sie mit der Campaign-Web-Benutzeroberfläche eine Vorschau Ihres Versandinhalts anzeigen können.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: db06e0f54984991e1d6b1056932a9974e340546e
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 85%

---


# Vorschau des Nachrichteninhalts {#preview-content}

Verwenden Sie die Inhaltssimulationsfunktion von [!DNL Campaign], um den Nachrichteninhalt vor dem Senden in einer Vorschau anzuzeigen. Auf diese Weise können Sie die Personalisierung steuern und überprüfen, wie sie Ihren Empfängerinnen und Empfängern angezeigt wird.

Gehen Sie wie folgt vor, um den Versandinhalt in einer Vorschau anzuzeigen.

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ Ihres Versands und klicken Sie dann auf [E-Mail-Designer](../email/get-started-email-designer.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

   ![](assets/simulate-button.png)

1. Um die Profile auszuwählen, die für die Vorschau Ihres personalisierten Inhalts verwendet werden, verwenden Sie folgende Funktionen:

   * **[!UICONTROL Testprofil(e) hinzufügen]** für die Vorschau von E-Mail- und SMS-Sendungen

   * **[!UICONTROL Abonnentin(nen) oder Abonnent(en) hinzufügen]** für die Vorschau von Push-Benachrichtigungen

1. Sie können Profile und Testprofile kombinieren, um eine Vorschau Ihrer E-Mail- oder SMS-Nachricht anzuzeigen.

   * Die Registerkarte **[!UICONTROL Testprofile]** enthält Testadressen für zusätzliche, fiktive Personen in der Datenbank.
     ![](assets/simulate-select-profiles.png)

     Testprofile können über das Menü **[!UICONTROL Kunden-Management]** > **[!UICONTROL Profile]** erstellt werden. [Weitere Informationen](../audience/test-profiles.md#create-test-profiles)


   * Die **[!UICONTROL Profile]** enthält alle in der **[!UICONTROL Profile und Zielgruppen]** Ordner aus dem [!DNL Campaign] Clientkonsole. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html?lang=de){target="_blank"}.

     Sie können Profile über das **[!UICONTROL Profile]** Registerkarte. [Weitere Informationen](../audience/about-recipients.md)


1. Beim Durchsuchen der Testprofilliste oder Profillisten können Sie Filter verwenden, um Ihre Suche zu verfeinern.

   ![](assets/simulate-test-profile-filter.png)

   Sie können beispielsweise eine Regel definieren, um nach allen Testprofilen mit dem Status **[!UICONTROL Interessent]** zu suchen. Erfahren Sie, wie Sie Regeln mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) hinzufügen.

1. Klicken Sie auf **[!UICONTROL Auswählen]**, um Ihre Auswahl zu bestätigen.

   Eine Vorschau des Versandinhalts wird im rechten Bereich des Bildschirms **[!UICONTROL Simulieren]** angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde.

   ![](assets/simulate-preview.png)

1. Wenn mehrere Profile hinzugefügt wurden, können Sie in der Liste zwischen diesen wechseln, um eine Vorschau des entsprechenden Versandinhalts anzuzeigen. Sie können auch weitere Testprofile hinzufügen und Ihre Auswahl mithilfe der entsprechenden Schaltflächen im linken Bereich löschen.

1. Beim Versand von E-Mails können Sie den **[!UICONTROL Zoom-Faktor]** einstellen und den Inhalt über das entsprechende Symbol oben rechts auf dem Desktop oder einem Mobilgerät in einer Vorschau anzeigen.

1. Auf dem Bildschirm **[!UICONTROL Simulieren]** können Sie auch folgende Aktionen durchführen:
   * Durchführen eines Testversands an bestimmte Empfängerinnen und Empfänger zu Validierungszwecken: [Weitere Informationen](test-deliveries.md)
   * Zugreifen auf die Protokolle der durchgeführten Testsendungen: [Weitere Informationen](test-deliveries.md#access-test-deliveries)
   * (Nur für E-Mails) Überprüfen des Renderings des Nachrichteninhalts in gängigen E-Mail-Clients: [Weitere Informationen](email-rendering.md)



