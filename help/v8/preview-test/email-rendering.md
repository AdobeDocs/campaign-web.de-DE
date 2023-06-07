---
audience: end-user
title: Testen des E-Mail-Rendering
description: Erfahren Sie, wie Sie Ihr E-Mail-Rendering in der Web-Benutzeroberfläche von Campaign testen können.
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Alpha" type="Positive"
source-git-commit: 6bd112c3ceb283435809379403c91ac9c8ed2756
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 9%

---


# Testen des E-Mail-Rendering {#email-rendering}

Bevor Sie Ihre E-Mail versenden, stellen Sie sicher, dass Ihre Nachricht den Empfängern in verschiedenen Web-Clients und Geräten optimal angezeigt wird.

Dazu können Sie Ihre **Litmus** Konto [!DNL Adobe Campaign] um sofort eine Vorschau Ihres E-Mail-Renderings in verschiedenen Kontexten anzuzeigen und die Kompatibilität mit den wichtigsten Desktops und Anwendungen (Webmail, Nachrichtendienst, Mobilgeräte usw.) zu überprüfen.

>[!CAUTION]
>
>Die Verwendung von E-Mail-Rendering in Campaign sendet eine Test-E-Mail an ein Drittanbietersystem. Indem Sie Ihr Litmus-Konto mit [!DNL Campaign], erkennen Sie an, dass Adobe nicht für die Daten verantwortlich ist, die Sie an diesen Dritten senden können. Die Litmus-E-Mail-Richtlinie zur Datenaufbewahrung gilt für diese E-Mails, einschließlich der Personalisierungsdaten, die in diese Testnachrichten aufgenommen werden können. Um auf solche Daten zuzugreifen oder sie zu löschen, müssen Sie sich direkt an Litmus wenden.

Für den Zugriff auf E-Mail-Rendering-Funktionen müssen Sie:

* Sie haben ein Litmus-Konto
* Auswählen von Testprofilen - Erfahren Sie mehr über [diesem Abschnitt](preview-content.md)

Gehen Sie dann wie folgt vor:

1. Im [Inhalt bearbeiten](../content/edit-content.md) oder im [Email Designer](../content/get-started-email-designer.md), klicken Sie auf die **[!UICONTROL Inhalt simulieren]** Schaltfläche.

1. Wählen Sie die **[!UICONTROL E-Mail rendern]** Schaltfläche.

   ![](assets/simulate-rendering-button.png)

1. Klicken **Verbinden Ihres Litmus-Kontos** oben rechts.

   ![](assets/simulate-rendering-litmus.png)

1. Geben Sie Ihre Anmeldedaten ein und melden Sie sich an.

   ![](assets/simulate-rendering-credentials.png)

1. Klicken Sie auf **Ausführen eines Tests** Schaltfläche zum Generieren einer E-Mail-Vorschau.

1. Prüfen Sie Ihren E-Mail-Inhalt in bevorzugten Desktop-, Mobile- und Web-basierten Clients.

   ![](assets/simulate-rendering-previews.png)

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
