---
audience: end-user
title: Erstellen Ihrer ersten E-Mail
description: Web-Dokumentation zu Campaign v8
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 75d579975023639840f35f673e63aab2a2d3a811
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 98%

---

# Senden Ihrer ersten E-Mail {#first-email}

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

In diesem Anwendungsbeispiel wird gezeigt, wie Sie Ihre erste E-Mail erstellen. Wir planen den Versand einer E-Mail zu einem bestimmten Datum an Kunden der Treuestufen Silber und Gold. Diese E-Mail wird mit einer vordefinierten Vorlage erstellt und umfasst eine Personalisierung anhand der Profilattribute.

![](assets/delivery-list.png)

## Erstellen der E-Mail {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Wählen Sie eine E-Mail-Vorlage aus"
>abstract="Eine Vorlage wird in der Adobe Campaign v8-Konsole definiert. Dies ist eine spezifische Versandkonfiguration, die vordefinierte Parameter wie Typologieregeln, Personalisierung oder Routing-Parameter enthält."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="E-Mail-Eigenschaften"
>abstract="Die Eigenschaften sind die üblichen Versandparameter, nach denen Sie Ihren Versand benennen und klassifizieren können. Wenn Ihr Versand auf einem erweiterten Schema basiert, das in der Adobe Campaign v8-Konsole definiert ist, stehen einige **benutzerdefinierte Optionen** zur Verfügung."

1. Erstellen Sie einen neuen Versand im Menü **[!UICONTROL Sendungen]**.

1. Wählen Sie den Kanal und die zu verwendende Vorlage für die **[!UICONTROL E-Mail]** und klicken Sie auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >Eine Vorlage ist eine spezifische Versandkonfiguration, die als Vorlage zur Wiederverwendung gespeichert wurde. Versandvorlagen werden von Admins in der Adobe Campaign-Konsole konfiguriert. [Erfahren Sie, wie Sie mit Versandvorlagen arbeiten können](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-delivery-templates/about-templates.html?lang=de){target=&quot;_blank&quot;}

   ![](assets/channel-template.png)

1. Geben Sie einen Titel für die E-Mail an und konfigurieren Sie zusätzliche Optionen entsprechend Ihren Anforderungen:

   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu,
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner,
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an,
   * **[!UICONTROL Art]**: Geben Sie die Art der E-Mail zu Klassifizierungszwecken an.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Wenn Sie Ihr Schema mit bestimmten benutzerdefinierten Feldern erweitert haben, können Sie in den **[!UICONTROL benutzerdefinierten Optionen]** darauf zugreifen.

   ![](assets/email-properties.png)

   Darüber hinaus sind erweiterte Einstellungen (Typologieregel, Zielgruppen-Mappings usw.) über die Schaltfläche neben dem Versandnamen verfügbar. Sie sind in der bei der E-Mail-Erstellung ausgewählten Vorlage vordefiniert. Sie können sie bei Bedarf bearbeiten.

## Erstellen des E-Mail-Inhalts {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Erfahren Sie, wie Sie mit E-Mail-Designer E-Mail-Inhalte gestalten."
>abstract="Erfahren Sie, wie Sie Inhalte gestalten."

In diesem Anwendungsbeispiel wird die E-Mail mit einer vordefinierten Vorlage erstellt. Detaillierte Informationen zur Konfiguration von E-Mail-Inhalten finden Sie in [diesem Abschnitt](../content/edit-content.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]**, um den Inhalt Ihrer E-Mail zu erstellen.

   Auf diesem Bildschirm können Sie den Inhalt der E-Mail konfigurieren und mit E-Mail-Designer gestalten.

   ![](assets/edit-content.png)

1. Geben Sie den Betreff Ihrer E-Mail an und personalisieren Sie ihn mithilfe des Ausdruckseditors. [Erfahren Sie, wie Sie Ihren Inhalt personalisieren können](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL E-Mail-Textkörper bearbeiten]**, um den Inhalt Ihrer E-Mail zu erstellen und zu gestalten.

   Wählen Sie die Methode zur Erstellung des Inhalts Ihrer E-Mail aus. In diesem Beispiel möchten wir eine bereits vorhandene Design-Vorlage verwenden.

   ![](assets/import-html.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Nach der Auswahl der Vorlage wird sie in E-Mail-Designer angezeigt, sodass sie bei Bedarf bearbeitet und personalisiert werden kann.

   In diesem Beispiel möchten wir eine Personalisierung zum E-Mail-Titel hinzufügen. Wählen Sie dazu die Komponente aus und klicken Sie auf **[!UICONTROL Personalisierung hinzufügen]**.

   ![](assets/add-perso.png)

1. Nach Fertigstellung des Inhalts speichern Sie diesen und klicken Sie auf den Pfeil, um zum E-Mail-Erstellungsbildschirm zurückzukehren.

   ![](assets/save-content.png)

## Definieren der Audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definieren der Audience"
>abstract="Wählen Sie die beste Audience für Ihre Marketing-Nachricht aus. Sie können eine bereits in einer Campaign v8-Instanz oder in Adobe Experience Platform definierte bestehende Audience auswählen oder mit Segment Builder eine neue Audience erstellen."

In diesem Anwendungsbeispiel senden wir die E-Mail an eine bereits bestehende Audience. Weitere Informationen zum Arbeiten mit Audiences finden Sie in [diesem Abschnitt](../audience/about-audiences.md).

1. Klicken Sie auf **[!UICONTROL Audience auswählen]** und wählen Sie eine bestehende Audience, die Sie ansprechen möchten, aus.

   In diesem Beispiel möchten wir eine bestehende Audience verwenden, die sich an Kunden der Treuepunktestufen Silber und Gold richtet.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Die in der Liste verfügbaren Audiences stammen entweder aus Ihrer Campaign V8-Instanz oder aus Adobe Experience Platform, wenn die Ziel-/Quellen-Integration in Ihrer Instanz implementiert wurde.

1. Nach Auswahl Ihrer Audience können Sie die Regel bei Bedarf bearbeiten.

   Sie können auch eine Kontrollgruppe einrichten, um das Verhalten der E-Mail-Empfänger im Vergleich zum Verhalten von Profilen zu analysieren, die nicht angesprochen wurden. [Erfahren Sie, wie Sie mit Kontrollgruppen arbeiten](../audience/control-group.md)

## Terminieren des Versands {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Terminieren des Versands"
>abstract="Definieren Sie das Datum und die genaue Uhrzeit für Ihren Versand. Wenn Sie den für Ihre Marketing-Nachricht am besten geeigneten Zeitpunkt auswählen, maximieren Sie die Öffnungsraten."

Um den Versand der E-Mail zu terminieren, klicken Sie auf **[!UICONTROL Aktivieren]** und geben Sie dann das gewünschte Datum und die gewünschte Uhrzeit für den Versand an.

Standardmäßig ist die Option **[!UICONTROL Vor dem Versand bestätigen]** aktiviert, d. h., Sie müssen den Versand zum angegebenen Zeitpunkt bestätigen, um die E-Mail zu senden. Deaktivieren Sie diese Option, damit die E-Mail zum geplanten Datum und zur geplanten Uhrzeit ohne Bestätigung gesendet werden kann.

![](assets/schedule.png)

## Anzeigen der Vorschau und Testen der E-Mail {#preview-test}

Sobald Ihre E-Mail fertig ist, können Sie sie in der Vorschau ansehen und testen, bevor Sie den Versand starten.

In diesem Anwendungsbeispiel werden wir die E-Mail mit vorhandenen Profilen in der Vorschau ansehen und einen Testversand an ein Testprofil senden, das nicht Teil der Zielgruppe ist.

Weitere Informationen zum Anzeigen einer Vorschau und zum Testen von E-Mails finden Sie in [diesem Abschnitt](../preview-test/preview-test.md).

1. Klicken Sie auf **[!UICONTROL Zum Senden überprüfen]**. Eine Vorschau Ihrer E-Mail wird zusammen mit allen konfigurierten Eigenschaften, Audience und Zeitplan angezeigt. Sie können jedes dieser Elemente über die Schaltfläche „Ändern“ bearbeiten.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]**, um eine Vorschau der E-Mail anzuzeigen und Testsendungen durchzuführen.

   ![](assets/review-email.png)

1. Wählen Sie im linken Seitenbereich die Profile aus, die für die Vorschau der E-Mail verwendet werden sollen.

1. Im rechten Bereich wird eine Vorschau der E-Mail basierend auf dem ausgewählten Profil angezeigt. Wenn Sie mehrere Profile hinzugefügt haben, können Sie zwischen diesen Profilen wechseln, um eine Vorschau der entsprechenden E-Mail anzuzeigen.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Um Testsendungen Ihrer E-Mail durchzuführen, klicken Sie auf die Schaltfläche **[!UICONTROL Test]** und wählen Sie die Profile aus, die den Testversand erhalten sollen.

   In diesem Beispiel möchten wir die Testsendungen an ein bestimmtes Testprofil senden, bei dem es sich um eine Testadresse handelt, die nicht Teil der Zielgruppe ist. [Erfahren Sie, wie Sie mit Testadressen arbeiten](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/about-seed-addresses.html?lang=de){target=&quot;_blank&quot;}

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >Sie können Ihre Nachrichten auch testen, indem Sie die Identität einiger Zielgruppenprofile übernehmen und die Testversandnachricht an die von Ihnen ausgewählte E-Mail-Adresse senden. [Erfahren Sie, wie Sie einen Testversand durchführen](../preview-test/preview-test.md)

1. Klicken Sie auf **[!UICONTROL Test-E-Mail senden]** und bestätigen Sie dann den Versand.

   Nachdem die Testsendungen durchgeführt wurden, können Sie ihren Status überprüfen, indem Sie auf die Schaltfläche **[!UICONTROL E-Mail-Testprotokoll anzeigen]** klicken.

## Senden und Überwachen der E-Mail {#prepare-send}

Nachdem Sie Ihre E-Mail geprüft und getestet haben, können Sie mit ihrer Vorbereitung beginnen und sie senden.

1. Klicken Sie auf **[!UICONTROL Vorbereiten]**, um mit der Vorbereitung der Nachricht zu beginnen. [Erfahren Sie, wie Sie eine E-Mail vorbereiten](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Sobald Ihre E-Mail versandbereit ist, klicken Sie auf **[!UICONTROL Senden]** und bestätigen Sie danach den Versand.

   Sie können den Versand in Echtzeit zusammen mit Statistiken verfolgen. Darüber hinaus ermöglicht die Schaltfläche **[!UICONTROL Protokolle]** den Zugriff auf detaillierte Informationen zum E-Mail-Versand. [Erfahren Sie, wie Sie Versand-Logs überwachen](../monitor/delivery-logs.md)
   ![](assets/logs.png)

1. Nachdem die E-Mail gesendet wurde, können Sie dedizierte [Berichte](../reporting/reports.md) für weitere Analysezwecke einsehen.

   ![](assets/reports.png)
