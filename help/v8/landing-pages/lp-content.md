---
title: Landingpage-spezifischen Inhalt definieren
description: Erfahren Sie, wie Sie Landingpage-spezifischen Inhalt im Campaign-Web erstellen.
feature: Landing Pages
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 5c3f02d4c95951693ac73de4a6e8810e1b662e53
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 7%

---

# Landingpage-spezifischen Inhalt definieren {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Verwenden von Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout einer Landingpage erstellen können. Verwenden Sie die Formular-Komponente, um bestimmte Inhalte zu definieren, über die Benutzer ihre Auswahl auswählen und übermitteln können."

Wenn Sie den Inhalt einer beliebigen Seite Ihrer Landingpage bearbeiten, ist er bereits vorausgefüllt.

Die primäre Seite ist die Seite, die den Benutzern sofort angezeigt wird, nachdem sie auf den Link zu Ihrer Landingpage geklickt haben, z. B. über eine E-Mail oder eine Website. Die primäre Seite ist bereits mit dem [Landingpage-spezifische Formularkomponente](#use-form-component) , damit Benutzer ihre Auswahl treffen und ihre Auswahl übermitteln können. Sie können auch [Landingpage-spezifische Stile](#lp-form-styles).

Um den Inhalt Ihrer Landingpage weiter zu gestalten, können Sie dieselben Komponenten wie für eine E-Mail verwenden. [Weitere Informationen](../email/content-components.md#add-content-components)

<!--
The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

Set the subscription form to the appropriate fields from the database to make sure it will work correctly.

The landing page default fields are already there for the selected template.

>[!NOTE]
>
>You can also create a click-through landing page without a **[!UICONTROL Form]** component. In that case, the landing page will be displayed to users, but they will not be required to submit any form. This can be useful if you only want to showcase a landing page without requiring any action from your recipients such as opt-in or opt out, or want to provide information that doesn't require user input.

Using the landing page content designer, you can also leverage contextual data coming from the primary page in a subpage. [Learn more](#use-primary-page-context)-->

## Formularkomponente verwenden {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Formularkomponentenfelder festlegen"
>abstract="Definieren Sie, wie die Empfänger ihre Auswahl auf Ihrer Landingpage sehen und übermitteln."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Was passiert, wenn auf die Schaltfläche geklickt wird"
>abstract="Definieren Sie, was beim Senden des Landingpage-Formulars durch Benutzer geschehen soll."

Um bestimmte Inhalte zu definieren, mit denen Benutzer ihre Auswahl auf Ihrer Landingpage festlegen und unterbreiten können, verwenden Sie das **[!UICONTROL Formular]** -Komponente. Gehen Sie dazu wie folgt vor.

1. Die Landingpage-spezifisch **[!UICONTROL Formular]** -Komponente bereits auf der Arbeitsfläche für die ausgewählte Vorlage angezeigt.

   >[!NOTE]
   >
   >Die **[!UICONTROL Formular]** -Komponente kann nur einmal auf derselben Seite verwendet werden.

1. Wählen Sie es aus. Die **[!UICONTROL Formularinhalt]** in der rechten Palette angezeigt, damit Sie die verschiedenen Felder des Formulars bearbeiten können.

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >Wechseln Sie zu **[!UICONTROL Stile]** jederzeit zum Bearbeiten der Stile Ihres Formularkomponenteninhalts. [Weitere Informationen](#lp-form-styles)

1. Erweitern Sie das erste Textfeld. Aus dem **[!UICONTROL Textfeld 1]** können Sie den Feldtyp, das Datenbankfeld, den Titel und den Text bearbeiten, der innerhalb des Felds angezeigt wird, bevor der Benutzer das Feld ausfüllt.

   ![](assets/lp-form-text-field.png)

1. Überprüfen Sie die **[!UICONTROL Formularfeld obligatorisch machen]** bei Bedarf. In diesem Fall kann das Formular der Landingpage nur gesendet werden, wenn der Benutzer dieses Feld ausgefüllt hat.

   >[!NOTE]
   >
   >Wenn ein Pflichtfeld nicht ausgefüllt wurde, erscheint eine Fehlermeldung, wenn der Benutzer das Formular sendet.

1. Checkbox hinzufügen. Wählen Sie aus, ob mit diesem Kontrollkästchen ein Dienst oder ein Feld aus der Datenbank aktualisiert werden soll.

   ![](assets/lp-form-checkbox.png)

   Definieren Sie, ob diese Checkbox Benutzern das Ein- und Ausschließen ermöglicht. Wählen Sie aus den beiden folgenden Optionen aus:

   * **[!UICONTROL Abonnieren, wenn aktiviert]**: Benutzer müssen das Kontrollkästchen zum Einverständnis aktivieren (Opt-in).
   * **[!UICONTROL Abmeldung bei aktivierter Option]**: Benutzer müssen das Kontrollkästchen aktivieren, um ihre Zustimmung zu entfernen (Opt-out).

1. Sie können beliebig viele Textfelder und/oder Kontrollkästchen löschen und hinzufügen.

1. Nachdem Sie alle gewünschten Kontrollkästchen und/oder Textfelder hinzugefügt haben, klicken Sie auf **[!UICONTROL Aktionsaufruf]** um den entsprechenden Abschnitt zu erweitern. Damit können Sie das Verhalten der Schaltfläche im **[!UICONTROL Formular]** -Komponente.

   ![](assets/lp-call-to-action.png)

1. Definieren Sie, was beim Klicken auf die Schaltfläche passieren soll:

   * **[!UICONTROL Bestätigungsseite]**: Der Benutzer wird zum **[!UICONTROL Bestätigung]** für die aktuelle Landingpage festgelegt ist.

   * **[!UICONTROL Umleitungs-URL]**: Geben Sie die URL der Seite ein, zu der die Benutzer umgeleitet werden.

1. Wenn Sie beim Senden des Formulars zusätzliche Aktualisierungen vornehmen möchten, wählen Sie **[!UICONTROL Zusätzliche Aktualisierungen]** auswählen **[!UICONTROL Opt-in]** oder **[!UICONTROL Opt-out]** und definieren Sie, ob Sie eine Abonnementliste, den Kanal oder nur die verwendete E-Mail-Adresse aktualisieren möchten.

   ![](assets/lp-form-additionnal-updates.png)

1. Speichern Sie den Inhalt, um zur [Landingpage-Eigenschaften](create-lp.md).

## Formularstile für Landingpages definieren {#lp-form-styles}

1. Um die Stile Ihres Formularkomponenteninhalts zu ändern, wechseln Sie jederzeit zum **[!UICONTROL Stil]** Registerkarte.

   ![](assets/lp_designer-form-style.png)

1. Die **[!UICONTROL Felder]** standardmäßig erweitert und ermöglicht es Ihnen, das Erscheinungsbild des Textfelds zu bearbeiten, z. B. die Beschriftung und Platzhalterschrift, die Position der Beschriftung, die Hintergrundfarbe des Felds oder den Feldrand.

   ![](assets/lp_designer-form-style-fields.png)

1. Erweitern Sie die **[!UICONTROL Kontrollkästchen]** -Abschnitt, um das Erscheinungsbild der Kontrollkästchen und des entsprechenden Texts zu definieren. Sie können beispielsweise die Schriftfamilie, die Schriftgröße oder die Rahmenfarbe des Kontrollkästchens anpassen.

   ![](assets/lp_designer-form-style-checkboxes.png)

1. Erweitern Sie die **[!UICONTROL Schaltflächen]** -Abschnitt, um das Erscheinungsbild der Schaltfläche im Komponentenformular zu ändern. Sie können beispielsweise die Schriftart ändern, einen Rahmen hinzufügen, die Beschriftungsfarbe beim Bewegen des Mauszeigers bearbeiten oder die Ausrichtung der Schaltfläche anpassen.

   ![](assets/lp_designer-form-style-buttons.png)

   Sie können eine Vorschau Ihrer Einstellungen anzeigen, z. B. die Farbe der Schaltflächenbeschriftung beim Bewegen des Mauszeigers, indem Sie die **[!UICONTROL Inhalt simulieren]** Schaltfläche. Weitere Informationen zum Testen von Landingpages [here](create-lp.md#test-landing-page).

1. Erweitern Sie die **[!UICONTROL Formularlayout]** um die Layouteinstellungen wie die Hintergrundfarbe, den Abstand oder den Rand zu bearbeiten.

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

