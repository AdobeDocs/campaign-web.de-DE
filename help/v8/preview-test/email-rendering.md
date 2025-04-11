---
audience: end-user
title: Testen des E-Mail-Renderings
description: Hinweise zum Testen Ihres E-Mail-Renderings in der Campaign Web-Benutzeroberfläche
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 44%

---

# Testen des E-Mail-Renderings {#email-rendering}

Stellen Sie vor dem Versand Ihrer E-Mail sicher, dass Ihre Nachricht für Empfänger und Empfängerinnen auf verschiedenen Web-Clients und Geräten optimal angezeigt wird.

Verwenden Sie dazu Ihr **Litmus**-Konto in [!DNL Adobe Campaign], um eine Vorschau Ihres E-Mail-Renderings in verschiedenen Kontexten anzuzeigen. Auf diese Weise können Sie die Kompatibilität mit den wichtigsten Desktop-Programmen, Webmail-Diensten, Mobilgeräten und mehr überprüfen.

>[!CAUTION]
>
>Beim E-Mail-Rendering in Campaign wird eine Testsendung an ein Fremdsystem gesendet. Indem Sie Ihr Litmus-Konto mit [!DNL Campaign] verbinden, erkennen Sie an, dass Adobe nicht für Daten verantwortlich ist, die Sie an diesen Drittanbieter senden. Die Richtlinie zur Aufbewahrung von E-Mail-Daten von Litmus gilt für diese E-Mails, einschließlich Personalisierungsdaten, die in diesen Testsendungen enthalten sein können. Um auf solche Daten zuzugreifen oder sie zu löschen, wenden Sie sich bitte direkt an Litmus.

Um auf E-Mail-Rendering-Funktionen zuzugreifen, müssen Sie die folgenden Voraussetzungen erfüllen:

* Ein Litmus-Konto besitzen.
* Auswählen von Profilen und/oder Testprofilen. Weitere Informationen dazu finden Sie in [diesem Abschnitt](preview-content.md).

Gehen Sie dann wie folgt vor:

1. Klicken Sie im Bildschirm [Inhalt bearbeiten](../email/edit-content.md) oder im [E-Mail-Designer](../email/get-started-email-designer.md) auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

1. Wählen Sie die Schaltfläche **[!UICONTROL E-Mail rendern]** aus.

   ![Schaltfläche „Inhalt simulieren“ im E-Mail-Editor](assets/simulate-rendering-button.png){zoomable="yes"}

1. Klicken Sie im oberen rechten Bereich auf **Litmus-Konto verbinden**.

   ![Litmus-Kontoverbindungsoption in der E-Mail-Rendering-Oberfläche](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. Geben Sie Ihre Anmeldedaten ein und melden Sie sich an.

   ![Litmus-Anmeldebildschirm des Kontos](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. Klicken Sie auf die Schaltfläche **Test ausführen**, um eine E-Mail-Vorschau zu erstellen.

1. Überprüfen Sie Ihre E-Mail-Inhalte in beliebten Desktop-, Mobile- und Web-basierten Clients.

   ![E-Mail-Rendering-Vorschauen auf verschiedenen Clients](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile, and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![Preview pane showing email rendering across selected clients](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->