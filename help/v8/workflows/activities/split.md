---
audience: end-user
title: Verwenden der Workflow-Aktivität „Aufspaltung“
description: Weitere Informationen zur Verwendung der Workflow-Aktivität „Aufspaltung“
badge: label="Alpha"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 100%

---


# Aufspaltung {#split}

Die Aktivität **Aufspaltung** ist eine Aktivität zur **Zielgruppenbestimmung**, mit der eingehende Populationen basierend auf unterschiedlichen Auswahlkriterien in mehrere Teilmengen segmentieren können, z. B. Filterregeln oder Populationsgröße.

## Konfiguration {#general}

Folgen Sie diesen Schritten, um die Aktivität **Aufspaltung** zu konfigurieren:

1. Fügen Sie eine Aktivität **Aufspaltung** zum Workflow hinzu.

1. Der Konfigurationsbereich für die Aktivität wird mit einer standardmäßigen Teilmenge geöffnet. Klicken Sie auf die Schaltfläche **Segment hinzufügen**, um so viele Teilmengen wie gewünscht zum Segmentieren der eingehenden Population hinzuzufügen.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Bei Ausführung der Aktivität „Aufspaltung“ wird die Population sukzessive in unterschiedliche Teilmengen segmentiert, und zwar in der Reihenfolge, in der diese zur Aktivität hinzugefügt werden. Wenn beispielsweise die erste Teilmenge 70 % der Anfangspopulation abruft, werden die Auswahlkriterien der nächsten hinzugefügten Teilmenge nur auf die restlichen 30 % angewendet usw.
   >
   > Stellen Sie vor der Konfiguration Ihrer Teilmengen sicher, dass Sie sie in der richtigen Reihenfolge hinzugefügt haben, da ihre Position nicht geändert werden kann.

1. Sobald die Teilmengen hinzugefügt wurden, zeigt die Aktivität für jede Teilmenge eine ausgehende Transition. Es wird dringend empfohlen, die Titel jeder Teilmenge zu ändern, um sie in der Workflow-Arbeitsfläche leicht zu identifizieren.

1. Konfigurieren Sie, wie jede Teilmenge die eingehende Population filtern soll. Gehen Sie dazu wie folgt vor:

   1. Öffnen Sie die Teilmenge, um ihre Eigenschaften anzuzeigen.

   1. Um eine Filterbedingung auf die Teilmenge anzuwenden, klicken Sie auf **[!UICONTROL Filter erstellen]** und konfigurieren Sie die gewünschte Filterregel. Es können beispielsweise Profile aus der eingehenden Population eingeschlossen werden, deren E-Mail-Adresse in der Datenbank vorhanden ist.

   1. Um die Anzahl der von der Teilmenge ausgewählten Profile zu begrenzen, muss **[!UICONTROL Grenzwert aktivieren]** aktiviert und die Anzahl oder der Prozentsatz der einzuschließenden Population angegeben werden.

      >[!NOTE]
      >
      >Beim Festlegen einer Populationsbegrenzung für eine Teilmenge können die ausgewählten Profile anhand eines bestimmten Profilattributs in auf- oder absteigender Reihenfolge sortiert werden. Schalten Sie dazu die Option **[!UICONTROL Sortierung aktivieren]** ein. Teilmengen können z. B. so eingeschränkt werden, dass nur die 50 Top-Profile mit dem höchsten Einkaufsbetrag einbezogen werden.

   ![](../assets/workflow-split-subset.png)

1. Nachdem Sie alle Teilmengen konfiguriert haben, kann die verbleibende Population ausgewählt werden, die keiner der Teilmengen entspricht, und in eine zusätzliche ausgehende Transition eingeschlossen werden. Schalten Sie dazu die Option **[!UICONTROL Komplement erzeugen]** ein.

   ![](../assets/workflow-split-complement.png)

Der Aktivität ist jetzt konfiguriert. Bei der Ausführung des Workflows wird die Population in die verschiedenen Teilmengen segmentiert, und zwar in der Reihenfolge, in der diese der Aktivität hinzugefügt wurden.

## Beispiel

Im folgenden Beispiel wird die Aktivität **[!UICONTROL Aufspaltung]** verwendet, um eine Zielgruppe basierend auf dem Kommunikationskanal, den wir verwenden möchten, in verschiedene Teilmengen zu unterteilen:

* **Teilmenge 1 „Push“**: Diese Teilmenge umfasst alle Profile, die unsere Mobile App installiert haben.
* **Teilmenge 2 „SMS“**: Benutzende von Mobiltelefonen: Für die verbleibende Population, die nicht in Teilmenge 1 fiel, wendet Teilmenge 2 eine Filterregel an, um Profile mit Mobiltelefonen in der Datenbank auszuwählen.
* **Komplement-Transition**: Diese Transition erfasst alle verbleibenden Profile, die weder Teilmenge 1 noch Teilmenge 2 entsprachen. Insbesondere enthält sie Profile, die weder die Mobile App installiert haben noch über ein Mobiltelefon verfügen, z. B. Benutzende, die die Mobile App nicht installiert haben oder keine registrierte Mobiltelefonnummer haben.

![](../assets/workflow-split-example.png)