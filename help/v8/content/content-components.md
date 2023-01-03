---
audience: end-user
title: Verwenden der Inhaltskomponenten von E-Mail-Designer
description: Erfahren Sie, wie Sie Inhaltskomponenten in E-Mails verwenden
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: fd85f2b799602b7c411b73e7b1c1cbd38c798857
workflow-type: ht
source-wordcount: '1397'
ht-degree: 100%

---

# Verwenden der Inhaltskomponenten von E-Mail-Designer {#content-components}

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Über Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout einer E-Mail gestalten können."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Über Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout einer Landingpage gestalten können."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Über Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout eines Fragments gestalten können."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Über Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout einer Vorlage gestalten können."

## Hinzufügen von Inhaltskomponenten {#add-content-components}

Gehen Sie wie folgt vor, um Ihrer E-Mail Inhaltskomponenten hinzuzufügen und diese an Ihre Anforderungen anzupassen.

1. Verwenden Sie in E-Mail-Designer einen vorhandenen Inhalt oder ziehen Sie per Drag-and-Drop **[!UICONTROL Strukturkomponenten]** in einen leeren Inhalt, um das Layout Ihrer E-Mail zu definieren. [Weitere Informationen](create-email-content.md)

1. Um den Abschnitt **[!UICONTROL Inhaltskomponenten]** zu öffnen, wählen Sie die entsprechende Schaltfläche im linken Bereich von E-Mail-Designer aus.

   ![](assets/email_designer_content_components.png)

1. Platzieren Sie die Inhaltskomponenten Ihrer Wahl mittels Drag-and-Drop in den relevanten Strukturkomponenten.

   ![](assets/email_designer_add_content_components.png)

   >[!NOTE]
   >
   >Sie können zu einer einzelnen Strukturkomponente und zu jeder Spalte einer Strukturkomponente mehrere Komponenten hinzufügen.

1. Passen Sie die Stilattribute für jede Komponente im Bereich **[!UICONTROL Komponenteneinstellungen]** auf der rechten Seite an. Beispielsweise können Sie den Textstil, den Abstand oder den Rand jeder Komponente ändern. [Weitere Informationen zu Ausrichtung und Abstand](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png)

Wenn Sie Ihre E-Mail-Inhalte von Grund auf neu erstellen, können Sie sie mithilfe von **[!UICONTROL Inhaltskomponenten]** durch das Einfügen unbearbeiteter, leerer Komponenten personalisieren.
Sie können beliebig viele **[!UICONTROL Inhaltskomponenten]** in eine **[!UICONTROL Strukturkomponente]**, die das Layout Ihrer E-Mail definiert, einfügen.

## Container {#container}

Sie können einen einfachen Container hinzufügen, in den Sie eine weitere Inhaltskomponente einfügen können. Auf diese Weise können Sie einen bestimmten Stil auf den Container anwenden, der sich von der darin verwendeten Komponente unterscheidet.

Sie können in diesen Container beispielsweise die Komponente **[!UICONTROL Container]** und anschließend die Komponente [Schaltfläche](#button) einfügen. Dann können Sie einen bestimmten Hintergrund für den Container und einen anderen für die Schaltfläche verwenden.

![](assets/email_designer_container_component.png)

## Schaltfläche {#buttons}

Verwenden Sie die Komponente **[!UICONTROL Schaltfläche]**, um eine oder mehrere Schaltflächen in Ihre E-Mail einzufügen und Ihre E-Mail-Audience auf eine bestimmte Seite weiterzuleiten.

1. Platzieren Sie die Komponente **[!UICONTROL Schaltfläche]** von den **[!UICONTROL Inhaltskomponenten]** per Drag-and-Drop in eine **[!UICONTROL Strukturkomponente]**.

   ![](assets/email_designer_13.png)

1. Klicken Sie auf die neu hinzugefügte Schaltfläche, um den Text anzupassen und um auf die **[!UICONTROL Komponenteneinstellungen]** im rechten Bereich von E-Mail-Designer zuzugreifen.

   ![](assets/email_designer_14.png)

1. Fügen Sie im Feld **[!UICONTROL Link]** die URL hinzu, zu der Sie Benutzende beim Anklicken der Schaltfläche umleiten möchten.

1. Wählen Sie mit der Dropdown-Liste die **[!UICONTROL Zielgruppe]** aus, mit der Ihre Audience umgeleitet werden soll:

   * **[!UICONTROL Keine]**: öffnet den Link im selben Fenster, in dem er angeklickt wurde (Standard).
   * **[!UICONTROL Leer]**: Öffnet den Link in einem neuen Fenster oder in einer neuen Registerkarte.
   * **[!UICONTROL Selbst]**: Öffnet den Link im selben Fenster, in dem er angeklickt wurde.
   * **[!UICONTROL Übergeordnet]**: Öffnet den Link im übergeordneten Fenster.
   * **[!UICONTROL Beliebteste]**: Öffnet den Link im Textkörper des Fensters.

   ![](assets/email_designer_15.png)

1. Sie können Ihre Schaltfläche weiter personalisieren, indem Sie Stilattribute wie **[!UICONTROL Rahmen]**, **[!UICONTROL Größe]**,**[!UICONTROL Rand]** usw. im Bereich **[!UICONTROL Komponenteneinstellungen]** ändern.

## Text {#text}

Verwenden Sie die Komponente **[!UICONTROL Text]**, um Text in Ihre E-Mail einzufügen und den Stil (Rahmen, Größe, Abstand usw.) mithilfe des Bereichs **[!UICONTROL Komponenteneinstellungen]** anzupassen.

1. Platzieren Sie aus **[!UICONTROL Inhaltskomponenten]** per Drag-and-Drop **[!UICONTROL Text]** in einer **[!UICONTROL Strukturkomponente]**.

   ![](assets/email_designer_11.png)

1. Klicken Sie auf die neu hinzugefügte Komponente, um den Text zu personalisieren und auf die **[!UICONTROL Komponenteneinstellungen]** im rechten Bereich von E-Mail Designer zugreifen zu können.

1. Ändern Sie den Text mit den folgenden in der Symbolleiste verfügbaren Optionen:

   ![](assets/email_designer_27.png)

   * **[!UICONTROL Textstil ändern]**: Fett, Kursiv, Unterstreichen oder Durchstreichen auf Ihren Text anwenden.
   * **Ausrichtung ändern**: Wählen Sie für Ihren Text zwischen linksbündig ausrichten, rechtsbündig ausrichten, zentriert oder Blocksatz.
   * **[!UICONTROL Liste erstellen]**: Eine Aufzählungs- oder nummerierte Liste zu Ihrem Text hinzufügen.
   * **[!UICONTROL Überschrift festlegen]**: Bis zu sechs Überschriftenebenen zu Ihrem Text hinzufügen.
   * **Schriftgröße**: Wählen Sie die Schriftgröße Ihres Textes in Pixel aus.
   * **[!UICONTROL Bild bearbeiten]**: Ein Bild oder ein Medienelement zu Ihrer Textkomponente hinzufügen.
   * **[!UICONTROL Quell-Code anzeigen]**: Den Quell-Code Ihres Textes anzeigen. Es kann nicht geändert werden.
   * **[!UICONTROL Duplizieren]**: Eine Kopie der Textkomponente hinzufügen.
   * **[!UICONTROL Löschen]**: Die ausgewählte Textkomponente aus der E-Mail löschen.
   * **[!UICONTROL Personalisierung hinzufügen]**: Personalisierungsfelder hinzufügen, um den Inhalt aus Ihren Profildaten anzupassen.
   * **[!UICONTROL Bedingten Inhalt aktivieren]**: Einen bedingten Inhalt hinzufügen, um den Inhalt der Komponente an die Zielprofile anzupassen.

1. Andere Stilattribute wie Textfarbe, Schriftfamilie, Rahmen, Abstand, Rand usw. können Sie im Bedienfeld **[!UICONTROL Komponenteneinstellungen]** anpassen.

   ![](assets/email_designer_12.png)

## Trennlinie {#divider}

Verwenden Sie die Komponente **[!UICONTROL Trennlinie]**, um das Layout und den Inhalt Ihrer E-Mail durch eine Trennlinie zu strukturieren.

Sie können Stilattribute wie Zeilenfarbe, Stil und Höhe in den **[!UICONTROL Komponenteneinstellungen]** anpassen.

![](assets/email_designer_16.png)

## HTML {#HTML}

Verwenden Sie die Komponente **[!UICONTROL HTML]**, um die unterschiedlichen Teile Ihrer existierenden HTML-Datei zu kopieren und einzufügen. Dadurch können Sie kostenfreie modulare HTML-Komponenten erstellen, um externe Inhalte wiederzuverwenden.

1. Ziehen Sie aus den **[!UICONTROL Inhaltskomponenten]** die **[!UICONTROL HTML]**-Komponente per Drag-and-Drop in eine **[!UICONTROL Strukturkomponente]**.

   ![](assets/email_designer_22.png)

1. Klicken Sie auf die neu hinzugefügte Komponente und dann in der kontextbezogenen Symbolleiste auf **[!UICONTROL Quell-Code anzeigen]**, um Ihren HTML-Code hinzuzufügen.

   ![](assets/email_designer_23.png)

>[!NOTE]
>
>Um die Kompatibilität von externen Inhalten mit E-Mail-Designer zu gewährleisten, empfiehlt Adobe, eine neue Nachricht zu erstellen und den Inhalt aus der existierenden E-Mail in Komponenten einzufügen.

## Bild {#image}

Verwenden Sie die Komponente **[!UICONTROL Bild]**, um eine Bilddatei von Ihrem Computer in Ihre E-Mail einzufügen.

1. Ziehen Sie aus den **[!UICONTROL Inhaltskomponenten]** das **[!UICONTROL Bild]** per Drag-and-Drop in eine **[!UICONTROL Strukturkomponente]**.

   ![](assets/email_designer_9.png)

1. Klicken Sie auf **[!UICONTROL Durchsuchen]**, um eine Bilddatei aus Ihren Assets auszuwählen.

1. Klicken Sie auf die neu hinzugefügte Komponente und richten Sie Ihre Bildeigenschaften mithilfe des Bedienfelds **[!UICONTROL Komponenteneinstellungen]** ein:

   * **[!UICONTROL Bildtitel]** ermöglicht Ihnen, den Titel für das Bild zu definieren.
   * **[!UICONTROL Alternativtext]** ermöglicht Ihnen, die zugeordnete Beschriftung zu Ihrem Bild zu definieren. Dies entspricht dem Alt-HTML-Attribut.

   ![](assets/email_designer_10.png)

1. Über den Bereich **[!UICONTROL Komponenteneinstellungen]** können Sie die anderen Stilattribute wie Rand, Umrandung usw. anpassen oder einen Link hinzufügen, um Ihre Audience zu einem anderen Inhalt weiterzuleiten.

## Video {#Video}

>[!CONTEXTUALHELP]
>id="ac_edition_video_email"
>title="Videoeinstellungen"
>abstract="Verwenden Sie diese Komponente, um ein Video in Ihre E-Mail einzufügen. Beachten Sie, dass Videos nicht auf allen E-Mail-Clients funktionieren. Wir empfehlen, ein Reservebild festzulegen."

>[!CONTEXTUALHELP]
>id="ac_edition_video_landing_page"
>title="Videoeinstellungen"
>abstract="Verwenden Sie diese Komponente, um ein Video in Ihre Landingpage einzufügen. Beachten Sie, dass Videos nicht in allen Nachrichten-Clients funktionieren. Wir empfehlen, ein Reservebild festzulegen."

>[!CONTEXTUALHELP]
>id="ac_edition_video_fragment"
>title="Videoeinstellungen"
>abstract="Verwenden Sie diese Komponente, um ein Video in Ihr Fragment einzufügen. Beachten Sie, dass Videos nicht in allen Nachrichten-Clients funktionieren. Wir empfehlen, ein Reservebild festzulegen."

>[!CONTEXTUALHELP]
>id="ac_edition_video_template"
>title="Videoeinstellungen"
>abstract="Verwenden Sie diese Komponente, um ein Video in Ihre Vorlage einzufügen. Beachten Sie, dass Videos nicht in allen Nachrichten-Clients funktionieren. Wir empfehlen, ein Reservebild festzulegen."


Verwenden Sie die Komponente **[!UICONTROL Video]**, um über einen URL-Link ein Video in Ihre E-Mail einzufügen.

1. Ziehen Sie aus den **[!UICONTROL Inhaltskomponenten]** das **[!UICONTROL Video]** per Drag-and-Drop in eine **[!UICONTROL Strukturkomponente]**.

   ![](assets/email_designer_17.png)

1. Klicken Sie auf die neu hinzugefügte Komponente, um mit der Konfiguration Ihrer **[!UICONTROL Inhaltskomponenten]** zu beginnen und auf die **[!UICONTROL Komponenteneinstellungen]** im rechten Bereich des E-Mail-Designers zugreifen zu können.

1. Geben Sie in das Feld **[!UICONTROL Video-Link]** in den **[!UICONTROL Komponenteneinstellungen]** Ihre Video-URL ein.

   ![](assets/email_designer_18.png)

1. Sie können dem Video ein **[!UICONTROL Standbild]** hinzufügen, das angezeigt wird, bis Ihre Audience auf die Wiedergabe-Schaltfläche klickt.

1. Passen Sie die anderen Stilattribute wie Stil, Rand, Rahmen usw. an, indem Sie das Bedienfeld **[!UICONTROL Komponenteneinstellungen]** verwenden.

## Social {#social}

Verwenden Sie die Komponente **[!UICONTROL Social]**, um Links zu Social-Media-Seiten in Ihre E-Mail einzufügen.

1. Ziehen Sie aus den **[!UICONTROL Inhaltskomponenten]** die Komponente **[!UICONTROL Social]** per Drag-and-Drop in eine **[!UICONTROL Strukturkomponente]**.

1. Klicken Sie auf die neu hinzugefügte Komponente.

1. Im Feld **[!UICONTROL Social]** der **[!UICONTROL Komponenteneinstellungen]** können Sie auswählen, welche Social Media Sie hinzufügen oder entfernen möchten.

   ![](assets/email_designer_20.png)

1. Wählen Sie die Größe Ihrer Symbole im Feld **[!UICONTROL Bildgröße]** .

1. Klicken Sie auf jedes Ihrer Social Media-Symbole, um die **[!UICONTROL URL]** zu konfigurieren, zu der Ihre Audience weitergeleitet wird.

   ![](assets/email_designer_21.png)

1. Bei Bedarf können Sie auch die Symbole der einzelnen Social Media im Feld **[!UICONTROL Bild]** ändern,

1. Passen Sie die anderen Stilattribute wie Stil, Rand, Rahmen usw. an, indem Sie das Bedienfeld **[!UICONTROL Komponenteneinstellungen]** verwenden.

## Karussell {#carousel-settings}

1. Ziehen Sie die Komponente **[!UICONTROL Karussell]** in eine Strukturkomponente.

1. Durchsuchen Sie Ihre Festplatte nach Bildern.

1. Wählen Sie in den **[!UICONTROL Einstellungen]** die Anzahl der gewünschten Miniaturansichten für das Karussell aus.

1. Wählen Sie ein Fallback-Bild von Ihrer Festplatte aus.

Die Karussell-Komponente ist nicht mit allen E-Mail-Programmen kompatibel. Wenn das Karussell vom E-Mail-Programm nicht unterstützt wird, laden Sie ein Fallback-Bild hoch.
