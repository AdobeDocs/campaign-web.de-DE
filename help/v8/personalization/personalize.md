---
title: Personalisieren von Inhalten in Campaign
description: Erfahren Sie, wie Sie Inhalte in der Web-Benutzeroberfläche von Adobe Campaign personalisieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 79%

---


# Personalisieren von Inhalten{#add-personalization}

## Betreffzeile einer Nachricht personalisieren {#personalize-subject-line}

Um eine Personalisierung im Feld **[!UICONTROL Betreffzeile]** der Nachricht hinzuzufügen, gehen Sie wie folgt vor:

1. Öffnen Sie einen Versand und klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**.
1. Klicken Sie auf **[!UICONTROL Personalisierungsdialogfeld öffnen]** rechts neben dem **[!UICONTROL Betreff]** -Feld für E-Mails oder **[!UICONTROL Titel]** Felder für Push-/SMS-Sendungen.

   ![](assets/perso-subject.png){width="600"}

1. Geben Sie die Betreffzeile oder den Titel ein und wählen Sie die hinzuzufügenden Personalisierungsattribute aus.

1. Klicken Sie auf **[!UICONTROL Bestätigen]**, um die Eingaben zu bestätigen. Die Personalisierungsattribute werden dem Inhalt hinzugefügt.

## Personalisieren des E-Mail-Inhalts {#personalize-emails}

Um den E-Mail-Inhalt zu personalisieren, öffnen Sie die Nachricht im E-Mail-Designer und:

1. Klicken Sie auf einen Textblock.
1. Wählen Sie in der kontextbasierten Symbolleiste **[!UICONTROL Personalisierung hinzufügen]**.

   ![](assets/perso-add-to-content.png)

1. Fügen Sie den Namen der Empfängerin oder des Empfängers in den Personalisierungseditor ein und bestätigen Sie die Eingabe.

   ![](assets/perso-add-name.png)

   Das Personalisierungsattribut wird dem E-Mail-Inhalt hinzugefügt.

   Sie können den Inhalt simulieren, um das Rendering zu überprüfen. [Weitere Informationen](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. Um einen Inhaltsbaustein zu Ihrer E-Mail hinzuzufügen, führen Sie dieselben Schritte aus und wählen im letzten Symbol einen Inhaltsbaustein:

   ![](assets/perso-insert-block.png)

1. Nach dem Einfügen wird der Inhaltsbaustein dem E-Mail-Inhalt hinzugefügt. Er wird bei der Versandvorbereitung automatisch an das Empfängerprofil angepasst, wenn die Personalisierung generiert wird.

   ![](assets/perso-content-block-in-email.png)

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

