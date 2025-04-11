---
audience: end-user
title: Verwenden der Workflow-Aktivität „Abstimmung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Abstimmung“ verwenden
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 41%

---

# Abstimmung {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Aktivität „Abstimmung“"
>abstract="Die Aktivität **Abstimmung** ist eine **Zielgruppenbestimmungs**-Aktivität, die die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle definiert. Zum Beispiel kann die Aktivität **Abstimmung** hinter der Aktivität **Datei laden** platziert werden, um nicht standardmäßige Daten in die Datenbank zu laden. In diesem Fall definiert die Aktivität **Abstimmung** die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in der externen Tabelle."

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

Die Aktivität **Abstimmung** ist eine **Targeting**-Aktivität, die die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in einer Arbeitstabelle definiert, z. B. Daten aus einer externen Datei.

Zum Beispiel kann die Aktivität **Abstimmung** hinter der Aktivität **Datei laden** platziert werden, um nicht standardmäßige Daten in die Datenbank zu laden. In diesem Fall definiert die Aktivität **Abstimmung** die Verknüpfung zwischen den Daten in der Adobe Campaign-Datenbank und den Daten in der Arbeitstabelle.

## Best Practices {#reconciliation-best-practices}

Während die Aktivität **Anreicherung** zusätzliche Daten definiert, die in Ihrem Workflow verarbeitet werden sollen (z. B. Daten aus mehreren Datensätzen kombinieren oder Links zu einer temporären Ressource erstellen), verknüpft die Aktivität **Abstimmung** nicht identifizierte Daten mit vorhandenen Ressourcen.

>[!NOTE]
>Abstimmvorgänge erfordern, dass die Daten der verknüpften Dimensionen bereits in der Datenbank vorhanden sind. Wenn Sie beispielsweise eine Datei mit Käufen importieren, die angibt, welches Produkt zu welchem Zeitpunkt und von welchem Kunden gekauft wurde, müssen das Produkt und der Client bereits in der Datenbank vorhanden sein.

## Konfigurieren der Abstimmungsaktivität {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Zielgruppendimension"
>abstract="Wählen Sie die neue Zielgruppendimension aus. Eine Dimension definiert die Zielpopulation: Empfänger, App-Abonnenten, Benutzer, Abonnenten und mehr. Standardmäßig ist die aktuelle Zielgruppendimension ausgewählt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Abstimmungsregeln"
>abstract="Abstimmregeln für die Deduplizierung auswählen. Um Attribute zu verwenden, wählen Sie die Option **Einfache Attribute** und dann die Felder für Quelle und Ziel aus. Um mithilfe des Abfrage-Modelers eine eigene Abstimmungsbedingung zu erstellen, wählen Sie die Option **Erweiterte Abstimmungsbedingungen**."
>additional-url="https://experienceleague.adobe.com/de/docs/campaign-web/v8/query-database/query-modeler-overview" text="Arbeiten mit dem Abfrage-Modeler"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Auswählen der Zielgruppendimension"
>abstract="Wählen Sie die Zielgruppendimension für Ihre eingehenden Daten zum Abstimmen aus."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=de#targeting-dimensions" text="Zielgruppendimensionen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Beibehalten nicht abgestimmter Daten"
>abstract="Standardmäßig werden nicht abgestimmte Daten in der ausgehenden Transition aufbewahrt und stehen dann in der Arbeitstabelle für die zukünftige Verwendung zur Verfügung. Um nicht abgestimmte Daten zu entfernen, deaktivieren Sie die Option **Nicht abgestimmte Daten beibehalten**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Abstimmungsattribut"
>abstract="Wählen Sie das Attribut aus, das zur Abstimmung der Daten verwendet werden soll, und klicken Sie auf Bestätigen ."

Gehen Sie wie folgt vor, um die Aktivität **Abstimmung** zu konfigurieren:

1. Fügen Sie **Workflow** Aktivität Abstimmung hinzu. Diese Aktivität sollte einer Transition folgen, die eine Population enthält, deren Zielgruppendimension nicht direkt aus Adobe Campaign stammt.

1. Wählen Sie die neue Zielgruppendimension aus. Eine Dimension definiert die Zielpopulation: Empfänger, App-Abonnenten, Benutzer, Abonnenten und mehr. [Erfahren Sie mehr über Zielgruppendimensionen](../../audience/about-recipients.md#targeting-dimensions)

1. Wählen Sie die für Abstimmung zu verwendenden Felder aus. Es können mehrere Abstimmkriterien definiert werden.

   1. Um Datenabstimmungsattribute zu verwenden, wählen Sie die Option **Einfache Attribute**. Das Feld **Source** listet die in der eingehenden Transition verfügbaren Felder auf, die abgeglichen werden sollen. Das Feld **Ziel** entspricht den Feldern der ausgewählten Zielgruppendimension. Daten werden abgestimmt, wenn Quelle und Ziel identisch sind. Wählen Sie beispielsweise die **E-Mail**-Felder, um Profile anhand ihrer E-Mail-Adresse zu deduplizieren.

      Um ein weiteres Abstimmkriterium hinzuzufügen, klicken Sie auf die Schaltfläche **Regel hinzufügen**. Wenn mehrere Join-Bedingungen angegeben sind, müssen sie alle überprüft werden, damit die Daten miteinander verknüpft werden können.

      ![Beispiel für Abstimmkriterien](../assets/workflow-reconciliation-criteria.png)

   1. Um andere Attribute zur Datenabstimmung zu verwenden, wählen Sie die Option **Erweiterte Abstimmungsbedingungen**. Anschließend können Sie mithilfe des Abfrage-Modelers eine eigene Abstimmungsbedingung erstellen. [Erfahren Sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md).

1. Filtern Sie die Daten mithilfe der Schaltfläche **Filter erstellen**, um sie abzugleichen. Auf diese Weise können Sie mithilfe des Abfrage-Modelers eine benutzerdefinierte Bedingung erstellen. [Erfahren Sie mehr über die Arbeit mit dem Abfrage-Modeler](../../query/query-modeler-overview.md).

Standardmäßig werden nicht abgestimmte Daten in der ausgehenden Transition aufbewahrt und stehen dann in der Arbeitstabelle für die zukünftige Verwendung zur Verfügung. Um nicht abgestimmte Daten zu entfernen, deaktivieren Sie die Option **Nicht abgestimmte Daten beibehalten**.

## Beispiel {#reconciliation-example}

Das folgende Beispiel zeigt einen Workflow zur Erstellung einer Profil-Audience, die direkt von einer importierten Datei mit neuen Kunden ausgeht. Es umfasst die folgenden Aktivitäten:

Der Workflow setzt sich folgendermaßen zusammen:

![Workflow-Beispiel](../assets/workflow-reconciliation-sample-1.0.png)

Er besteht aus den folgenden Aktivitäten:

* Eine [Datei laden](load-file.md)-Aktivität lädt eine Datei hoch, die aus einem externen Tool extrahierte Profildaten enthält.

  Beispiel:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Eine Aktivität **Abstimmung** identifiziert die eingehenden Daten als Profile, indem sie die Felder **E-Mail** und **Geburtsdatum** als Abstimmkriterien verwendet.

  ![Beispiel für eine Abstimmungsaktivität](../assets/workflow-reconciliation-sample-1.1.png)

* Eine [Zielgruppe speichern](save-audience.md)-Aktivität erstellt auf Grundlage dieser Aktualisierungen eine neue Zielgruppe. Sie können auch die Aktivität **Zielgruppe speichern** durch eine Aktivität **Ende** ersetzen, wenn keine bestimmte Zielgruppe erstellt oder aktualisiert werden muss. Empfängerprofile werden in jedem Fall aktualisiert, sobald Sie den Workflow ausführen.

## Kompatibilität {#reconciliation-compat}

Die **Abstimmungsaktivität** ist nicht in der Client-Konsole vorhanden. Alle **Anreicherung** Aktivitäten, die in der Client-Konsole mit aktivierten Abstimmoptionen erstellt wurden, werden in **Web-Benutzeroberfläche von Campaign als**-Aktivitäten angezeigt.