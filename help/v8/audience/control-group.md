---
audience: end-user
title: Festlegen einer Kontrollgruppe
description: Erfahren Sie, wie Sie in der Campaign Web-Benutzeroberfläche eine Kontrollgruppe für Ihre Nachrichten einrichten
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 41%

---

# Festlegen einer Kontrollgruppe {#control-group}

Eine Kontrollgruppe ist eine vom Versand ausgeschlossene Unterpopulation. Sie können eine Kontrollgruppe definieren, um zu vermeiden, dass Nachrichten an einen Teil Ihrer Audience gesendet werden, und das Verhalten nach dem Versand mit der Hauptzielgruppe vergleichen. Mit dieser Option können Sie die Wirkung Ihrer Kampagne messen.

➡️ [Entdecken Sie diese Funktion im Video](create-audience.md#video)

## Aktivieren einer Kontrollgruppe {#add-a-control-group}

Um eine Kontrollgruppe hinzuzufügen, aktivieren Sie die entsprechende Option, wenn Sie die Zielgruppe Ihres Versands definieren. Die Kontrollgruppe kann nach dem Zufallsprinzip aus der Hauptzielgruppe extrahiert oder aus einer bestimmten Population ausgewählt werden. Es gibt daher zwei Möglichkeiten, eine Kontrollgruppe zu definieren:

* Extrahieren Sie eine Reihe von Profilen aus der Hauptzielgruppe.
* Schließen Sie einige Profile aus einer Liste oder basierend auf in einer Abfrage definierten Kriterien aus.

Beim Definieren einer Kontrollgruppe können Sie beide Methoden kombinieren.

Alle Profile, die bei der Versandvorbereitung in der Kontrollgruppe enthalten sind, werden aus der Hauptzielgruppe entfernt. Sie erhalten die Nachricht nicht.

>[!CAUTION]
>
>Sie können keine Kontrollgruppen verwenden, wenn Sie die Zielgruppen-Population [aus einer externen Datei](file-audience.md) laden.

Um eine Kontrollgruppe zu einem Versand hinzuzufügen, aktivieren Sie den Umschalter **[!UICONTROL Kontrollgruppe aktivieren]** im Abschnitt **Audience** des Bildschirms für die Versanderstellung.

![Optionsfeld Kontrollgruppe aktivieren im Bildschirm zur Versanderstellung](assets/control-group1.png)

## Aus Zielgruppe extrahieren {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extraktionsmodus"
>abstract="Eine Kontrollgruppe ist ein Satz von Profilen, die vom Versand ausgeschlossen sind. Um eine Kontrollgruppe zu definieren, können Sie nach dem Zufallsprinzip oder basierend auf einer Sortierung einen Prozentsatz oder eine feste Anzahl von Profilen aus der Zielgruppenpopulation extrahieren."

### Erstellen einer Kontrollgruppe {#build-extract-target}

Um eine Kontrollgruppe zu definieren, wählen Sie nach dem Zufallsprinzip oder basierend auf einer Sortierung einen Prozentsatz oder eine feste Anzahl von Profilen aus der Zielpopulation aus. Wenn Sie eine zusätzliche Population hinzufügen, wählen Sie die Option **Keine Extraktion** und wählen Sie die zusätzliche Population [wie hier beschrieben](#extra-population).

Legen Sie zunächst fest, wie die Profile aus der Zielgruppe extrahiert werden sollen: zufällig oder auf der Grundlage einer Sortierung.

Wählen Sie unter dem Abschnitt **Kontrollgruppe** einen **Extraktionsmodus**:

* **Zufällig**: Bei der Versandvorbereitung extrahiert Adobe Campaign nach dem Zufallsprinzip eine Anzahl von Profilen, die dem Prozentwert oder der maximalen Anzahl entsprechen, die als Größenbeschränkung festgelegt wurde.
* **Nach Attribut(en) sortiert**: Mit dieser Option wird eine Gruppe von Profilen auf der Grundlage bestimmter Attribute in einer bestimmten Sortierreihenfolge ausgeschlossen.

Verwenden Sie dann den Abschnitt **Größenbeschränkung**, um die Anzahl der Profile festzulegen, die aus der Hauptzielgruppe extrahiert werden sollen. Dabei kann es sich um eine Rohanzahl (z. B. 50 Profile, die ausgeschlossen werden sollen) oder einen Prozentsatz der ursprünglichen Zielgruppe handeln (z. B. 5 % der Hauptzielgruppe).

### Beispiel einer Kontrollgruppe {#control-group-sample}

Gehen Sie wie folgt vor, um beispielsweise eine Kontrollgruppe mit den 100 jüngsten Profilen zu erstellen:

1. Wählen Sie das Feld **Alter** als Sortierkriterium aus. Lassen Sie die Sortieroption **Aufsteigend**.
1. Fügen Sie das Feld **Erstellungsdatum** hinzu. Wechseln Sie zur Sortieroption **Absteigend**.
1. Definieren Sie 100 als Schwellenwert im Abschnitt **Größenbeschränkung**.

   ![Kontrollgruppenkonfiguration für die jüngsten Profile](assets/control-group2.png){zoomable="yes"}

Diese 100 jüngsten Profile werden dann aus der Hauptzielgruppe ausgeschlossen.

### Überprüfen Sie Ihre Kontrollgruppe {#check-control-group}

Anzeigen der Protokolle zur Überprüfung und Identifizierung der ausgeschlossenen Profile Betrachten Sie beispielsweise einen zufälligen Ausschluss von fünf Profilen.

![Beispiel für ausgeschlossene Profile in Protokollen](assets/control-group4.png){zoomable="yes"}

Überprüfen Sie nach der Versandvorbereitung, wie die Ausschlüsse angewendet wurden:

* Aktivieren Sie im Versand-Dashboard vor dem Versand den KPI **Ausschließen**.

  ![Versand-Dashboard mit dem KPI „Ausschließen“](assets/control-group5.png){zoomable="yes"}

* In den Versandlogs wird in der Registerkarte „Logs“ der Ausschlussschritt angezeigt.

  ![Versandlogs mit Ausschlussschritt](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* Auf **Registerkarte** Ausschlussgründe“ wird die Anzahl der ausgeschlossenen Profile für jede Typologieregel angezeigt.

  ![Registerkarte „Ausschlussgründe“ mit Typologieregel-Ausschlüssen](assets/control-group7.png){zoomable="yes"}

Weitere Informationen über Versandlogs finden Sie in [diesem Abschnitt](../monitor/delivery-logs.md).

## Hinzufügen einer zusätzlichen Population {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Zusätzliche Population"
>abstract="Eine Kontrollgruppe ist ein Satz von Profilen, die vom Versand ausgeschlossen sind. Sie können eine bestimmte Population aus der Versand-Zielgruppe ausschließen, indem Sie eine existierende Zielgruppe auswählen oder eine Abfrage definieren."

Eine andere Möglichkeit, eine Kontrollgruppe zu definieren, besteht darin, eine bestimmte Population in einer bestehenden Audience auszuwählen oder eine Abfrage zu definieren.

Klicken Sie im Abschnitt **Zusätzliche Population** des Definitionsbildschirms der **Kontrollgruppe** auf die Schaltfläche **[!UICONTROL Zielgruppe auswählen]**.

![Bildschirm zur Auswahl der zusätzlichen Population](assets/control-group3.png){zoomable="yes"}

* Um eine vorhandene Zielgruppe zu verwenden, klicken Sie auf **Zielgruppe auswählen**. Weiterführende Informationen finden Sie in [diesem Abschnitt](add-audience.md).
* Um eine neue Abfrage zu definieren, wählen Sie **Eigene erstellen** und definieren Sie die Ausschlusskriterien mithilfe des Abfrage-Modelers. Weiterführende Informationen finden Sie in [diesem Abschnitt](../query/query-modeler-overview.md).

Die Profile, die in der Audience enthalten sind oder mit dem Ergebnis der Abfrage übereinstimmen, werden **der Versandzielgruppe** ausgeschlossen“. Sie erhalten keine Nachricht.

## Vergleichen der Ergebnisse {#control-group-results}

Extrahieren Sie nach dem Versand die Versandlogs, um das Verhalten zwischen den Profilen, die die Nachricht nicht erhalten haben, und der tatsächlichen Zielgruppe zu vergleichen. Versandlogs zum Erstellen einer neuen Zielgruppenbestimmung verwenden.

Um zu sehen, welche Profile aus der Zielgruppe entfernt wurden, überprüfen Sie die **Versandlogs**. Weitere Informationen finden Sie in [diesem Abschnitt](#check-control-group).