---
audience: end-user
title: Verbessertes E-Mail-Authoring-Erlebnis
description: Erfahren Sie, wie Sie die E-Mail-Erstellung mit wiederverwendbaren Themen und Modulen optimieren können, um die Konsistenz und Effizienz des Designs Ihrer Kampagnen sicherzustellen.
badge: label="Eingeschränkte Verfügbarkeit" type="Informative"
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: E-Mail-Themen, Module, Wiederverwendbarkeit, Markenkonsistenz, E-Mail-Design, benutzerdefiniertes CSS, Optimierung für Mobilgeräte
exl-id: c9e02bca-032d-4771-ad53-5bbebabc4c5d
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '2077'
ht-degree: 100%

---

# Anwenden von Designs auf Ihren E-Mail-Inhalt {#apply-email-themes}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Designs im E-Mail-Designer (LA)"
>abstract="Wenden Sie wiederverwendbare Design-Stile und -Variablen an, um den E-Mail-Inhalt mit Ihrer Marke konsistent zu halten. Diese Funktion ist nur für eine ausgewählte Gruppe von Organisationen verfügbar (eingeschränkte Verfügbarkeit)."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_email_apply_theme"
>title="Anwenden eines Designs auf Ihre E-Mail"
>abstract="Wählen Sie ein Design für Ihre E-Mail aus, um schnell einen bestimmten Stil anzuwenden, der zu Ihrer Marke und Ihrem Design passt."

>[!AVAILABILITY]
>
>Diese Funktion ist eingeschränkt verfügbar. Wenden Sie sich an den Adobe-Support, um Zugang zu erhalten.

Mit Themen können technisch nicht versierte Benutzende wiederverwendbare Inhalte erstellen, die zu einer bestimmten Marke und Design-Sprache passen, indem sie zusätzlich zu den Standardvorlagen benutzerdefinierte Stile hinzufügen<!-- to achieve brand specific results-->.

Diese Funktion ermöglicht es Marketing-Fachleuten, visuell ansprechende, markenkonforme E-Mails schneller und mit weniger Aufwand zu erstellen und gleichzeitig erweiterte Anpassungsoptionen für individuelle Design-Anforderungen bereitzustellen.

## Schutzmechanismen und Einschränkungen {#themes-guardrails}

* Wenn Sie eine E-Mail von Grund auf neu erstellen, können Sie mit der Erstellung Ihres Inhalts beginnen, indem Sie über ein Thema schnell einen bestimmten Stil anwenden, der zu Ihrer Marke und Ihrer Gestaltung passt.

  Wenn Sie den Modus „Manuelle Formatierung“ auswählen, können Sie keine Themen anwenden, es sei denn, Sie setzen Ihre E-Mail zurück.

* [Fragmente](../content/fragments.md) sind nicht zwischen dem Modus „Themen verwenden“ und „Manuelle Formatierung“ kompatibel.

   * Themenfragmente sind nicht in E-Mail-Inhalten verfügbar, die ohne die Verwendung von Themen erstellt wurden.

   * Damit ein [Fragment](../content/fragments.md) in einem Themeninhalt genutzt werden kann, muss dieses Fragment selbst mithilfe von Themen erstellt worden sein. [Weitere Informationen](#leverage-themes-fragment)

   * Wenn Sie ein Fragment im E-Mail-Inhalt verwenden, stellen Sie sicher, dass Sie ein für dieses Fragment definiertes Thema anwenden. Andernfalls kann es zu Anzeigeproblemen kommen, insbesondere in Outlook 2021 und früheren Versionen. [Weitere Informationen](#leverage-themes-fragment)

* Wenn Sie einen in HTML erstellten Inhalt verwenden, befinden Sie sich im [Kompatibilitätsmodus](existing-content.md). Sie können keine Themen direkt auf diesen Inhalt anwenden.

   * Um Themen anzuwenden, müssen Sie zunächst den importierten Inhalt [als neue Vorlage](../content/create-email-templates.md#save-as-template) speichern und diese Vorlage dann in einen themenkompatiblen Inhalt konvertieren. Anschließend können Sie diese Vorlage verwenden, um E-Mail-Inhalte zu erstellen. In [diesem Abschnitt](#theme-convertor) erfahren Sie, wie Sie eine mit manueller Formatierung erstellte Vorlage konvertieren.

   * Sie können auch weiterhin Ihre importierten HTML-Inhalte konvertieren. [Weitere Informationen](existing-content.md)

  <!--To fully leverage all the capabilities of the Email Designer, including themes, you must either create a new content in Use Themes mode, or convert your imported HTML content. [Learn more](existing-content.md)-->

* Wenn Sie benutzerdefinierte Web-Schriftarten (einschließlich Google-Schriftarten) in Ihren Themen verwenden, beachten Sie, dass viele E-Mail-Clients diese nicht unterstützen. Definieren Sie immer geeignete Ersatzschriftarten in Ihrem Thema, um die Lesbarkeit für alle E-Mail-Clients sicherzustellen.

   * Gmail und Yahoo! laden keine externen Web-Schriftarten und greifen auf die Systemschriftarten zurück, unabhängig von der in Ihrem HTML/CSS angegebenen Schriftfamilie.
   * Die einzigen von Gmail unterstützten Google-Schriftarten sind Roboto und Google Sans.
   * Zu den E-Mail-Clients, die Web-Schriftarten *unterstützen*, gehören unter anderem Apple Mail, iOS Mail, Android Mail, Thunderbird und Outlook für macOS.

<!--If you apply a theme to a content using a [fragment](../content/fragments.md) created with Manual Styling mode, the rendering may not be optimal.-->

## Design erstellen {#create-and-edit-themes}

Gehen Sie wie folgt vor, um ein Thema zu definieren, das Sie in künftigen E-Mail-Inhalten nutzen können.

1. Erstellen Sie zu Beginn eine neue [Inhaltsvorlage](../content/create-email-templates.md).

1. Wählen Sie die Option **[!UICONTROL Designs erstellen oder bearbeiten]** aus.

   ![Inhaltsvorlagen-Editor, der die Option „Designs erstellen oder bearbeiten“ anzeigt](assets/theme-create.png)

1. Wählen Sie ein Adobe-Thema aus. Wählen Sie in diesem Beispiel das **[!UICONTROL Standardthema]** aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![Themenauswahl mit ausgewähltem Standardthema und Schaltfläche „Erstellen“](assets/theme-select.png)

1. Sie können auch eine benutzerdefinierte Vorlage auf der Registerkarte **[!UICONTROL Meine Themen]** auswählen und auf **[!UICONTROL Bearbeiten]** klicken, um sie zu aktualisieren.

   ![Registerkarte „Meine Themen“ mit Liste benutzerdefinierter Themen und hervorgehobener Option „Bearbeiten“](assets/theme-edit.png)

1. Beginnen Sie auf der Registerkarte **[!UICONTROL Allgemeine Einstellungen]** mit der Definition Ihres Themas, indem Sie ihm einen bestimmten Namen geben, der zu Ihrer Marke passt. Sie können die standardmäßige Darstellungsfeldbreite für Ihre E-Mails anpassen<!--and also export the current theme for reuse-->.

   <!--![General settings tab for theme name, viewport width, and export](assets/theme-general-settings.png)-->

1. Verwenden Sie die Leiste rechts, um durch die verschiedenen Registerkarten zu navigieren und Ihre Design-Einstellungen zu aktualisieren.

   ![Rechte Leiste des Themen-Editors mit Registerkarten für Farben, Text, Abstand und anderen Design-Einstellungen](assets/theme-right-pane.png)

1. Auf der Registerkarte **[!UICONTROL Farben]**:

   * Verwenden Sie die Schaltfläche **[!UICONTROL Bearbeiten]**, um eine **[!UICONTROL Farbpalette]** mit Standardfarben für Ihre Marke einzurichten. Wählen Sie **[!UICONTROL Voreinstellung]** aus, um schnell ein Farbschema zu erstellen oder jede Farbe Ihres Themas individuell anzupassen. Sie können auch eine Kombination aus beiden verwenden.

     ![Animation der Bearbeitung der Themen-Farbpalette mit Voreinstellungen und benutzerdefinierten Farben](assets/theme-colors.gif)

   * Klicken Sie auf **[!UICONTROL Variante hinzufügen]**, um mehrere Farbvarianten zu erstellen, z. B. den Hell- und Dunkelmodus, wobei jede Variante Ihres Themas über eine eigene Farbpalette und Nuancensteuerelemente verfügt.

     ![Farbvarianten im Themen-Editor mit „Variante hinzufügen“ für zusätzliche Paletten](assets/theme-colors-variant.png)

   * Klicken Sie für jede Variante auf das Symbol **[!UICONTROL Bearbeiten]**, um ein einzelnes Element zu bearbeiten. Sie können die von Ihnen erstellte Standardpalette oder beliebige benutzerdefinierte Farben verwenden.

     ![Animation der Bearbeitung einzelner Farben innerhalb einer Themen-Farbvariante](assets/theme-colors-edit-variant.gif)

1. In den **[!UICONTROL Texteinstellungen]** können Sie die globale Schriftart festlegen, die Sie für Ihr gesamtes Themen verwenden möchten. Wenn Sie eine detaillierte Steuerung wünschen, können Sie auch jeden Überschrift- und Absatztyp bearbeiten und Schriftart, -größe, -stil usw. anpassen.

   ![Registerkarte „Texteinstellungen“ für globale Schriftarten und Überschrift- oder Absatzstile in einem Thema](assets/theme-text.png)

   >[!NOTE]
   >
   >Beachten Sie bei der Auswahl benutzerdefinierter Web-Schriftarten, dass viele E-Mail-Clients wie Gmail und Yahoo! externe Web-Schriftarten nicht unterstützen, sondern auf Systemschriftarten zurückgreifen. Erwägen Sie die Verwendung von Ersatzschriftarten, um sicherzustellen, dass Ihr Inhalt in allen E-Mail-Clients korrekt angezeigt wird. [Weitere Informationen](#themes-guardrails)

1. Wählen Sie auf der Registerkarte **[!UICONTROL Abstand]** ein einzelnes Element aus der Liste aus, um den Abstand zwischen den verschiedenen Komponenten ordnungsgemäß festzulegen.

   <!--![Spacing tab listing structure elements to adjust spacing between components](assets/theme-spacing.png)-->

1. Mit den anderen Registerkarten auf der rechten Seite können Sie jedes Schaltflächenelement, jede Trennlinie, zusätzliche Bildformatierungen und den Raster-Layout-Abstand für dieses Thema separat verwalten.

   ![Steuerelemente für Schaltflächenstile in der rechten Leiste des Themen-Editors](assets/theme-buttons.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**, um dieses Thema für die zukünftige Verwendung zu speichern. Es wird jetzt auf der Registerkarte **[!UICONTROL Meine Themen]** angezeigt.

<!--A little strange upon hitting Save, because once the theme is created, you need to hit Close to go back to Design your template screen, then click Cancel if you don't want to proceed with template creation.-->

## Anwenden von Themen auf E-Mail-Inhalt {#apply-themes-email}

Gehen Sie wie folgt vor, um standardmäßige oder benutzerdefinierte Stilthemen auf eine Inhaltsvorlage oder eine E-Mail anzuwenden.

1. Erstellen Sie in [!DNL Adobe Campaign] [einen E-Mail-Versand](create-email.md) oder verwenden Sie einen vorhandenen Versand bzw. erstellen Sie eine E-Mail-[Inhaltsvorlage](../content/create-email-templates.md#create-template-from-scratch) und [bearbeiten Sie den E-Mail-Inhalt](get-started-email-designer.md#start-authoring).

1. Sie können eine der folgenden Aktionen auswählen:

   * Wählen Sie eine integrierte [E-Mail-Vorlage](../content/use-email-templates.md) aus, um den E-Mail-Designer zu öffnen. Ein für jede Vorlage spezifisches Standardthema wird automatisch angewendet.

   * Entwerfen Sie [neuen Inhalt von Grund auf](create-email-content.md) und wählen Sie **[!UICONTROL Themen verwenden]**, um mit einem vordefinierten Stilthema zu beginnen.

     ![E-Mail-Designer-Startbildschirm mit Option „Themen verwenden“ und „Manuelle Formatierung“](assets/theme-from-scratch.png)

     >[!CAUTION]
     >
     >Wenn Sie den Modus „Manuelle Formatierung“ auswählen, können Sie keine Themen anwenden, es sei denn, Sie setzen Ihr Design zurück.
     >
     >Damit ein [Fragment](../content/fragments.md) in einem Themeninhalt genutzt werden kann, muss dieses Fragment selbst mithilfe von Themen erstellt worden sein. [Weitere Informationen](#leverage-themes-fragment)

1. Wählen Sie im E-Mail-Designer in der rechten Leiste die Schaltfläche **[!UICONTROL Themen]** aus. Das Standardthema oder das Thema der Vorlage wird angezeigt. Sie können zwischen den beiden Farbvarianten für dieses Thema wechseln.

   ![E-Mail-Designer-Arbeitsfläche mit Panel „Themen“, das das aktive Thema und die Farbvarianten anzeigt](assets/theme-default-hero.png)

1. Klicken Sie auf den Pfeil neben dem aktuell verwendeten Thema. Die Liste der verfügbaren benutzerdefinierten Themen und Adobe-Themen wird angezeigt.

   ![Erweitertes Dropdown-Menü „Themen“, das Adobe-Themen und „Meine Themen“ anzeigt](assets/theme-hero-change.png)

1. Klicken Sie auf **[!UICONTROL Meine Themen]** und wählen Sie das von Ihnen erstellte Thema aus.

   ![Liste „Meine Themen“ mit einem benutzerseitig erstellten Thema, das in der Themen-Auswahl ausgewählt wurde](assets/theme-select-custom.png)

1. Klicken Sie auf eine Stelle außerhalb der Dropdown-Liste. Die Stile des ausgewählten benutzerdefinierten Themas werden automatisch auf alle E-Mail-Komponenten angewendet.Sie können zwischen den Farbvarianten wechseln, falls vorhanden.

1. Wenn ein Thema in einer Inhaltsvorlage ausgewählt ist, können Sie auf die Schaltfläche **[!UICONTROL Design bearbeiten]** klicken, um es zu aktualisieren. [Weitere Informationen](#create-and-edit-themes)

   ![Inhaltsvorlage im E-Mail-Designer mit der Schaltfläche „Design bearbeiten“ im Panel „Themen“](assets/theme-edit-in-template.png){width="40%"}

   >[!NOTE]
   >
   >Diese Option ist nicht verfügbar, wenn Themen im E-Mail-Inhalt verwendet werden.

1. Wenn Sie ein Thema mit mehreren Farbvarianten verwenden, können Sie eine bestimmte Variante für eine bestimmte Strukturkomponente auswählen. Auf diese Weise können Sie eine Farbvariante für den gesamten Inhalt definieren und eine andere Variante für nur eine bestimmte Struktur verwenden.

   >[!NOTE]
   >
   >Diese Aktion kann nicht für Inhaltskomponenten ausgeführt werden.

   Wählen Sie dazu eine Strukturkomponente aus, klicken Sie auf der Registerkarte **[!UICONTROL Stile]** rechts auf die Option ]**Variante eines bestimmten Themas verwenden**[!UICONTROL  und wenden Sie die gewünschte Variante auf diese Struktur an.

   ![Ausgewählte Struktur mit der Option „Variante eines bestimmten Themas verwenden“ auf der Registerkarte „Stile“](assets/theme-structure-variant.png)

   In diesem Beispiel wird die erste Farbvariante des aktuellen Themas auf den gesamten E-Mail-Inhalt angewendet, die dritte Farbvariante wird jedoch auf die ausgewählte Struktur angewendet. Sie können sehen, dass sich die Hintergrundfarben des Textkörpers und des Ansichtsfensters für diese spezifische Struktur vom Rest des Inhalts unterscheiden.

Sie können jederzeit zwischen Themen wechseln. Der E-Mail-Inhalt bleibt unverändert, aber die Stile werden aktualisiert, um das neue Thema widerzuspiegeln.

### Entsperren von Stilen {#unlocking-styles}

Wenn eine Komponente ausgewählt ist, können Sie den Stil mithilfe des entsprechenden Symbols auf der Registerkarte **[!UICONTROL Stile]** entsperren.

![Registerkarte „Stile“ in einer ausgewählten Komponente, auf der das Symbol „Stil entsperren“ angezeigt wird](assets/theme-unlock-style.png){width="90%"}

Das ausgewählte Thema wird weiterhin auf diese Komponente angewendet, Sie können jedoch die Stilelemente überschreiben. Wenn Sie Themen ändern, wird das neue Thema nur auf die Stilelemente angewendet, die nicht überschrieben wurden.<!--can you revert this action?-->

Wenn Sie beispielsweise eine Textkomponente entsperren, können Sie <!--the font size from 11 to 14 and -->die Schriftfarbe von Schwarz auf Rot ändern:

![Entsperrte Textkomponente mit benutzerdefinierter roter Textfarbe auf weißem Hintergrund](assets/theme-unlock-style-ex-white.png){width="80%" align="center" zoomable="yes"}

Wenn Sie Themen ändern, <!--the font size is still 14 and -->bleibt die Schriftfarbe für diese Komponente weiterhin rot, aber die Hintergrundfarbe für diese Komponente ändert sich mit dem neuen Design:

![Derselbe entsperrte Text mit roter Farbe und aktualisiertem Hintergrund von einem neuen Design](assets/theme-unlock-style-ex-colored.png){width="80%"}

## Verwenden von Themen in einem Fragment {#leverage-themes-fragment}

Damit ein [Fragment](#apply-themes-email) in einem Themeninhalt genutzt werden kann, muss dieses Fragment selbst mithilfe von Themen erstellt worden sein. Andernfalls können Sie dieses Fragment nicht in Ihrem Themeninhalt verwenden.

Gehen Sie wie folgt vor, um ein mit Themen kompatibles Fragment zu erstellen.

1. Erstellen Sie in [!DNL Adobe Campaign] ein visuelles Fragment und klicken Sie auf **[!UICONTROL Erstellen]**, um den Inhalt Ihres Fragments zu gestalten.[Weitere Informationen](../content/create-fragment.md#create-from-scratch)

1. Wählen Sie **[!UICONTROL Themen verwenden]** aus, um mit einem vordefinierten Stilthema zu beginnen.

   ![Fragment-E-Mail-Designer-Startoptionen mit ausgewählter Option „Themen verwenden“](assets/fragment-use-themes.png){width="100%"}

   >[!CAUTION]
   >
   >Wenn Sie den Modus „Manuelle Formatierung“ auswählen, können Sie keine Themen anwenden, es sei denn, Sie setzen Ihr Fragmentthema zurück.

1. Sobald Sie den E-Mail-Designer geöffnet haben, können Sie mit der Erstellung Ihres Fragments beginnen.

1. Klicken Sie in der rechten Leiste auf die Schaltfläche **[!UICONTROL Themen]**. Das Standardthema wird angezeigt. Sie können zwischen den verschiedenen Farbvarianten für dieses Thema wechseln.

   ![Inhaltsfragmente im E-Mail-Designer mit der Leiste „Themen“, die das Standardthema anzeigt](assets/fragment-default-theme.png){width="100%" align="center" zoomable="yes"}

1. Sie können andere Themen auswählen, um eine Vorschau Ihres Fragmentinhalts anzuzeigen. Wählen Sie dazu den Pfeil neben dem Standardthema aus und klicken Sie auf **[!UICONTROL Designs auswählen]**.

   ![Themen-Kopfzeile mit Pfeil und Steuerelement „Design auswählen“ für die Fragmentvorschau](assets/fragment-select-themes.png){width="40%"}

1. Sie können zwischen den Registerkarten **[!UICONTROL Adobe-Designs]** und **[!UICONTROL Meine Themen]** navigieren und bis zu fünf kompatible Themen (aus beiden Registerkarten) für Ihr Fragment auswählen.

   ![Dialogfeld zum Auswählen kompatibler Themen mit der Registerkarte „Adobe-Designs“ und „Meine Themen“](assets/fragment-select-compatible-themes.png){width=70%}

   >[!CAUTION]
   >
   >Wenn Sie ein Fragment in einem E-Mail-Inhalt verwenden, stellen Sie sicher, dass Sie ein für dieses Fragment definiertes [Thema anwenden](#apply-themes-email). Andernfalls kann es zu Anzeigeproblemen kommen, insbesondere in Outlook 2021 und früheren Versionen. 

1. Klicken Sie auf **[!UICONTROL Schließen]**.

1. Wählen Sie erneut den Pfeil neben dem **[!UICONTROL Standardthema]** aus. Sie können jetzt zwischen den verschiedenen, gerade ausgewählten Themen wechseln, um das Rendering jedes Stils in der Vorschau anzuzeigen.

   ![Fragment-Arbeitsfläche mit mehreren Themen, die für die Vorschau im Panel „Themen“ ausgewählt wurden](assets/fragment-selected-themes.png){width=90%}

1. Klicken Sie erneut auf **[!UICONTROL Designs auswählen]**, um weitere Themen hinzuzufügen oder Ihre Auswahl zu ändern.

## Erstellen einer mit Themen kompatiblen Vorlage {#theme-convertor}

In [!DNL Adobe Campaign] können Sie eine mit manueller Formatierung erstellte Vorlage in einen themenkompatiblen Inhalt konvertieren. Dies kann besonders dann nützlich sein, wenn Sie Inhaltsvorlagen erstellt haben, bevor Themen in [!DNL Adobe Campaign] eingeführt wurden, oder wenn Sie externe Inhalte importieren.

>[!NOTE]
>
> Nur **E-Mail-Vorlagen** können in themenkompatible Inhalte konvertiert werden. Einzelne E-Mails können nicht konvertiert werden. Sie müssen Ihren Inhalt zuerst als Vorlage speichern.

1. Öffnen Sie eine [Inhaltsvorlage](../content/create-email-templates.md) für E-Mails und bearbeiten Sie deren Inhalt mit dem E-Mail-Designer.

1. Wählen Sie in der rechten Leiste das Symbol **[!UICONTROL Themen]** aus und klicken Sie auf die Schaltfläche **[!UICONTROL Thema aus Inhalt generieren]**.

   ![Panel „Themen“ mit hervorgehobener Schaltfläche „Thema aus Inhalt generieren“](assets/generate-theme.png){width=100%}

1. Das Fenster **[!UICONTROL Thema erstellen]** wird geöffnet. [!DNL Adobe Campaign] erkennt automatisch die Stilelemente und konsolidiert sie in einem neuen Thema.

   ![Erstellen eines Dialogfelds „Thema erstellen“, in dem die im Vorlageninhalt erkannten Stile zusammengefasst werden](assets/generate-theme-create-window.png){width=90%}

1. Geben Sie einen Namen für Ihr Thema an.

1. Nehmen Sie Ihre eigenen Anpassungen vor, als würden Sie ein Thema von Grund auf neu erstellen, indem Sie z. B. eine Farbvariante hinzufügen, Schriftarten bearbeiten usw. [Weitere Informationen](#create-and-edit-themes)

   ![Generiertes Thema im Editor mit Farbpaletten- und Variantensteuerelementen](assets/generate-theme-colors.png){width=90%}

1. Klicken Sie auf **[!UICONTROL Speichern]**, um dieses neue Thema zur Wiederverwendung zu speichern. Sie können dieses Thema nun wie jedes andere Thema auf Ihre Inhalte anwenden. [Weitere Informationen](#apply-themes-email)
