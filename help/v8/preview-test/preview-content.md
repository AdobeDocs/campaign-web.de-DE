---
audience: end-user
title: Vorschau des Versandinhalts
description: Erfahren Sie, wie Sie mit der Campaign-Web-Benutzeroberfläche eine Vorschau Ihres Versandinhalts anzeigen können.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha"
source-git-commit: 4a439abca9c7b1f2cc5d82214efb0aae033a996c
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 40%

---


# Vorschau des Versandinhalts {#preview-content}

Verwenden Sie die [!DNL Campaign] Inhaltssimulation , um den Inhalt Ihrer Nachricht vor dem Versand in einer Vorschau anzuzeigen. Auf diese Weise können Sie die Personalisierung steuern und überprüfen, wie sie Ihren Empfängerinnen und Empfängern angezeigt wird.

Gehen Sie wie folgt vor, um eine Vorschau des Versandinhalts anzuzeigen.

1. Navigieren Sie zum Bildschirm Inhalt bearbeiten Ihres Versands.

   <!--email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).-->

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

   ![](assets/simulate-button.png)

1. Um die Profile auszuwählen, die für die Vorschau Ihres personalisierten Inhalts verwendet werden, verwenden Sie:

   * **[!UICONTROL Hinzufügen von Testprofilen]** für die Vorschau von E-Mail- und SMS-Sendungen

   * **[!UICONTROL Abonnenten hinzufügen]** für die Vorschau von Push-Benachrichtigungen

1. Sie können Testprofile und Profile kombinieren, um eine Vorschau Ihrer E-Mail- oder SMS-Nachricht anzuzeigen.

   * Die Registerkarte **[!UICONTROL Testprofile]** enthält Testadressen für zusätzliche, fiktive Personen in der Datenbank.

     >[!NOTE]
     >
     >Testprofile können in der [!DNL Campaign]-Konsole im Ordner **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Testadressen]** erstellt werden. Weitere Informationen finden Sie in der Dokumentation zu [Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=de){target="_blank"}.

   * Die Registerkarte **[!UICONTROL Profile]** listet alle Empfängerinnen und Empfänger auf, die über die [!DNL Campaign]-Konsole im Ordner **[!UICONTROL Profile und Zielgruppen]** gespeichert wurden. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html?lang=de){target="_blank"}.

   ![](assets/simulate-select-profiles.png)

1. Klicken **[!UICONTROL Auswählen]** um Ihre Auswahl zu bestätigen.

   Eine Vorschau des Versandinhalts wird im rechten Bereich des **[!UICONTROL Simulieren]** angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde.

   ![](assets/simulate-preview.png)

1. Wenn Sie mehrere Profile hinzugefügt haben, können Sie in der Liste zwischen ihnen wechseln, um die Vorschau des entsprechenden Versandinhalts anzuzeigen. Sie können auch weitere Testprofile hinzufügen und Ihre Auswahl mithilfe der entsprechenden Schaltflächen im linken Bereich löschen.

1. Bei E-Mail-Sendungen können Sie die **[!UICONTROL Zoomfaktor]** und zeigen Sie Ihre Inhalte auf dem Desktop oder Mobilgerät mithilfe des entsprechenden Symbols oben rechts an.

1. Auf dem Bildschirm **[!UICONTROL Simulieren]** können Sie auch folgende Aktionen durchführen:
   * Testsendungen zur Validierung an bestimmte Empfänger senden - [Weitere Infos](test-deliveries.md)
   * Zugriff auf die Protokolle der gesendeten Testsendungen - [Weitere Infos](test-deliveries.md#access-proofs)
   * Nur für E-Mail: Überprüfen Sie das Rendering des Nachrichteninhalts in gängigen E-Mail-Clients - [Weitere Infos](email-rendering.md)



