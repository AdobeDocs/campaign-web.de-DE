---
audience: end-user
title: Durchführen von Testsendungen
description: Erfahren Sie, wie Sie Testsendungen definieren und senden
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 60%

---

# Durchführen von Testsendungen {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Vorschaumodus"
>abstract="Erstellen Sie eine Vorschau und testen Sie die Nachricht, indem Sie die Testpopulation zur Hauptzielgruppe hinzufügen."

Nachdem der Nachrichteninhalt definiert wurde, können Sie ihn in der Vorschau anzeigen und testen, indem Sie Testsendungen an Testprofile senden. Wenn Sie personalisierte Inhalte eingefügt haben, können Sie mithilfe von Testprofildaten überprüfen, wie diese Inhalte in der Nachricht angezeigt werden.

Um mögliche Fehler im Nachrichteninhalt oder in den Personalisierungseinstellungen zu erkennen, senden Sie Testsendungen an Testprofile, bevor Sie sie an die Zielgruppe senden. Bei jeder Änderung sollte ein Testversand durchgeführt werden, um den aktuellen Inhalt zu validieren. Die Übermittlung von Testsendungen ist ein wichtiger Schritt zur Validierung Ihrer Kampagne und zur Identifizierung potenzieller Probleme. Die Empfängerinnen und Empfänger eines Testversands können verschiedene Elemente wie Links, Opt-out-Links, Bilder oder Mirrorseiten überprüfen sowie Fehler bei Rendering, Inhalt, Personalisierungseinstellungen und Versandkonfiguration erkennen.

## Inhalt mit Testprofilen simulieren {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Testpopulation"
>abstract="Wählen Sie einen Testpopulationsmodus aus."

Stellen Sie vor dem Testversand sicher, dass Sie eine Zielgruppe für Ihren Versand definieren. [Weitere Informationen](../audience/add-audience.md)

So testen Sie Ihre Nachrichteninhalte:

1. Bearbeiten Sie den Inhalt Ihres Versands.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.
1. Klicken Sie auf **[!UICONTROL Testversand durchführen]** zum Senden von Testsendungen.

   ![](assets/simulate-test-button-email.png){zoomable=&quot;yes&quot;}

1. Wählen Sie die Testversand-Empfänger aus.

   Je nach Nachrichtenkanal kann ein Testversand an die folgenden Empfängertypen gesendet werden:

   * Für SMS und E-Mails können Sie [Testprofile](#test-profiles) verwenden, die bestimmte zusätzliche Empfängerinnen und Empfänger in der Datenbank sind. Sie können auch die [Substitution durch Hauptzielgruppe](#substitution-profiles) -Modus, der den Testversand an eine E-Mail-Testadresse oder Telefonnummer sendet und Personalisierungsdaten eines vorhandenen Profils verwendet. Auf diese Weise wird Ihnen die Nachricht so wie Ihren Empfängerinnen und Empfängern angezeigt. Sie erhalten so eine genaue Darstellung des Inhalts, den das Profil empfangen wird.

   * Für Push-Nachrichten können Sie [Abonnenten](#subscribers) verwenden: fiktive Abonnentinnen und Abonnenten, die zur Datenbank hinzugefügt werden. Sie werden in der [!DNL Campaign]-Konsole angezeigt. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=de){target="_blank"}

   Eine detaillierte Konfiguration für jeden Modus finden Sie unten.

## Verwenden von Testprofilen {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Testversand-Zielgruppe"
>abstract="Sie können eine zweite Datei als „Testversand-Zielgruppe“ hochladen, wenn Sie Ihren Versand testen möchten, bevor Sie ihn an die Hauptzielgruppe senden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Profile hochladen"
>abstract="Sie können eine zweite Datei mit zusätzlichen Profilen hochladen, wenn Sie Ihren Versand mit einem anderen Satz als dem für die Hauptzielgruppe verwendeten testen möchten."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Vorlagendatei"
>abstract="Hinweis: Die Formatierung der Datei muss mit der Originaldatei übereinstimmen.<br/>Unterstützte Dateiformate: txt, csv. Maximale Dateigröße: 15 MB. Verwenden Sie die erste Zeile für Spaltentitel."

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Testprofile in Hauptzielgruppe einbeziehen"
>abstract="Aktivieren Sie diese Option, um die endgültige Nachricht auch an die Testversand-Empfänger zu senden."

Testprofile sind zusätzliche Empfängerinnen und Empfänger in der Datenbank. Sie können über das Menü **[!UICONTROL Kunden-Management]** > **[!UICONTROL Profile]** erstellt werden. [Weitere Informationen](../audience/test-profiles.md#create-test-profiles)

Die Schritte zum Senden von Testsendungen an Testprofile werden nachfolgend beschrieben.

1. Klicken Sie im Versandinhalt auf die Schaltfläche **[!UICONTROL Inhalt simulieren]** und der **[!UICONTROL Testversand durchführen]** Schaltfläche.

1. Aus dem **[!UICONTROL Modus]** Dropdown-Liste auswählen **[!UICONTROL Testprofile]** , um fiktive Empfänger auszuwählen, die den Testversand oder SMS-Versand erhalten.

   ![](assets/simulate-profile-mode.png){zoomable=&quot;yes&quot;}

1. Wenn Sie bereits Profile in [Vorschau der Nachricht erzeugen](preview-content.md) im Bildschirm der Inhaltsimulation werden diese Profile als Testversand-Empfänger vorausgewählt. Sie können Ihre Auswahl löschen und/oder zusätzliche Empfängerinnen und Empfänger über die Schaltfläche **[!UICONTROL Testprofil(e) hinzufügen]** hinzufügen.

1. Beim Durchsuchen der Testprofile oder Profillisten können Sie Filter verwenden, um Ihre Suche zu verfeinern. Sie können beispielsweise eine Regel definieren, um nach allen Testprofilen mit dem Status **[!UICONTROL Interessent]** zu suchen. Erfahren Sie, wie Sie Regeln mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) hinzufügen.

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Um den Testversand-Empfängern auch die endgültige Nachricht zu senden, wählen Sie die **[!UICONTROL Testpopulation in die Hauptzielgruppe einbeziehen]** -Option.

   ![](assets/simulate-include-test.png){zoomable=&quot;yes&quot;}

1. Nach Auswahl der Testprofile können Sie [Testversand durchführen](#send-test).

## Ersetzen von Profildaten {#substitution-profiles}

Verwenden Sie die Profilersetzung, um Testsendungen an eine bestimmte E-Mail-Adresse bzw. Telefonnummer zu senden und dabei Daten aus einem vorhandenen Profil der [!DNL Adobe Campaign]-Datenbank anzuzeigen. Dieser Modus kann nur ausgewählt werden, wenn die Zielgruppe des Versands definiert wurde.

Gehen Sie wie folgt vor, um Profildaten aus der Hauptzielgruppe zu ersetzen:

1. Klicken Sie im Versandinhalt auf die Schaltfläche **[!UICONTROL Inhalt simulieren]** und der **[!UICONTROL Testversand durchführen]** Schaltfläche.

1. Aus dem **[!UICONTROL Modus]** Dropdown-Liste auswählen **[!UICONTROL Ersatz aus Hauptzielgruppe]** , um einen Testversand an eine bestimmte E-Mail-Adresse oder Telefonnummer zu senden und dabei Daten aus einem bestehenden Profil anzuzeigen.

   >[!CAUTION]
   >
   >Wenn Sie keine [Zielgruppe](../audience/about-recipients.md) für den Versand ausgewählt haben, ist die Option **[!UICONTROL Aus Hauptzielgruppe ersetzen]** ausgegraut und Sie können keine Ersatzprofile auswählen.

1. Klicken Sie auf **[!UICONTROL Adresse hinzufügen]** und geben Sie die E-Mail-Adresse oder Telefonnummer an, an die der Testversand gesendet wird.

   ![](assets/simulate-add-substitution-address.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Sie können eine beliebige E-Mail-Adresse oder Telefonnummer eingeben. Auf diese Weise können Sie Testsendungen an alle Empfänger senden, selbst wenn diese keine Benutzer von sind [!DNL Adobe Campaign].

1. Wählen Sie das Profil aus der Zielgruppe aus, die Sie für den Versand als Ersatz definiert haben. Sie können auch [!DNL Adobe Campaign] ein zufälliges Profil aus der Zielgruppe auswählen lassen. Die Profildaten des ausgewählten Profils werden im Testversand angezeigt.

1. Bestätigen Sie die Empfängerin oder den Empfänger und wiederholen Sie den Vorgang, um beliebig viele E-Mail-Adressen oder Telefonnummern hinzuzufügen.

   ![](assets/simulate-profile-substitute.png){zoomable=&quot;yes&quot;}

1. Um den Testversand-Empfängern auch die endgültige Nachricht zu senden, wählen Sie die **[!UICONTROL Testpopulation in die Hauptzielgruppe einbeziehen]** -Option.

1. Nach Auswahl der Ersatzprofile können Sie [Testversand durchführen](#send-test).

## Testsendungen an App-Abonnenten senden {#subscribers}

Bei der Erstellung mit Push-Benachrichtigungen können Testsendungen nur an Ihre App-Abonnenten gesendet werden. Gehen Sie wie folgt vor, um diese auszuwählen.

1. Klicken Sie im Inhalt Ihres Push-Versands auf die Schaltfläche **[!UICONTROL Inhalt simulieren]** und der **[!UICONTROL Testversand durchführen]** Schaltfläche.

   ![](assets/simulate-test-button-push.png){zoomable=&quot;yes&quot;}

1. Wenn Sie bereits Abonnentinnen oder Abonnenten ausgewählt haben, um eine [orschau des Versands](preview-content.md) im Bildschirm zur Inhaltsimulation anzuzeigen, werden diese Profile als Testabonnentinnen oder Testabonnenten vorausgewählt.

   Über die dedizierte Schaltfläche können Sie Ihre Auswahl löschen und/oder zusätzliche Abonnentinnen oder Abonnenten hinzufügen.

   ![](assets/simulate-test-subscribers.png){zoomable=&quot;yes&quot;}

1. Um die endgültige Push-Benachrichtigung auch an die Testabonnentinnen oder Testabonnenten zu senden, wählen Sie die Option **[!UICONTROL Testpopulation in Hauptzielgruppe einbeziehen]** aus.

1. Nach Auswahl der Abonnenten können Sie [Testversand durchführen](#send-test).

## Durchführen des Testversands {#send-test}

Gehen Sie wie folgt vor, um den Testversand an die ausgewählten Empfänger zu senden.

1. Klicken Sie auf **[!UICONTROL Testversand durchführen]** Schaltfläche.

1. Bestätigen Sie das Senden.

   ![](assets/simulate-send-test.png){zoomable=&quot;yes&quot;}

1. Senden Sie so viele Testsendungen wie nötig, bis Sie den Inhalt Ihres Versands fertig gestellt haben.

Anschließend können Sie den Versand an die Hauptzielgruppe vorbereiten und durchführen. In den folgenden Abschnitten erfahren Sie mehr dazu:

* [Senden der E-Mail](../monitor/prepare-send.md)
* [Senden der Push-Benachrichtigung](../push/send-push.md#send-push)
* [Senden Ihres SMS-Versands](../sms/send-sms.md#send-sms)

## Zugreifen auf Testsendungen {#access-test-deliveries}

Sobald die Testsendungen gesendet wurden, können Sie über **[!UICONTROL Inhalt simulieren]** angezeigt.

Diese Protokolle ermöglichen den Zugriff auf alle Testsendungen, die für den ausgewählten Versand durchgeführt werden, und die Visualisierung spezifischer Versandstatistiken. [Erfahren Sie, wie Sie Versandlogs überwachen](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable=&quot;yes&quot;}

Sie können auch auf gesendete Testsendungen über die [Versandliste](../msg/gs-messages.md), wie bei jedem Versand.

![](assets/simulate-deliveries-list.png){zoomable=&quot;yes&quot;}
