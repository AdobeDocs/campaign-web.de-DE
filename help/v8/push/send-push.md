---
audience: end-user
title: Senden eines Push-Benachrichtigungs-Versands
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Push-Benachrichtigungs-Versand senden.
badge: label="Alpha"
source-git-commit: 1b8657b7f91a1d83e3b65801b6593dfe3dfbac82
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 55%

---

# Vorschau und Senden eines Push-Benachrichtigungs-Versands {#send-push-delivery}

## Vorschau Ihres Push-Benachrichtigungs-Versands {#preview-push}

Nachdem Sie den Nachrichteninhalt definiert haben, können Sie Testabonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen. Wenn Sie personalisierten Inhalt eingefügt haben, können Sie mithilfe von Testprofildaten untersuchen, wie dieser Inhalt in der Nachricht angezeigt wird. Dadurch können Sie sicherstellen, dass die Nachricht korrekt wiedergegeben und die personalisierten Elemente entsprechend integriert werden.

Die wichtigsten Schritte zur Vorschau Ihres SMS-Versands sind: Weitere Informationen zur Versandvorschau finden Sie unter [diesem Abschnitt](../preview-test/preview-content.md).

1. Verwenden Sie auf Ihrer Seite mit den Versandinhalten die **[!UICONTROL Inhalt simulieren]** um eine Vorschau Ihres personalisierten Inhalts anzuzeigen.

   ![](assets/push_send_1.png)

1. Klicken **[!UICONTROL Abonnenten hinzufügen]** , um ein oder mehrere Profile auszuwählen, um deren Daten im Inhalt der Push-Benachrichtigung in der Vorschau anzuzeigen.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. Im rechten Bereich finden Sie eine Vorschau der Push-Benachrichtigung, in der personalisierte Elemente dynamisch durch Daten aus dem ausgewählten Profil ersetzt werden.

   ![](assets/push_send_7.png)

Sie können nun Ihre Push-Benachrichtigung überprüfen und an Ihre Zielgruppe senden.

## Testen des Push-Benachrichtigungs-Versands {#test-push}

Durch die Verwendung von **Adobe Campaign** können Sie Push-Benachrichtigungen testen, bevor Sie sie an Ihre Hauptzielgruppe senden. Dieser Schritt ist bei der Validierung Ihres Versands und der Identifizierung von Problemen wichtig.
Empfängerinnen und Empfänger von Testsendungen können Elemente wie Links, Bilder und Personalisierungseinstellungen überprüfen, um eine optimale Leistung zu gewährleisten und Fehler zu erkennen. Dieser Prozess hilft Ihnen, Ihre Push-Benachrichtigungen zu verfeinern und zu optimieren, bevor sie Ihre Hauptzielgruppe erreichen.

![](../assets/do-not-localize/book.png) Erfahren Sie, wie Sie Test-Push-Benachrichtigungen senden in [diesem Abschnitt](../preview-test/test-deliveries.md#subscribers).

![](assets/push_send_6.png)

## Senden Ihres Push-Benachrichtigungs-Versands {#send-push}

1. Nachdem Sie den Inhalt Ihrer Push-Benachrichtigung personalisiert haben, klicken Sie auf der Seite **[!UICONTROL Versand]** auf **[!UICONTROL Überprüfen und Senden]**.

   ![](assets/push_send_2.png)

1. Klicken **[!UICONTROL Vorbereiten]** und überwachen den Fortschritt und die Statistiken.

   Wenn Fehler auftreten, finden Sie im Menü „Protokolle“ detaillierte Informationen zum Fehler.

   ![](assets/push_send_3.png)

1. Senden Sie die Nachrichten, indem Sie auf **[!UICONTROL Senden]** klicken, um mit dem endgültigen Versandprozess fortzufahren.

1. Bestätigen Sie den Sendevorgang durch Klicken auf die Schaltfläche **[!UICONTROL Senden]** oder **[!UICONTROL Nach Zeitplan senden]**.

   ![](assets/push_send_4.png)

Nach dem Versand können Sie Ihre KPI-Daten (Key Performance Indicator) von Ihrer Versandseite und Daten aus der **[!UICONTROL Protokolle]** Menü.

Nun können Sie beginnen, mit integrierten Berichten die Wirkung Ihrer Nachricht zu messen. [Weitere Informationen](../reporting/push-report.md)
