---
audience: end-user
title: Verwenden der Workflow-Aktivität „Dateiextraktion“
description: Informationen dazu, wie Sie die Workflow-Aktivität „Dateiextraktion“ verwenden
exl-id: fa50ab5b-2539-4517-9d7b-93315f1e505c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 100%

---

# Dateiextraktion {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Dateiextraktion"
>abstract="Die Aktivität **Dateiextraktion** erlaubt den Export von in Adobe Campaign enthaltenen Daten in Form einer externen Datei. Die Daten können dann mithilfe der Aktivität „Datei übertragen“ an einen Server-Speicherort wie SFTP, Cloud-Speicherplatz oder Ihren Kampagnen-Server exportiert werden."

Die Aktivität **Dateiextraktion** ist eine **Daten-Management-Aktivität**. Durch diese Aktivität können Sie in Adobe Campaign enthaltene Daten in Form einer externen Datei exportieren. Die Daten können dann mithilfe der Aktivität „Datei übertragen“ an einen Server-Speicherort wie SFTP, Cloud-Speicherplatz oder Ihren Kampagnen-Server exportiert werden.

Fügen Sie zum Konfigurieren der Aktivität **Datei extrahieren** eine Aktivität **Datei extrahieren** in Ihren Workflow ein und führen Sie dann die folgenden Schritte aus.

## Konfigurieren der zu extrahierenden Datei {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Zu extrahierende Datei"
>abstract="Wählen Sie die zu extrahierende Datei aus."

Im Abschnitt **[!UICONTROL Zu extrahierende Datei]** können Sie die Dateieigenschaften und die einzuschließenden Daten konfigurieren.

![Screenshot mit den Konfigurationsoptionen für die zu extrahierende Datei](../assets/extract-file-file.png)

1. Geben Sie im Feld **[!UICONTROL Dateiname]** den gewünschten Namen für die zu extrahierende Datei an. 

   Sie können den Namen der Datei mit Ereignisvariablen, Bedingungen und Datums-/Uhrzeitfunktionen personalisieren. Klicken Sie dazu auf das Symbol **[!UICONTROL Personalisierungsdialog öffnen]**, um den Ausdruckseditor zu öffnen. [Erfahren Sie, wie Sie mit Ereignisvariablen und dem Ausdruckseditor arbeiten.](../event-variables.md)

1. Geben Sie die Spalten an, die in der extrahierten Datei enthalten sein sollen. Gehen Sie dazu wie folgt vor:

   1. Klicken Sie auf die **[!UICONTROL Spalte „Ausgabe hinzufügen“]**.
   1. Wählen Sie das Attribut aus, das in der Spalte angezeigt werden soll, und bestätigen Sie dann die Auswahl. Die verfügbaren Attribute sind abhängig von der Zielgruppendimension des Workflows. [Erfahren Sie, wie Sie Attribute auswählen und zu den Favoriten hinzufügen](../../get-started/attributes.md).
   1. Nachdem die Spalte hinzugefügt wurde, können Sie den **[!UICONTROL Titel]** und das zugehörige **[!UICONTROL Attribut]** ändern.
   1. Wenn Sie eine Umwandlung auf die Spaltenwerte anwenden möchten, wählen Sie sie aus der Dropdown-Liste aus. Sie können beispielsweise alle Werte in der ausgewählten Spalte in Großbuchstaben umwandeln.

1. Wiederholen Sie diese Schritte, um so viele Spalten hinzuzufügen, wie in der Extraktionsdatei erforderlich sind. Um die Position einer Spalte zu ändern, verwenden Sie die Pfeile nach oben und unten.

1. Um alle doppelten Zeilen aus der extrahierten Datei zu entfernen, schalten Sie die Option **[!UICONTROL Duplikate löschen (Auflistung)]** ein.

1. Um die extrahierte Datei anhand eines Attributs zu sortieren, schalten Sie die Option **[!UICONTROL Sortierung aktivieren]** ein und wählen Sie dann das Attribut aus, nach dem die Datei sortiert werden soll, sowie die gewünschte Sortiermethode (aufsteigend oder absteigend). Sie können jedes Attribut aus der aktuellen Zielgruppendimension sortieren, unabhängig davon, ob es zu den Spalten der Datei hinzugefügt wurde oder nicht.

## Konfigurieren des Formats der extrahierten Datei {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Zielformat"
>abstract="Wählen Sie die verschiedenen Optionen aus, um zu konfigurieren, wie die extrahierte Datei formatiert werden soll."

Im Abschnitt **[!UICONTROL Zielformat]** können Sie konfigurieren, wie die extrahierte Datei formatiert werden soll.

1. Wählen Sie das **[!UICONTROL Ausgabeformat]** für die extrahierte Datei: **Text**, **Text in Spalten mit fester Breite**, **CSV (Excel)** oder **XML**.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Extraktionsformat]**, um auf bestimmte Optionen im Zusammenhang mit dem ausgewählten Format zuzugreifen. Erweitern Sie den folgenden Abschnitt, um weitere Informationen zu erhalten.

+++ Verfügbare Optionen für das Extraktionsformat

   * **[!UICONTROL Erste Zeile für Spaltenüberschrift verwenden]** (Text-/CSV[Excel]-Format): Schalten Sie diese Option ein, um die erste Spalte als Kopfzeile zu verwenden.
   * **[!UICONTROL Spaltentrennzeichen]** (Textformat): Geben Sie das Zeichen an, das in der Ausgabedatei als Spaltentrennzeichen verwendet werden soll.
   * **[!UICONTROL Zeichenfolgen-Trennzeichen]** (Textformat): Geben Sie an, wie Zeichenfolgen in der Ausgabedatei getrennt werden sollen.
   * **[!UICONTROL Zeilenumbruch]** (Textformat): Geben Sie an, wie Zeilenenden in der Ausgabedatei getrennt werden sollen.
   * **[!UICONTROL Kodierung]**: Wählen Sie die Kodierung für die Ausgabedatei aus.
   * **[!UICONTROL Datumsformat und Trennzeichen]**: Geben Sie an, wie Datumsangaben in der Ausgabedatei formatiert werden sollen.
   * **[!UICONTROL Zahlenformat]**: Geben Sie an, wie Zahlen in der Ausgabedatei formatiert werden sollen.
   * **[!UICONTROL Label anstelle der internen Werte der Auflistungen exportieren]**: Schalten Sie diese Option ein, wenn Sie Auflistungswerte exportieren und Spaltentitel abrufen möchten, die leichter verständlich sind als interne IDs.

+++

   ![Screenshot mit den Konfigurationsoptionen für die zu extrahierende Datei](../assets/extract-file-format.png)

## Hinzufügen eines Nachbearbeitungsschritts {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Nachbearbeitung"
>abstract="Definieren Sie einen Nachbearbeitungsschritt, wie beispielsweise Komprimieren oder Verschlüsseln."

Mit dem **[!UICONTROL Skript zur Änderung des Exports]** können Sie eine Verarbeitungsphase anwenden, die während der Datenextraktion ausgeführt wird, z. B. Komprimieren oder Verschlüsseln. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Script bearbeiten]**. 

Der Ausdruckseditor wird geöffnet und Sie können den Befehl eingeben, der auf die Datei angewendet werden soll. Der linke Seitenbereich enthält vordefinierte Syntaxen, die Sie zum Erstellen Ihres Skripts verwenden können. [Erfahren Sie, wie Sie mit Ereignisvariablen und dem Ausdruckseditor arbeiten](../event-variables.md).

![Screenshot mit dem Skripteditor für die Nachbearbeitung](../assets/extract-file-script.png)

## Weitere Optionen {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Ausgehende Transition"
>abstract="Schalten Sie die Option **Ausgehende Transition erzeugen** ein, um eine ausgehende Transition nach der aktuellen Aktivität hinzuzufügen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Fehler verarbeiten"
>abstract="Die Option **Fehler verarbeiten** einschalten, um eine fehlerhafte ausgehende Transition hinzuzufügen."

Sobald die Extraktion der Ausgabedatei konfiguriert wurde, stehen zusätzliche Optionen im Zusammenhang mit Transitionen und der Fehlerverwaltung zur Verfügung:

* **[!UICONTROL Ausgehende Transition erstellen]**: Schalten Sie diese Option ein, um eine ausgehende Transition hinzuzufügen und deren Titel zu konfigurieren.
* **[!UICONTROL Keine Datei erstellen, wenn die eingehende Transition leer ist]**: Schalten Sie diese Option ein, um die Dateiextraktion zu überspringen, wenn die eingehende Transition keine Daten enthält.
* **[!UICONTROL Fehler verarbeiten]**: Schalten Sie diese Option ein, um eine ausgehende Transition hinzuzufügen, wenn bei der Dateiextraktion ein Fehler auftritt.

## Beispiel {#example}

Im folgenden Beispiel folgt auf eine Aktivität **Zielgruppe erstellen** die Aktivität **Dateiextraktion**, um alle Zielgruppenprofile in eine CSV-Datei zu extrahieren.

![Screenshot eines beispielhaften Workflows mit der Aktivität „Zielgruppe erstellen“, gefolgt von der Aktivität „Dateiextraktion“](../assets/extract-file-example.png)

* Das Feld **[!UICONTROL Dateiname]** ist so konfiguriert, dass es das Datum der Extraktion enthält.

  ![Screenshot mit der Konfiguration des Dateinamens und dem darin enthaltenen Datum](../assets/extract-file-example-name.png)

* Es werden Spalten hinzugefügt, die die Vor- und Nachnamen der Profile, ihre Kunden-IDs und die Erstellungsdaten in der Datenbank anzeigen.

  ![Screenshot mit der Konfiguration der Spalten in der extrahierten Datei](../assets/extract-file-example-columns.png)