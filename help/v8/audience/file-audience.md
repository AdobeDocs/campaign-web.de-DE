---
audience: end-user
title: Empfänger aus einer Datei auswählen
description: Erfahren Sie, wie Sie mit Empfängern aus einer externen Datei E-Mail-Zielgruppen erstellen können.
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 7893f3132689446db388613ad5ec033ca5f26bf5
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 23%

---

# Empfänger aus einer Datei auswählen {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Datei auswählen"
>abstract="Wählen Sie die hochzuladende lokale Datei aus. Unterstützte Formate sind TXT und CSV. Passen Sie Ihr Dateiformat an die unten verlinkte Beispieldatei an."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Spaltendefinition"
>abstract="Überprüfen Sie das Format der Spalten, die aus Ihrer lokalen Datei eingefügt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formatierungsparameter"
>abstract="Überprüfen Sie die Formatierungsparameter für Ihre Datei."

Sie können Kontakte aus einer externen Datei hochladen. Diese Funktion ist nur für E-Mail-Sendungen verfügbar. Unterstützte Dateiformate sind: Text (TXT) und kommagetrennte Werte (CSV). Profile werden nicht zur Datenbank hinzugefügt, aber alle Felder in der Eingabedatei können personalisiert werden.

>[!NOTE]
>
>Sie können einen Import-Workflow erstellen, um mehrere Profile in der Datenbank hinzuzufügen oder zu aktualisieren. Weitere Informationen


Gehen Sie wie folgt vor, um Profile aus einer lokalen Datei direkt über die Benutzeroberfläche auszuwählen:

1. Wählen Sie im Fenster zur Erstellung des E-Mail-Versands im **Zielgruppe** klicken Sie auf die **Zielgruppe auswählen** und wählen Sie die **Aus Datei auswählen** -Option.

   ![](assets/select-from-file.png)

1. Wählen Sie die hochzuladende lokale Datei aus.
1. Im mittleren Bereich des Bildschirms können Sie eine Vorschau der Daten anzeigen und deren Zuordnung überprüfen.
1. Wählen Sie die Spalte aus, die die E-Mail-Adresse enthält. **Adressfeld** Dropdown-Liste. Sie können auch die Spalte Blockierungsliste auswählen, wenn diese Informationen in der Eingabedatei enthalten sind.
1. Passen Sie die Spalteneinstellungen an und wie Daten aus den verfügbaren Optionen formatiert werden.
1. Klicken Sie auf **Bestätigen**, wenn die Einstellungen korrekt sind.

Bei der Erstellung und Personalisierung des Nachrichteninhalts können Sie im Personalisierungseditor Felder aus der Eingabedatei auswählen.

![](assets/select-external-perso.png)

## Beispieldatei {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Beispieldatei"
>abstract="Unterstützte Dateiformate: txt, csv. Erste Zeile für Spaltentitel verwenden."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
