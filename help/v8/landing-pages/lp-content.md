---
title: Definieren des Inhalts für die Landingpage
description: Erfahren Sie, wie Sie in Campaign Web Landingpage-spezifische Inhalte erstellen
feature: Landing Pages
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 5e5c731fa76684407080d9a1aa6f8a81de7ebc92
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 48%

---

# Definieren des Inhalts für die Landingpage {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Verwenden von Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout einer Landingpage gestalten können. Verwenden Sie die Formularkomponente, um bestimmte Inhalte zu definieren, über die Benutzerinnen und Benutzer ihre Auswahl auswählen und übermitteln können."

Wenn Sie den Inhalt einer beliebigen Seite Ihrer Landingpage bearbeiten, ist er bereits vorausgefüllt.

Die erste Seite, die den Benutzern sofort angezeigt wird, nachdem sie auf den Link zu Ihrer Landingpage geklickt haben, ist bereits mit dem [Landingpage-spezifische Formularkomponente](#use-form-component) für die ausgewählte Vorlage<!-- to enable users to select and submit their choices-->. Sie können auch [Stile für Ihre Landingpage](#lp-form-styles).

Um den Inhalt Ihrer Landingpage weiter zu gestalten, können Sie dieselben Komponenten wie für eine E-Mail verwenden. [Weitere Informationen](../email/content-components.md#add-content-components)

Der Inhalt der **[!UICONTROL Bestätigung]**, **[!UICONTROL Fehler]** und **[!UICONTROL Ablauf]** -Seiten sind ebenfalls vorausgefüllt. Bearbeiten Sie sie nach Bedarf.

## Verwenden von Formularkomponenten {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Festlegen der Formularkomponentenfelder"
>abstract="Definieren Sie, wie die Empfängerinnen und Empfänger ihre Auswahl auf Ihrer Landingpage sehen und übermitteln."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Was passiert, wenn auf die Schaltfläche geklickt wird"
>abstract="Definieren Sie, was passieren soll, wenn Benutzende das Landingpage-Formular übermitteln."

Um bestimmte Inhalte zu definieren, mit denen Benutzende ihre Auswahl auf Ihrer Landingpage festlegen und übermitteln können, verwenden Sie die **[!UICONTROL Formularkomponente]**. Gehen Sie dazu wie folgt vor.

1. Die Landingpage-spezifische **[!UICONTROL Formularkomponente]** wird bereits auf der Arbeitsfläche für die ausgewählte Vorlage angezeigt.

   >[!NOTE]
   >
   >Die **[!UICONTROL Formularkomponente]** kann nur einmal auf derselben Seite verwendet werden.

1. Wählen Sie sie aus. Die Registerkarte **[!UICONTROL Formularinhalt]** in der rechten Palette wird angezeigt, damit Sie die verschiedenen Felder des Formulars bearbeiten können.

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >Sie können jederzeit zur Registerkarte **[!UICONTROL Stile]** wechseln, um die Stile Ihres Formularkomponenteninhalts zu bearbeiten. [Weitere Informationen](#lp-form-styles)

1. Erweitern Sie das erste Textfeld, falls vorhanden, oder fügen Sie mithilfe der **[!UICONTROL Hinzufügen]** Schaltfläche. Aus dem **[!UICONTROL Textfeld 1]** können Sie den Feldtyp, das zu aktualisierende Datenbankfeld, den Titel und den Text bearbeiten, der innerhalb des Felds angezeigt wird, bevor Benutzer einen Wert eingeben.

   ![](assets/lp-form-text-field.png)

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Formularfeld zum Pflichtfeld machen]**. In diesem Fall kann das Formular der Landingpage nur gesendet werden, wenn der Benutzer dieses Feld ausgefüllt hat.

   >[!NOTE]
   >
   >Wenn ein Pflichtfeld nicht ausgefüllt wurde, erscheint eine Fehlermeldung, wenn der Benutzer das Formular sendet.

1. Erweitern Sie das Kontrollkästchen, falls vorhanden, oder fügen Sie mithilfe des **[!UICONTROL Hinzufügen]** Schaltfläche. Wählen Sie aus, ob mit diesem Kontrollkästchen ein Dienst oder ein Feld aus der Datenbank aktualisiert werden soll.

   ![](assets/lp-form-checkbox.png)

   Wenn Sie **[!UICONTROL Abonnements und Dienste]**, wählen Sie einen Dienst aus der Liste aus und wählen Sie zwischen den beiden folgenden Optionen:

   * **[!UICONTROL Anmelden, falls aktiviert]**: Benutzer müssen das Kontrollkästchen zum Einverständnis aktivieren (Opt-in).
   * **[!UICONTROL Abmelden wenn aktiviert]**: Benutzende müssen das Kontrollkästchen aktivieren, um ihr Einverständnis zu entfernen (Opt-out).

   Wenn Sie **[!UICONTROL Feld]**, wählen Sie ein Feld aus der Attributliste aus und wählen Sie zwischen den beiden folgenden Optionen:

   * **[!UICONTROL Ja, wenn aktiviert]**<!--TBC-->

   * **[!UICONTROL Nein, überprüft]**<!--TBC-->

1. Sie können so viele Felder löschen und hinzufügen (wie Textfelder, Optionsfelder, Kontrollkästchen, Dropdown-Listen usw.) nach Bedarf.

1. Nachdem alle Felder hinzugefügt oder aktualisiert wurden, klicken Sie auf **[!UICONTROL Aktionsaufruf]** um den entsprechenden Abschnitt zu erweitern. Damit können Sie das Verhalten der Schaltfläche in der **[!UICONTROL Formularkomponente]** festlegen.

   ![](assets/lp-call-to-action.png)

1. Definieren Sie, was beim Klicken auf die Schaltfläche passieren soll:

   * **[!UICONTROL Bestätigungsseite]**: Die Person wird zur **[!UICONTROL Bestätigungsseite]** weitergeleitet, die für die aktuelle Landingpage festgelegt ist.

   * **[!UICONTROL Umleitungs-URL]**: Geben Sie die URL der Seite ein, zu der die Benutzenden umgeleitet werden sollen.

1. Wenn Sie beim Senden des Formulars zusätzliche Aktualisierungen vornehmen möchten, wählen Sie **[!UICONTROL Zusätzliche Aktualisierungen]** und wählen Sie das Element aus, das Sie aktualisieren möchten:
   * Ein Anmeldedienst - definieren Sie in diesem Fall, ob Sie Benutzer beim Senden des Formulars anmelden oder abwählen möchten.
   * Die beim Ausfüllen des Formulars verwendete E-Mail.
   * Alle Kanäle - Beim Senden des Formulars werden die Benutzer (je nach ausgewählter Vorlage) an/aus allen Nachrichten Ihrer Marke auf allen Kanälen angemeldet oder abgemeldet.
   * Ein Feld aus der Datenbank: Wählen Sie ein Feld aus der Attributliste aus und legen Sie fest, ob es beim Senden des Formulars auf True oder False gesetzt werden soll.

   ![](assets/lp-form-additionnal-updates.png)

1. Speichern Sie den Inhalt, um zu den [Eigenschaften der Landingpage](create-lp.md#create-landing-page) zurückzukehren.

## Definieren der Formularstile für die Landingpage {#lp-form-styles}

1. Um die Stile Ihres Formularkomponenteninhalts zu ändern, wechseln Sie jederzeit zum **[!UICONTROL Stile]** Registerkarte.

1. Die **[!UICONTROL Textfeld]** -Abschnitt wird standardmäßig erweitert. Sie können damit das Erscheinungsbild der Textfelder bearbeiten, z. B. die Beschriftungsschrift, die Position der Beschriftung, die Hintergrundfarbe des Felds oder den Feldrand.

   ![](assets/lp-text-styles.png)

1. Erweitern Sie die **[!UICONTROL Kontrollkästchen]** -Abschnitt, um das Erscheinungsbild der Kontrollkästchen und des entsprechenden Texts zu definieren. Sie können beispielsweise die Schriftfamilie und -größe oder die Rahmenfarbe des Kontrollkästchens anpassen.

   ![](assets/lp-checkbox-style.png)

1. Erweitern und bearbeiten Sie alle anderen Abschnitte, die anderen von Ihnen hinzugefügten Feldern entsprechen (Optionsfeld, Dropdown-Liste, Datum und Uhrzeit usw.) in Ihr Formular ein.

1. Erweitern Sie die **[!UICONTROL Aktionsaufruf]** -Abschnitt, um das Erscheinungsbild der Schaltfläche im Komponentenformular zu ändern. Sie können beispielsweise die Schriftart ändern, einen Rahmen hinzufügen, die Beschriftungsfarbe beim Bewegen des Mauszeigers bearbeiten oder die Ausrichtung der Schaltfläche anpassen.

   ![](assets/lp-call-to-action-style.png)

   Sie können eine Vorschau einiger Ihrer Einstellungen anzeigen, z. B. die Farbe der Schaltflächenbeschriftung beim Bewegen des Mauszeigers, indem Sie die Schaltfläche **[!UICONTROL Inhalt simulieren]** verwenden. [Weitere Informationen](create-lp.md#test-landing-page)

1. Speichern Sie Ihre Änderungen.
