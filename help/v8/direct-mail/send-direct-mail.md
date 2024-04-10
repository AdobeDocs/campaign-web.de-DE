---
audience: end-user
title: Vorschau und Senden eines Briefpostversands
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Briefpostversand in einer Vorschau anzeigen und senden.
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 100%

---

# Vorschau und Senden eines Briefpostversands {#send-direct-mail}

Nachdem Sie die Extraktionsdatei für den Briefpostversand konfiguriert haben, können Sie anhand von Testprofilen eine Vorschau davon anzuzeigen. Wenn Sie personalisierte Inhalte eingefügt haben, können Sie mithilfe von Testprofildaten prüfen, wie diese Inhalte in den Spalten angezeigt werden. Dadurch können Sie sicherstellen, dass der Dateiinhalt korrekt gerendert wird und dass die personalisierten Elemente entsprechend integriert werden.

Wenn die Extraktionsdatei fertig ist, können Sie den Briefpostversand durchführen, um die Datei zu generieren und an Ihren Briefpost-Dienstleister weiterzugeben. [Erfahren Sie, wie Sie einen Briefpostversand durchführen](#dm-send).

## Anzeigen der Extraktionsdatei in einer Vorschau {#preview-dm}

Die wichtigsten Schritte, um die Extraktionsdatei in einer Vorschau anzuzeigen, werden im Folgenden beschrieben. Weitere Informationen über die Vorschau von Sendungen finden Sie in [diesem Abschnitt](../preview-test/preview-content.md).

1. Auf der Seite für den Versandinhalt können Sie über die Option **[!UICONTROL Inhalt simulieren]** personalisierten Inhalt in einer Vorschau anzeigen.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Klicken Sie auf **[!UICONTROL Testprofil(e) hinzufügen]**, um mindestens ein Profil auszuwählen und die zugehörigen Daten im Inhalt der Extraktionsdatei in einer Vorschau anzuzeigen.

1. Im rechten Bereich sehen Sie eine Vorschau der Extraktionsdatei, in der personalisierte Elemente dynamisch durch Daten aus dem ausgewählten Profil ersetzt werden.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Durchführen von Testsendungen {#test-dm}

Mit **Adobe Campaign** haben Sie die Möglichkeit, Testsendungen zu verschicken, bevor Sie sie an Ihre Hauptzielgruppe senden. Dieser Schritt ist bei der Validierung Ihres Versands und der Identifizierung von Problemen wichtig. Empfängerinnen und Empfänger von Testsendungen können Elemente wie Personalisierungseinstellungen überprüfen, um eine optimale Performance sicherzustellen und Fehler zu erkennen. Dieser Prozess hilft Ihnen, Ihre Extraktionsdatei zu verfeinern und zu optimieren, bevor sie Ihre Hauptzielgruppe erreicht.

Beim Briefpostversand wird durch Testsendungen eine Beispieldatei der Extraktionsdatei anhand von Daten aus den ausgewählten Testprofilen generiert. Gehen Sie wie folgt vor, um darauf zuzugreifen:

1. Klicken Sie im Bildschirm „Inhalt simulieren“ auf die Schaltfläche **[!UICONTROL Testversand durchführen]** und führen Sie dieselben Schritte aus wie bei jedem anderen Versandtyp, um einen Testversand durchzuführen. [Durchführen eines Testversands](../preview-test/test-deliveries.md)

1. Sobald der Testversand durchgeführt wurde, können Sie über die Schaltfläche **[!UICONTROL Testsendungen anzeigen]** oder die Versandliste darauf zugreifen. [Erfahren Sie, wie Sie auf durchgeführte Testsendungen zugreifen](../preview-test/test-deliveries.md#access-test-deliveries).

1. Klicken Sie im Testversand-Dashboard auf die Schaltfläche **[!UICONTROL Datei in Vorschau anzeigen]**, um eine Vorschau der Extraktionsdatei anzuzeigen.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Nur die ersten 100 Zeilen werden in der Vorschaudatei dargestellt.

## Durchführen eines Briefpostversands {#send-dm}

Sobald Ihre Briefpost für den Versand an Ihre Kundinnen und Kunden bereit ist, können Sie den Versand durchführen, um mit der Datenextraktion in der angegebenen Extraktionsdatei zu beginnen. Gehen Sie dazu wie folgt vor:

1. Nachdem Sie den Inhalt Ihrer Extraktionsdatei gestaltet haben, klicken Sie auf der Seite **[!UICONTROL Versand]** auf **[!UICONTROL Überprüfen und senden]**.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Klicken Sie auf **[!UICONTROL Vorbereiten]** und überwachen Sie den Fortschritt und die bereitgestellten Statistiken.

   Wenn Fehler auftreten, finden Sie im Menü **[!UICONTROL Protokolle]** detaillierte Informationen zum Fehler.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Senden Sie die Nachrichten, indem Sie auf **[!UICONTROL Senden]** klicken, um mit dem endgültigen Versandprozess fortzufahren.

1. Bestätigen Sie den Sendevorgang durch Auswahl der Schaltfläche **[!UICONTROL Senden]**.

   Wenn der Briefpostversand zeitlich geplant wurde, klicken Sie auf die Schaltfläche **[!UICONTROL Nach Zeitplan senden]**. Weitere Informationen zur Versandplanung finden Sie in [diesem Abschnitt](../msg/gs-messages.md#schedule-the-delivery-sending).

Nach dem Versand wird die Extraktionsdatei automatisch generiert und an den Speicherort exportiert, der im in den [erweiterten Einstellungen](../advanced-settings/delivery-settings.md) der Versandvorlage ausgewählten externen Konto **[!UICONTROL Routing]** angegeben ist.

Sie können die Daten Ihrer KPIs (Key Performance Indicators) über Ihre Versandseite und weitere Daten über das Menü **[!UICONTROL Protokolle]** nachverfolgen.

Nun können auch damit beginnen, mit integrierten Berichten die Wirkung Ihrer Nachricht zu messen. [Weitere Informationen](../reporting/direct-mail.md)
