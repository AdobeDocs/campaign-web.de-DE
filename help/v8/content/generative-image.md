---
audience: end-user
title: Generative Inhalte
description: Erfahren Sie, wie Sie mit dem KI-Assistenten Bilder generieren
source-git-commit: c51877d1926e1a8a6766ea1a5aa00f826071a3fc
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 45%

---

# Erstellen von Bildern mit dem KI-Assistenten {#generative-image}

>[!IMPORTANT]
>
>Bevor Sie mit der Verwendung dieser Funktion beginnen, lesen Sie die entsprechenden Informationen unter [Schutzmechanismen und Einschränkungen](generative-gs.md#generative-guardrails).
></br>
>
>Sie müssen einer [Benutzervereinbarung](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} zustimmen, bevor Sie den KI-Assistenten in Adobe Campaign Web verwenden können. Weitere Informationen erhalten Sie beim Adobe-Support.

Verwenden Sie den KI-Assistenten in Adobe Campaign Web, um ansprechende visuelle Inhalte zu erstellen, die Ihre Nachrichten für E-Mails, Landingpages und Push-Benachrichtigungen optimieren. Der KI-Assistent hilft Ihnen, Bilder zu generieren und zu optimieren, um sicherzustellen, dass Ihr Inhalt visuell ansprechend und auf Ihre Marke abgestimmt ist.

## Für E-Mail und Landingpages {#email-web-channels}

Der KI-Assistent kann vollständige visuelle Erlebnisse für Ihre E-Mail-Sendungen und Landingpages generieren. Mit dieser Funktion können Sie markeninterne, aufmerksamkeitsstarke Bilder erstellen, die über digitale Touchpoints hinweg bei Ihrer Zielgruppe Anklang finden.

### Zugreifen auf und Konfigurieren {#access-configure}

Um mit dem Generieren von Bildern mit dem KI-Assistenten zu beginnen, richten Sie zunächst Ihren Versand ein und öffnen Sie den Inhaltseditor. Gehen Sie wie folgt vor, um Ihren Arbeitsbereich vorzubereiten und auf das Bedienfeld KI-Assistent zuzugreifen.

1. Versand erstellen und konfigurieren:

   * **E-**: Nachdem Sie den E-Mail-Versand erstellt und konfiguriert haben, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../email/create-email-content.md)
   * **Landingpage**: Klicken Sie nach der Erstellung und Konfiguration Ihrer Landingpage auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../landing-pages/create-lp.md)

1. Wählen Sie das Asset aus, das Sie mit dem KI-Assistenten ändern möchten, und rufen Sie das Menü **[!UICONTROL KI-Assistent]** auf.

   ![Screenshot mit Auswahl der Textkomponente in Adobe Campaign Web](assets/image-genai-1.png){zoomable="yes"}

### Inhalt erzeugen {#generate-content}

Erfahren Sie, wie Sie mit dem KI-Assistenten effektive Eingabeaufforderungen erstellen und Bildeinstellungen konfigurieren können, um visuell überzeugende Bilder zu generieren. Passen Sie Parameter wie Seitenverhältnis, visuelle Intensität und Beleuchtung an, um Bilder zu erstellen, die Ihren Marken- und Kampagnenzielen entsprechen.

1. Aktivieren Sie für den KI-Assistenten die Option **[!UICONTROL Referenzstil]**, um neue Inhalte basierend auf dem ausgewählten Inhalt zu personalisieren.

1. Wählen Sie Ihre **[!UICONTROL Marke]** aus, um sicherzustellen, dass die von KI generierten Inhalte mit Ihren Markenspezifikationen übereinstimmen. [Weitere Informationen](brands.md) zu Marken.

1. Passen Sie den Inhalt an, indem Sie im Feld **[!UICONTROL Prompt]** beschreiben, was Sie generieren möchten.

   Wenn Sie Hilfe bei der Erstellung Ihrer Eingabeaufforderung benötigen, rufen Sie die **[!UICONTROL Eingabeaufforderungsbibliothek]** auf, die eine Vielzahl von Ideen für die Eingabeaufforderung bereitstellt, um Ihre Sendungen zu verbessern. [Erfahren Sie mehr über Best Practices zur Eingabeaufforderung](ai-assistant-prompting-guide.md)

   ![Screenshot mit der Prompt-Bibliothek für die Bildgenerierung in Adobe Campaign Web](assets/image-genai-2.png){zoomable="yes"}

1. Passen Sie Ihren Prompt mit der Option **[!UICONTROL Texteinstellungen]** an:

   * **[!UICONTROL Seitenverhältnis]**: Bestimmen Sie die Breite und Höhe des Assets. Wählen Sie aus gängigen Verhältnissen wie 16:9, 4:3, 3:2 oder 1:1 oder geben Sie eine benutzerdefinierte Größe ein.
   * **[!UICONTROL Inhaltstyp]**: Kategorisieren Sie die Art des visuellen Elements, wobei zwischen verschiedenen Arten der visuellen Darstellung wie Fotos, Grafiken oder Kunst unterschieden wird.
   * **[!UICONTROL Visuelle Intensität]**: Steuern Sie die Wirkung des Bildes durch Anpassen seiner Intensität. Durch eine niedrigere Einstellung (2) wird das Erscheinungsbild weicher, während eine höhere Einstellung (10) das Bild lebendiger macht.
   * **[!UICONTROL Farbe und Ton]**: Passen Sie die Gesamterscheinung der Farben und die vermittelte Stimmung oder Atmosphäre an.
   * **[!UICONTROL Beleuchtung]**: Ändern Sie die Beleuchtung in einem Bild, um dessen Atmosphäre zu prägen und bestimmte Elemente hervorzuheben.
   * **[!UICONTROL Komposition]**: Ordnen Sie Elemente innerhalb des Rahmens eines Bildes an.

     ![Screenshot mit Optionen für Bildeinstellungen in Adobe Campaign Web](assets/image-genai-4.png){zoomable="yes"}

1. Klicken Sie im Menü **[!UICONTROL Referenzinhalt]** auf **[!UICONTROL Datei hochladen]**, um jedes Marken-Asset hinzuzufügen, das Inhalte enthält, die zusätzlichen Kontext-KI-Assistenten bereitstellen können oder ein zuvor hochgeladenes Asset auswählen.

   Zuvor hochgeladene Dateien sind in der Dropdown **[!UICONTROL Liste „Hochgeladener]**&quot; verfügbar. Aktivieren Sie einfach die Assets, die in den Generierungsprozess einbezogen werden sollen.

1. Sobald Sie mit der Konfiguration des Prompts zufrieden sind, klicken Sie auf **[!UICONTROL Generieren]**.

### Verfeinern und abschließen {#refine-finalize}

Nachdem Sie Bildvarianten erstellt haben, können Sie die Ergebnisse überprüfen, die Markenausrichtung überprüfen und die beste Option für Ihren Inhalt auswählen.

1. Durchsuchen Sie die generierte **[!UICONTROL Varianten]**.

1. Klicken Sie auf das Prozentsymbol, um den **[!UICONTROL Markenausrichtungswert]** anzuzeigen und Abweichungen von Ihrer Marke zu ermitteln.

   Weitere Informationen finden Sie unter [Markenausrichtungswert](../content/brands-score.md).

   ![](assets/image-genai-3.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Vorschau]**, um eine Vollbildversion der ausgewählten Variante anzuzeigen, oder auf **[!UICONTROL Anwenden]**, um Ihren aktuellen Inhalt zu ersetzen.

1. Wählen Sie **[!UICONTROL Ähnliche generieren]** aus, wenn Sie dieser Variante ähnliche Bilder anzeigen möchten.

1. Öffnen Sie die Registerkarte **[!UICONTROL Markenausrichtung]**, um die Übereinstimmung Ihres Inhalts mit den [Markenrichtlinien](../content/brands.md) anzuzeigen.

1. Klicken Sie auf **[!UICONTROL Auswählen]**, sobald Sie den passenden Inhalt gefunden haben.

1. Klicken Sie nach der Definition des Nachrichteninhalts auf die Schaltfläche **[!UICONTROL Inhalte simulieren]**, um das Rendern zu steuern, und überprüfen Sie die Personalisierungseinstellungen mit Testprofilen. [Weitere Informationen](../preview-test/preview-content.md)

1. Überprüfen und Aktivieren Ihres Inhalts:
   * **E-**: Wenn Sie Inhalt, Zielgruppe und Zeitplan definiert haben, können Sie den E-Mail-Versand vorbereiten. [Weitere Informationen](../monitor/prepare-send.md)
   * **Landingpage**: Sobald Ihre Landingpage fertig ist, können Sie sie veröffentlichen, um sie für die Verwendung in einer Nachricht verfügbar zu machen. [Weitere Informationen](../landing-pages/create-lp.md)

## Für mobile Kanäle {#mobile-channels}

Der KI-Assistent ermöglicht es Ihnen, ansprechende Bilder für Push-Benachrichtigungen zu generieren, sodass Sie visuell ansprechende Mobilkommunikation erstellen können, die die Aufmerksamkeit Ihrer Zielgruppe auf sich zieht und sie anspricht.

### Zugreifen auf und Konfigurieren {#mobile-access-configure}

Um mit dem Generieren von Bildern für Push-Benachrichtigungen mit dem KI-Assistenten zu beginnen, richten Sie zunächst Ihren Versand ein und öffnen Sie den KI-Assistenten.

1. Nachdem Sie Ihren Push-Benachrichtigungs-Versand erstellt und konfiguriert haben, klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../push/create-push.md)

1. Rufen Sie das Menü **[!UICONTROL KI-Assistenten anzeigen]** auf.

   ![Screenshot mit dem Menü „KI-Assistenten anzeigen“](assets/push-img-1.png){zoomable="yes"}

### Inhalt erzeugen {#mobile-generate-content}

Nach dem Zugriff auf den KI-Assistenten können Sie die Generierungseinstellungen anpassen, um Bilder zu erstellen, die Ihrer Marke entsprechen und Ihre Push-Benachrichtigungsziele unterstützen. Konfigurieren Sie die Eingabeaufforderung und Bildparameter, um für mobile Displays optimierte Visualisierungen zu generieren.

1. Wählen Sie Ihre **[!UICONTROL Marke]** aus, um sicherzustellen, dass die von KI generierten Inhalte mit Ihren Markenspezifikationen übereinstimmen. [Weitere Informationen](brands.md) zu Marken.

1. Passen Sie den Inhalt an, indem Sie im Feld **[!UICONTROL Prompt]** beschreiben, was Sie generieren möchten.

   Wenn Sie Hilfe bei der Erstellung Ihrer Eingabeaufforderung benötigen, rufen Sie die **[!UICONTROL Eingabeaufforderungsbibliothek“ auf]** die eine Vielzahl von Ideen für die Eingabeaufforderung zur Verbesserung Ihrer Kampagnen bietet. [Erfahren Sie mehr über Best Practices zur Eingabeaufforderung](ai-assistant-prompting-guide.md)

   ![KI-Assistent mit Eingabeaufforderungsfeld und Optionen](assets/push-img-2.png){zoomable="yes"}

1. Wählen Sie **[!UICONTROL Bild]** aus, um nur Assets zu generieren.

1. Wählen Sie Ihre **[!UICONTROL Bildeinstellungen]** aus:

   * **[!UICONTROL Inhaltstyp]**: Kategorisieren Sie die Art des visuellen Elements, wobei zwischen verschiedenen Arten der visuellen Darstellung wie Fotos, Grafiken oder Kunst unterschieden wird.
   * **[!UICONTROL Visuelle Intensität]**: Steuern Sie die Wirkung des Bildes durch Anpassen seiner Intensität. Durch eine niedrigere Einstellung (2) wird das Erscheinungsbild weicher, während eine höhere Einstellung (10) das Bild lebendiger und visuell eindringlicher macht.
   * **[!UICONTROL Beleuchtung]**: Passen Sie die Beleuchtung in einem Bild, die dessen Atmosphäre prägt und bestimmte Elemente hervorhebt.
   * **[!UICONTROL Komposition]**: Ordnen Sie Elemente innerhalb des Rahmens eines Bildes an.

     ![Screenshot mit Optionen für Bildeinstellungen](assets/push-img-3.png){zoomable="yes"}

1. Klicken Sie im Menü **[!UICONTROL Referenzinhalt]** auf **[!UICONTROL Datei hochladen]**, um jedes Marken-Asset hinzuzufügen, das Inhalte enthält, die zusätzlichen Kontext-KI-Assistenten bereitstellen können oder ein zuvor hochgeladenes Asset auswählen.

   Zuvor hochgeladene Dateien sind in der Dropdown **[!UICONTROL Liste „Hochgeladener]**&quot; verfügbar. Aktivieren Sie einfach die Assets, die in den Generierungsprozess einbezogen werden sollen.

1. Wenn der Prompt fertig ist, klicken Sie auf **[!UICONTROL Generieren]**.

### Verfeinern und abschließen {#mobile-refine-finalize}

Nachdem Sie Bildvarianten für Ihre Mobile-Nachrichten generiert haben, können Sie die Ergebnisse optimieren, um sicherzustellen, dass sie Ihren genauen Anforderungen entsprechen.

1. Navigieren Sie nach der Generierung durch **[!UICONTROL Varianten]**.

1. Klicken Sie auf das Prozentsymbol, um den **[!UICONTROL Markenausrichtungswert]** anzuzeigen und Abweichungen von Ihrer Marke zu ermitteln.

   Weitere Informationen finden Sie unter [Markenausrichtungswert](../content/brands-score.md).

   ![](assets/push-img-4.png){zoomable="yes"}

1. Klicken Sie **[!UICONTROL Vorschau]**, um die **[!UICONTROL Varianten]** zu durchsuchen.

1. Öffnen Sie die Registerkarte **[!UICONTROL Markenausrichtung]**, um die Übereinstimmung Ihres Inhalts mit den [Markenrichtlinien](brands.md) zu prüfen.

1. Klicken Sie auf **[!UICONTROL Auswählen]**, sobald Sie den passenden Inhalt gefunden haben.

Nachdem Sie Inhalt, Zielgruppe und Zeitplan definiert haben, bereiten Sie den Push-Versand vor. [Weitere Informationen](../monitor/prepare-send.md)
