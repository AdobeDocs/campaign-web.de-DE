---
title: Inhalt in Campaign personalisieren
description: Erfahren Sie, wie Sie Ihren Inhalt in der Adobe Campaign-Web-Benutzeroberfläche personalisieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 2d23b04b81ab625de0936fdf058f6ac8bd1017c3
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 7%

---

# Personalisieren von Inhalten{#add-personalization}

![](../assets/do-not-localize/badge.png)

Sie können den Nachrichteninhalt wie folgt personalisieren:

* Dynamisches Einfügen **Personalisierungsfelder**

   Personalisierungsfelder werden zur Personalisierung Ihrer Nachrichten auf erster Ebene verwendet. Sie können jedes in der Datenbank verfügbare Feld aus dem Personalisierungseditor auswählen. Bei einem Versand können Sie ein beliebiges Feld auswählen, das mit dem Empfänger, der Nachricht oder dem Versand in Verbindung steht. Diese Personalisierungsattribute können in die Betreffzeile oder den Hauptteil Ihrer Nachrichten eingefügt werden.

   ![](assets/perso-subject-line.png)

   Mit der obigen Syntax wird die Stadt des Empfängers in Ihren Inhalt eingefügt: &lt;%= recipient.location.city %>.

* Vordefiniertes Einfügen **Inhaltsbausteine**

   Campaign verfügt über eine Reihe von Gestaltungsbausteinen, die ein bestimmtes Rendering enthalten, das Sie in Ihre Sendungen einfügen können. Sie können beispielsweise ein Logo, eine Grußnachricht oder einen Link zur Mirrorseite der Nachricht hinzufügen. Inhaltsbausteine sind über einen eigenen Eintrag im Personalisierungs-Editor verfügbar.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## E-Mail-Betreffzeile personalisieren {#personalize-subject-line}

So fügen Sie Personalisierung in der **[!UICONTROL Betreff]** Gehen Sie wie folgt vor:

1. Klicken Sie auf **Personalisierungsdialogfeld öffnen** rechts neben dem **Betreff** -Feld.
1. Geben Sie den Betreffzeileninhalt ein und wählen Sie die hinzuzufügenden Personalisierungsattribute aus.
1. Klicken Sie zur Validierung auf Bestätigen . Die Personalisierungsattribute werden der Betreffzeile hinzugefügt.

![](assets/perso-subject.png)

## E-Mail-Inhalt personalisieren {#personalize-emails}

Um den E-Mail-Inhalt zu personalisieren, öffnen Sie die Nachricht in Email Designer und:

1. Klicken Sie in einen Textblock.
1. Wählen Sie in der dedizierten Symbolleiste die Option **Personalisierung hinzufügen**.

   ![](assets/perso-add-to-content.png)

1. Fügen Sie den Namen des Empfängers in den Personalisierungs-Editor ein und bestätigen Sie die Eingabe.

   ![](assets/perso-add-name.png)

   Das Personalisierungsattribut wird dem E-Mail-Inhalt hinzugefügt.

   Sie können den Inhalt simulieren, um das Rendering zu überprüfen. [Weitere Informationen](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## Links in E-Mails personalisieren {#personalize-links}

So personalisieren Sie eine **link**:

1. Wählen Sie einen Textblock oder ein Bild aus.
1. Wählen Sie in der dedizierten Symbolleiste die Option **Personalisierung hinzufügen**.

   ![](assets/perso-link.png)

1. Verwenden Sie den Personalisierungs-Editor, um den Link zu definieren und zu personalisieren.

## Personalisieren von Angeboten {#personalize-offers}

Sie können auch den Personalisierungseditor nutzen, wenn Sie den Darstellungen Ihrer Angebote Textinhalte hinzufügen.
