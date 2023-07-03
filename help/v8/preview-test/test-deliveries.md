---
audience: end-user
title: Durchführen von Testsendungen
description: Erfahren Sie, wie Sie Testsendungen definieren und durchführen.
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha"
source-git-commit: 1b8657b7f91a1d83e3b65801b6593dfe3dfbac82
workflow-type: ht
source-wordcount: '941'
ht-degree: 100%

---

# Durchführen von Testsendungen {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Vorschaumodus"
>abstract="Erstellen Sie eine Vorschau und testen Sie die Nachricht, indem Sie die Testpopulation zur Hauptzielgruppe hinzufügen."

**[!UICONTROL Adobe Campaign]** ermöglicht es Ihnen, eine Nachricht zu testen, bevor Sie sie an die Hauptzielgruppe senden.

Testsendungen (früher als „Testversand“ bezeichnet) sind ein wichtiger Schritt bei der Validierung Ihrer Kampagne und Identifizierung potenzieller Probleme.

Die Empfängerinnen und Empfänger eines Tests können verschiedene Elemente wie Links, Opt-out-Links, Bilder oder Mirrorseiten überprüfen sowie Fehler bei Rendering, Inhalt, Personalisierungseinstellungen und Versandkonfiguration erkennen.

## Auswählen der Empfängerinnen und Empfänger des Tests {#test-recipients}



>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Testpopulation"
>abstract="Wählen Sie einen Testpopulationsmodus aus."



Je nach verwendetem Kanal können Testnachrichten an drei Empfängertypen gesendet werden:

* [Testprofile](#test-profiles): Senden von **Test-E-Mails und Test-SMS** an Testadressen, bei denen es sich um zusätzliche Empfängerinnen und Empfänger in der Datenbank handelt.

  Diese können in der [!DNL Campaign]-Konsole im Ordner **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Testadressen]** erstellt werden. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=de){target="_blank"}

* [Aus Hauptzielgruppe ersetzen](#substitution-profiles): Senden von **Test-E-Mails und Test-SMS** an eine bestimmte E-Mail-Adresse oder Telefonnummer, wobei die Identität eines vorhandenen Profils angenommen wird.

  Auf diese Weise wird Ihnen die Nachricht wie Ihren Empfängerinnen und Empfängern angezeigt. Sie erhalten so eine genaue Darstellung des Inhalts, den das Profil empfangen wird.

* [Abonnentinnen und Abonnenten](#subscribers): Senden von **Test-Push-Benachrichtigungen** an fiktive Abonnentinnen oder Abonnenten, die zur Datenbank hinzugefügt wurden.

  Sie können wie Testprofile in der [!DNL Campaign]-Konsole im Ordner **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Testadressen]** erstellt werden. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=de){target="_blank"}

Um die Empfängerinnen und Empfänger für einen Testversand auszuwählen, gehen Sie entsprechend dem gewünschten Profiltyp wie folgt vor:

### Testprofile {#test-profiles}


1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ für den E-Mail- oder SMS-Versand und klicken Sie dann auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Test]**.

   >[!NOTE]
   >
   >Wenn Sie bereits Profile für eine [Versandvorschau](preview-content.md) ausgewählt haben, werden diese im linken Bereich aufgelistet.

   ![](assets/simulate-test-button-email.png)

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Modus]** die Option **[!UICONTROL Testprofile]** aus, um fiktive Empfängerinnen und Empfänger für den E-Mail- oder SMS-Testversand auszuwählen.

   ![](assets/simulate-profile-mode.png)

1. Wenn Sie bereits Profile ausgewählt haben, um eine [Vorschau der Nachricht](preview-content.md) im Bildschirm zur Inhaltsimulation anzuzeigen, werden diese Profile als Testempfängerinnen und Testempfänger vorausgewählt. Sie können Ihre Auswahl löschen und/oder zusätzliche Empfängerinnen und Empfänger über die Schaltfläche **[!UICONTROL Testprofil(e) hinzufügen]** hinzufügen.

   >[!NOTE]
   >
   >Standardmäßig ist der Modus **[!UICONTROL Testprofile verwenden]** ausgewählt.

1. Um die endgültige Nachricht auch an die Empfängerinnen und Empfänger des Testversands zu senden, wählen Sie die Option **[!UICONTROL Testpopulation in Hauptzielgruppe einbeziehen]** aus.

1. Sobald die Testprofile ausgewählt sind, können Sie den [Testversand durchführen](#send-test).

### Ersatzprofile {#substitution-profiles}

Verwenden Sie Ersatzprofile, um eine Test-E-Mail oder Test-SMS an eine bestimmte E-Mail-Adresse oder Telefonnummer zu senden und dabei Daten aus einem vorhandenen Profil der [!DNL Campaign]-Datenbank anzuzeigen.

1. Stellen Sie vor einem Testversand sicher, dass Sie eine Zielgruppe für den Versand definieren. [Weitere Informationen](../audience/about-audiences.md)

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ für den E-Mail- oder SMS-Versand und klicken Sie dann auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Test]**.

   ![](assets/simulate-test-button-email.png)

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Modus]** die Option **[!UICONTROL Aus Hauptzielgruppe ersetzen]** aus, um einen Test an eine bestimmte E-Mail-Adresse oder Telefonnummer zu senden und dabei Daten aus einem vorhandenen Profil anzuzeigen.

   >[!CAUTION]
   >
   >Wenn Sie keine [Zielgruppe](../audience/about-audiences.md) für den Versand ausgewählt haben, ist die Option **[!UICONTROL Aus Hauptzielgruppe ersetzen]** ausgegraut und Sie können keine Ersatzprofile auswählen.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Adresse hinzufügen]** und geben Sie die empfangende E-Mail-Adresse oder Telefonnummer für den Testversand an.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >Sie können eine beliebige E-Mail-Adresse oder Telefonnummer eingeben. So können Sie Tests an beliebige Empfängerinnen und Empfänger senden, auch wenn es sich bei diesen um keine [!DNL Adobe Campaign]-Benutzerinnen und -Benutzer handelt.

1. Wählen Sie das Profil aus der Zielgruppe aus, die Sie für den Versand als Ersatz definiert haben. Sie können auch [!DNL Adobe Campaign] ein zufälliges Profil aus der Zielgruppe auswählen lassen. Die Profildaten aus dem ausgewählten Profil werden beim Testversand angezeigt.

1. Bestätigen Sie die Empfängerin oder den Empfänger und wiederholen Sie den Vorgang, um beliebig viele E-Mail-Adressen oder Telefonnummern hinzuzufügen.

   ![](assets/simulate-profile-substitute.png)

1. Um die endgültige Nachricht auch an die Empfängerinnen und Empfänger des Testversands zu senden, wählen Sie die Option **[!UICONTROL Testpopulation in Hauptzielgruppe einbeziehen]** aus.

1. Sobald die Ersatzprofile ausgewählt sind, können Sie den [Testversand durchführen](#send-test).

### Abonnentinnen und Abonnenten {#subscribers}

Beim Arbeiten mit Push-Benachrichtigungen ist ein Testversand nur an Abonnentinnen oder Abonnenten möglich. Gehen Sie wie folgt vor, um diese auszuwählen.

1. Navigieren Sie zum Bildschirm „Inhalt bearbeiten“ für den Versand und klicken Sie dann auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Test]**.

   ![](assets/simulate-test-button-push.png)

1. Wenn Sie bereits Abonnentinnen oder Abonnenten ausgewählt haben, um eine [orschau des Versands](preview-content.md) im Bildschirm zur Inhaltsimulation anzuzeigen, werden diese Profile als Testabonnentinnen oder Testabonnenten vorausgewählt.

   Über die dedizierte Schaltfläche können Sie Ihre Auswahl löschen und/oder zusätzliche Abonnentinnen oder Abonnenten hinzufügen.

   ![](assets/simulate-test-subscribers.png)

1. Um die endgültige Push-Benachrichtigung auch an die Testabonnentinnen oder Testabonnenten zu senden, wählen Sie die Option **[!UICONTROL Testpopulation in Hauptzielgruppe einbeziehen]** aus.

1. Sobald die Abonnentinnen oder Abonnenten ausgewählt sind, können Sie den [Testversand durchführen](#send-test).

## Durchführen des Testversands {#send-test}

Gehen Sie wie folgt vor, um den Testversand an die ausgewählten Empfängerinnen und Empfänger durchzuführen.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Test senden]**.

1. Bestätigen Sie das Senden.

   ![](assets/simulate-send-test.png)

1. Senden Sie so viele Tests wie nötig, bis Sie die endgültigen Inhalte für Ihren Versand festgelegt haben.

Anschließend können Sie den Versand an die Hauptzielgruppe vorbereiten und durchführen. In den folgenden Abschnitten erfahren Sie mehr dazu:

* [Senden der E-Mail](../monitor/prepare-send.md)
* [Senden der Push-Benachrichtigung](../push/send-push.md#send-push)
* [Senden Ihres SMS-Versands](../sms/send-sms.md#send-sms)

## Zugreifen auf durchgeführte Testsendungen {#access-proofs}

Nach den Testsendungen können Sie über die Schaltfläche **[!UICONTROL Testprotokoll anzeigen]** auf spezifische Protokolle zugreifen.

Diese Protokolle ermöglichen den Zugriff auf alle gesendeten Tests für den ausgewählten Versand sowie die Visualisierung bestimmter Versandstatistiken. [Erfahren Sie, wie Sie Versandlogs überwachen](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Wie bei jedem Versand können Sie auch über die [Versandliste](../msg/gs-messages.md) auf gesendete Tests zugreifen.

![](assets/simulate-deliveries-list.png)
