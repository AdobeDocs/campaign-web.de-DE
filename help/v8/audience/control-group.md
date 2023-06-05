---
audience: end-user
title: Festlegen einer Kontrollgruppe
description: Erfahren Sie, wie Sie in der Web-Benutzeroberfläche von Campaign eine Kontrollgruppe für Ihre Nachrichten einrichten.
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Alpha" type="Positive"
source-git-commit: 3ebe92659916cf2fa4cacb8d28b79d7b6d5359f3
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# Festlegen einer Kontrollgruppe {#control-group}

Eine Kontrollgruppe ist eine vom Versand ausgeschlossene Unterpopulation. Sie können eine Kontrollgruppe definieren, um zu verhindern, dass Nachrichten an einen Teil Ihrer Audience gesendet werden, und das Verhalten nach dem Versand mit der Hauptzielgruppe vergleichen. Mit dieser Option können Sie die Wirkung Ihrer Kampagne messen.

Um eine Kontrollgruppe hinzuzufügen, aktivieren Sie die Option bei der Definition der Zielgruppe Ihres Versands. Die Kontrollgruppe kann nach dem Zufallsprinzip aus der Hauptzielgruppe extrahiert und/oder aus einer bestimmten Population ausgewählt werden. Daher gibt es zwei Möglichkeiten, eine Kontrollgruppe zu definieren:

* Extrahieren Sie eine Reihe von Profilen aus der Hauptzielgruppe.
* Schließen Sie einige Profile aus einer Liste oder basierend auf in einer Abfrage definierten Kriterien aus.

Beim Definieren einer Kontrollgruppe können Sie beide Methoden kombinieren.

Alle Profile, die bei der Versandvorbereitung zur Kontrollgruppe gehören, werden aus der Hauptzielgruppe entfernt. Sie erhalten die Nachricht nicht.

>[!CAUTION]
>
>Kontrollgruppen können beim Laden der Zielpopulation nicht verwendet werden [aus einer externen Datei](file-audience.md).

Um einem Versand eine Kontrollgruppe hinzuzufügen, aktivieren Sie die **[!UICONTROL Kontrollgruppe aktivieren]** Umschalten von der **Zielgruppe** im Bereich der Versanderstellung.

![Option &quot;Kontrollgruppe aktivieren&quot;](assets/control-group1.png)


## Aus Zielgruppe extrahieren {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extraktionsmodus"
>abstract="Um eine Kontrollgruppe zu definieren, können Sie nach dem Zufallsprinzip oder basierend auf einer Sortierung einen Prozentsatz oder eine feste Anzahl von Profilen aus der Zielgruppenpopulation extrahieren."


### Kontrollgruppe erstellen {#build-extract-target}

Um eine Kontrollgruppe zu definieren, können Sie nach dem Zufallsprinzip oder basierend auf einer Sortierung einen Prozentsatz oder eine feste Anzahl von Profilen aus der Zielgruppenpopulation extrahieren. Wenn Sie eine zusätzliche Population hinzufügen möchten, wählen Sie die **Keine Extraktion** und wählen Sie die zusätzliche Population aus [wie hier beschrieben](#extra-population).

Definieren Sie zunächst, wie die Profile aus der Zielgruppe extrahiert werden: zufällig oder basierend auf einer Sortierung.

Unter dem **Kontrollgruppe** wählen Sie eine **Extraktionsmodus**:

* **Zufällig**: Bei der Versandvorbereitung extrahiert Adobe Campaign nach dem Zufallsprinzip eine gewisse Anzahl von Profilen, die dem Prozentsatz oder der maximalen Anzahl entspricht, die als Größenbegrenzung festgelegt wurde.

* **Nach Attribut(en) sortiert**: Mit dieser Option können Sie anhand bestimmter Attribute in einer bestimmten Reihenfolge eine Gruppe von Profilen ausschließen.

   ![](assets/control-group2.png)

Verwenden Sie dann die **Größenbeschränkung** um die Anzahl der Profile festzulegen, die aus der Hauptzielgruppe extrahiert werden sollen. Dabei kann es sich um eine Rohnummer oder einen Prozentsatz der ursprünglichen Zielgruppe handeln.

### Kontrollgruppe überprüfen {#check-extract-target}

Sie können die Protokolle anzeigen, um die ausgeschlossenen Profile zu überprüfen und zu identifizieren. Nehmen wir als Beispiel einen zufälligen Ausschluss von fünf Profilen.

![](assets/control-group4.png)

Nach der Versandvorbereitung können Sie überprüfen, wie die Ausschlüsse angewendet wurden:

* Aktivieren Sie im Versand-Dashboard vor dem Versand die Option **Ausschließen** KPI.

   ![](assets/control-group5.png)

* In den Versandlogs wird im Tab Logs der Ausschlussschritt angezeigt.

   ![](assets/control-group-sample-logs.png)


* Die **Ausschlusslogs** -Tab zeigt jedes Profil und den zugehörigen Ausschluss an **Grund**.

   ![](assets/control-group6.png)

* Die **Ausschlussgründe** zeigt die Anzahl der ausgeschlossenen Profile für jede Typologieregel an.

   ![](assets/control-group7.png)

Weitere Informationen über Versandlogs finden Sie in [diesem Abschnitt](../monitor/delivery-logs.md).

## Zusätzliche Population hinzufügen {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Zusätzliche Population"
>abstract="Eine andere Möglichkeit, eine Kontrollgruppe zu definieren, besteht darin, eine bestimmte Population mithilfe einer bestehenden Audience oder durch Definition einer Abfrage aus der Zielgruppe auszuschließen."

Eine andere Möglichkeit, eine Kontrollgruppe zu definieren, besteht darin, eine bestimmte Population mithilfe einer bestehenden Audience oder durch Definition einer Abfrage aus der Zielgruppe auszuschließen.

Klicken Sie im Abschnitt **Zusätzliche Population** des Definitionsbildschirms der **Kontrollgruppe** auf die Schaltfläche **[!UICONTROL Audience auswählen]**.

![](assets/control-group3.png)

* Um eine vorhandene Audience zu verwenden, klicken Sie auf **Audience auswählen**. Näheres dazu finden Sie in [diesem Abschnitt](add-audience.md).

* Um eine neue Abfrage zu definieren, wählen Sie **Eigene erstellen** aus und definieren Sie die Ausschlusskriterien mit dem Regel-Builder. Näheres dazu finden Sie in [diesem Abschnitt](segment-builder.md).

Die Profile, die in der Audience enthalten sind oder mit dem Ergebnis der Abfrage übereinstimmen, werden aus der Zielgruppe ausgeschlossen.