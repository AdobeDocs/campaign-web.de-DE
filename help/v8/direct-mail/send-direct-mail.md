---
audience: end-user
title: Briefpost-Versand in der Vorschau ansehen und senden
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Briefpost-Versand in der Vorschau anzeigen und senden können.
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 18%

---

# Briefpost-Versand in der Vorschau ansehen und senden {#send-direct-mail}

Nachdem Sie die Extraktionsdatei für Ihren Briefpost-Versand konfiguriert haben, können Sie Testprofile verwenden, um eine Vorschau davon anzuzeigen. Wenn Sie personalisierten Inhalt eingefügt haben, können Sie mithilfe von Testprofildaten untersuchen, wie dieser Inhalt in den Spalten angezeigt wird. Dadurch können Sie sicherstellen, dass der Dateiinhalt korrekt wiedergegeben und die personalisierten Elemente entsprechend integriert werden.

Wenn die Extraktionsdatei fertig ist, können Sie den Briefpost-Versand senden, um die Datei zu generieren und für Ihren Briefpost-Dienstleister freizugeben. [Erfahren Sie, wie Sie Ihren Briefpost-Versand senden.](#dm-send)

## Vorschau der Extraktionsdatei anzeigen {#preview-dm}

Die wichtigsten Schritte zur Vorschau Ihrer Extraktionsdatei sind: Weitere Informationen über die Vorschau von Sendungen finden Sie in [diesem Abschnitt](../preview-test/preview-content.md).

1. Auf der Seite für den Versandinhalt können Sie über die Option **[!UICONTROL Inhalt simulieren]** personalisierten Inhalt in einer Vorschau anzeigen.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Klicks **[!UICONTROL Hinzufügen von Testprofilen]** , um ein oder mehrere Profile auszuwählen, um deren Daten im Inhalt der Extraktionsdatei in der Vorschau anzuzeigen.

1. Im rechten Bereich finden Sie eine Vorschau der Extraktionsdatei, in der personalisierte Elemente dynamisch durch Daten aus dem ausgewählten Profil ersetzt werden.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Durchführen von Testsendungen {#test-dm}

Mit **Adobe Campaign** haben Sie die Möglichkeit, Testsendungen zu verschicken, bevor Sie sie an Ihre Hauptzielgruppe senden. Dieser Schritt ist bei der Validierung Ihres Versands und der Identifizierung von Problemen wichtig. Testempfänger können Elemente wie Personalisierungseinstellungen überprüfen, eine optimale Leistung sicherstellen und Fehler erkennen. Auf diese Weise können Sie Ihre Extraktionsdatei verfeinern und optimieren, bevor Sie Ihre Hauptzielgruppe erreichen.

Beim Briefpost-Versand erzeugt der Testversand eine Beispieldatei der Extraktionsdatei anhand von Daten aus den ausgewählten Testprofilen. Gehen Sie wie folgt vor, um darauf zuzugreifen:

1. Klicken Sie im Bildschirm zur Inhaltsimulation auf die **[!UICONTROL Testversand durchführen]** und führen Sie dieselben Schritte aus wie bei jedem Versand, um einen Testversand durchzuführen. [Durchführen eines Testversands](../preview-test/test-deliveries.md)

1. Sobald der Testversand durchgeführt wurde, können Sie über **[!UICONTROL Testsendungen anzeigen]** oder in der Versandliste. [Erfahren Sie, wie Sie auf gesendete Testsendungen zugreifen können](../preview-test/test-deliveries.md#access-test-deliveries)

1. Klicken Sie im Testversand-Dashboard auf die Schaltfläche **[!UICONTROL Vorschau der Datei]** -Schaltfläche, um eine Vorschau der Extraktionsdatei anzuzeigen.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Nur die ersten 100 Zeilen werden in der Vorschaudatei angezeigt.

## Briefpost-Versand senden {#send-dm}

Sobald Ihre Briefpost für den Versand an Ihre Kunden bereit ist, können Sie den Versand senden, um die Datenextraktion in der angegebenen Extraktionsdatei zu starten. Gehen Sie dazu wie folgt vor:

1. Nachdem Sie den Inhalt Ihrer Extraktionsdatei entworfen haben, klicken Sie auf **[!UICONTROL Überprüfen und Senden]** aus dem **[!UICONTROL Versand]** Seite.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Klicken Sie auf **[!UICONTROL Vorbereiten]** und überwachen Sie den Fortschritt und die bereitgestellten Statistiken.

   Wenn Fehler auftreten, lesen Sie den Abschnitt **[!UICONTROL Protokolle]** für detaillierte Informationen zum Fehler.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Senden Sie die Nachrichten, indem Sie auf **[!UICONTROL Senden]** klicken, um mit dem endgültigen Versandprozess fortzufahren.

1. Bestätigen Sie den Sendevorgang durch Auswahl der Schaltfläche **[!UICONTROL Senden]**.

   Wenn der Briefpost-Versand geplant wurde, klicken Sie auf die Schaltfläche **[!UICONTROL Senden als geplant]** Schaltfläche. Weitere Informationen zur Versandplanung finden Sie in [diesem Abschnitt](../msg/gs-messages.md#schedule-the-delivery-sending).

Nach dem Versand wird die Extraktionsdatei automatisch erzeugt und an den im Feld **[!UICONTROL Routing]** Externes Konto, das im [Erweiterte Einstellungen](../advanced-settings/delivery-settings.md).

Sie können Ihre KPI-Daten (Key Performance Indicators) von Ihrer Bereitstellungsseite und Daten aus der **[!UICONTROL Protokolle]** Menü.

Sie können auch mit integrierten Berichten beginnen, die Wirkung Ihrer Nachricht zu messen. [Weitere Informationen](../reporting/direct-mail.md)
