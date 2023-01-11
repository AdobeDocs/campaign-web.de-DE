---
audience: end-user
title: Einrichten einer Kontrollgruppe
description: Web-Dokumentation zu Campaign v8
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: 6d678442c0fe396f45a635c60837932f424d0763
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 77%

---

# Einrichten einer Kontrollgruppe {#control-group}

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

Mithilfe von Kontrollgruppen können Sie vermeiden, dass Nachrichten an einen Teil Ihrer Audience gesendet werden, um die Wirkung Ihrer Kampagnen zu messen.

Erstellen Sie dazu eine Kontrollgruppe, wenn Sie die Audience Ihres Versands definieren. Profile werden der Kontrollgruppe nach dem Zufallsprinzip hinzugefügt, gefiltert oder ungefiltert oder auf der Grundlage von Kriterien. Sie können dann das Verhalten der Zielgruppe, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die nicht in der Zielgruppe enthalten waren.

Die Kontrollgruppe kann nach dem Zufallsprinzip aus der Hauptzielgruppe extrahiert und/oder aus einer bestimmten Population ausgewählt werden. Daher gibt es zwei Möglichkeiten, eine Kontrollgruppe zu definieren:

* Extrahieren Sie eine Reihe von Profilen aus der Hauptzielgruppe.
* Schließen Sie einige Profile basierend auf in einer Abfrage definierten Kriterien aus.

Beim Definieren einer Kontrollgruppe können Sie beide Methoden verwenden.

Alle Profile, die bei der Vorbereitung des Versands in die Kontrollgruppe eingehen, werden aus der Hauptzielgruppe entfernt. Sie erhalten die Nachricht nicht, nachdem diese gesendet wurde.

Um eine Kontrollgruppe zu erstellen, klicken Sie im Abschnitt **Audience** des Assistenten zur Versanderstellung auf die Schaltfläche **[!UICONTROL Kontrollgruppe festlegen]**.

![](assets/control-group1.png)

## Aus Zielgruppe extrahieren {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Aus Zielgruppe extrahieren"
>abstract="TBC"

Um eine Kontrollgruppe zu definieren, können Sie nach dem Zufallsprinzip oder basierend auf einer Sortierung einen Prozentsatz oder eine feste Anzahl von Profilen aus der Zielgruppe extrahieren.

Definieren Sie zunächst, wie die Profile aus der Zielgruppe extrahiert werden: zufällig oder basierend auf einer Sortierung.

Wählen Sie im Abschnitt **Aus Zielgruppe extrahieren** einen **Ausschlusstyp**:

* **Zufällige Auswahl**:: Beim Vorbereiten des Versands extrahiert Adobe Campaign nach dem Zufallsprinzip eine Anzahl von Profilen, die dem Prozentwert oder der maximalen Anzahl entsprechen, die Sie als Größenbeschränkung festlegen.

   ![](assets/control-group.png)

* **Nach Attribut(en) sortiert**: Mit dieser Option können Sie eine Gruppe von Profilen ausschließen, die auf bestimmten Attributen in einer bestimmten Sortierreihenfolge basieren.

   ![](assets/control-group2.png)

Definieren Sie dann die **Größenbeschränkung**: Hierzu müssen Sie festlegen, wie Sie die Anzahl der Profile begrenzen, die Sie aus der Hauptzielgruppe extrahieren.

**Beispiel**

Sie können die Protokolle anzeigen, um die ausgeschlossenen Profile zu überprüfen und zu identifizieren. Nehmen wir als Beispiel einen zufälligen Ausschluss von fünf Profilen.

![](assets/control-group4.png)

Nach der Versandvorbereitung können Sie die Ausschlüsse auf den folgenden Bildschirmen anzeigen:

* Die **Ausschließen** KPI im Versand-Dashboard vor dem Versand.

   ![](assets/control-group5.png)

* Die **Ausschlusslogs** Anzeigen jedes Profils und der zugehörigen Ausschlüsse **Grund**.

   ![](assets/control-group6.png)

* Die **Ausschlussgründe** die Anzahl der ausgeschlossenen Profile für jede Typologieregel anzeigen.

   ![](assets/control-group7.png)

Weiterführende Informationen zu Versandlogs finden Sie in diesem Abschnitt [Abschnitt](../monitor/delivery-logs.md).

## Zusätzliche Population {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Zusätzliche Population"
>abstract="TBC"

Eine andere Möglichkeit, eine Kontrollgruppe zu definieren, besteht darin, eine bestimmte Population mithilfe einer bestehenden Audience oder durch Definieren einer Abfrage aus der Zielgruppe auszuschließen.

Klicken Sie im Abschnitt **Zusätzliche Population** des Definitionsbildschirms der **Kontrollgruppe** auf die Schaltfläche **[!UICONTROL Audience auswählen]**.

![](assets/control-group3.png)

* Um eine vorhandene Audience zu verwenden, klicken Sie auf **Audience auswählen**. Näheres dazu finden Sie in [diesem Abschnitt](add-audience.md).

* Um eine neue Abfrage zu definieren, wählen Sie **Erstellen eigener** und definieren die Ausschlusskriterien mithilfe des Regel-Builders. Näheres dazu finden Sie in [diesem Abschnitt](segment-builder.md).

Die in der Audience enthaltenen oder dem Ergebnis der Abfrage entsprechenden Profile werden aus der Zielgruppe ausgeschlossen.