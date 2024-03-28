---
audience: end-user
title: Verwenden der Workflow-Aktivität „Abstimmung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Abstimmung“ verwenden
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 97%

---

# Abstimmung {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Aktivität „Abstimmung“"
>abstract="Die Aktivität **Abstimmung** ist eine Aktivität zur **Zielgruppenbestimmung**, mit der Sie die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle definieren können. Zum Beispiel kann die Aktivität **Abstimmung** hinter der Aktivität **Datei laden** platziert werden, um nicht standardmäßige Daten in die Datenbank zu laden. In diesem Fall können Sie über die **Abstimmung** die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in der externen Tabelle festlegen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Abstimmung – Feld auswählen"
>abstract="Abstimmung – Feld auswählen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Abstimmung – Bedingung erstellen"
>abstract="Abstimmung – Bedingung erstellen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Abstimmung – Komplement erzeugen"
>abstract="Abstimmung – Komplement erzeugen"

Die Aktivität **Abstimmung** ist eine Aktivität zur **Zielgruppenbestimmung**, mit der Sie die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle definieren können, beispielsweise aus einer externen Datei geladene Daten. 

Zum Beispiel kann die Aktivität **Abstimmung** hinter der Aktivität **Datei laden** platziert werden, um nicht standardmäßige Daten in die Datenbank zu laden. In diesem Fall wird können Sie über die Aktivität **Abstimmung** die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in der Arbeitstabelle festlegen.

## Best Practices {#reconciliation-best-practices}

Mit der Aktivität **Anreicherung** können Sie zusätzliche Daten definieren, die in Ihrem Workflow verarbeitet werden sollen. So können Sie mit der Aktivität **Anreicherung** Daten aus mehreren Datensätzen kombinieren oder Verknüpfungen zu einer temporären Ressource erstellen. Dagegen ermöglicht Ihnen die Aktivität **Abstimmung**, nicht identifizierte Daten mit bestehenden Ressourcen zu verknüpfen.

>[!NOTE]
>Der Abstimmungsvorgang setzt voraus, dass die Daten der verknüpften Dimensionen bereits in der Datenbank vorhanden sind. Wenn Sie beispielsweise eine Datei mit Kaufdaten importieren möchten, in der verzeichnet ist, welches Produkt wann von welcher Kundin und welchem Kunden gekauft wurde, müssen sowohl das Produkt als auch die Person bereits in der Datenbank angelegt sein.

## Konfigurieren der Abstimmungsaktivität {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Zielgruppendimension"
>abstract="Wählen Sie die neue Zielgruppendimension aus. Mit einer Dimension können Sie die Zielgruppen definieren: Empfängerinnen und Empfänger, Abonnentinnen und Abonnenten der App, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw. Standardmäßig ist die aktuelle Zielgruppendimension ausgewählt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Abstimmungsregeln"
>abstract="Wählen Sie die für die Deduplizierung zu verwendenden Abstimmungsregeln aus. Um Attribute zu verwenden, wählen Sie die Option **Einfache Attribute** und dann die Quell- und Zielfelder aus. Um mithilfe des Abfrage-Modelers eine eigene Abstimmbedingung zu erstellen, wählen Sie die Option **Erweiterte Abstimmbedingungen** aus."
>additional-url="https://experienceleague.adobe.com/de/docs/campaign-web/v8/query-database/query-modeler-overview" text="Arbeiten mit dem Abfrage-Modeler"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Auswählen der Zielgruppendimension"
>abstract="Wählen Sie die Zielgruppendimension für Ihre eingehenden Daten zum Abstimmen aus."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=de#targeting-dimensions" text="Zielgruppendimensionen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Beibehalten nicht abgestimmter Daten"
>abstract="Standardmäßig werden nicht abgestimmte Daten in der ausgehenden Transition beibehalten und stehen in der Arbeitstabelle zur späteren Verwendung zur Verfügung. Um nicht abgestimmte Daten zu entfernen, deaktivieren Sie die Option **Nicht abgestimmte Daten beibehalten**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Abstimmungsattribut"
>abstract="Wählen Sie das Attribut aus, das zur Abstimmung der Daten verwendet werden soll, und klicken Sie auf „Bestätigen“."

Gehen Sie wie folgt vor, um die Aktivität **Abstimmung** zu konfigurieren:

1. Ziehen Sie eine **Abstimmungs**-Aktivität per Drag-and-Drop in Ihren Workflow. Diese Aktivität sollten nach einer Transition mit einer Population eingefügt werden, deren Zielgruppendimension nicht direkt aus Adobe Campaign stammt.

1. Wählen Sie die neue Zielgruppendimension aus. Mit einer Dimension können Sie die Zielgruppen definieren: Empfängerinnen und Empfänger, Abonnentinnen und Abonnenten der App, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw. [Erfahren Sie mehr über Zielgruppendimensionen](../../audience/about-recipients.md#targeting-dimensions)

1. Wählen Sie die für Abstimmung zu verwendenden Felder aus. Es können mehrere Abstimmkriterien definiert werden.

   1. Um Datenabstimmungsattribute zu verwenden, wählen Sie die Option **Einfache Attribute**. Das Feld **Quelle** enthält die in der eingehenden Transition zur Verfügung stehenden Felder, die abgestimmt werden sollen. Das Feld **Ziel** entspricht den Feldern der ausgewählten Zielgruppendimension. Daten werden abgestimmt, wenn Quelle und Ziel gleich sind. Wählen Sie beispielsweise die **E-Mail**-Felder, um Profile anhand ihrer E-Mail-Adresse zu deduplizieren.

      Um weitere Abstimmungskriterien hinzuzufügen, klicken Sie auf die Schaltfläche **Regel hinzufügen**. Wenn mehrere Bedingungen für die Verknüpfung angegeben werden, müssen ALLE erfüllt sein, damit die Relation hergestellt werden kann.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. Um andere Attribute zur Datenabstimmung zu verwenden, wählen Sie die Option **Erweiterte Abstimmungsbedingungen**. Anschließend können Sie mithilfe des Abfrage-Modelers eine eigene Abstimmungsbedingung erstellen. [Erfahren Sie, wie Sie mit dem Abfragemodell arbeiten.](../../query/query-modeler-overview.md).

1. Über die Schaltfläche **Filter erstellen** können Sie die abzustimmende Daten filtern. Auf diese Weise können Sie mithilfe des Abfragemodells eine benutzerdefinierte Bedingung erstellen. [Erfahren sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md)

Standardmäßig werden nicht abgestimmte Daten in der ausgehenden Transition beibehalten und stehen in der Arbeitstabelle zur zukünftigen Verwendung zur Verfügung. Um nicht abgestimmte Daten zu entfernen, deaktivieren Sie die Option **Nicht abgestimmte Daten beibehalten**.

## Beispiel {#reconciliation-example}

Das folgende Beispiel zeigt einen Workflow zur Erstellung einer Profil-Audience, die direkt von einer importierten Datei mit neuen Kunden ausgeht. Er setzt sich aus folgenden Aktivitäten zusammen:

Der Workflow setzt sich folgendermaßen zusammen:

![](../assets/workflow-reconciliation-sample-1.0.png)


Er besteht aus den folgenden Aktivitäten:

* Eine [Datei laden](load-file.md)-Aktivität lädt eine Datei mit Profildaten hoch, die aus einem externen Tool extrahiert wurden.

  Beispiel:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Eine **Abstimmungsaktivität**, die die eingehenden Daten als Profile identifiziert, indem die Felder **E-Mail** und **Geburtsdatum** als Abstimmkriterien verwendet werden.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* Eine Aktivität [Zielgruppe speichern](save-audience.md), um eine neue Zielgruppe auf der Grundlage dieser Aktualisierungen zu erstellen. Sie können die Aktivität **Zielgruppe speichern** auch durch die Aktivität **Ende** ersetzen, wenn keine bestimmte Zielgruppe erstellt oder aktualisiert werden muss. Empfängerprofile werden in jedem Fall aktualisiert, sobald Sie den Workflow ausführen.


## Kompatibilität {#reconciliation-compat}

Die **Abstimmungsaktivität** ist nicht in der Client-Konsole vorhanden. Alle **Anreicherungsaktivitäten**, die in der Client-Konsole mit aktivierten Abstimmungsoptionen erstellt wurden, werden als **Abstimmungsaktivitäten** in der Campaign Web-Benutzeroberfläche angezeigt.
