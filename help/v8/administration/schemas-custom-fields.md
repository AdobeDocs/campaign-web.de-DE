---
title: Bearbeiten benutzerdefinierter Felder
description: Erfahren Sie, wie Sie benutzerdefinierte Felder und ihre Sichtbarkeit in der Benutzeroberfläche konfigurieren.
exl-id: 1b531722-0935-4787-a673-60d97f776936
source-git-commit: 6f835141111dbacac0b6e1156f744d3f8db9ae24
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 95%

---

# Bearbeiten benutzerdefinierter Felder {#fields}

>[!CONTEXTUALHELP]
>id="acw_schema_detail_screen_configuration"
>title="Konfiguration des Detailbildschirms"
>abstract="Legen Sie fest, welche benutzerdefinierten Felder auf Detailbildschirmen angezeigt werden, und gliedern Sie sie in Abschnitte. Sammlungslisten hinzufügen, um verwandte Daten in Profilbildern anzuzeigen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/conf/schemas/schemas-collection-lists.html?lang=de" text="Hinzufügen von Sammlungslisten"

Benutzerdefinierte Felder sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zu vorkonfigurierten Schemata hinzugefügt werden. Sie ermöglichen es Ihnen, Schemata anzupassen, indem neue Attribute entsprechend den Anforderungen Ihrer Organisation eingefügt werden.

Benutzerdefinierte Felder können auf verschiedenen Bildschirmen angezeigt werden, z. B. in den Profildetails der Benutzeroberfläche. Sie können steuern, welche Felder sichtbar sind und wie sie in der Oberfläche angezeigt werden.

Weitere Informationen zum Bildschirm-„Bildschirmdefinition“ und zum Zugriff darauf finden Sie im Abschnitt [Zugreifen auf die Bildschirmdefinition](schemas-browse-access.md#screen-def).

So fügen Sie der Liste benutzerdefinierte Felder hinzu:

1. Navigieren Sie zum Menü **[!UICONTROL Schemata]** und suchen Sie mithilfe der Filter nach bearbeitbaren Schemata.

1. Wählen Sie den Schemanamen in der Liste aus, um das Schema zu öffnen, und klicken Sie in der Ansicht der Schemadetails auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**, um die Bildschirmdefinition aufzurufen.

1. Klicken Sie oberhalb der Tabelle **[!UICONTROL Liste der benutzerdefinierten Felder]** auf das Symbol mit den Auslassungspunkten und wählen Sie **[!UICONTROL Attribute auswählen]**, um ein oder mehrere benutzerdefinierte Felder auszuwählen, die in der Benutzeroberfläche angezeigt werden sollen.
   ![Bildschirm für benutzerdefinierte Felder mit bearbeitbaren Attributen](assets/schemas-custom5.png)
1. Wählen Sie die benutzerdefinierten Felder aus, die Sie hinzufügen möchten, und bestätigen Sie die Auswahl.

   ![Bildschirm für benutzerdefinierte Felder mit bearbeitbaren Attributen](assets/schemas-custom2.png)

   >[!NOTE]
   >
   > Sie können auch die Option **[!UICONTROL Liste der benutzerdefinierten Felder automatisch ausfüllen]** auswählen, um der Benutzeroberfläche alle für das Schema definierten benutzerdefinierten Felder hinzuzufügen.

Nachdem benutzerdefinierte Felder hinzugefügt wurden, können Sie sie in der Vorschau anzeigen, neu anordnen, als obligatorisch festlegen, ihre Einstellungen bearbeiten oder in Unterabschnitten organisieren.

## Konfigurieren von Feldeinstellungen {#field-settings}

Um bestimmte Einstellungen für jedes benutzerdefinierte Feld zu konfigurieren, klicken Sie in der Liste in der Zeile des gewünschten Felds auf das Symbol mit den Auslassungspunkten und wählen Sie **[!UICONTROL Bearbeiten]** aus.

![Dialog „Attributeinstellungen“](assets/schemas-attribute-settings.png)

Folgende Einstellungen sind verfügbar:

* **[!UICONTROL Attribut:]** Der Name des benutzerdefinierten Felds (schreibgeschützt).
* **[!UICONTROL Titel (benutzerdefiniert)]**: Der Titel, der in der Benutzeroberfläche angezeigt werden soll. Wenn kein Titel angegeben wird, wird der im Schema definierte Titel angezeigt.
* **[!UICONTROL In folgenden Fällen sichtbar]**: Definieren Sie eine Bedingung mithilfe eines xtk-Ausdrucks, der steuert, wann das Feld angezeigt wird. Blenden Sie beispielsweise dieses Feld aus, wenn ein anderes Feld leer ist.
* **[!UICONTROL Pflichtfeld]**: Legt das Feld in der Benutzeroberfläche als Pflichtfeld fest.
* **[!UICONTROL Schreibgeschützt]**: Legt das Feld in der Benutzeroberfläche als schreibgeschützt fest. Benutzende können den Wert des Felds nicht bearbeiten.
* **[!UICONTROL Filtereinstellungen]** (für Felder vom Typ „Link“): Verwenden Sie den Abfrage-Modeler, um Regeln für die Anzeige eines benutzerdefinierten Felds vom Typ „Link“ anzugeben. Beschränken Sie beispielsweise Listenwerte auf Grundlage der Eingabe eines anderen Felds.

  +++Beispiel anzeigen

  Sie können mit der Syntax `$(<field-name>)` auch den Wert referenzieren, der in andere Felder in Ihren Bedingungen eingegeben wurde. Auf diese Weise können Sie auf den aktuellen Wert eines Felds verweisen, wie er im Formular eingegeben wurde, auch wenn dieser noch nicht in der Datenbank gespeichert wurde.

  Im folgenden Beispiel prüft die Bedingung, ob der Wert des Felds @ref mit dem im Feld @refCom eingegebenen Wert übereinstimmt. Wenn Sie dagegen `@refCom` anstelle von `$(@refCom)` verwenden, wird auf den Wert des Felds @ref verwiesen, so wie in der Datenbank vorhanden.

  ![Screenshot mit einem Beispiel für Filtereinstellungen für benutzerdefinierte Felder](assets/custom-fields-ref.png)

  +++

* **[!UICONTROL Zwei Spalten umfassen]**: Standardmäßig werden benutzerdefinierte Felder in der Benutzeroberfläche in zwei Spalten angezeigt. Diese Option einschalten, um das benutzerdefinierte Feld über die gesamte Breite des Bildschirms und nicht in zwei Spalten anzuzeigen.

## Vorschau von benutzerdefinierten Feldern {#preview}

Klicken Sie auf **[!UICONTROL Vorschau]**, um die benutzerdefinierten Felder auf einem Beispielbildschirm anzuzeigen. Auf diese Weise können Sie sehen, wie die Felder in der Benutzeroberfläche angezeigt werden, einschließlich der Felder, die als Pflichtfelder markiert sind.

![Vorschau benutzerdefinierter Felder](assets/schemas-custom4.png)

## Organisieren von Feldern in Unterabschnitten {#separator}

Sie können Trennzeichen hinzufügen, um benutzerdefinierte Felder in der Benutzeroberfläche zu gruppieren und so die Lesbarkeit zu verbessern. Gehen Sie dazu wie folgt vor:

1. Klicken Sie oberhalb der Tabelle **[!UICONTROL Liste der benutzerdefinierten Felder]** auf das Symbol mit den Auslassungspunkten und wählen Sie **[!UICONTROL Trennzeichen hinzufügen]** aus.

1. Der Liste wird eine neue Zeile für das Trennzeichen hinzugefügt. Klicken Sie in der Zeile „Trennzeichen“ auf das Symbol mit den Auslassungspunkten und wählen Sie **[!UICONTROL Bearbeiten]**.

1. Geben Sie einen **[!UICONTROL Label]** für das Trennzeichen ein und legen Sie (optional) eine **[!UICONTROL In folgenden Fällen sichtbar]**-Bedingung fest, um zu steuern, wann das Trennzeichen angezeigt wird.

   ![Dialog „Trennzeicheneigenschaften“](assets/schemas-custom3.png)

1. Verschieben Sie das Trennzeichen mithilfe der Pfeile nach oben und unten an die gewünschte Position. Die unter dem Trennzeichen aufgelisteten Felder werden darunter gruppiert.

   In diesem Beispiel werden die Felder „Interessante Sammlungen“ und „Marke“ im Unterabschnitt „Sammlung“ gruppiert.

   | Konfiguration benutzerdefinierter Felder | Rendern in der Benutzeroberfläche |
   |  ---  |  ---  |
   | ![Screenshot mit der Konfiguration eines Trennzeichens](assets/custom-fields-separator.png){zoomable="yes"} | ![Screenshot, der das Rendern eines Unterabschnitts in der Benutzeroberfläche zeigt](assets/custom-fields-section.png){zoomable="yes"} |
