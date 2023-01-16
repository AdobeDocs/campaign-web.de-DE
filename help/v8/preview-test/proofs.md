---
audience: end-user
title: Test-E-Mails senden
description: Erfahren Sie, wie Sie Test-E-Mails definieren und senden
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 8398c0cacb2e6e2198e295787bb5e4e25af74e6e
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 8%

---

# Test-E-Mails senden {#send-proofs}

![](../assets/do-not-localize/badge.png)

Der Versand von Test-E-Mails ist ein wichtiger Schritt zur Validierung Ihrer E-Mail-Kampagne und zur Identifizierung potenzieller Probleme. Durch den Versand von Test-E-Mails können Sie verschiedene Elemente wie Links, Opt-out-Links, Bilder und Mirrorseiten überprüfen und Fehler erkennen.

Test-E-Mails können an zwei Empfängertypen gesendet werden:

* **Testprofile**: Testadressen, bei denen es sich um zusätzliche fiktive Empfänger in der Datenbank handelt, mit Test-E-Mails versenden,

* **Substitution durch Hauptzielgruppe**: Testversand-E-Mails an eine bestimmte E-Mail-Adresse senden, während die Identität eines vorhandenen Profils übernommen wird. Auf diese Weise können Sie die E-Mail so erleben, wie sie die Empfänger erhalten. So erhalten Sie eine genaue Darstellung der Nachricht, die das Profil empfangen wird.

## Testempfänger auswählen {#recipients}

1. Rufen Sie den Bildschirm zur Inhaltsimulation der E-Mail auf und klicken Sie auf die Schaltfläche **[!UICONTROL Test]** Schaltfläche.

   ![](assets/test-button.png)

1. Verwenden Sie die **[!UICONTROL Modus]** Dropdown-Liste zur Auswahl des Empfängertyps, der die Test-E-Mail erhalten soll:

   * **Testprofile**: die Test-E-Mail an Testadressen senden, die zusätzliche fiktive Empfänger in der Datenbank sind,

   * **Substitution durch Hauptzielgruppe**: die Test-E-Mail an eine bestimmte E-Mail-Adresse senden, während die Identität eines vorhandenen Profils übernommen wird. Auf diese Weise können Sie die E-Mail so erleben, wie sie die Empfänger erhalten. So erhalten Sie eine genaue Darstellung der Nachricht, die das Profil empfangen wird.

   ![](assets/test-mode.png)

   >[!NOTE]
   >
   >Standardmäßig wird die **[!UICONTROL Testprofile]** ausgewählt ist. Wenn Sie bereits Profile ausgewählt haben, um die E-Mail im Bildschirm der Inhaltsimulation in der Vorschau anzuzeigen, werden diese Profile als Testempfänger vorausgewählt. Sie können Ihre Auswahl löschen und/oder zusätzliche Empfänger hinzufügen.

1. Um Test-E-Mails an Ersatzprofile zu senden, wählen Sie die **[!UICONTROL Substitution durch Zielgruppe]** -Modus und führen Sie dann die folgenden Schritte aus:

   1. Klicken Sie auf **[!UICONTROL Adresse hinzufügen]** und geben Sie die E-Mail-Adresse an, an die die Test-E-Mail gesendet werden soll.

      Sie können eine beliebige E-Mail-Adresse eingeben. So können Sie Testadressen an beliebige Benutzer senden, auch wenn diese nicht Adobe Campaign V8 verwenden.

   1. Wählen Sie das Profil aus der Zielgruppe aus, das zum Senden der Test-E-Mail verwendet werden soll. Sie können Adobe Campaign auch ein zufälliges Profil aus der Zielgruppe auswählen lassen.

   1. Bestätigen Sie den Empfänger und wiederholen Sie den Vorgang, um beliebig viele Adressen hinzuzufügen.

      ![](assets/substitution.png)

1. Nachdem die Testempfänger ausgewählt wurden, können Sie die Test-E-Mail senden. [Erfahren Sie, wie Sie Test-E-Mails senden.](#send)

   >[!NOTE]
   >
   >Wenn Sie die endgültige E-Mail-Nachricht an die Empfänger der Test-E-Mail senden möchten, aktivieren Sie die **[!UICONTROL Testpopulation in die Hauptzielgruppe einbeziehen]** aktiviert.

## Test-E-Mail senden {#send}

Um die Test-E-Mail an die ausgewählten Empfänger zu senden, klicken Sie auf **[!UICONTROL Test-E-Mail senden]** validieren Sie dann den Versand.

![](assets/send-proof.png)

Senden Sie so viele Test-E-Mails wie nötig, bis Sie den Inhalt Ihres Versands fertig gestellt haben. Danach können Sie die E-Mail an die Hauptzielgruppe senden. [Erfahren Sie, wie Sie Ihre E-Mail vorbereiten und senden](../monitor/prepare-send.md)

## Auf gesendete Test-E-Mails zugreifen {#access-proofs}

Sobald die Test-E-Mails gesendet wurden, können Sie über die **[!UICONTROL Anzeigen des E-Mail-Testprotokolls]** Schaltfläche.

Diese Protokolle ermöglichen den Zugriff auf alle Test-E-Mails, die für den ausgewählten Versand gesendet werden, und die Visualisierung spezifischer Statistiken bezüglich des Versands. [Erfahren Sie, wie Sie Versand-Logs überwachen](../monitor/delivery-logs.md)

![](assets/proof-log.png)

Sie können wie bei jedem Versand auch über die Versandliste auf die gesendeten Test-E-Mails zugreifen.

![](assets/delivery-list.png)
