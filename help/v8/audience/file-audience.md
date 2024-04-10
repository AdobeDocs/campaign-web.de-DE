---
audience: end-user
title: Laden einer E-Mail-Zielgruppe aus einer Datei
description: Erfahren Sie, wie Sie Profile aus einer externen Datei laden, um eine E-Mail-Zielgruppe zu erstellen.
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 64%

---

# Laden einer E-Mail-Zielgruppe aus einer Datei {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Auswahl der Datei"
>abstract="Wählen Sie die hochzuladende lokale Datei aus. Unterstützte Formate sind TXT und CSV. Richten Sie Ihr Dateiformat an der unten verlinkten Beispieldatei aus."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Spaltendefinition"
>abstract="Überprüfen Sie das Spaltenformat der externen Datei."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formatierungsparameter"
>abstract="Definieren Sie das Format der externen Datei, sodass die Daten korrekt importiert werden können."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Anzeige der Datei in der Vorschau"
>abstract="Überprüfen Sie die Spaltenvorschau der externen Datei. Dieser Bildschirm zeigt nur maximal 30 Einträge an."

Mit der Web-Benutzeroberfläche von Adobe Campaign können Sie Profile auswählen, die in einer externen Datei gespeichert sind. Sobald die Profile geladen wurden, können alle Felder aus der Eingabedatei zur Personalisierung Ihres Versands verwendet werden [Erfahren Sie, wie Sie Ihre Inhalte personalisieren können](../personalization/personalize.md).

Profile aus der Eingabedatei werden nicht zur Datenbank hinzugefügt. Sie sind nur für diesen eigenständigen E-Mail-Versand geladen und verfügbar.

>[!NOTE]
>
>Auf dieser Seite wird beschrieben, wie Sie beim Erstellen eines eigenständigen E-Mail-Versands externe Profile aus einer Datei laden. Informationen zum Laden von Daten aus einer Datei im Kontext eines Workflows finden Sie unter [Diese Seite](../workflows/activities/load-file.md).

## Wichtige Informationen {#must-read}

* Diese Funktion ist verfügbar für **E-Mail-Sendungen** Nur.
* Unterstützte Dateiformate sind: Text (TXT) und kommagetrennte Werte (CSV).
* Sie können keine [Kontrollgruppen](control-group.md) verwenden, wenn Sie die Zielgruppenpopulation aus einer externen Datei laden.

## Eingabedatei auswählen und konfigurieren {#upload}

Gehen Sie wie folgt vor, um Profile aus einer Datei in Ihren E-Mails auszuwählen:

1. Öffnen Sie einen vorhandenen E-Mail-Versand oder [erstellen Sie einen neuen](../email/create-email.md).
1. In der **Zielgruppe** klicken Sie auf das Symbol **Zielgruppe auswählen** Schaltfläche und anschließend Auswählen **Aus Datei auswählen**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. Wählen Sie die zu ladende lokale Datei aus. Das Dateiformat muss dem [Musterdatei](#sample-file).
1. Im mittleren Abschnitt des Bildschirms können Sie eine Vorschau der Datenzuordnung anzeigen, um sie zu überprüfen.

   ![](assets/select-from-file-map.png)

1. Geben Sie die Spalte an, die die E-Mail-Adresse aus der **Adressfeld** Dropdown-Liste. Sie können auch die Spalte „Blockierungsliste“ auswählen, wenn diese Informationen in der Eingabedatei enthalten sind.
1. Passen Sie die Spalteneinstellungen an und wählen Sie aus den verfügbaren Optionen aus, wie die Daten formatiert werden.
1. Klicken Sie auf **Bestätigen**, wenn die Einstellungen korrekt sind.

Beim Erstellen des Nachrichteninhalts können Sie eine Personalisierung hinzufügen, indem Sie Felder aus der Eingabedatei verwenden. [Erfahren Sie, wie Sie Inhalte personalisieren](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## Beispieldatei {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Laden einer Zielgruppe aus einer Datei"
>abstract="Unterstützte Dateiformate sind TXT und CSV. Erste Zeile für Spaltentitel verwenden. Dateiformat an die Beispieldatei anpassen, die im folgenden Link bereitgestellt wird."

Stellen Sie beim Laden einer externen Datei in Zielprofile in Ihren Sendungen sicher, dass die Eingabedatei den folgenden Empfehlungen entspricht:

* Unterstützte Formate sind TXT und CSV.
* Die erste Zeile in der Datei ist die Spaltenüberschrift.
* Passen Sie Ihr Dateiformat an die unten stehende Beispieldatei an:

  ```javascript
  {
  lastname,firstname,city,birthdate,email,denylist
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
  }
  ```

## Erstellen einer E-Mail-Vorschau und Testen einer E-Mail {#test}

Campaign Web ermöglicht Ihnen die Vorschau und das Versenden von Testsendungen, wenn Sie eine Zielgruppe verwenden, die aus einer Datei hochgeladen wurde. Gehen Sie dazu wie folgt vor:

1. Klicken Sie auf die **[!UICONTROL Schaltfläche „Inhalt simulieren“]** im Bearbeitungsbildschirm des Versandinhalts und klicken Sie dann auf die Schaltfläche **[!UICONTROL Testprofil(e) hinzufügen]**.

1. Die in der hochgeladenen Datei enthaltenen Profile werden angezeigt. Wählen Sie die Profile aus, die Sie für die Vorschau Ihres Inhalts verwenden möchten, und klicken Sie auf **[!UICONTROL Auswählen]**.

1. Eine Vorschau des Versandinhalts wird im rechten Bereich des Bildschirms angezeigt. Personalisierte Elemente werden durch die Daten aus dem Profil ersetzt, das im linken Bereich ausgewählt wurde. [Weitere Informationen zur Inhaltsvorschau eines Versands](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. Um Testsendungen durchzuführen, klicken Sie auf die Schaltfläche **[!UICONTROL Testsendung durchführen]**.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Testprofile hochladen]** und wählen Sie die TXT- oder CSV-Datei aus, die Ihre Testversand-Empfängerinnen und -Empfänger enthält.

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass das Dateiformat mit dem Format übereinstimmt, das für das Hochladen Ihrer Zielgruppe verwendet wird. Bei Formatfehlern wird ein Warnhinweis angezeigt.

1. Wenn die Testversand-Profile hinzugefügt wurden und Sie bereit sind, die Testsendungen durchzuführen, klicken Sie auf die Schaltfläche **[!UICONTROL Testversand durchführen]** und bestätigen dann das Senden.

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. Sie können den Versand der Testsendung jederzeit mithilfe der Schaltfläche **[!UICONTROL Testsendung anzeigen]** überwachen. [Weitere Informationen zur Überwachung von Testsendungen](../preview-test/test-deliveries.md#access-test-deliveries)
