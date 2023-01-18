---
audience: end-user
title: Senden Ihrer ersten E-Mail
description: Erfahren Sie, wie Sie Ihre erste E-Mail mit der Campaign-Web-Benutzeroberfläche senden.
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 24%

---

# Senden Ihrer ersten E-Mail {#first-email}

![](../assets/do-not-localize/badge.png)

Erfahren Sie, wie Sie Ihre erste Targeting-E-Mail erstellen. In diesem Anwendungsfall planen Sie den Versand einer E-Mail an Silver- und Gold-Mitglieder zu einem bestimmten Datum.

Basierend auf einer vordefinierten Designvorlage bietet die E-Mail auch personalisierte Inhalte, die auf Kundenprofilattributen basieren.

![](assets/delivery-list.png)

## Erstellen der E-Mail {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Wählen Sie eine E-Mail-Vorlage aus"
>abstract="Eine E-Mail-Vorlage ist eine spezifische Versandkonfiguration, die vordefinierte Einstellungen wie Typologieregeln, Personalisierung oder Routing-Parameter enthält. Vorlagen werden in der Campaign-Clientkonsole definiert."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="E-Mail-Eigenschaften"
>abstract="Die Eigenschaften sind die üblichen Versandparameter, nach denen Sie Ihren Versand benennen und klassifizieren können. Wenn Ihr Versand auf einem erweiterten Schema basiert, das in der Adobe Campaign v8-Konsole definiert ist, stehen einige **benutzerdefinierte Optionen** zur Verfügung."

1. Gehen Sie zur Erstellung eines neuen Versands zu **[!UICONTROL Sendungen]** Menü und wählen Sie **[!UICONTROL Email]** als Kanal.

1. Wählen Sie die gewünschte Vorlage aus und klicken Sie auf **[!UICONTROL Versand erstellen]**.

   >[!NOTE]
   >
   >Vorlagen sind vorkonfigurierte Versandeinstellungen, die für die zukünftige Verwendung gespeichert werden. Sie können von Administratoren in der Adobe Campaign-Konsole erstellt werden. [Erfahren Sie, wie Sie mit Versandvorlagen arbeiten können](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html?lang=de){target="_blank"}.

   ![](assets/channel-template.png)

1. Geben Sie einen Titel für die E-Mail an und konfigurieren Sie zusätzliche Optionen entsprechend Ihren Anforderungen:

   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu,
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner,
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an,
   * **[!UICONTROL Art]**: Geben Sie die Art der E-Mail zu Klassifizierungszwecken an.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Wenn Sie Ihr Schema mit bestimmten benutzerdefinierten Feldern erweitert haben, können Sie sie im **[!UICONTROL Benutzerdefinierte Optionen]** Abschnitt.

   ![](assets/email-properties.png)

   Erweiterte Einstellungen wie Typologieregeln und Zielgruppen-Mappings sind über die Schaltfläche neben dem Versandnamen zugänglich. Diese Einstellungen sind in der ausgewählten Vorlage vorkonfiguriert, können jedoch bei Bedarf für diese E-Mail bearbeitet werden.

## Erstellen des E-Mail-Inhalts {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Erfahren Sie, wie Sie E-Mail-Inhalte erstellen"
>abstract="Erfahren Sie, wie Sie Email Designer verwenden."

In diesem Anwendungsfall verwenden Sie eine vordefinierte Vorlage, um unsere E-Mail zu erstellen.

Detaillierte Anweisungen zur Konfiguration des E-Mail-Inhalts finden Sie unter [diesem Abschnitt](../content/edit-content.md).

1. Um mit der Erstellung des E-Mail-Inhalts zu beginnen, klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]** Schaltfläche.

   Dadurch gelangen Sie zu einer dedizierten Benutzeroberfläche, über die Sie den E-Mail-Inhalt konfigurieren und mit Email Designer entwerfen können.

   ![](assets/edit-content.png)

1. Geben Sie die Betreffzeile Ihrer E-Mail ein und personalisieren Sie sie mithilfe des Ausdruckseditors. [Erfahren Sie, wie Sie Ihren Inhalt personalisieren können](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten des E-Mail-Hauptteils]** Schaltfläche.

   Wählen Sie die Methode zur Erstellung des Inhalts Ihrer E-Mail aus. Verwenden Sie in diesem Beispiel eine vordefinierte Designvorlage.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Nachdem Sie die Vorlage ausgewählt haben, wird sie in Email Designer angezeigt, wo Sie alle erforderlichen Änderungen vornehmen und Personalisierungen hinzufügen können.

   Um beispielsweise Personalisierung zum E-Mail-Titel hinzuzufügen, wählen Sie den Baustein aus und klicken Sie auf **[!UICONTROL Personalisierung hinzufügen]**.

   ![](assets/add-perso.png)

1. Sobald Sie mit dem Inhalt zufrieden sind, speichern und schließen Sie Ihren Entwurf. Klicken **[!UICONTROL Speichern]** , um zum E-Mail-Erstellungsbildschirm zurückzukehren.

   ![](assets/save-content.png)

## Definieren der Audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definieren der Audience"
>abstract="Wählen Sie die beste Audience für Ihre Marketing-Nachricht aus. Sie können eine bereits in einer Campaign v8-Instanz oder in Adobe Experience Platform definierte Audience auswählen oder mit dem Regel-Builder eine neue Audience erstellen."

In diesem Anwendungsbeispiel senden Sie die E-Mail an eine bestehende Audience. Weitere Anweisungen zum Arbeiten mit Zielgruppen finden Sie unter [diesem Abschnitt](../audience/about-audiences.md).

1. Um die Audience für die E-Mail auszuwählen, klicken Sie auf die **[!UICONTROL Zielgruppe auswählen]** und wählen Sie eine existierende Zielgruppe aus der Liste aus.

   In diesem Beispiel möchten wir eine bestehende Audience verwenden, die sich an Kunden der Treuepunktestufen Silber und Gold richtet.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Die in der Liste verfügbaren Zielgruppen stammen entweder aus Ihrer Campaign v8-Instanz oder aus Adobe Experience Platform, wenn die Ziel-/Quellen-Integration in Ihrer Instanz konfiguriert wurde.
   >
   >Die Ziel-/Quellen-Integration ermöglicht es Ihnen, Experience Platform-Segmente an Adobe Campaign zu senden und Versand- und -Trackinglogs von Campaign an Adobe Experience Platform zu senden. [Erfahren Sie, wie Sie mit Campaign und Adobe Experience Platform arbeiten](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html?lang=de){target="_blank"}.

1. Nach Auswahl der Audience können Sie die Zielgruppe durch Anwendung zusätzlicher Regeln weiter verfeinern.

   Sie können auch eine Kontrollgruppe einrichten, um das Verhalten der E-Mail-Empfänger im Vergleich zu den Empfängern, die nicht kontaktiert wurden, zu analysieren. [Erfahren Sie, wie Sie mit Kontrollgruppen arbeiten](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Terminieren des Versands {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Terminieren des Versands"
>abstract="Definieren Sie das Datum und die genaue Uhrzeit für Ihren Versand. Durch die Auswahl der für Ihre Marketing-Nachricht am besten geeigneten Zeit können Sie die Öffnungsraten maximieren."

Um den Versand der E-Mail zu planen, klicken Sie auf **[!UICONTROL Aktivieren]** und legen Sie das gewünschte Datum und die gewünschte Uhrzeit für den Versand fest.

Standardmäßig wird die **[!UICONTROL Vor dem Versand bestätigen]** aktiviert ist, müssen Sie den Versand bestätigen, bevor die E-Mail zum geplanten Datum und zur geplanten Uhrzeit gesendet wird. Wenn Sie die E-Mail automatisch am geplanten Datum und zur geplanten Uhrzeit versenden möchten, können Sie diese Option deaktivieren.

![](assets/schedule.png)

## Anzeigen der Vorschau und Testen der E-Mail {#preview-test}

Bevor Sie Ihre E-Mail versenden, können Sie sie in der Vorschau anzeigen und testen, um sicherzustellen, dass sie Ihren Erwartungen entspricht.

In diesem Anwendungsbeispiel zeigen Sie die E-Mail-Vorschau an und senden Testversionen an bestimmte E-Mail-Adressen, während Sie einige der Zielgruppenprofile imitieren.

Weitere Informationen zum Anzeigen einer Vorschau und zum Testen von E-Mails finden Sie in [diesem Abschnitt](../preview-test/preview-test.md).

1. Um die E-Mail zu überprüfen und zu senden, klicken Sie auf **[!UICONTROL Überprüfen und Senden]**. Daraufhin wird eine Vorschau Ihrer E-Mail zusammen mit allen konfigurierten Eigenschaften, Zielgruppen und Zeitplänen angezeigt. Sie können jedes dieser Elemente bearbeiten, indem Sie auf die Schaltfläche Ändern klicken.

1. Um eine Vorschau der E-Mail anzuzeigen und Testversionen zu senden, klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]** Schaltfläche.

   ![](assets/review-email.png)

1. Wählen Sie links die Profile aus, die Sie für die Vorschau der E-Mail verwenden möchten.

   Im rechten Bereich wird eine Vorschau der E-Mail auf der Basis des ausgewählten Profils angezeigt. Wenn Sie mehrere Profile hinzugefügt haben, können Sie zwischen diesen Profilen wechseln, um eine Vorschau der entsprechenden E-Mail anzuzeigen.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Um Testversionen Ihrer E-Mail zu senden, klicken Sie auf die Schaltfläche **[!UICONTROL Test]** und wählen Sie den gewünschten Modus aus.

   Verwenden Sie in diesem Beispiel die **[!UICONTROL Ersatz aus Hauptzielgruppe]** -Modus, der Testversionen an bestimmte E-Mail-Adressen sendet und dabei einige der Profile stellvertretend agiert, auf die die E-Mail abzielt.

   ![](assets/proof-mode.png)

1. Klicken **[!UICONTROL Adresse hinzufügen]** und geben Sie die E-Mail-Adresse(n) an, an die die Testversionen gesendet werden.

   Wählen Sie für jede E-Mail-Adresse das Profil aus, das stellvertretend agieren soll. Sie können Adobe Campaign auch ein zufälliges Profil aus der Zielgruppe auswählen lassen.

   ![](assets/proof-test-profile.png)

1. Klicken **[!UICONTROL Test-E-Mail senden]** und bestätigen Sie den Versand.

   Testversionen werden mithilfe des ausgewählten Profils mit der **[Proof x]** -Präfix.

   ![](assets/proof-sent.png)

   Sie können den Status des Versands überprüfen und auf die gesendeten Test-E-Mails zugreifen, indem Sie auf die **[!UICONTROL Anzeigen des E-Mail-Testprotokolls]** im Bildschirm &quot;Inhalt simulieren&quot;.

## Senden und Überwachen der E-Mail {#prepare-send}

Nach der Überprüfung und dem Testen Ihrer E-Mail können Sie die Vorbereitung starten und sie senden.

1. Um die Vorbereitung der E-Mail zu starten, klicken Sie auf **[!UICONTROL Vorbereiten]**. [Erfahren Sie, wie Sie eine E-Mail vorbereiten](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Sobald Ihre E-Mail versandbereit ist, klicken Sie auf die Schaltfläche **[!UICONTROL Senden]** Schaltfläche (oder **[!UICONTROL Senden als geplant]** wenn Sie den Versand geplant haben) und bestätigen Sie den Versand.

1. Während des Versandvorgangs können Sie den Fortschritt verfolgen und Statistiken in Echtzeit direkt in diesem Bildschirm anzeigen.

   ![](assets/sent-mail.png)

   Sie können auch auf detaillierte Informationen zum Versand zugreifen, indem Sie auf die **[!UICONTROL Protokolle]** Schaltfläche. [Erfahren Sie, wie Sie Versand-Logs überwachen](../monitor/delivery-logs.md)

1. Nach dem Versand der E-Mail können Sie auf spezielle Berichte zugreifen, die Sie für weitere Analysen nutzen können, indem Sie auf die Schaltfläche **[!UICONTROL Berichterstellung]** Schaltfläche.

![](assets/reports.png)
