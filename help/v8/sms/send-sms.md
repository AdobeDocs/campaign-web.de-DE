---
audience: end-user
title: Senden eines SMS-Versands
description: Erfahren Sie, wie Sie SMS mit Adobe Campaign Web senden
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 100%

---

# Vorschau und Senden eines SMS-Versands {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Metrik „Neu in Quarantäne“"
>abstract="Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannte Benutzende, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten."

## Vorschau Ihres SMS-Versands {#preview-sms}

Nachdem Sie den Nachrichteninhalt definiert haben, zeigen Sie mithilfe von Testprofilen eine Vorschau an und führen Sie einen Testversand durch. Wenn personalisierte Inhalte enthalten sind, überprüfen Sie mithilfe von Testprofildaten, wie diese Inhalte in der Nachricht angezeigt werden. Dadurch wird sichergestellt, dass die Nachricht wie beabsichtigt angezeigt wird und personalisierte Informationen korrekt dargestellt werden.

Die wichtigsten Schritte zum Anzeigen eines SMS-Versands in einer Vorschau sind: Weitere Informationen über die Vorschau von Sendungen finden Sie in [diesem Abschnitt](../preview-test/preview-content.md).

1. Auf der Seite für den Versandinhalt können Sie über die Option **[!UICONTROL Inhalt simulieren]** personalisierten Inhalt in einer Vorschau anzeigen.

   ![Vorschau personalisierter SMS-Inhalte](assets/sms_send_1.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Testprofil(e) hinzufügen]**, um ein oder mehrere Testprofile auszuwählen.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. Im rechten Bereich sehen Sie eine Vorschau des SMS-Versands, in der personalisierte Elemente dynamisch durch Daten aus dem ausgewählten Profil ersetzt werden.

   ![Vorschaubereich mit personalisiertem SMS-Versand](assets/sms_send_3.png){zoomable="yes"}

Überprüfen Sie Ihre SMS-Nachricht und senden Sie sie Ihrer Zielgruppe.

## Testen Ihres SMS-Versands {#test-sms}

Testen Sie mit **Adobe Campaign** eine Nachricht, bevor Sie sie an die Hauptzielgruppe senden. Dadurch wird Ihre E-Mail-Kampagne validiert und potenzielle Probleme werden erkannt.

Testsendungen sind ein entscheidender Schritt, um die Qualität und Effektivität Ihres Versands sicherzustellen. Empfängerinnen und Empfänger von Testsendungen überprüfen verschiedene Elemente wie Links, Abmelde-Links und Bilder und identifizieren Fehler bei Rendering, Inhalt, Personalisierungseinstellungen und SMS-Konfiguration. Dieser Prozess ermöglicht es, Ihre SMS gründlich zu überprüfen und zu optimieren, bevor sie Ihre Hauptzielgruppe erreichen.

![Buchsymbol für Testsendungen](../assets/do-not-localize/book.png) In [diesem Abschnitt](../preview-test/test-deliveries.md) erfahren Sie, wie Sie Testsendungen durchführen.

![Testen des SMS-Versands](assets/sms_send_6.png){zoomable="yes"}

## Senden Ihres SMS-Versands {#send-sms}

1. Nachdem Sie den Inhalt Ihrer SMS personalisiert haben, klicken Sie auf der Seite **[!UICONTROL Versand]** auf **[!UICONTROL Überprüfen und versenden]**.

   ![Überprüfen und Durchführen eines SMS-Versands](assets/sms_send_4.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Vorbereiten]** und überwachen Sie den Fortschritt und die bereitgestellten Statistiken.

   Wenn Fehler auftreten, finden Sie im Menü „Logs“ detaillierte Informationen dazu.

1. Senden Sie die Nachrichten, indem Sie auf **[!UICONTROL Senden]** klicken, um mit dem endgültigen Versandprozess fortzufahren.

   ![Durchführen eines SMS-Versands](assets/sms_send_5.png){zoomable="yes"}

   Wenn der SMS-Versand geplant wurde, klicken Sie auf die Schaltfläche **[!UICONTROL Nach Zeitplan senden]**. Weitere Informationen zur Versandplanung finden Sie in [diesem Abschnitt](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Bestätigen Sie den Sendevorgang durch Auswahl der Schaltfläche **[!UICONTROL Senden]**.

Verfolgen Sie nach dem Versand Ihre KPI(Key Performance Indicator)-Daten über Ihre Versandseite und weitere Daten über das Menü **[!UICONTROL Logs]**.

Messen Sie die Wirkung Ihrer Nachricht mit integrierten Berichten. [Weitere Informationen](../reporting/sms-report.md)