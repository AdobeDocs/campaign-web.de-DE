---
audience: end-user
title: Senden eines SMS-Versands
description: Erfahren Sie, wie Sie SMS mit Adobe Campaign Web senden
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 36%

---

# Vorschau und Senden eines SMS-Versands {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Metrik „Neu in Quarantäne“"
>abstract="Gesamtzahl der Adressen, die infolge eines fehlgeschlagenen Versands unter Quarantäne gestellt wurden (unbekannte Benutzende, ungültige Domain), im Verhältnis zur Anzahl der zu versendenden Nachrichten."

## Vorschau Ihres SMS-Versands {#preview-sms}

Nachdem Sie den Nachrichteninhalt definiert haben, können Sie ihn mithilfe von Testprofilen in der Vorschau anzeigen und testen. Wenn personalisierte Inhalte enthalten sind, überprüfen Sie mithilfe von Testprofildaten, wie diese Inhalte in der Nachricht angezeigt werden. Dadurch wird sichergestellt, dass die Nachricht wie beabsichtigt angezeigt wird und personalisierte Informationen korrekt dargestellt werden.

Die wichtigsten Schritte zum Anzeigen eines SMS-Versands in einer Vorschau sind: Weitere Informationen über die Vorschau von Sendungen finden Sie in [diesem Abschnitt](../preview-test/preview-content.md).

1. Auf der Seite für den Versandinhalt können Sie über die Option **[!UICONTROL Inhalt simulieren]** personalisierten Inhalt in einer Vorschau anzeigen.

   ![Vorschau personalisierter SMS-Inhalte](assets/sms_send_1.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Testprofil(e) hinzufügen]**, um ein oder mehrere Testprofile auszuwählen.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. Im rechten Bereich sehen Sie sich eine Vorschau des SMS-Versands an, in dem personalisierte Elemente dynamisch durch Daten aus dem ausgewählten Profil ersetzt werden.

   ![Vorschaufenster mit personalisiertem SMS-Versand](assets/sms_send_3.png){zoomable="yes"}

Überprüfen Sie Ihre SMS-Nachricht und senden Sie sie an Ihre Audience.

## Testen Ihres SMS-Versands {#test-sms}

Testen Sie mit **Adobe Campaign** eine Nachricht, bevor Sie sie an die Hauptzielgruppe senden. Dieser Schritt validiert Ihre E-Mail-Kampagne und identifiziert potenzielle Probleme.

Testsendungen sind von entscheidender Bedeutung, um die Qualität und Effektivität Ihres Versands sicherzustellen. Testversand-Empfänger überprüfen verschiedene Elemente wie Links, Opt-out-Links und Bilder und identifizieren Fehler bei Rendering, Inhalt, Personalisierungseinstellungen und SMS-Konfiguration. Dieser Prozess bewertet und optimiert Ihre SMS gründlich, bevor sie Ihre Hauptzielgruppe erreicht.

![Buchsymbol für Testsendungen](../assets/do-not-localize/book.png) Erfahren Sie in [diesem Abschnitt](../preview-test/test-deliveries.md), wie Sie einen Testversand durchführen können.

![SMS-Versand testen](assets/sms_send_6.png){zoomable="yes"}

## Senden Ihres SMS-Versands {#send-sms}

1. Nachdem Sie den Inhalt Ihrer SMS personalisiert haben, klicken Sie auf der Seite **[!UICONTROL Versand]** auf **[!UICONTROL Überprüfen und versenden]**.

   ![SMS-Versand überprüfen und senden](assets/sms_send_4.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Vorbereiten]** und überwachen Sie den Fortschritt und die bereitgestellten Statistiken.

   Wenn Fehler auftreten, finden Sie im Menü „Protokolle“ detaillierte Informationen zum Fehler.

1. Senden Sie die Nachrichten, indem Sie **[!UICONTROL Senden]** klicken, um mit dem endgültigen Versandprozess fortzufahren.

   ![SMS-Versand durchführen](assets/sms_send_5.png){zoomable="yes"}

   Wenn der SMS-Versand geplant ist, klicken Sie auf die Schaltfläche **[!UICONTROL Nach Zeitplan senden]**. Weitere Informationen zur Versandplanung finden Sie in [diesem Abschnitt](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Bestätigen Sie den Sendevorgang durch Auswahl der Schaltfläche **[!UICONTROL Senden]**.

Nach dem Versand verfolgen Sie Ihre KPI-Daten (Key Performance Indicator) von Ihrer Versandseite und Daten über das Menü **[!UICONTROL Protokolle]**.

Beginnen Sie mit der Messung der Wirkung Ihrer Nachricht mit integrierten Berichten. [Weitere Informationen](../reporting/sms-report.md)