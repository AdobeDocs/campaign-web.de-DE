---
title: Definieren des Inhalts für die Landingpage
description: Erfahren Sie, wie Sie in Campaign Web Landingpage-spezifische Inhalte erstellen
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 56%

---

# Definieren des Inhalts für die Landingpage {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Verwenden von Inhaltskomponenten"
>abstract="Inhaltskomponenten sind leere Platzhalter für Inhalte, mit denen Sie das Layout einer Landingpage gestalten können. Um spezifische Inhalte zu definieren, die es den Benutzenden ermöglichen, ihre Auswahl zu treffen und abzusenden, können Sie die Formularkomponente nutzen."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definieren der primären Seiteneinstellungen"
>abstract="Die Primärseite wird Benutzern sofort angezeigt, nachdem sie auf den Link zu Ihrer Landingpage geklickt haben, z. B. über eine E-Mail oder eine Website."

Sie können den Inhalt einer beliebigen Seite Ihrer Landingpage bearbeiten.

Die erste Seite, die Benutzern sofort angezeigt wird, nachdem sie auf den Link zu Ihrer Landingpage geklickt haben, ist bereits mit der [Landingpage-spezifischen Formularkomponente](#use-form-component) für die ausgewählte Vorlage vorausgefüllt<!-- to enable users to select and submit their choices-->.

Der Inhalt der **[!UICONTROL Bestätigungs]**-, **[!UICONTROL Fehler]**- und **[!UICONTROL Ablauf]**-Seiten ist ebenfalls vorausgefüllt. Bearbeiten Sie den Inhalt nach Bedarf. 

Sie können auch [Stile für Ihre Landingpage](#lp-form-styles) definieren.

So gestalten Sie den Inhalt Ihrer Landingpage weitergehend:

* Verwenden Sie dieselben Komponenten wie für das Entwerfen einer E-Mail. [Weitere Informationen](../email/content-components.md#add-content-components)

* Fügen Sie Ihren Landingpages bedingte Inhalte auf die gleiche Weise hinzu wie bei einer E-Mail. [Weitere Informationen](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >Diese Funktion ist nur eingeschränkt verfügbar. Sie ist Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und kann nicht in anderen Umgebungen bereitgestellt werden.

## Verwenden von Formularkomponenten {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Festlegen der Formularkomponentenfelder"
>abstract="Definieren Sie, wie die Empfängerinnen und Empfänger ihre Auswahl auf Ihrer Landingpage sehen und übermitteln."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Was passiert, wenn auf die Schaltfläche geklickt wird"
>abstract="Definieren Sie, was passieren soll, wenn Benutzende das Landingpage-Formular übermitteln."

Um spezifische Inhalte zu definieren, die es den Benutzenden ermöglichen, eine Auswahl auf der Landingpage zu treffen und abzusenden, bearbeiten Sie die **[!UICONTROL Formular]**-Komponente. Gehen Sie dazu wie folgt vor.

1. Die Landingpage-spezifische **[!UICONTROL Formularkomponente]** wird bereits auf der Arbeitsfläche für die ausgewählte Vorlage angezeigt.

   >[!NOTE]
   >
   >Die **[!UICONTROL Formularkomponente]** kann nur einmal auf derselben Seite verwendet werden.

1. Wählen Sie sie aus. Die Registerkarte **[!UICONTROL Formularinhalt]** in der rechten Palette wird angezeigt, damit Sie die verschiedenen Felder des Formulars bearbeiten können.

   ![Formularkomponente wird auf der Arbeitsfläche angezeigt](assets/lp-form-component.png){zoomable="yes"}

   >[!NOTE]
   >
   >Sie können jederzeit zur Registerkarte **[!UICONTROL Stile]** wechseln, um die Stile Ihres Formularkomponenteninhalts zu bearbeiten. [Weitere Informationen](#lp-form-styles)

1. Erweitern Sie das erste Textfeld, falls vorhanden, oder fügen Sie eines mithilfe der Schaltfläche **[!UICONTROL Hinzufügen]** hinzu. Bearbeiten Sie im Abschnitt **[!UICONTROL Textfeld 1]** den Feldtyp, das zu aktualisierende Datenbankfeld, die Bezeichnung und den Text, der innerhalb des Felds angezeigt wird, bevor Benutzer einen Wert eingeben.

   ![Textfeldeinstellungen in der Formularkomponente](assets/lp-form-text-field.png){zoomable="yes"}

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Formularfeld zum Pflichtfeld machen]**. In diesem Fall kann das Formular der Landingpage nur gesendet werden, wenn der Benutzer dieses Feld ausgefüllt hat.

   >[!NOTE]
   >
   >Wenn ein Pflichtfeld nicht ausgefüllt wurde, wird beim Senden der Seite durch den Benutzer eine Fehlermeldung angezeigt.

1. Erweitern Sie das Kontrollkästchen, falls vorhanden, oder fügen Sie eines mithilfe der Schaltfläche **[!UICONTROL Hinzufügen]** hinzu. Wählen Sie aus, ob mit diesem Kontrollkästchen ein Dienst oder ein Feld aus der Datenbank aktualisiert werden soll.

   ![Kontrollkästchen-Einstellungen in der Formularkomponente](assets/lp-form-checkbox.png){zoomable="yes"}

   Wenn Sie **[!UICONTROL Abonnements und Services]** auswählen, wählen Sie einen [Dienst](../audience/manage-services.md) aus der Liste aus und legen Sie eine der beiden folgenden Optionen fest:

   * **[!UICONTROL Anmelden wenn aktiviert]**: Benutzende müssen das Kontrollkästchen zum Einverständnis aktivieren (Opt-in).
   * **[!UICONTROL Abmelden wenn aktiviert]**: Benutzende müssen das Kontrollkästchen aktivieren, um ihr Einverständnis zu entfernen (Opt-out).

   Wenn Sie **[!UICONTROL Feld]** auswählen, wählen Sie ein Feld aus der [Attributliste](../get-started/attributes.md) aus und legen Sie eine der beiden folgenden Optionen fest:

   * **[!UICONTROL Ja, wenn aktiviert]**.
   * **[!UICONTROL Nein, falls aktiviert]**.

1. Löschen Sie so viele Felder wie nötig (z. B. Textfelder, Optionsschaltflächen, Kontrollkästchen, Dropdown-Listen usw.) und fügen Sie sie hinzu.

1. Nachdem alle Felder hinzugefügt oder aktualisiert wurden, klicken Sie auf **[!UICONTROL Handlungsaufforderung]**, um den entsprechenden Abschnitt zu erweitern. Damit können Sie das Verhalten der Schaltfläche in der **[!UICONTROL Formularkomponente]** festlegen. [Weitere Informationen dazu](#define-actions-on-form-submission)

   ![Aktionseinstellungen in der Formularkomponente](assets/lp-call-to-action.png){zoomable="yes"}

1. Speichern Sie den Inhalt, um zu den [Eigenschaften der Landingpage](create-lp.md#create-landing-page) zurückzukehren.

### Definieren von Aktionen bei der Formularübermittlung {#define-actions-on-form-submission}

1. Definieren Sie, was beim Klicken auf die Schaltfläche geschieht:

   * **[!UICONTROL Bestätigungsseite]**: Standardmäßig wird der Benutzer zur Seite **[!UICONTROL Bestätigung]** umgeleitet, die für die aktuelle Landingpage festgelegt ist.

   * **[!UICONTROL Umleitungs-URL]**: Geben Sie die URL der Seite ein, zu der die Benutzer umgeleitet werden.

   * **[!UICONTROL Landingpage]**: Wählen Sie eine andere Landingpage aus, zu der Benutzer weitergeleitet werden sollen. Konfigurieren Sie die ausgewählte Landingpage entsprechend.

1. Um beim Senden des Formulars zusätzliche Aktualisierungen vorzunehmen, wählen Sie **[!UICONTROL Zusätzliche]**) und das Element aus, das Sie aktualisieren möchten:
   * Ein Abonnement [Dienst](../audience/manage-services.md) - legen Sie fest, ob Benutzer beim Senden des Formulars ein- oder ausgeschlossen werden sollen. Wenn Sie beim Entwerfen einer E-Mail einen **[!UICONTROL Landingpage]**-Link zu dieser Landingpage definieren, wird automatisch der ausgewählte Service verwendet. [Weitere Informationen zum Einfügen von Links](../email/message-tracking.md)

     >[!NOTE]
     >
     >Wenn Sie für diese Landingpage mehrere Dienste verwenden möchten, verwenden Sie die nachstehend beschriebene Option **[!UICONTROL Dienst über URL]**.

   * Der Kanal - die E-Mail-Adresse, die beim Ausfüllen des Formulars verwendet wird.
   * Alle Kanäle : Beim Senden des Formulars werden Benutzende (je nach ausgewählter Vorlage) für alle Nachrichten Ihrer Marke auf allen Kanälen an/von allen Nachrichten abgemeldet.
   * Ein Feld aus der Datenbank: Wählen Sie ein Feld aus der Attributliste aus und legen Sie fest, ob es beim Senden des Formulars auf „True“ oder „False“ gesetzt werden soll.

   ![Zusätzliche Aktualisierungseinstellungen in der Formularkomponente](assets/lp-form-additionnal-updates.png){zoomable="yes"}

1. Wählen Sie die Option **[!UICONTROL Dienst über URL]** aus, damit die Landingpage für mehrere Dienste verwendet werden kann, wodurch sie dynamisch wird. Definieren Sie, ob Benutzende bei der Formularübermittlung angemeldet oder abgemeldet werden sollen.

   >[!AVAILABILITY]
   >
   >Diese Funktion ist nur eingeschränkt verfügbar. Sie ist Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und kann nicht in anderen Umgebungen bereitgestellt werden.

   ![Service von URL-Einstellungen in der Formularkomponente](assets/lp-form-service-from-url.png){zoomable="yes"}

   Wenn Sie beim Entwerfen einer E-Mail einen **[!UICONTROL Landingpage]**-Link zu dieser Landingpage definieren, können Sie einen beliebigen Service aus der Liste auswählen. Sie können dann bei der Definition anderer Links zu dieser Landingpage andere Dienste auswählen. [Weitere Informationen zum Einfügen von Links](../email/message-tracking.md)

   ![E-Mail-Link zu Landingpage-Einstellungen](assets/email-link-to-landing-page.png){zoomable="yes"}

1. Senden Sie bei der Übermittlung Ihrer Landingpage eine Nachricht. [Weitere Informationen finden Sie hier](#lp-message)

### Senden einer Nachricht nach der Einreichung {#lp-message}

>[!AVAILABILITY]
>
>Diese Funktion ist nur eingeschränkt verfügbar. Sie ist Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und kann nicht in anderen Umgebungen bereitgestellt werden.

Gehen Sie wie folgt vor, um nach dem Senden einer Landingpage automatisch eine Bestätigungsnachricht zu senden:

1. Aktivieren Sie im Abschnitt **[!UICONTROL HANDLUNGSAUFFORDERUNG]** die Option **[!UICONTROL Bestätigungs-E-Mail senden]**.

1. Wählen Sie in der dazugehörigen Dropdown-Liste die zu sendende Transaktionsnachrichtenvorlage aus.

![Bestätigungs-E-Mail-Einstellungen in der Formularkomponente](assets/lp-confirmation.png){zoomable="yes"}

## Definieren der Formularstile für die Landingpage {#lp-form-styles}

1. Um die Stile Ihres Formularkomponenteninhalts zu ändern, können Sie jederzeit zur Registerkarte **[!UICONTROL Stil]** wechseln.

1. Der Abschnitt **[!UICONTROL Textfeld]** wird standardmäßig erweitert. Er ermöglicht es Ihnen, das Erscheinungsbild des Textfelds zu bearbeiten, z. B. die Schriftart für Titel, die Position der Titel, die Hintergrundfarbe des Felds oder des Feldrands.

   ![Stileinstellungen für Textfelder](assets/lp-text-styles.png){zoomable="yes"}

1. Klappen Sie den Abschnitt **[!UICONTROL Kontrollkästchen]** aus, um das Erscheinungsbild der Kontrollkästchen und des entsprechenden Texts zu definieren. Passen Sie beispielsweise die Schriftfamilie und -größe oder die Rahmenfarbe des Kontrollkästchens an.

   ![Checkbox-Stileinstellungen](assets/lp-checkbox-style.png){zoomable="yes"}

1. Erweitern und bearbeiten Sie alle anderen Abschnitte, die anderen ggf. von Ihnen zum Formular hinzugefügten Feldern entsprechen (Optionsfeld, Dropdown-Liste, Datum, Uhrzeit usw.).

1. Erweitern Sie den Abschnitt **[!UICONTROL Handlungsaufforderung]**, um das Erscheinungsbild der Schaltfläche im Komponentenformular zu ändern. Ändern Sie beispielsweise die Schriftart, fügen Sie einen Rahmen hinzu, bearbeiten Sie die Titelfarbe beim Bewegen des Mauszeigers oder passen Sie die Ausrichtung der Schaltfläche an.

   ![Stileinstellungen für Aktionsaufrufe](assets/lp-call-to-action-style.png){zoomable="yes"}

   Zeigen Sie einige Ihrer Einstellungen, z. B. die Farbe der Schaltflächenbeschriftung beim Bewegen des Mauszeigers, in der Vorschau an, indem Sie die Schaltfläche **[!UICONTROL Inhalt simulieren]** verwenden. [Weitere Informationen](create-lp.md#test-landing-page)

1. Speichern Sie Ihre Änderungen.