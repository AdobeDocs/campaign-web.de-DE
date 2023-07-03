---
audience: end-user
title: Ansprechen von Empfängerinnen und Empfängern aus einer Datei
description: Erfahren Sie, wie Sie mit Empfängerinnen und Empfängern aus einer externen Datei eine E-Mail-Zielgruppe erstellen können.
badge: label="Alpha"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '326'
ht-degree: 100%

---

# Laden einer E-Mail-Zielgruppe aus einer Datei {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Auswahl der Datei"
>abstract="Wählen Sie die hochzuladende lokale Datei aus. Unterstützte Formate sind TXT und CSV. Richten Sie Ihr Dateiformat an der unten verlinkten Beispieldatei aus."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Spaltendefinition"
>abstract="Überprüfen Sie das Format der Spalten, die aus Ihrer lokalen Datei eingefügt werden sollen."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Formatierungsparameter"
>abstract="Überprüfen Sie die Formatierungsparameter für Ihre Datei."

Sie können Kontakte aus einer externen Datei hochladen. Profile werden nicht zur Datenbank hinzugefügt, aber alle Felder in der Eingabedatei können [personalisiert](../personalization/gs-personalization.md) werden. Unterstützte Dateiformate sind: Text (TXT) und kommagetrennte Werte (CSV).

>[!CAUTION]
>
>* Diese Funktion ist nur für **eigenständige E-Mail-Sendungen** verfügbar. Sie kann nicht in Workflows oder in SMS- oder Push-Sendungen verwendet werden.
>
>* Sie können keine [Kontrollgruppen](control-group.md) verwenden, wenn Sie die Zielgruppen-Population aus einer externen Datei laden.


Gehen Sie wie folgt vor, um Profile aus einer lokalen Datei direkt über die E-Mail-Benutzeroberfläche anzuvisieren:

1. Öffnen Sie einen vorhandenen E-Mail-Versand oder [erstellen Sie einen neuen](../email/create-email.md).
1. Klicken Sie im Fenster zur Erstellung des E-Mail-Versands im Abschnitt **Zielgruppe** auf die Schaltfläche **Zielgruppe auswählen** und wählen Sie die Option **Aus Datei auswählen** aus.

   ![](assets/select-from-file.png)

1. Wählen Sie die hochzuladende lokale Datei aus. Das Format muss der [Beispieldatei](#sample-file) entsprechen.
1. Im mittleren Abschnitt des Bildschirms können Sie eine Vorschau der Datenzuordnung anzeigen, um sie zu überprüfen.
1. Wählen Sie in der Dropdown-Liste **Adressfeld** die Spalte aus, die die E-Mail-Adresse enthält. Sie können auch die Spalte „Blockierungsliste“ auswählen, wenn diese Informationen in der Eingabedatei enthalten sind.
1. Passen Sie die Spalteneinstellungen an und wählen Sie aus den verfügbaren Optionen aus, wie Daten formatiert werden.
1. Klicken Sie auf **Bestätigen**, wenn die Einstellungen korrekt sind.

Bei der Erstellung und Personalisierung des Nachrichteninhalts können Sie im [Personalisierungseditor](../personalization/gs-personalization.md) Felder aus der Eingabedatei auswählen.

![](assets/select-external-perso.png)


## Beispieldatei {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Beispieldatei"
>abstract="Unterstützte Dateiformate: txt, csv. Verwenden Sie die erste Zeile für Spaltentitel."

Unterstützte Formate sind TXT und CSV. Die erste Zeile ist die Spaltenüberschrift.

Passen Sie Ihr Dateiformat an die unten stehende Beispieldatei an:

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
