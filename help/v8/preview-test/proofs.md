---
audience: end-user
title: Test-E-Mails senden
description: Erfahren Sie, wie Sie Test-E-Mails definieren und senden
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 8438c7ab35c2423beddbb36db2fcf52f661876bf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 62%

---

# Test-E-Mails senden {#send-proofs}

![](../assets/do-not-localize/badge.png)

Der Versand von Test-E-Mails ist ein wichtiger Schritt zur Validierung Ihrer E-Mail-Kampagne und zur Identifizierung potenzieller Probleme. Durch den Versand von Test-E-Mails können Sie verschiedene Elemente wie Links, Opt-out-Links, Bilder und Mirrorseiten überprüfen und Fehler erkennen.

Test-E-Mails können an zwei Empfängertypen gesendet werden:

* **Testprofile**: Testadressen, bei denen es sich um zusätzliche fiktive Empfänger in der Datenbank handelt, mit Test-E-Mails versenden,
* **Ersatzprofile**: Testversand-E-Mails an eine bestimmte E-Mail-Adresse senden, während die Identität eines vorhandenen Profils übernommen wird. Auf diese Weise können Sie die E-Mail so erleben, wie sie die Empfänger erhalten. So erhalten Sie eine genaue Darstellung der Nachricht, die das Profil empfangen wird.

## Auswählen der Testversand-Empfänger {#recipients}

1. Öffnen Sie den Bildschirm zur Erstellung des E-Mail-Inhalts und klicken Sie auf **[!UICONTROL Inhalt simulieren]**.

1. Klicken Sie auf **[!UICONTROL Test]** und verwenden Sie dann die Dropdown-Liste **[!UICONTROL Modus]** zur Auswahl des Empfängertyps für die Testsendungen:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Durchführen eines Testversands an Testprofile

1. Wählen Sie den Modus **[!UICONTROL Testprofile verwenden]**.

1. Fügen Sie die Testprofile hinzu, die die Test-E-Mails erhalten sollen.

   <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

   ![](assets/test-profiles-audience.png)

### Durchführen eines Testversands an Ersatzprofile

1. Wählen Sie den Modus **[!UICONTROL Ersatz der Zielgruppe]**.

1. Fügen Sie die E-Mail-Adresse(n) hinzu, an die die Testsendungen gesendet werden sollen.

   >[!NOTE]
   >
   >Sie können eine beliebige E-Mail-Adresse angeben. Auf diese Weise können Sie Testsendungen an beliebige Benutzer senden, auch wenn diese nicht Nutzer von Adobe Campaign V8 sind.

1. Wählen Sie für jede E-Mail-Adresse das zu verwendende Profil aus der Zielgruppe aus. Sie können Adobe Campaign auch ein zufälliges Profil aus der Zielgruppe auswählen lassen.

   ![](assets/substitution.png)

Nach Auswahl der Testversand-Empfänger können Sie die Test-E-Mail versenden. [Erfahren Sie, wie Sie einen Testversand durchführen](#send)

>[!NOTE]
>
>Wenn Sie die endgültige E-Mail-Nachricht an die Testversand-Empfänger senden möchten, aktivieren Sie die Option **[!UICONTROL Testpopulation in Hauptzielgruppe einbeziehen]**.

## Versenden der Testsendungen {#send}

Um die Testsendungen an die ausgewählten Empfänger zu senden, klicken Sie auf **[!UICONTROL Test-E-Mail senden]** und bestätigen Sie dann den Versand.

![](assets/send-proof.png)

Senden Sie so viele Testsendungen wie nötig, bis Sie die endgültigen Inhalte Ihres Versands festgelegt haben. Danach können Sie die E-Mail an die Hauptzielgruppe senden. [Erfahren Sie, wie Sie Ihre E-Mail vorbereiten und senden](../monitor/prepare-send.md)

## Testsendungen aufrufen {#access-proofs}

Sobald die Testsendungen gesendet wurden, können Sie über die Schaltfläche **[!UICONTROL Test-E-Mail-Protokoll anzeigen]** auf dedizierte Protokolle zugreifen. Diese Protokolle ermöglichen den Zugriff auf alle Testsendungen, die für den ausgewählten Versand durchgeführt werden, und die Visualisierung spezifischer Versandstatistiken.

![](assets/proof-log.png)

Sie können auch auf Testsendungen aus der Versandliste zugreifen, wie bei jedem Versand.

![](assets/delivery-list.png)
