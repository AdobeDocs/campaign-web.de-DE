---
audience: end-user
title: Erstellen einer Zielgruppe mit dem Campaign-Regel-Builder
description: Erfahren Sie, wie Sie mit dem Regel-Builder arbeiten
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: ht
source-wordcount: '613'
ht-degree: 100%

---

# Arbeiten mit dem Regel-Builder {#segment-builder}

Mit Regel-Builder können Sie die Population definieren, die mit Ihrem Versand angesprochen werden soll, indem Sie in der Datenbank enthaltene Daten filtern. Sie können damit eine Zielgruppe aus einem Workflow erstellen, indem Sie die Aktivität **[!UICONTROL Zielgruppe erstellen]** verwenden, oder beim Erstellen eines Versands eine Zielgruppe direkt als einmalige Zielgruppe erstellen.

* [Informationen zum Erstellen und Speichern einer Zielgruppe](create-audience.md)
* [Erfahren Sie, wie Sie eine einmalige Zielgruppe für einen Versand erstellen.](one-time-audience.md)

## Die Palette

Die Palette auf der linken Seite enthält alle Elemente, nach denen Sie filtern können, um Ihre Zielgruppe zu erstellen. Verwenden Sie die Suchleiste, um Elemente schnell zu finden. Verschieben Sie die in der Palette enthaltenen Kacheln in die mittlere Arbeitsfläche, damit sie konfiguriert und berücksichtigt werden können.

![Die Benutzeroberfläche der Palette mit Filteroptionen und Registerkarten](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

Die Palette ist in zwei Registerkarten unterteilt:

* **Attribute**: Diese Registerkarte bietet Zugriff auf alle verfügbaren Felder des Schemas. Die Liste der Felder hängt von dem in der E-Mail-Vorlage definierten Zielgruppenbestimmungsschema ab.

* **Zielgruppen**: Auf dieser Registerkarte können Sie über einen Filter eine der vorhandenen Zielgruppen auswählen, die in der Campaign Classic-Konsole oder in Adobe Experience Platform definiert sind. Weitere Informationen dazu, wie Sie Zielgruppen überwachen und erstellen, erfahren Sie in [diesem Abschnitt](manage-audience.md).

  >[!NOTE]
  >
  >Um Adobe Experience Platform-Zielgruppen zu nutzen, müssen Sie die Integration mit Zielen konfigurieren. Weitere Informationen finden Sie in der [Dokumentation zu Adobe Experience Platform-Zielen](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=de){target="_blank"}.

## Die Arbeitsfläche

Die Arbeitsfläche ist der zentrale Bereich, in dem Sie die Regeln basierend auf den aus der Palette hier abgelegten Elementen konfigurieren und kombinieren können. Um eine neue Regel hinzuzufügen, ziehen Sie eine Kachel aus der Palette auf die Arbeitsfläche. Je nach Art der hinzuzufügenden Daten werden Ihnen dann kontextspezifische Optionen angezeigt.

![Die Benutzeroberfläche der Arbeitsfläche mit Optionen für die Regelkonfiguration](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## Der Bereich „Regeleigenschaften“

Auf der rechten Seite können Sie im Bereich **Regeleigenschaften** die folgenden Aktionen ausführen.

![Der Bereich „Regeleigenschaften“ mit den verfügbaren Aktionen](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Ergebnisse anzeigen:** Zeigt die Liste der von der Zielgruppe angesprochenen Profile an.
* **Code-Ansicht**: Zeigt eine Code-basierte Version der Zielgruppe in SQL an.
* **Erweiterte Attribute anzeigen**: Aktivieren Sie diese Option, um die vollständige Liste der Attribute in der linken Palette anzuzeigen: Knoten, Gruppierungen, 1:1-Links und 1:n-Links.
* **Berechnen**: Aktualisiert und zeigt die Anzahl der Profile an, die von Ihrer Abfrage angesprochen werden.
* **Filter auswählen oder speichern**: Verwenden Sie einen vordefinierten Filter, um Ihre Abfrage zu filtern, oder speichern Sie Ihre Abfrage als neuen Filter, um sie später erneut zu verwenden. [Erfahren Sie, wie Sie mit vordefinierten Filtern arbeiten](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >In dieser Produktversion sind einige vordefinierte Filter nicht in der Benutzeroberfläche verfügbar. Sie können sie dennoch verwenden. [Weitere Informationen](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **Attribute**: Zeigt eine Beschreibung der erstellten Zielgruppe an.

## Beispiel

In diesem Beispiel wird eine Zielgruppe erstellt, die alle Kunden und Kundinnen beinhaltet, die in Atlanta oder Seattle leben und nach 1980 geboren wurden.

1. Suchen Sie in der Registerkarte **Attribute** der Palette nach dem Feld **Geburtsdatum**. Ziehen Sie die Kachel und legen Sie sie auf der Arbeitsfläche ab.

   ![Hinzufügen des Felds „Geburtsdatum“ zur Arbeitsfläche](assets/segment-builder6.png){zoomable="yes"}

1. Wählen Sie auf der Arbeitsfläche den Operator **Nach** und geben Sie das gewünschte Datum ein.

   ![Konfigurieren des Operators „Nach“ für das Feld „Geburtsdatum“](assets/segment-builder7.png){zoomable="yes"}

1. Suchen Sie in der Palette nach dem Feld **Ort** und fügen Sie es unterhalb der ersten Regel zur Arbeitsfläche hinzu.

   ![Hinzufügen des Felds „Ort“ zur Arbeitsfläche](assets/segment-builder8.png){zoomable="yes"}

1. Geben Sie im Textfeld den Vornamen des Ortes ein und drücken Sie dann die Eingabetaste.

   ![Eingeben des ersten Ortsnamens in das Feld „Ort“](assets/segment-builder9.png){zoomable="yes"}

1. Wiederholen Sie diese Aktion für den zweiten Stadtnamen.

   ![Eingeben des zweiten Stadtnamen in das Feld „Stadt“](assets/segment-builder10.png){zoomable="yes"}

1. Klicken Sie auf **Ergebnisse anzeigen**, um die Liste und die Anzahl der Empfangenen anzuzeigen, die der Abfrage entsprechen. Fügen Sie Spalten hinzu, um die Daten zu visualisieren und zu überprüfen. Fügen Sie für dieses Beispiel die Spalte **Stadt** hinzu, um „Atlanta“ und „Seattle“ zu sehen.

   ![Anzeigen von Ergebnissen mit hinzugefügter Spalte „Stadt“](assets/segment-builder11.png){zoomable="yes"}

1. Klicken Sie auf **Bestätigen**.