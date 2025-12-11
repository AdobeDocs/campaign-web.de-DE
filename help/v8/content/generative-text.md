---
audience: end-user
title: Generative Inhalte
description: Informationen zum Generieren von Textinhaltserlebnissen mit dem KI-Assistenten
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: ht
source-wordcount: '1441'
ht-degree: 100%

---

# Generieren von Text mit dem KI-Assistenten {#generative-text}

>[!IMPORTANT]
>
>Bevor Sie mit der Verwendung dieser Funktion beginnen, lesen Sie die entsprechenden Informationen unter [Schutzmechanismen und Einschränkungen](generative-gs.md#generative-guardrails).
></br>
>
>Sie müssen einer [Benutzervereinbarung](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} zustimmen, bevor Sie den KI-Assistenten in Adobe Campaign Web verwenden können. Weitere Informationen erhalten Sie beim Adobe-Support.

Verwenden Sie den KI-Assistenten in Adobe Campaign Web, um ansprechenden Text zu generieren, der bei Ihrer Zielgruppe Anklang findet. Unabhängig davon, ob Sie E-Mail-Versionen verbessern, überzeugende Landingpage-Inhalte erstellen, Push-Benachrichtigungen schreiben oder SMS-Texte verfassen, hilft Ihnen der KI-Assistent, eine klare, wirkungsvolle Kommunikation zu erreichen.

## Für E-Mail und Landingpages {#email-web-channels}

Der KI-Assistent kann hochwertige Textinhalte für Ihre E-Mail-Sendungen und Landingpages generieren. Mit dieser Funktion können Sie überzeugendes markenkonformes Messaging erstellen, das über digitale Touchpoints hinweg bei Ihrer Zielgruppe Anklang findet.

### Zugreifen und Konfigurieren {#access-configure}

Bevor Sie mit dem Generieren von Textinhalten mit dem KI-Assistenten beginnen können, müssen Sie Ihren Versand einrichten und auf den Inhaltseditor zugreifen. Gehen Sie wie folgt vor, um Ihren Arbeitsbereich vorzubereiten und das Panel „KI-Assistent“ zu öffnen.

1. Erstellen Sie einen Versand und konfigurieren Sie ihn:

   * **E-Mail**: Nachdem Sie Ihren E-Mail-Versand erstellt und konfiguriert haben, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../email/create-email-content.md)
   * **Landingpage**: Nachdem Sie Ihre Landingpage erstellt und konfiguriert haben, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../landing-pages/create-lp.md)

1. Wählen Sie eine **[!UICONTROL Textkomponente]** aus, um bestimmte Inhalte zu erfassen, und rufen Sie das Menü **[!UICONTROL KI-Assistent]** auf.

   ![Screenshot mit Auswahl der Textkomponente in Adobe Campaign Web](assets/text-genai-1.png){zoomable="yes"}

### Generieren von Inhalt {#generate-content}

Erfahren Sie, wie Sie klare Prompts erstellen, Einstellungen optimieren und maßgeschneiderte Texte mit dem KI-Assistenten generieren können, um sicherzustellen, dass Ihr Messaging mit Ihren Marken- und Kommunikationszielen übereinstimmt.

1. Wählen Sie Ihre **[!UICONTROL Marke]** aus, um sicherzustellen, dass die von KI generierten Inhalte mit Ihren Markenspezifikationen übereinstimmen. [Weitere Informationen](brands.md) zu Marken.

1. Passen Sie den Inhalt an, indem Sie im Feld **[!UICONTROL Prompt]** beschreiben, was Sie generieren möchten.

   Wenn Sie Hilfe bei der Erstellung Ihres Prompts benötigen, finden Sie in der **[!UICONTROL Prompt-Bibliothek]** eine Vielzahl von Ideen für Prompts, mit denen Sie Ihre Sendungen verbessern können. [Weitere Informationen zu Best Practices für Prompts](ai-assistant-prompting-guide.md)

   ![Screenshot mit der Prompt-Bibliothek in Adobe Campaign Web](assets/text-genai-2.png){zoomable="yes"}

1. Passen Sie Ihren Prompt mit der Option **[!UICONTROL Texteinstellungen]** an:

   * **[!UICONTROL Kommunikationsstrategie]**: Wählen Sie den am besten geeigneten Kommunikationsstil für den generierten Text aus.
   * **[!UICONTROL Sprachen]**: Wählen Sie die Sprache Ihrer generierten Inhalte aus.
   * **[!UICONTROL Ton]**: Stellen Sie sicher, dass der Ton Ihrer E-Mail bei Ihrer Zielgruppe ankommt. Je nachdem, ob Sie informativ, humorvoll oder überzeugend klingen möchten, passt der KI-Assistent die Nachricht entsprechend an.
   * **Textlänge**: Wählen Sie mit dem Regler die gewünschte Textlänge aus.

     ![Screenshot mit Optionen für Texteinstellungen in Adobe Campaign Web](assets/text-genai-4.png){zoomable="yes"}

1. Klicken Sie im Menü **[!UICONTROL Referenzinhalt]** auf **[!UICONTROL Datei hochladen]**, um beliebige Marken-Assets mit Inhalten hinzuzufügen, die zusätzlichen Kontext für den KI-Assistenten liefern können. Alternativ können Sie ein zuvor hochgeladenes Asset auswählen.

   Zuvor hochgeladene Dateien sind in der Dropdown-Liste **[!UICONTROL Hochgeladener Referenzinhalt]** verfügbar. Aktivieren Sie einfach die Assets, die in den Generierungsprozess einbezogen werden sollen.

1. Wenn der Prompt fertig ist, klicken Sie auf **[!UICONTROL Generieren]**.

### Verfeinern und Fertigstellen {#refine-finalize}

Erfahren Sie, wie Sie den generierten Text überprüfen, Anpassungen vornehmen und Personalisierung anwenden können, um Ihre Inhalte fertigzustellen sowie hochwertige und ansprechende Nachrichten zu erstellen, die versandbereit sind.

1. Sehen Sie sich die generierten **[!UICONTROL Varianten]** an.

1. Klicken Sie auf das Prozentsymbol, um den **[!UICONTROL Markenausrichtungswert]** anzuzeigen und Abweichungen von Ihrer Marke zu ermitteln.

   Weitere Informationen finden Sie unter [Markenausrichtungswert](brands-score.md).

   ![](assets/text-genai-6.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Vorschau]**, um eine Vollbildversion der ausgewählten Variante anzuzeigen, oder auf **[!UICONTROL Anwenden]**, um Ihren aktuellen Inhalt zu ersetzen.

1. Navigieren Sie im Fenster **[!UICONTROL Vorschau]** zur Option **[!UICONTROL Verfeinern]**, um auf zusätzliche Anpassungsfunktionen zuzugreifen:

   * **[!UICONTROL Als Referenzinhalt verwenden]**: Die gewählte Variante dient hierbei als Referenzinhalt für die Generierung anderer Ergebnisse.
   * **[!UICONTROL Ausführlich]**: Gehen Sie genauer auf bestimmte Themen ein und liefern Sie zusätzliche Details, um das Verständnis und die Interaktion zu verbessern.
   * **[!UICONTROL Zusammenfassen]**: Fassen Sie die wichtigsten Punkte in klaren, prägnanten Aussagen zusammen, die die Aufmerksamkeit der Leserinnen und Leser wecken und sie zum Weiterlesen animieren.
   * **[!UICONTROL Neu formulieren]**: Formulieren Sie Ihre Nachricht auf verschiedene Arten um, sodass Ihr Text frisch und für verschiedene Zielgruppen ansprechend bleibt.
   * **[!UICONTROL Einfachere Sprache verwenden]**: Vereinfachen Sie Ihren Text, damit er für eine breitere Zielgruppe verständlich und zugänglich ist.
   * **[!UICONTROL Übersetzen]**: Vereinfachen Sie Ihren Text, damit er für eine breitere Zielgruppe verständlich und zugänglich ist.

   Sie können auch den **[!UICONTROL Ton]** und die **[!UICONTROL Kommunikationsstrategie]** Ihres Textes ändern.

   ![Screenshot mit Verfeinerungsoptionen in Adobe Campaign Web](assets/text-genai-5.png){zoomable="yes"}

1. Öffnen Sie die Registerkarte **[!UICONTROL Markenausrichtung]**, um die Übereinstimmung Ihres Inhalts mit den [Markenrichtlinien](../content/brands.md) anzuzeigen.

1. Klicken Sie auf **[!UICONTROL Auswählen]**, sobald Sie den passenden Inhalt gefunden haben.

1. Fügen Sie Personalisierungsfelder ein, um Ihre Inhalte auf der Grundlage von Profildaten anzupassen. Klicken Sie danach auf die Schaltfläche **[!UICONTROL Inhalte simulieren]**, um das Rendern zu steuern, und überprüfen Sie die Personalisierungseinstellungen mit Testprofilen. [Weitere Informationen](../preview-test/preview-content.md)

1. Überprüfen und aktivieren Sie Ihren Inhalt:
   * **E-Mail**: Wenn Sie Inhalt, Zielgruppe und Zeitplan definiert haben, können Sie den E-Mail-Versand vorbereiten. [Weitere Informationen](../monitor/prepare-send.md)
   * **Landingpage**: Sobald Ihre Landingpage fertig ist, können Sie sie veröffentlichen, um sie für die Verwendung in einer Nachricht verfügbar zu machen. [Weitere Informationen](../landing-pages/create-lp.md)

## Für Mobile-Kanäle {#mobile-channels}

Der KI-Assistent kann überzeugende Textinhalte für Ihre Push-Benachrichtigungen und SMS-Nachrichten generieren und Ihnen dabei helfen, ansprechende Mobile-Kommunikation zu erstellen, die über alle Mobile-Touchpoints hinweg bei Ihrer Zielgruppe Anklang findet.

### Zugreifen und Konfigurieren {#mobile-access-configure}

Bevor Sie mit dem Generieren von Text mit dem KI-Assistenten für Mobile-Kanäle beginnen, müssen Sie Ihren Versand einrichten und auf den KI-Assistenten zugreifen.

1. Erstellen Sie einen Mobile-Versand und konfigurieren Sie ihn:
   * **Push-Benachrichtigungen**: Nachdem Sie Ihren Push-Benachrichtigungsversand erstellt und konfiguriert haben, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../push/create-push.md)
   * **SMS**: Nachdem Sie Ihren SMS-Versand erstellt und konfiguriert haben, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../sms/create-sms.md)

1. Personalisieren Sie Ihre Nachricht nach Bedarf:
   * **Push-Benachrichtigungen**: [Weitere Informationen](../push/content-push.md)
   * **SMS**: [Weitere Informationen](../sms/content-sms.md)

1. Rufen Sie das Menü **[!UICONTROL KI-Assistenten anzeigen]** auf.

   ![Screenshot mit dem Menü „KI-Assistenten anzeigen“](assets/sms-genai-1.png){zoomable="yes"}

### Generieren von Inhalt {#mobile-generate-content}

Nachdem Sie auf den KI-Assistenten zugegriffen haben, können Sie die Generierungseinstellungen so konfigurieren, dass Mobile-Inhalte erstellt werden, die Ihren Marken- und Versandzielen entsprechen. Passen Sie Textparameter an, fügen Sie Marken-Assets hinzu und geben Sie Prompts ein, um die KI beim Generieren relevanter Varianten zu unterstützen.

1. Wählen Sie Ihre **[!UICONTROL Marke]** aus, um sicherzustellen, dass die von KI generierten Inhalte mit Ihren Markenspezifikationen übereinstimmen. [Weitere Informationen](brands.md) zu Marken.

1. Passen Sie den Inhalt an, indem Sie im Feld **[!UICONTROL Prompt]** beschreiben, was Sie generieren möchten.

   Wenn Sie Hilfe bei der Erstellung Ihres Prompts benötigen, finden Sie in der **[!UICONTROL Prompt-Bibliothek]** eine Vielzahl von Ideen für Prompts, mit denen Sie Ihren Versand verbessern können. [Weitere Informationen zu Best Practices für Prompts](ai-assistant-prompting-guide.md)

   ![KI-Assistent mit Feld „Prompt“ und Optionen](assets/sms-genai-2.png){zoomable="yes"}

1. **Wählen Sie für Push-Benachrichtigungen** das zu generierende Textfeld aus: **[!UICONTROL Titel]**, **[!UICONTROL Untertitel]** und/oder **[!UICONTROL Nachricht]**.

1. Passen Sie Ihr Prompt mit der Option **[!UICONTROL Texteinstellungen]** an:

   * **[!UICONTROL Kommunikationsstrategie]**: Wählen Sie den am besten geeigneten Kommunikationsstil für den generierten Text aus.
   * **[!UICONTROL Sprachen]**: Wählen Sie die Sprache Ihrer generierten Inhalte aus.
   * **[!UICONTROL Ton]**: Der Ton sollte bei Ihrer Zielgruppe Anklang finden. Je nachdem, ob Sie informativ, humorvoll oder überzeugend klingen möchten, kann der KI-Assistent die Nachricht entsprechend anpassen.
   * **[!UICONTROL Länge]**: Legen Sie die Länge Ihres Inhalts mit dem Schieberegler fest.

     ![Panel „Texteinstellungen“](assets/sms-genai-3.png){zoomable="yes"}

1. Klicken Sie im Menü **[!UICONTROL Referenzinhalt]** auf **[!UICONTROL Datei hochladen]**, um beliebige Marken-Assets mit Inhalten hinzuzufügen, die zusätzlichen Kontext für den KI-Assistenten liefern können. Alternativ können Sie ein zuvor hochgeladenes Asset auswählen.

   Zuvor hochgeladene Dateien sind in der Dropdown-Liste **[!UICONTROL Hochgeladener Referenzinhalt]** verfügbar. Aktivieren Sie einfach die Assets, die in den Generierungsprozess einbezogen werden sollen.

1. Wenn der Prompt fertig ist, klicken Sie auf **[!UICONTROL Generieren]**.

### Verfeinern und Fertigstellen {#mobile-refine-finalize}

Nachdem Sie Textvarianten für Ihre Mobile-Nachrichten generiert haben, können Sie die Ergebnisse anpassen, um sicherzustellen, dass sie genau Ihren Anforderungen entsprechen. Überprüfen Sie die Markenausrichtung, passen Sie den Ton und die Sprache an und bereiten Sie den Inhalt für die Aktivierung vor.

1. Sehen Sie sich nach der Generierung die **[!UICONTROL Varianten]** an.

1. Klicken Sie auf das Prozentsymbol, um den **[!UICONTROL Markenausrichtungswert]** anzuzeigen und Abweichungen von Ihrer Marke zu ermitteln.

   Weitere Informationen finden Sie unter [Markenausrichtungswert](brands-score.md).

   ![Menü „Verfeinern“](assets/sms-genai-4.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Vorschau]**, um eine Vollbildversion der ausgewählten Variante anzuzeigen, oder auf **[!UICONTROL Anwenden]**, um Ihren aktuellen Inhalt zu ersetzen.

1. Navigieren Sie zur Option **[!UICONTROL Verfeinern]** im Fenster **[!UICONTROL Vorschau]**, um auf zusätzliche Anpassungsfunktionen zuzugreifen:

   * **[!UICONTROL Als Referenzinhalt verwenden]**: Die gewählte Variante dient hierbei als Referenzinhalt für die Generierung anderer Ergebnisse.

   * **[!UICONTROL Neu formulieren]**: Schreiben Sie die Nachricht um und behalten Sie dabei seine Bedeutung bei. Mit dieser Option können Sie alternative Formulierungen generieren, den Lesefluss verbessern oder die Ausdrucksweise anpassen, ohne die Kernbotschaft zu ändern.

   * **[!UICONTROL Einfachere Sprache verwenden]**: Nutzen Sie den KI-Assistenten, um Ihren Text zu vereinfachen, damit er für eine breitere Zielgruppe verständlich und zugänglich ist.

   * **[!UICONTROL Übersetzen]**: Vereinfachen Sie Ihren Text, damit er für eine breitere Zielgruppe verständlich und zugänglich ist.

   * **[!UICONTROL Ton ändern]**: Passen Sie den Ton der Nachricht an Ihren Kommunikationsstil an, d. h. lassen Sie sie freundlicher, professioneller, dringender oder inspirierender klingen.

   * **[!UICONTROL Kommunikationsstrategie ändern]**: Ändern Sie den Messaging-Ansatz basierend auf Ihren Zielen, beispielsweise um Dringlichkeit zu erzeugen oder aufregende Anreize zu betonen.

     ![Generierte Textvarianten mit Markenausrichtungswert](assets/sms-genai-5.png){zoomable="yes"}

1. Öffnen Sie die Registerkarte **[!UICONTROL Markenausrichtung]**, um die Übereinstimmung Ihres Inhalts mit den [Markenrichtlinien](brands.md) zu prüfen.

1. Klicken Sie auf **[!UICONTROL Auswählen]**, sobald Sie den passenden Inhalt gefunden haben.

1. Fügen Sie Personalisierungsfelder ein, um Ihre Inhalte auf der Grundlage von Profildaten anzupassen. Klicken Sie danach auf die Schaltfläche **[!UICONTROL Inhalte simulieren]**, um das Rendern zu steuern, und überprüfen Sie die Personalisierungseinstellungen mit Testprofilen. [Weitere Informationen](../personalization/personalize.md)

1. Überprüfen und aktivieren Sie Ihren Inhalt:
   * **Push-Benachrichtigung**: Wenn Sie Inhalt, Zielgruppe und Zeitplan definiert haben, können Sie den Push-Benachrichtigungsversand vorbereiten. [Weitere Informationen](../push/send-push.md)
   * **SMS**: Sobald Ihre SMS fertig ist, können Sie sie veröffentlichen, um sie für die Verwendung in einer Nachricht verfügbar zu machen. [Weitere Informationen](../sms/send-sms.md)
