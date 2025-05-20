---
audience: end-user
title: Arbeiten mit dem Abfrage-Modeler
description: Lernen Sie, mit dem Abfrage-Modeler von Adobe Campaign Web zu arbeiten.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 80%

---

# Arbeiten mit dem Abfrage-Modeler {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Neuer Regel-Builder"
>abstract="Es ist nun ein neuer Regel-Builder verfügbar, der Sie bei der Definition komplexer Bedingungen in einer verbesserten Benutzeroberfläche unterstützt. Sie können bei Bedarf vom alten zum neuen Regel-Builder wechseln."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Neuer Abfrage-Modeler"
>abstract="Adobe Campaign Web verfügt über einen Abfrage-Modeler, der den Prozess des Filterns von Datenbanken vereinfacht, um spezifische Zielgruppen auf der Grundlage verschiedener Kriterien auszuwählen. Dies schließt die Verwendung erweiterter Ausdrücke und Operatoren ein. Der Abfrage-Modeler ist in jedem Kontext verfügbar, in dem Sie Regeln zum Filtern von Daten definieren müssen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Abfrage-Modeler"
>abstract="Definieren Sie Filterkriterien für Empfängerinnen und Empfänger oder jede andere Zielgruppendimension aus der Datenbank. Nutzen Sie Ihre Adobe Experience Platform-Zielgruppe, um die Zielgruppe weiter zu verfeinern und die Wirkung der Kampagne zu maximieren."

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Zielgruppe verfeinern"
>abstract="Diese Regeln können nur in der Client-Konsole geändert werden."

Die Adobe Campaign Web-Benutzeroberfläche verfügt über einen Abfrage-Modeler, der das Filtern von Datenbanken anhand verschiedener Kriterien vereinfacht. Dadurch wird die vollständige Kompatibilität mit den in der Client-Konsole erstellten Abfragen sichergestellt und ein nahtloser Übergang zur Web-Benutzeroberfläche ermöglicht.

Außerdem verwaltet der Abfrage-Modeler sehr komplexe und lange Abfragen effizient – und das bei höherer Flexibilität und Genauigkeit. Außerdem werden vordefinierte Filter in Bedingungen unterstützt, sodass Sie Ihre Abfragen mühelos präzisieren und gleichzeitig erweiterte Ausdrücke und Operatoren für umfassende Zielgruppen-Targeting- und Segmentierungsstrategien nutzen können.

## Zugreifen auf den Abfrage-Modeler

Der Abfrage-Modeler ist in jedem Kontext verfügbar, in dem Sie Regeln zum Filtern von Daten definieren müssen.

| Verwendung | Beispiel |
|  ---  |  ---  |
| **Zielgruppen definieren**: Geben Sie die Population an, die Sie in Ihren Nachrichten oder Workflows ansprechen möchten, und erstellen Sie mühelos neue Zielgruppen, die auf Ihre Anforderungen zugeschnitten sind. [Weitere Informationen zum Erstellen von Zielgruppen](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild, das den Zugriff auf die Benutzeroberfläche zur Zielgruppenerstellung zeigt] |
| **Workflow-Aktivitäten anpassen**: Wenden Sie Regeln innerhalb von Workflow-Aktivitäten an, z. B. **Aufspaltung** und **Abstimmung**, um sie an Ihre spezifischen Anforderungen anzupassen.  [Weitere Informationen zu Workflow-Aktivitäten](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild, das den Zugriff auf Optionen zur Workflow-Anpassung zeigt] |
| **Vordefinierte Filter**: Erstellen Sie vordefinierte Filter, die bei verschiedenen Filtervorgängen als Abkürzungen dienen, unabhängig davon, ob Sie mit Datenlisten arbeiten oder die Zielgruppe für einen Versand bilden.  [Erfahren Sie, wie Sie mit vordefinierten Filtern arbeiten](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild, das den Zugriff auf vordefinierte Filter zeigt] |
| **Berichtsdaten filtern**: Fügen Sie Regeln hinzu, um die in Berichten angezeigten Daten zu filtern. [Informationen zum Arbeiten mit Profilen](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild, das die Filterung von Daten in Berichten zeigt] |
| **Listen anpassen**: Erstellen Sie benutzerdefinierte Regeln, um die in Listen angezeigten Daten zu filtern, wie z. B. Empfängerinnen und Empfänger oder Sendungslisten. [Informationen zum Filtern von Listen](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Bild, das die Anpassung von Listenfiltern zeigt] |
| **Bedingten Inhalt erstellen**: Gestalten Sie den E-Mail-Inhalt dynamisch, indem Sie Bedingungen erstellen, die festlegen, welche Inhalte den verschiedenen Empfangenden angezeigt werden sollen, und so personalisierte und relevante Nachrichten sicherstellen. [Informationen zum Erstellen von bedingten Inhalten](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [Bild, das die Erstellung von bedingten Inhalten zeigt] |

>[!NOTE]
>
>Beim Zugriff auf ein in der Client-Konsole erstelltes Objekt, in dem Regeln wie eine Zielgruppe oder ein vordefinierter Filter angewendet wurden, wird möglicherweise der Abschnitt **[!UICONTROL Zielgruppe verfeinern]** angezeigt. Dies bedeutet, dass zusätzliche Parameter zur Verfeinerung der Regel-Zielgruppe konfiguriert wurden. Diese Parameter können nur in der Konsole geändert werden.
>
>![Bild, das einen Warnhinweis zur Verfeinerung von Zielgruppen zeigt](assets/target-warning.png){zoomable="yes"}

## Benutzeroberfläche des Abfrage-Modellierers {#interface}

Der Abfrage-Modeler bietet eine zentrale Arbeitsfläche, auf der Sie Ihre Abfrage erstellen, sowie einen rechten Bereich mit Informationen zu Ihrer Abfrage.

>[!IMPORTANT]
>
>Eine brandneue Benutzeroberfläche für den Abfrage-Modellierer ist verfügbar. Mit dem neuen Regel-Builder können Sie Ihre Abfrage dank der vereinfachten Benutzeroberfläche einfacher erstellen. Um zu diesem Erlebnis zu wechseln, drücken Sie die Umschalttaste in der oberen rechten Ecke. Sie können jederzeit zum klassischen Abfrage-Modellierer zurückkehren, indem Sie einfach den Umschalter drücken, um die neue Benutzeroberfläche zu deaktivieren. Sie können in dieser neuen Benutzeroberfläche dieselben Prinzipien wie beim Abfrage-Modellierer anwenden.
>![Bild, das den Umschalter für die neue Benutzeroberfläche des Regel-Builders zeigt](assets/query-modeler-toggle.png){zoomable="yes"}


>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Neues Regel-Builder-Erlebnis"
>abstract="Verwenden Sie diesen Umschalter, um zwischen dem klassischen Abfrage-Modeler und dem neuen Regel-Builder-Erlebnis zu wechseln. Mit dem neuen Rule Builder können Abfragen dank der vereinfachten und intuitiven Benutzeroberfläche leichter erstellt werden."

![Bild, das die Benutzeroberfläche des Abfrage-Modelers zeigt](assets/query-interface.png){zoomable="yes"}

### Die zentrale Arbeitsfläche {#canvas}

Der Abfrage-Modeler bietet eine zentrale Arbeitsfläche, auf der Sie die verschiedenen Komponenten hinzufügen und kombinieren können, um Ihre Abfrage zu erstellen. [So erstellen Sie eine Abfrage](build-query.md)

>[!BEGINTABS]

>[!TAB Klassischer Abfrage-Modellierer]

Die Symbolleiste in der rechten unteren Ecke der Arbeitsfläche bietet Optionen zum einfachen Bearbeiten der Abfragekomponenten und zum Navigieren auf der Arbeitsfläche:

* **Mehrfachauswahl-Modus**: Wählen Sie mehrere Filterkomponenten aus, um sie zu kopieren und am gewünschten Ort einzufügen.
* **Drehen**: Dreht die Arbeitsfläche vertikal.
* **An Bildschirm anpassen**: Passt die Vergrößerung der Arbeitsfläche an Ihren Bildschirm an.
* **Verkleinern**/**Vergrößern**: Verkleinert bzw. vergrößert die Arbeitsfläche.
* **Karte anzeigen**: Öffnet einen Snapshot der Arbeitsfläche mit Ihrer aktuellen Position.

>[!TAB Neues Rule Builder-Erlebnis]

Die Symbolleiste oben rechts in der Arbeitsfläche bietet Optionen zum einfachen Bearbeiten der Abfragekomponenten und Navigieren auf der Arbeitsfläche:

* **Auswahl nach oben**: Verschiebt die Komponente um eine Zeile nach oben.
* **Auswahl nach unten verschieben**: Verschieben der Komponente in einer Zeile nach unten.
* **Gruppenauswahl**: Fügen Sie zwei Komponenten in eine Gruppe ein.
* **Auswahl aufheben**: Trennen Sie die Komponenten einer einzelnen Gruppe.
* **Alle**: Alle Gruppen erweitern.
* **Alle reduzieren**: Alle Gruppen reduzieren.
* **Alle entfernen**: Entfernen Sie alle Gruppen und Komponenten.

>[!ENDTABS]

### Der Bereich „Regeleigenschaften“ {#rule-properties}

Das Fenster **[!UICONTROL Regeleigenschaften]** rechts enthält Informationen zu Ihrer Abfrage. Damit können Sie verschiedene Vorgänge ausführen, um Ihre Abfrage zu überprüfen und sicherzustellen, dass sie Ihren Anforderungen entspricht. Dieser Bereich wird beim Einrichten einer Abfrage zum Erstellen einer Zielgruppe angezeigt. [So überprüfen und validieren Sie Ihre Abfrage](build-query.md#check-and-validate-your-query)
