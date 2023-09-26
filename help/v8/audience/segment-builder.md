---
audience: end-user
title: Erstellen einer Zielgruppe mit dem Campaign-Regel-Builder
description: Erfahren Sie, wie Sie mit dem Regel-Builder arbeiten
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 75%

---

# Arbeiten mit dem Regel-Builder {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Zielgruppen"
>abstract="Das Aufbauen einer Zielgruppe für einen Versand war nie einfacher! Mit unserem aktuellen Regel-Builder können Sie jetzt Filterkriterien für Empfängerinnen und Empfänger oder eine andere Zielgruppendimension von der Datenbank aus definieren. Machen Sie sich Ihre Adobe Experience Platform-Zielgruppe zunutze, um Ihre Zielgruppe weiter zu präzisieren und die Wirkung Ihrer Kampagne zu maximieren."

Mit dem Rule Builder können Sie die Zielgruppe Ihres Versands definieren, indem Sie in der Datenbank enthaltene Daten filtern. Sie können damit eine Audience aus einem Workflow erstellen, indem Sie eine **[!UICONTROL Audience erstellen]** oder direkt bei der Erstellung eines Versands zur Erstellung einer einmaligen Zielgruppe.

* [Erfahren Sie, wie Sie eine Zielgruppe erstellen](create-audience.md)
* [Erfahren Sie, wie Sie eine einmalige Zielgruppe für einen Versand erstellen.](one-time-audience.md)

## Die Palette

Die Palette auf der linken Seite enthält alle Elemente, nach denen Sie filtern können, um Ihre Audience zu erstellen. Sie können die Suchleiste verwenden, um Elemente schnell zu finden. Die in der Palette enthaltenen Kacheln müssen in die mittlere Arbeitsfläche verschoben werden, damit sie konfiguriert und berücksichtigt werden können.

![](assets/segment-builder2.png){width="70%" align="left"}

Die Palette ist in zwei Registerkarten unterteilt:

* **Attribute**: Auf dieser Registerkarte können Sie auf alle verfügbaren Felder des Schemas zugreifen. Die Liste der Felder hängt von dem in der E-Mail-Vorlage definierten Zielgruppenbestimmungsschema ab.

* **Audiences**: Auf dieser Registerkarte können Sie über einen Filter eine der vorhandenen Audiences auswählen, die in der Campaign Classic-Konsole oder in Adobe Experience Platform definiert sind. [Erfahren Sie, wie Sie Audiences überwachen und verwalten.](manage-audience.md)

  >[!NOTE]
  >
  >Um Adobe Experience Platform-Audiences zu nutzen, müssen Sie die Integration mit Zielen konfigurieren. Weitere Informationen finden Sie in der Dokumentation zu [Adobe Experience Platform-Zielen](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=de){target="_blank"}.

## Die Arbeitsfläche

Die Arbeitsfläche ist der zentrale Bereich des Bildschirms, in dem Sie die Regeln basierend auf den aus der Palette hier abgelegten Elementen konfigurieren und kombinieren können. Um eine neue Regel hinzuzufügen, ziehen Sie eine Kachel aus der Palette auf die Arbeitsfläche. Je nach Art der hinzuzufügenden Daten werden Ihnen dann kontextspezifische Optionen angezeigt.

![](assets/segment-builder4.png){width="70%" align="left"}

## Der Bereich mit den Regeleigenschaften

Auf der rechten Seite wird die **Regeleigenschaften** können Sie die unten aufgeführten Aktionen ausführen.

![](assets/segment-builder5.png){width="70%" align="left"}

* **Ergebnisse anzeigen:** zeigt die Liste der von der Audience angesprochenen Empfänger an.
* **Code-Ansicht**: Zeigt eine Code-basierte Version der Audience in SQL an.
* **Erweiterte Attribute anzeigen**: Aktivieren Sie diese Option, wenn Sie die vollständige Liste der Attribute in der linken Palette anzeigen möchten: Knoten, Gruppierungen, 1:1-Links, 1:n-Links.
* **berechnen**: aktualisiert die Anzahl der Profile, die in der Zielgruppe Ihrer Abfrage enthalten sind, und zeigt sie an.
* **Filter auswählen oder speichern**: Verwenden Sie einen vordefinierten Filter, um Ihre Abfrage zu filtern, oder speichern Sie Ihre Abfrage als neuen Filter, um sie später erneut zu verwenden. [Erfahren Sie, wie Sie mit vordefinierten Filtern arbeiten.](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >In dieser Produktversion sind einige vordefinierte Filter nicht in der Benutzeroberfläche verfügbar. Sie können sie dennoch verwenden. [Weitere Informationen](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Attribute**: zeigt eine Beschreibung der erstellten Audience an.

## Beispiel

In diesem Beispiel erstellen wir eine Zielgruppe für alle Kunden und Kundinnen, die in Atlanta oder Seattle leben und nach 1980 geboren wurden.

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

1. Klicken Sie auf **Ergebnisse anzeigen**, um die Liste und die Anzahl der Empfangenen anzuzeigen, die der Abfrage entsprechen. Sie können auch Spalten hinzufügen, um die Daten zu visualisieren und zu überprüfen. Fügen Sie für unser Beispiel die Spalte **Stadt** hinzu. Atlanta und Seattle sollten hier zu sehen sein.

   ![](assets/segment-builder11.png)

1. Klicken Sie auf **Bestätigen**.
