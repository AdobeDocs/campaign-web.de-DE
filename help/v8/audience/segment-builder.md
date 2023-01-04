---
audience: end-user
title: Arbeiten mit dem Segment Builder
description: Web-Dokumentation zu Campaign v8
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: bf55b13011f7d2bdafcc55b1b2539c4ce590dd85
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 98%

---

# Arbeiten mit dem Segment Builder {#segment-builder}

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

In diesem Abschnitt wird beschrieben, wie Sie beim Entwerfen einer neuen E-Mail eine Audience erstellen. Die erstellte Audience kann nur in dieser E-Mail verwendet werden.

Mit Segment Builder können Sie die Audience Ihrer Nachricht definieren, indem Sie in der Adobe Campaign-Datenbank enthaltene Daten filtern. Informationen zur Auswahl einer bereits bestehenden Audience finden Sie in [diesem Abschnitt](add-audience.md).

Weitere Informationen zum Segment Builder finden Sie in der [Dokumentation zum Segmentierungs-Service](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

Gehen Sie wie folgt vor, um beim Entwerfen einer E-Mail eine neue Audience zu erstellen:

1. Klicken Sie im Abschnitt **Audience** des Assistenten zur Versanderstellung auf die Schaltflache **[!UICONTROL Audience auswählen]** .

   ![](assets/segment-builder0.png)

1. Wählen Sie **Eigene erstellen** aus. Der Segment Builder wird angezeigt.

   ![](assets/segment-builder.png)

## Die Palette

Die Palette auf der linken Seite enthält alle Elemente, nach denen Sie filtern können, um Ihre Audience zu erstellen. Die in der Palette enthaltenen Kacheln müssen in die mittlere Arbeitsfläche verschoben werden, damit sie konfiguriert und berücksichtigt werden können. Die Palette ist in zwei Registerkarten unterteilt:

* **Attribute**: Auf dieser Registerkarte können Sie auf alle verfügbaren Felder des Schemas zugreifen. Die Liste der Felder hängt von dem in der E-Mail-Vorlage definierten Zielgruppenbestimmungsschema ab.

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **Audiences**: In dieser Registerkarte können Sie mithilfe der in der Campaign Classic-Konsole definierten bestehenden Audiences filtern.

   ![](assets/segment-builder3.png){width="70%" align="left"}

Sie können die Suchleiste verwenden, um Elemente schnell zu finden.

## Die Arbeitsfläche

Die Arbeitsfläche ist der zentrale Bereich des Bildschirms, in dem Sie die Regeln basierend auf den aus der Palette hier abgelegten Elementen konfigurieren und kombinieren können. Um eine neue Regel hinzuzufügen, ziehen Sie eine Kachel aus der Palette auf die Arbeitsfläche. Anschließend erhalten Sie je nach hinzugefügtem Datentyp kontextspezifische Optionen.

![](assets/segment-builder4.png){width="70%" align="left"}

## Der Bereich mit den Regeleigenschaften

Auf der rechten Seite können Sie im Bereich **Regeleigenschaften** die folgenden Aktionen ausführen:

![](assets/segment-builder5.png){width="70%" align="left"}

* **Ergebnisse anzeigen:** zeigt die Liste der von der Audience angesprochenen Empfänger an
* **Code-Ansicht**: Zeigt eine Code-basierte Version der Audience in SQL an.
* **Erweiterte Attribute anzeigen**: Aktivieren Sie diese Option, wenn Sie die vollständige Liste der Attribute in der linken Palette anzeigen möchten: Knoten, Gruppierungen, 1:1-Links, 1:n-Links.
* **Attribute**: zeigt eine Beschreibung der erstellten Audience an.

## Beispiel

In diesem Beispiel erstellen wir eine Audience, um alle Kunden anzusprechen, die in Atlanta oder Seattle leben und nach 1980 geboren wurden.

1. Suchen Sie in der Registerkarte **Attribute** der Palette nach dem Feld **Geburtsdatum**. Ziehen Sie die Kachel und legen Sie sie auf der Arbeitsfläche ab.

   ![](assets/segment-builder6.png)

1. Wählen Sie auf der Arbeitsfläche den Operator **Nach** und geben Sie das gewünschte Datum ein.

   ![](assets/segment-builder7.png)

1. Suchen Sie in der Palette nach dem Feld **Ort** und fügen Sie es unterhalb der ersten Regel zur Arbeitsfläche hinzu.

   ![](assets/segment-builder8.png)

1. Geben Sie im Textfeld den Vornamen des Ortes ein und drücken Sie dann die Eingabetaste.

   ![](assets/segment-builder9.png)

1. Wiederholen Sie diese Aktion für den zweiten Stadtnamen.

   ![](assets/segment-builder10.png)

1. Klicken Sie auf **Ergebnisse anzeigen**, um die Liste und die Anzahl der Empfänger anzuzeigen, die der Abfrage entsprechen.

   ![](assets/segment-builder11.png)

1. Klicken Sie auf **Bestätigen**.

Ihre Audience ist definiert und kann in Ihrer E-Mail verwendet werden.