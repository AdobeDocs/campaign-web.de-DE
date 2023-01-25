---
title: Personalisieren von Inhalten in Campaign
description: Erfahren Sie, wie Sie Inhalte in der Web-Benutzeroberfläche von Adobe Campaign personalisieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 51bd6f405ad151e2264d69c57ffe5e1783077203
workflow-type: ht
source-wordcount: '653'
ht-degree: 100%

---

# Personalisieren von Inhalten{#add-personalization}

![](../assets/do-not-localize/badge.png)

Sie können den Nachrichteninhalt wie folgt personalisieren:

* Einfügen von dynamischen **Personalisierungsfeldern**

   Personalisierungsfelder werden für die oberste Ebene der Nachrichtenpersonalisierung verwendet. Sie können jedes in der Datenbank verfügbare Feld aus dem Personalisierungseditor auswählen. Für einen Versand können Sie jedes Feld auswählen, das sich auf die Empfängerin oder den Empfänger, die Nachricht oder den Versand bezieht. Diese Personalisierungsattribute können in die Betreffzeile oder in den Text Ihrer Nachrichten eingefügt werden.

   ![](assets/perso-subject-line.png)

   Mit der folgenden Syntax wird die Stadt des Empfängers bzw. der Empfängerin in Ihren Inhalt eingefügt: &lt;%= recipient.location.city %>.

* Einfügen von vordefinierten **Inhaltsbausteinen**

   Campaign verfügt über eine Reihe von Gestaltungsbausteinen, die ein bestimmtes Rendering ermöglichen, das Sie in Ihre Sendungen einfügen können. Sie können zum Beispiel ein Logo, eine Grußbotschaft oder einen Link zur Mirror-Seite der Nachricht hinzufügen. Inhaltsbausteine sind über einen eigenen Eintrag im Personalisierungseditor verfügbar.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personalisieren der Betreffzeile der E-Mail {#personalize-subject-line}

Um eine Personalisierung im Feld **[!UICONTROL Betreffzeile]** der Nachricht hinzuzufügen, gehen Sie wie folgt vor:

1. Klicken Sie auf **Personalisierungsdialog öffnen** rechts neben dem Feld **Betreffzeile**.
1. Geben Sie den Inhalt der Betreffzeile ein und wählen Sie die Personalisierungsattribute, die Sie hinzufügen möchten.
1. Klicken Sie auf **Bestätigen**, um die Eingaben zu bestätigen. Die Personalisierungsattribute werden der Betreffzeile hinzugefügt.

![](assets/perso-subject.png)

## Personalisieren des E-Mail-Inhalts {#personalize-emails}

Um den E-Mail-Inhalt zu personalisieren, öffnen Sie die Nachricht im E-Mail-Designer und:

1. Klicken Sie auf einen Textblock.
1. Wählen Sie in der kontextbasierten Symbolleiste **Personalisierung hinzufügen**.

   ![](assets/perso-add-to-content.png)

1. Fügen Sie den Namen der Empfängerin oder des Empfängers in den Personalisierungseditor ein und bestätigen Sie die Eingabe.

   ![](assets/perso-add-name.png)

   Das Personalisierungsattribut wird dem E-Mail-Inhalt hinzugefügt.

   Sie können den Inhalt simulieren, um das Rendering zu überprüfen. [Weitere Informationen](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

Um einen Inhaltsbaustein zu Ihrer E-Mail hinzuzufügen, führen Sie dieselben Schritte aus und wählen im letzten Symbol einen Inhaltsbaustein:

![](assets/perso-insert-block.png)

Nach dem Einfügen wird der Inhaltsbaustein wie unten dargestellt zum E-Mail-Inhalt hinzugefügt. Er wird in der Versandvorbereitungsphase bei der Generierung der Personalisierung automatisch an das Empfängerprofil angepasst.

![](assets/perso-content-block-in-email.png)


Integrierte Inhaltsbausteine sind:
* **[!UICONTROL Ermöglicht durch Adobe Campaign]**: Hiermit wird das Logo „Ermöglicht durch Adobe Campaign“ eingefügt.
* **[!UICONTROL Formatierungsfunktion für Eigennamen]**: Hiermit wird die JavaScript-Funktion **[!UICONTROL toSmartCase]** generiert, mit der der erste Buchstabe eines jeden Worts in einen Großbuchstaben umgewandelt wird.
* **[!UICONTROL Grußformeln]**: Hiermit werden Grußformeln zum Empfängernamen hinzugefügt, z. B. „Guten Tag, Max Mustermann“.
* **[!UICONTROL Logo einfügen]**: Fügt ein Logo ein, das in den Instanzeinstellungen definiert ist.
* **[!UICONTROL Link zur Mirror-Seite]**: Hiermit wird der Link zur Mirror-Seite „Wenn die Nachricht nicht richtig angezeigt wird, bitte hier klicken“ eingefügt.
* **[!UICONTROL Mirror-Seiten-URL]**: Hiermit wird die Mirror-Seiten-URL eingefügt, damit Versand-Designer den Link prüfen können.
* **[!UICONTROL Annahme-URL eines Angebots im Einzelmodus]**: Hiermit wird eine URL eingefügt, die es ermöglicht, ein Angebot auf **[!UICONTROL Angenommen]** zu setzen.
* **[!UICONTROL Anmeldungsseiten-URL]**: Hiermit wird eine Abonnement-URL eingefügt.
* **[!UICONTROL Anmelde-Link]**: Hiermit wird ein Anmelde-Link eingefügt. Dieser Link wird in den Instanzeinstellungen definiert. Der Standardinhalt lautet: „Klicken Sie hier, um sich zu registrieren.“
* **[!UICONTROL Anmelde-Link (mit Werber)]**: Hiermit wird ein Anmelde-Link eingefügt, über den der Besucher bzw. die Besucherin sowie der Versand identifiziert werden können. Dieser Link wird in den Instanzeinstellungen definiert.
* **[!UICONTROL Anmeldebestätigung]**: Hiermit wird ein Link eingefügt, mit dem die Anmeldung bestätigt werden kann.
* **[!UICONTROL Teilen-Links der sozialen Netzwerke]** : Hiermit werden Schaltflächen eingefügt, mit denen der Empfänger bzw. die Empfängerin einen Link zum Inhalt der Mirror-Seite freigeben kann.
* **[!UICONTROL Stil der Inhalts-E-Mails]** und **[!UICONTROL Stil der Benachrichtigungen]**: Hiermit wird Code erstellt, mit dem eine E-Mail mit nativen HTML-Stilen formatiert werden kann.
* **[!UICONTROL Abmelde-Link]**: Fügt einen Link ein, der es ermöglicht, das Abo aller Sendungen zu kündigen (Blockierungsliste). Der standardmäßig verknüpfte Inhalt ist: „Sie erhalten diese Nachricht, da Sie mit ***Name Ihres Unternehmens*** oder einem Tochterunternehmen in Kontakt standen. Um keine Nachrichten mehr von ***Name Ihres Unternehmens*** zu erhalten, klicken Sie hier.“


## Personalisieren von Links in E-Mails {#personalize-links}

So personalisieren Sie einen **Link**:

1. Wählen Sie einen Textblock oder ein Bild aus.
1. Wählen Sie in der kontextbezogenen Symbolleiste **Link einfügen**.

   ![](assets/perso-link.png)

1. Geben Sie den Link-Titel ein und verwenden Sie die Schaltfläche **Link einfügen**, um den Link zu personalisieren.

   ![](assets/perso-link-insert-icon.png)

1. Verwenden Sie den Personalisierungseditor, um den Link zu definieren und zu personalisieren, und bestätigen Sie ihn dann.

   ![](assets/perso-link-edit.png)


## Personalisieren von Angeboten {#personalize-offers}

Sie können mit dem Personalisierungseditor auch Textinhalte zu den Darstellungen Ihrer Angebote hinzufügen. Weiterführende Informationen finden Sie in [diesem Abschnitt](../content/offers.md).
