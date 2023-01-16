---
title: Inhalt in Campaign personalisieren
description: Erfahren Sie, wie Sie Ihren Inhalt in der Adobe Campaign-Web-Benutzeroberfläche personalisieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 46d8ac555e554faef91bcc817890466780387d0d
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 27%

---

# Personalisieren von Inhalten{#add-personalization}

![](../assets/do-not-localize/badge.png)

Sie können den Nachrichteninhalt wie folgt personalisieren:

* Dynamisches Einfügen **Personalisierungsfelder**

   Personalisierungsfelder werden zur Personalisierung Ihrer Nachrichten auf erster Ebene verwendet. Sie können jedes in der Datenbank verfügbare Feld aus dem Personalisierungseditor auswählen. Bei einem Versand können Sie ein beliebiges Feld auswählen, das mit dem Empfänger, der Nachricht oder dem Versand in Verbindung steht. Diese Personalisierungsattribute können in die Betreffzeile oder den Text Ihrer Nachrichten eingefügt werden.

   ![](assets/perso-subject-line.png)

   Mit der folgenden Syntax wird die Stadt des Empfängers in Ihren Inhalt eingefügt: &lt;%= recipient.location.city %>.

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
1. Klicken **Bestätigen** validieren. Die Personalisierungsattribute werden der Betreffzeile hinzugefügt.

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

Gehen Sie wie folgt vor, um einen Inhaltsbaustein zu Ihrer E-Mail hinzuzufügen:

![](assets/perso-insert-block.png)

Nach dem Einfügen wird der Inhaltsbaustein wie unten dargestellt zum E-Mail-Inhalt hinzugefügt. Er wird bei der Personalisierung automatisch an das Empfängerprofil angepasst, wenn die Versandvorbereitung erfolgt.

![](assets/perso-content-block-in-email.png)


Integrierte Inhaltsbausteine sind:
* **[!UICONTROL Aktiviert von Adobe Campaign]** : fügt das Logo &quot;Aktiviert durch Adobe Campaign&quot;ein.
* **[!UICONTROL Formatierungsfunktion für Eigennamen]**: Hiermit wird die JavaScript-Funktion **[!UICONTROL toSmartCase]** erstellt, mit der der erste Buchstabe eines jeden Worts in einen Großbuchstaben umgewandelt wird.
* **[!UICONTROL Grußformeln]**: Hiermit werden Grußformeln mit dem Empfängernamen eingefügt, z. B. &quot;Guten Tag, Max Mustermann&quot;.
* **[!UICONTROL Logo einfügen]**: Hiermit wird ein natives Logo eingefügt, das beim Konfigurieren der Instanz definiert wurde.
* **[!UICONTROL Link zur Mirror-Seite]**: Hiermit wird der Link zur Mirror-Seite „Wenn die Nachricht nicht richtig angezeigt wird, bitte hier klicken“ eingefügt.
* **[!UICONTROL Mirrorseiten-URL]**: Hiermit wird die Mirrorseiten-URL eingefügt, damit Versanddesigner den Link prüfen können.
* **[!UICONTROL Annahme-URL des Angebots im Einzelmodus]** : fügt eine URL ein, mit der ein Interaction-Angebot auf **[!UICONTROL Akzeptiert]**.
* **[!UICONTROL URL der Registrierungsseite]** : fügt eine Anmelde-URL ein.
* **[!UICONTROL Anmelde-Link]**: Hiermit wird ein Anmelde-Link eingefügt. Dieser Link muss beim Konfigurieren der Instanz definiert werden. Der Standardinhalt lautet: &quot;Klicken Sie hier, um sich zu registrieren.&quot;
* **[!UICONTROL Registrierungslink (mit Werber)]**: Hiermit wird ein Anmelde-Link eingefügt, über den der Besucher und der Versand identifiziert werden kann. Der Link wurde beim Konfigurieren der Instanz definiert.
* **[!UICONTROL Anmeldebestätigung]**: Hiermit wird ein Link eingefügt, mit dem die Anmeldung bestätigt werden kann.
* **[!UICONTROL Teilen-Links sozialer Netzwerke]** : Hiermit werden Schaltflächen eingefügt, mit denen der Empfänger einen Link zum Inhalt der Mirrorseite freigeben kann.
* **[!UICONTROL Stil der Inhalts-E-Mails]** und **[!UICONTROL Stil der Benachrichtigungen]**: Hiermit wird Code erstellt, mit dem eine E-Mail mit nativen HTML-Stilen formatiert werden kann.
* **[!UICONTROL Abmelde-Link]**: Hiermit wird ein Link zur Abmeldung von allen Nachrichten (Blockierungsliste) eingefügt. Der standardmäßig verknüpfte Inhalt ist: &quot;Sie erhalten diese Nachricht, da Sie mit `<your rganization name>` oder einem Affiliate. So empfangen Sie keine Nachrichten mehr von `<your rganization name>` Klicken Sie hier.&quot;


## Links in E-Mails personalisieren {#personalize-links}

So personalisieren Sie eine **link**:

1. Wählen Sie einen Textblock oder ein Bild aus.
1. Wählen Sie in der dedizierten Symbolleiste die Option **Link einfügen**.

   ![](assets/perso-link.png)

1. Geben Sie den Link-Titel ein und verwenden Sie die **Link einfügen** -Schaltfläche, um den Link zu personalisieren.

   ![](assets/perso-link-insert-icon.png)

1. Verwenden Sie den Personalisierungs-Editor, um den Link zu definieren und zu personalisieren und zu bestätigen.

   ![](assets/perso-link-edit.png)


## Personalisieren von Angeboten {#personalize-offers}

Sie können auch den Personalisierungseditor nutzen, wenn Sie den Darstellungen Ihrer Angebote Textinhalte hinzufügen. Weiterführende Informationen finden Sie in [diesem Abschnitt](../content/offers.md).
