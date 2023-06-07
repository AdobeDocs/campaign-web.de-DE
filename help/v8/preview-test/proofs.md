---
audience: end-user
title: Senden von Test-E-Mails
description: Erfahren Sie, wie Sie Test-E-Mails definieren und senden
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positive"
source-git-commit: c6ebdf23c22cb197a816684108c782aa2180dc1e
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 41%

---

# Senden von Test-E-Mails {#send-test-emails}

**[!UICONTROL Adobe Campaign]** ermöglicht es Ihnen, eine Nachricht zu testen, bevor Sie sie an die Hauptzielgruppe senden.

Der Versand von Test-E-Mails ist ein wichtiger Schritt zur Validierung Ihrer E-Mail-Kampagne und zur Identifizierung potenzieller Probleme.

Die Empfänger eines Tests können verschiedene Elemente wie Links, Opt-out-Links, Bilder und Mirrorseiten überprüfen sowie Fehler in Rendering, Inhalt, Personalisierungseinstellungen und E-Mail-Konfiguration erkennen.

## Auswählen der Empfängerinnen und Empfänger des Testversands {#test-recipients}

Test-E-Mails können an zwei Empfängertypen gesendet werden:

* **Testprofile** - Testadressen, die zusätzliche fiktive Empfänger in der Datenbank sind. Sie können im [!DNL Campaign] in die **[!UICONTROL Ressourcen]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Testadressen]** Ordner. [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/creating-seed-addresses.html){target="_blank"}

* **Ersatz aus Hauptzielgruppe** - Senden von Test-E-Mails an eine bestimmte E-Mail-Adresse, während die Identität eines vorhandenen Profils übernommen wird. Auf diese Weise wird Ihnen die E-Mail so angezeigt wie Ihren Empfängerinnen und Empfängern und Sie erhalten eine genaue Darstellung der Nachricht, die Ihre Profile empfangen werden.

Gehen Sie wie folgt vor, um die Empfänger des E-Mail-Tests auszuwählen.

1. Auf E-Mail zugreifen [Inhalt bearbeiten](../content/edit-content.md) oder auf [Email Designer](../content/get-started-email-designer.md)und klicken Sie dann auf **[!UICONTROL Inhalt simulieren]** Schaltfläche.

1. Klicken Sie auf **[!UICONTROL Test]** Schaltfläche.

   ![](assets/simulate-test-button.png)

1. Verwenden Sie die Dropdown-Liste **[!UICONTROL Modus]**, um den Empfängertyp auszuwählen, der die Test-E-Mail erhalten soll:

   * **Testprofile** Zielgruppe fiktiver Empfänger

   * **Ersatz aus Hauptzielgruppe** , um einen Test an eine bestimmte E-Mail-Adresse zu senden und dabei Daten aus einem vorhandenen Profil anzuzeigen.

   ![](assets/simulate-profile-mode.png)

   >[!NOTE]
   >
   >Standardmäßig wird die **[!UICONTROL Verwenden von Testprofilen]** ausgewählt ist. Wenn Sie bereits Profile ausgewählt haben, um die E-Mail im Inhaltsimulations-Bildschirm in der Vorschau anzuzeigen, werden diese Profile als Testempfänger vorausgewählt. Sie können Ihre Auswahl löschen und/oder zusätzliche Empfängerinnen und Empfänger hinzufügen.

1. Um Test-E-Mails an Ersatzprofile zu senden, wählen Sie die **[!UICONTROL Aus Zielgruppe ersetzen]** -Modus und führen Sie dann die folgenden Schritte aus:

   1. Klicken Sie auf die Schaltfläche **[!UICONTROL Adresse hinzufügen]** und geben Sie die E-Mail-Adresse an, an die die Test-E-Mail gesendet werden soll.

      Sie können eine beliebige E-Mail-Adresse eingeben. Dadurch können Sie Testadressen an beliebige Benutzer senden, selbst wenn diese keine Benutzer von sind [!DNL Adobe Campaign].

   1. Wählen Sie das Profil aus der Zielgruppe aus, das als Ersatz verwendet werden soll. Sie können auch [!DNL Adobe Campaign] Wählen Sie ein zufälliges Profil aus der Zielgruppe aus. Die Profildaten aus dem ausgewählten Profil werden in der Test-E-Mail angezeigt.

   1. Bestätigen Sie die Empfängerin oder den Empfänger und wiederholen Sie den Vorgang, um beliebig viele Adressen hinzuzufügen.

      ![](assets/simulate-profile-substitute.png)

1. Nach Auswahl der Testempfänger können Sie [Test-E-Mail senden](#send-test).

   >[!NOTE]
   >
   >Um auch die endgültige E-Mail-Nachricht an die Empfänger der Test-E-Mail zu senden, wählen Sie die **[!UICONTROL Testpopulation in die Hauptzielgruppe einbeziehen]** -Option.

## Senden der Test-E-Mail {#send-test}

Gehen Sie wie folgt vor, um die Test-E-Mail an die ausgewählten Empfänger zu senden.

1. Klicken **[!UICONTROL Test-E-Mail senden]**.

1. Bestätigen Sie den Versand.

   ![](assets/simulate-send-test.png)

1. Senden Sie so viele Test-E-Mails wie nötig, bis Sie den Inhalt Ihres Versands endgültig festgelegt haben.

Danach können Sie [E-Mail vorbereiten und senden](../monitor/prepare-send.md) zur Hauptzielgruppe hinzugefügt.

## Zugriff auf gesendete Test-E-Mails {#access-proofs}

Nachdem die Test-E-Mails gesendet wurden, können Sie über die Schaltfläche **[!UICONTROL Test-E-Mail-Protokoll anzeigen]** auf spezifische Protokolle zugreifen.

Diese Protokolle ermöglichen den Zugriff auf alle Test-E-Mails für den ausgewählten Versand sowie die Visualisierung bestimmter Versandstatistiken. [Erfahren Sie, wie Sie Versandlogs überwachen](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Sie können auch auf gesendete Test-E-Mails über die [Versandliste](../msg/gs-messages.md), wie bei jedem Versand.

![](assets/simulate-deliveries-list.png)
