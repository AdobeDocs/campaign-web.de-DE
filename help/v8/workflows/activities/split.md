---
audience: end-user
title: Verwenden der Workflow-Aktivität „Aufspaltung“
description: Weitere Informationen zur Verwendung der Workflow-Aktivität „Aufspaltung“
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: ht
source-wordcount: '905'
ht-degree: 100%

---

# Aufspaltung {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Aktivität „Aufspaltung“"
>abstract="Mit der Aktivität **Aufspaltung** können Sie eingehende Populationen basierend auf unterschiedlichen Auswahlkriterien in mehrere Teilmengen segmentieren, z. B. Filterregeln oder Populationsgröße."

Die Aktivität **Aufspaltung** ist eine Aktivität zur **Zielgruppenbestimmung**, mit der Sie eingehende Populationen basierend auf unterschiedlichen Auswahlkriterien in mehrere Teilmengen segmentieren können, z. B. Filterregeln oder Populationsgröße.

## Konfigurieren der Aufspaltungsaktivität {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segmente für die Aktivität „Aufspaltung“"
>abstract="Fügen Sie beliebig viele Teilmengen hinzu, um die eingehende Population zu segmentieren.<br/></br>Bei Ausführung der Aktivität **Aufspaltung** wird die Population sukzessive in unterschiedliche Teilmengen segmentiert, und zwar in der Reihenfolge, in der diese zur Aktivität hinzugefügt werden. Vergewissern Sie sich vor dem Start Ihres Workflows, dass Sie die Teilmengen mithilfe der Pfeilschaltflächen in der für Sie passenden Reihenfolge angeordnet haben."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Filter „Aufspaltungsaktivität“"
>abstract="Um eine Filterbedingung auf die Teilmenge anzuwenden, klicken Sie auf **[!UICONTROL Filter erstellen]** und konfigurieren Sie die gewünschte Regel mit dem Abfrage-Modeler. Es können beispielsweise Profile aus der eingehenden Population eingeschlossen werden, deren E-Mail-Adresse in der Datenbank vorhanden ist."
>additional-url="https://experienceleague.adobe.com/de/docs/campaign-web/v8/query-database/query-modeler-overview" text="Arbeiten mit dem Abfrage-Modeler"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Begrenzung der Aufspaltungsaktivität"
>abstract="Um die Anzahl der von der Teilmenge ausgewählten Profile zu begrenzen, muss **[!UICONTROL Grenzwert aktivieren]** aktiviert und die Anzahl oder der Prozentsatz der einzuschließenden Population angegeben werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Sortierung der Aufspaltungsaktivität"
>abstract="Beim Festlegen einer Populationsbegrenzung für eine Teilmenge können die ausgewählten Profile anhand eines bestimmten Profilattributs in auf- oder absteigender Reihenfolge sortiert werden. Schalten Sie dazu die Option **Sortierung aktivieren** ein. Teilmengen können z. B. so eingeschränkt werden, dass nur die 50 Top-Profile mit dem höchsten Einkaufsbetrag einbezogen werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Aufspaltung – Komplement erzeugen"
>abstract="Nachdem Sie alle Teilmengen konfiguriert haben, kann die verbleibende Population ausgewählt werden, die keiner der Teilmengen entspricht, und in eine zusätzliche ausgehende Transition eingeschlossen werden. Schalten Sie dazu die Option **Komplement erzeugen** ein."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Alle Teilmengen in derselben Tabelle erzeugen"
>abstract="Aktivieren Sie diese Option, um alle Teilmengen in einer ausgehenden Transition zu gruppieren."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Leere Transition überspringen"
>abstract="Aktivieren Sie die Option **[!UICONTROL Leere Transition überspringen]**, um die ausgehende Transition für diese Teilmenge zu deaktivieren, wenn die Eingangspopulation leer ist."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="Überlappen von Ausgabepopulationen ermöglichen"
>abstract="Überlappen von Ausgabepopulationen ermöglichen"

Folgen Sie diesen Schritten, um die Aktivität **Aufspaltung** zu konfigurieren:

1. Fügen Sie eine Aktivität **Aufspaltung** zum Workflow hinzu.

1. Der Konfigurationsbereich für die Aktivität wird mit einer standardmäßigen Teilmenge geöffnet. Klicken Sie auf die Schaltfläche **Segment hinzufügen**, um so viele Teilmengen wie gewünscht zum Segmentieren der eingehenden Population hinzuzufügen.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Bei Ausführung der Aktivität **Aufspaltung** wird die Population sukzessive in unterschiedliche Teilmengen segmentiert, und zwar in der Reihenfolge, in der diese zur Aktivität hinzugefügt werden. Wenn beispielsweise die erste Teilmenge 70 % der Anfangspopulation abruft, werden die Auswahlkriterien der nächsten hinzugefügten Teilmenge nur auf die restlichen 30 % angewendet usw.
   >
   >Vergewissern Sie sich vor dem Start Ihres Workflows, dass Sie die Teilmengen in der für Sie passenden Reihenfolge angeordnet haben. Verwenden Sie dazu die Pfeilschaltflächen, um die Position einer Teilmenge zu ändern.

1. Sobald die Teilmengen hinzugefügt wurden, zeigt die Aktivität für jede Teilmenge eine ausgehende Transition. Es wird dringend empfohlen, die Titel jeder Teilmenge zu ändern, um sie in der Workflow-Arbeitsfläche leicht zu identifizieren.

1. Konfigurieren Sie, wie jede Teilmenge die eingehende Population filtern soll. Gehen Sie dazu wie folgt vor:

   1. Öffnen Sie die Teilmenge, um ihre Eigenschaften anzuzeigen.

   1. Um eine Filterbedingung auf die Teilmenge anzuwenden, klicken Sie auf **[!UICONTROL Filter erstellen]** und konfigurieren Sie die gewünschte Filterregel mit dem Abfrage-Modeler. Es können beispielsweise Profile aus der eingehenden Population eingeschlossen werden, deren E-Mail-Adresse in der Datenbank vorhanden ist.  [Erfahren Sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md)

   1. Um die Anzahl der von der Teilmenge ausgewählten Profile zu begrenzen, muss **[!UICONTROL Grenzwert aktivieren]** aktiviert und die Anzahl oder der Prozentsatz der einzuschließenden Population angegeben werden.

   1. Um eine Transition zu deaktivieren, wenn die Eingangspopulation leer ist, aktivieren Sie die Option **[!UICONTROL Leere Transition überspringen]**. Wenn kein Profil mit der Teilmenge übereinstimmt, geht der Workflow nicht zur nächsten Aktivität über.

      ![](../assets/workflow-split-subset.png)


      >[!NOTE]
      >
      >Beim Festlegen einer Populationsbegrenzung für eine Teilmenge können die ausgewählten Profile anhand eines bestimmten Profilattributs in auf- oder absteigender Reihenfolge sortiert werden. Schalten Sie dazu die Option **[!UICONTROL Sortierung aktivieren]** ein. Teilmengen können z. B. so eingeschränkt werden, dass nur die 50 Top-Profile mit dem höchsten Einkaufsbetrag einbezogen werden.

1. Nachdem Sie alle Teilmengen konfiguriert haben, kann die verbleibende Population ausgewählt werden, die keiner der Teilmengen entspricht, und in eine zusätzliche ausgehende Transition eingeschlossen werden. Schalten Sie dazu die Option **[!UICONTROL Komplement erzeugen]** ein.

   ![](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >Die Option **[!UICONTROL Alle Teilmengen in derselben Tabelle generieren]** ermöglicht die Gruppierung aller Teilmengen in einer ausgehenden Transition.

Der Aktivität ist jetzt konfiguriert. Bei der Ausführung des Workflows wird die Population in die verschiedenen Teilmengen segmentiert, und zwar in der Reihenfolge, in der diese der Aktivität hinzugefügt wurden.

## Beispiel{#split-example}

Im folgenden Beispiel wird die Aktivität **[!UICONTROL Aufspaltung]** verwendet, um eine Zielgruppe basierend auf dem Kommunikationskanal, den wir verwenden möchten, in verschiedene Teilmengen zu unterteilen:

* **Teilmenge 1 „Push“**: Diese Teilmenge umfasst alle Profile, die unsere Mobile App installiert haben.
* **Teilmenge 2 „SMS“**: Benutzende von Mobiltelefonen: Für die verbleibende Population, die nicht in Teilmenge 1 fiel, wendet Teilmenge 2 eine Filterregel an, um Profile mit Mobiltelefonen in der Datenbank auszuwählen.
* **Komplement-Transition**: Diese Transition erfasst alle verbleibenden Profile, die weder Teilmenge 1 noch Teilmenge 2 entsprachen. Insbesondere enthält sie Profile, die weder die Mobile App installiert haben noch über ein Mobiltelefon verfügen, z. B. Benutzende, die die Mobile App nicht installiert haben oder keine registrierte Mobiltelefonnummer haben.

![](../assets/workflow-split-example.png)
