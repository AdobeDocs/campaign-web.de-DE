---
audience: end-user
title: Importieren von Empfängerinnen und Empfängern aus einer Datei
description: Erfahren Sie, wie Sie Empfängerinnen und Empfänger aus einer externen Datei importieren
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f103fe804deccc83638a3e56a03f6e715e68e550
workflow-type: ht
source-wordcount: '175'
ht-degree: 100%

---

# Importieren von Empfängerinnen und Empfängern aus einer Datei {#audience-from-file}

Sie können Kontakte über die Versand-Schnittstelle hinzufügen oder aktualisieren, indem Sie eine Textdatei (TXT) oder eine Datei mit durch Komma getrennten Werten (CSV) hochladen. Sie werden dann der Datenbank hinzugefügt.

>[!NOTE]
>
>Sie können auch einen Import-Workflow erstellen, um mehrere Profile hinzuzufügen oder zu aktualisieren.


Gehen Sie wie folgt vor, um Profile aus einer lokalen Datei direkt über die Benutzeroberfläche hinzuzufügen:

1. Klicken Sie im Fenster zur Versanderstellung auf die Schaltfläche **Audience auswählen** und wählen Sie die Option **Aus Datei auswählen** aus.
1. Wählen Sie die hochzuladende lokale Datei aus.
1. Definieren Sie die Spalteneinstellungen und die Formatierung der Daten. Sie können mit dem Umschalter **Spalte ignorieren** eine Spalte überspringen.
1. Im mittleren Abschnitt des Bildschirms können Sie eine Vorschau der Datenzuordnung anzeigen.
1. Klicken Sie auf **Bestätigen**, wenn die Einstellungen korrekt sind.

Bei der Erstellung und Personalisierung des Nachrichteninhalts können Sie im Personalisierungseditor Felder aus der Eingabedatei auswählen.

## Beispieldatei {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Beispieldatei"
>abstract="Unterstützte Dateiformate: txt, csv, xls. Erste Zeile für Spaltentitel verwenden."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
