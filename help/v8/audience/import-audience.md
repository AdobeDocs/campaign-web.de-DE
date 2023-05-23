---
audience: end-user
title: Empfänger aus einer Datei auswählen
description: Erfahren Sie, wie Sie mit Empfängern aus einer externen Datei E-Mail-Zielgruppen erstellen können.
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Empfänger aus einer Datei auswählen {#audience-from-file}

Sie können Kontakte aus einer externen Datei hochladen. Diese Funktion ist nur für E-Mail-Sendungen verfügbar. Folgende Formate werden unterstützt: Textdatei (TXT) oder eine kommagetrennte Wertdatei (CSV). Sie werden dann der Datenbank hinzugefügt.

>[!NOTE]
>
>Sie können einen Import-Workflow erstellen, um mehrere Profile hinzuzufügen oder zu aktualisieren.  Weitere Informationen


Gehen Sie wie folgt vor, um Profile aus einer lokalen Datei direkt über die Benutzeroberfläche auszuwählen:

1. Klicken Sie im Erstellungsfenster des E-Mail-Versands auf die Schaltfläche **Zielgruppe auswählen** und wählen Sie die **Aus Datei auswählen** -Option.

   ![](assets/select-from-file.png)

1. Wählen Sie die hochzuladende lokale Datei aus.
1. Im mittleren Abschnitt des Bildschirms können Sie eine Vorschau der Datenzuordnung anzeigen.
1. Wählen Sie die Spalte aus, die die E-Mail-Adresse enthält. **Adressfeld** Dropdown-Liste.
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
