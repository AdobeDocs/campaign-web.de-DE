---
audience: end-user
title: Bearbeiten des E-Mail-Inhalts
description: Erfahren Sie, wie Sie den E-Mail-Inhalt in der Campaign Web-Benutzeroberfläche bearbeiten können
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 51%

---

# Konfigurieren des E-Mail-Inhalts {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definieren des E-Mail-Inhalts"
>abstract="Der Bildschirm **Inhalt bearbeiten** ermöglicht es Ihnen, grundlegende Elemente Ihrer Nachricht zu definieren, wie etwa die Absenderadresse und die Betreffzeile, zusätzliche Aktionen wie das Hinzufügen von Anhängen oder Angeboten durchzuführen und auf die E-Mail-Designer zuzugreifen, um Ihrer Nachricht ein optimiertes Aussehen zu verleihen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Festlegen der E-Mail-Eigenschaften"
>abstract="Im Abschnitt **Grundlegende Details** können die Adresse der Absenderin bzw. des Absenders und die Antwortadresse aktualisiert und die Betreffzeile mithilfe des Ausdruckseditors definiert werden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Anhängen von Dateien an eine E-Mail"
>abstract="Wählen Sie eine oder mehrere Dateien aus, die Sie in Ihre Nachricht einfügen möchten. Zur Vermeidung von Leistungsproblemen wird empfohlen, nicht mehr als einen Anhang pro E-Mail hinzuzufügen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Bearbeiten des Trackings"
>abstract="Standardmäßig ist das Tracking für den Versand aktiviert, d. h. alle im Nachrichteninhalt enthaltenen Links werden verfolgt. Sie können diese Option hier deaktivieren."
>additional-url="https://experienceleague.adobe.com/de/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Hinzufügen von Links und Nachverfolgen von Nachrichten"

Der E-Mail-Bildschirm **[!UICONTROL Inhalt bearbeiten]** ermöglicht Ihnen Folgendes:

* Definieren Sie grundlegende Elemente Ihrer Nachricht, z. B. die Absenderadresse und die Betreffzeile.
* Führen Sie zusätzliche Aktionen durch, z. B. das Hinzufügen von Anhängen oder das Einrichten von Angeboten.
* Greifen Sie auf [E-Mail-Designer](get-started-email-designer.md#start-authoring) zu, um mit der Erstellung des richtigen Inhalts Ihrer E-Mail zu beginnen.

>[!NOTE]
>
>Alle bearbeitbaren Textfelder dieses Bildschirms können mithilfe von Personalisierungsfeldern ausgefüllt werden. [Erfahren Sie, wie Sie Inhalte personalisieren](../personalization/personalize.md)

Gehen Sie wie folgt vor, um den Inhalt einer E-Mail zu konfigurieren oder zu bearbeiten.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]** im Bildschirm [E-Mail-Versand-Dashboard](../email/create-email.md).

   ![Screenshot, der die Schaltfläche „Inhalt bearbeiten“ im Dashboard des E-Mail-Versands zeigt.](assets/email-edit-content-button.png){zoomable="yes"}

1. Der Bildschirm zur Bearbeitung des E-Mail-Inhalts wird geöffnet.

   ![Screenshot mit dem Dashboard zur Bearbeitung von E-Mail-Inhalten.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Wenn Sie eine neue E-Mail konfigurieren, sind die Felder **[!UICONTROL Absendername]** und **[!UICONTROL Absender-E-Mail]** bereits ausgefüllt.

1. Das Feld **[!UICONTROL Absendername]** wird in der E-Mail-Vorlage definiert. Wenn Sie ihn ändern möchten, verwenden Sie einen Namen, der von den Empfängerinnen und Empfängern leicht erkannt werden kann, z. B. den Namen Ihrer Marke, um die Öffnungsrate Ihrer Sendungen zu erhöhen.

   >[!NOTE]
   >
   >Um das Erlebnis der Empfängerinnen und Empfänger weiter zu verbessern, können Sie den Namen einer Person hinzufügen, z. B. „Eva von Luma“.

1. Das Adressfeld **[!UICONTROL Absender-E-Mail]** wird ebenfalls in der E-Mail-Vorlage definiert. Stellen Sie sicher, dass die Adress-Domain mit der Subdomain übereinstimmt, die Sie an Adobe delegiert haben.

   >[!NOTE]
   >
   >Sie können den Teil vor dem „@“ ändern, nicht aber die Domain-Adresse.

1. Erweitern Sie den Abschnitt **[!UICONTROL Antwortfelder]**. Name und Adresse der Absenderin bzw. des Absenders werden standardmäßig für Antworten verwendet. Adobe empfiehlt jedoch die Verwendung einer bestehenden echten Adresse, z. B. der Kundenunterstützung Ihrer Marke. Wenn ein Empfänger eine Antwort sendet, kann das Kundenunterstützungs-Team sie bearbeiten.

   ![Screenshot mit dem Abschnitt Antwortfelder im E-Mail-Inhaltseditor.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Definieren Sie die **[!UICONTROL Betreffzeile]** der E-Mail. Geben Sie den Betreff direkt in das entsprechende Feld ein oder öffnen Sie den Ausdruckseditor, um [Personalisierung](../personalization/personalize.md) mithilfe verschiedener Attribute, Ausdrucksfragmente oder Angebote hinzuzufügen.

1. Wenn Sie eine Datei an die E-Mail anhängen möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Anlage hinzufügen]** und wählen Sie eine oder mehrere Dateien aus.

   >[!NOTE]
   >
   >Zur Vermeidung von Leistungsproblemen wird empfohlen, nicht mehr als einen Anhang pro E-Mail hinzuzufügen.

   <!--limitation on size + number of files?-->

1. Wenn Sie mit Ihrer E-Mail Angebote versenden möchten, wählen Sie diese über die Schaltfläche **[!UICONTROL Angebote einrichten]** aus.

   Sie können sie dann mithilfe von Personalisierungsfeldern in die E-Mail einfügen. [Erfahren Sie, wie Sie Angebote senden](../msg/offers.md)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL E-Mail-Text bearbeiten]**, um den Inhalt der E-Mail mithilfe des [E-Mail-Designers](get-started-email-designer.md#start-authoring) zu strukturieren und zu gestalten. Weitere Informationen zum Entwerfen von E-Mail-Inhalten finden Sie in den folgenden Abschnitten:

   * [Verfassen von E-Mails von Grund auf neu](create-email-content.md)
   * [Gestalten Ihrer Inhalte](get-started-email-style.md)

   >[!NOTE]
   >
   >Sie können auch den Mauszeiger über die E-Mail-Vorschau bewegen und **[!UICONTROL E-Mail-Designer öffnen]** auswählen.

1. Standardmäßig ist für den Versand Tracking aktiviert. Sie können diese Option im Bereich **[!UICONTROL Optionale Funktionen]** deaktivieren. [Erfahren Sie, wie Sie Links hinzufügen und das Tracking verwalten](message-tracking.md).

1. Nachdem Sie den Inhalt Ihrer E-Mail definiert haben, können Sie vor dem Versand mit der Schaltfläche **[!UICONTROL Inhalt simulieren]** überprüfen, wie die E-Mail dargestellt wird. [Erfahren Sie, wie Sie Ihre E-Mail in der Vorschau anzeigen und testen können](../preview-test/preview-test.md).