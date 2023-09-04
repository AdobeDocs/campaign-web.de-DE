---
audience: end-user
title: Anzeigen des Versandinhalts in einer Vorschau
description: Erfahren Sie, wie Sie mit der Web-Benutzeroberfläche von Campaign den Versandinhalt in einer Vorschau anzeigen können.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Beta"
source-git-commit: 95d44fa2c44a346aad3aab1962e84917532cc966
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 95%

---


# Anzeigen des Versandinhalts in einer Vorschau {#preview-content}

Verwenden Sie die Inhaltssimulationsfunktion von [!DNL Campaign], um den Nachrichteninhalt vor dem Senden in einer Vorschau anzuzeigen. Auf diese Weise können Sie die Personalisierung steuern und überprüfen, wie sie Ihren Empfängerinnen und Empfängern angezeigt wird.

Gehen Sie wie folgt vor, um den Versandinhalt in einer Vorschau anzuzeigen.

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ Ihres Versands.

   <!--email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).-->

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

   ![](assets/simulate-button.png)

1. Um die Profile auszuwählen, die für die Vorschau Ihres personalisierten Inhalts verwendet werden, verwenden Sie folgende Funktionen:

   * **[!UICONTROL Testprofil(e) hinzufügen]** für die Vorschau von E-Mail- und SMS-Sendungen

   * **[!UICONTROL Abonnentin(nen) oder Abonnent(en) hinzufügen]** für die Vorschau von Push-Benachrichtigungen

1. Sie können Testprofile und Profile miteinander kombinieren, um Ihre E-Mail- oder SMS-Nachricht in einer Vorschau anzuzeigen.

   * Die Registerkarte **[!UICONTROL Testprofile]** enthält Testadressen für zusätzliche, fiktive Personen in der Datenbank.

     >[!NOTE]
     >
     >Testprofile können in der [!DNL Campaign]-Konsole im Ordner **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Testadressen]** erstellt werden. Weitere Informationen finden Sie unter [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=de){target="_blank"}.

   * Die Registerkarte **[!UICONTROL Profile]** listet alle Empfängerinnen und Empfänger auf, die über die [!DNL Campaign]-Konsole im Ordner **[!UICONTROL Profile und Zielgruppen]** gespeichert wurden. Weitere Informationen finden Sie unter [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html?lang=de){target="_blank"}.

   ![](assets/simulate-select-profiles.png)

1. Klicken Sie auf **[!UICONTROL Auswählen]**, um Ihre Auswahl zu bestätigen.

   Eine Vorschau des Versandinhalts wird im rechten Bereich des Bildschirms **[!UICONTROL Simulieren]** angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde.

   ![](assets/simulate-preview.png)

1. Wenn mehrere Profile hinzugefügt wurden, können Sie in der Liste zwischen diesen wechseln, um eine Vorschau des entsprechenden Versandinhalts anzuzeigen. Sie können auch weitere Testprofile hinzufügen und Ihre Auswahl mithilfe der entsprechenden Schaltflächen im linken Bereich löschen.

1. Beim Versand von E-Mails können Sie den **[!UICONTROL Zoom-Faktor]** einstellen und den Inhalt über das entsprechende Symbol oben rechts auf dem Desktop oder einem Mobilgerät in einer Vorschau anzeigen.

1. Auf dem Bildschirm **[!UICONTROL Simulieren]** können Sie auch folgende Aktionen durchführen:
   * Durchführen eines Testversands an bestimmte Empfängerinnen und Empfänger zu Validierungszwecken: [Weitere Informationen](test-deliveries.md)
   * Zugreifen auf die Protokolle der durchgeführten Testsendungen: [Weitere Informationen](test-deliveries.md#access-proofs)
   * (Nur für E-Mails) Überprüfen des Renderings des Nachrichteninhalts in gängigen E-Mail-Clients: [Weitere Informationen](email-rendering.md)



