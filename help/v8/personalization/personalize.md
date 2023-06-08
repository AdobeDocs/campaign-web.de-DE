---
title: Personalisieren von Inhalten in Campaign
description: Erfahren Sie, wie Sie Inhalte in der Web-Benutzeroberfläche von Adobe Campaign personalisieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

---


# Personalisieren von Inhalten{#add-personalization}

Die Personalisierung kann jedem Versand mithilfe des Ausdruckseditors hinzugefügt werden.

Ein Personalisierungs-Tag verwendet immer die folgende Syntax: `<%=table.field%>`.Um beispielsweise den in der Empfängertabelle gespeicherten Empfängernamen einzufügen, verwendet das Personalisierungs-Tag die Syntax &lt;%= recipient.lastName %> .

Bei der Vorbereitung eines Versands werden diese Tags automatisch von Adobe Campaign interpretiert und durch den Feldwert für einen bestimmten Empfänger ersetzt. Der physische Austausch kann dann bei der Simulation Ihres Inhalts angezeigt werden.

Um einem Versand Personalisierungs-Tags hinzuzufügen, klicken Sie auf das Symbol Personalisierungsdialogfeld öffnen , auf das über Textbearbeitungsfelder wie die Betreffzeile oder den SMS-Textkörper zugegriffen werden kann.

![](assets/perso-access.png)

Der Ausdruckseditor wird angezeigt. Personalisierungsfelder sind in drei Menüs auf der linken Bildschirmseite unterteilt. Über diese Menüs haben Sie Zugriff auf alle in der Adobe Campaign-Datenbank verfügbaren Felder.

| Menü | Beschreibung |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | Die **[!UICONTROL Empfänger]** listet alle in der Empfängertabelle definierten Felder auf, z. B. den Namen, das Alter oder die Adresse des Empfängers. |
| ![](assets/do-not-localize/perso-message-menu.png) | Die **[!UICONTROL Nachricht]** enthält alle Felder, die mit den Versandlogs in Verbindung stehen, d. h. alle Nachrichten, die über alle Kanäle an Empfänger oder Geräte gesendet werden, z. B. das Datum des letzten Ereignisses mit einem bestimmten Empfänger |
| ![](assets/do-not-localize/perso-delivery-menu.png) | Die **[!UICONTROL Versand]** listet alle Felder auf, die mit den für die Durchführung des Versands erforderlichen Parametern verknüpft sind, wie z. B. den Versandkanal, den Titel usw. |

>[!NOTE]
>
>Standardmäßig enthält die Liste alle Felder der ausgewählten Tabelle (Empfänger, / Nachricht / Versand). Wenn Sie Felder aus mit der ausgewählten Tabelle verknüpften Tabellen einbeziehen möchten, aktivieren Sie die **[!UICONTROL Erweiterte Attribute anzeigen]** Option unterhalb der Liste.

Um ein Personalisierungsfeld hinzuzufügen, platzieren Sie den Cursor an der gewünschten Stelle in Ihrem Inhalt und klicken Sie auf die Schaltfläche + , um es einzufügen.

![](assets/perso-insert-field.png)

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


## Personalisieren von Angeboten {#personalize-offers}

Sie können mit dem Personalisierungseditor auch Textinhalte zu den Darstellungen Ihrer Angebote hinzufügen. Weiterführende Informationen finden Sie in [diesem Abschnitt](../content/offers.md).

