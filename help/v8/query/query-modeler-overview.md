---
audience: end-user
title: Arbeiten mit dem Abfrage-Modeler
description: Lernen Sie, mit dem Abfrage-Modeler von Adobe Campaign Web zu arbeiten.
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 9c72d73b5279a01492ea3ccd295e513e91f0c050
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 60%

---

# Arbeiten mit dem Abfrage-Modeler {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Neues Abfragemodell"
>abstract="Adobe Campaign Web verfügt über einen Abfrage-Modeler, der den Prozess des Filterns von Datenbanken vereinfacht, um spezifische Zielgruppen auf der Grundlage verschiedener Kriterien auszuwählen. Dies schließt die Verwendung erweiterter Ausdrücke und Operatoren ein. Der Abfrage-Modeler ist in jedem Kontext verfügbar, in dem Sie Regeln zum Filtern von Daten definieren müssen."

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Neues Abfragemodell"
>abstract="Adobe Campaign Web verfügt über einen Abfrage-Modeler, der den Prozess des Filterns von Datenbanken vereinfacht, um spezifische Zielgruppen auf der Grundlage verschiedener Kriterien auszuwählen. Dies schließt die Verwendung erweiterter Ausdrücke und Operatoren ein. Der Abfrage-Modeler ist in jedem Kontext verfügbar, in dem Sie Regeln zum Filtern von Daten definieren müssen."

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Abfrage-Modeler"
>abstract="Definieren Sie Filterkriterien für Empfängerinnen und Empfänger oder jede andere Zielgruppendimension aus der Datenbank. Nutzen Sie Ihre Adobe Experience Platform-Zielgruppe, um die Zielgruppe weiter zu verfeinern und die Wirkung der Kampagne zu maximieren."

Adobe Campaign Web verfügt über einen Abfrage-Modeler, der den Prozess des Filterns von Datenbanken vereinfacht, um spezifische Zielgruppen auf der Grundlage verschiedener Kriterien auszuwählen. Dies schließt die Verwendung erweiterter Ausdrücke und Operatoren ein.

## Zugreifen auf den Abfrage-Modeler

Der Abfrage-Modeler ist in jedem Kontext verfügbar, in dem Sie Regeln zum Filtern von Daten definieren müssen.

| Verwendung | Beispiel |
|  ---  |  ---  |
| **Zielgruppen definieren**: Geben Sie die Population an, die Sie in Ihren Nachrichten oder Workflows ansprechen möchten, und erstellen Sie mühelos neue Zielgruppen, die auf Ihre Anforderungen zugeschnitten sind. | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **Workflow-Aktivitäten anpassen**: Wenden Sie Regeln innerhalb von Workflow-Aktivitäten an, z. B. Aufspaltung und Abstimmung, um sie an Ihre spezifischen Anforderungen anzupassen. | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **Vordefinierte Filter**: Erstellen Sie vordefinierte Filter, die bei verschiedenen Filtervorgängen als Abkürzungen dienen, unabhängig davon, ob Sie mit Datenlisten arbeiten oder die Zielgruppe für einen Versand bilden. | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **Berichtsdaten filtern**: Fügen Sie eine Regel hinzu, um die in Berichten angezeigten Daten zu filtern. | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **Listen anpassen**: Erstellen Sie benutzerdefinierte Regeln, um die in Listen angezeigten Daten zu filtern, wie z. B. Empfänger, Versandlisten usw. | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->

## Benutzeroberfläche des Abfrage-Modelers {#interface}

Das Abfragemodell bietet eine zentrale Arbeitsfläche, auf der Sie Ihre Abfrage erstellen, und einen rechten Bereich, der Informationen zu Ihrer Abfrage enthält.

![](assets/query-interface.png)

### Die zentrale Arbeitsfläche {#canvas}

Auf der zentralen Arbeitsfläche des Abfragemodells können Sie die verschiedenen Komponenten hinzufügen und kombinieren, um Ihre Abfrage zu erstellen. [Erfahren Sie, wie Sie eine Abfrage erstellen](build-query.md)

Die Symbolleiste oben rechts auf der Arbeitsfläche bietet Optionen zum einfachen Bearbeiten der Abfragekomponenten und Navigieren auf der Arbeitsfläche:

* **Mehrfach-Auswahlmodus**: Wählen Sie mehrere Filterkomponenten aus, die kopiert und am gewünschten Speicherort eingefügt werden sollen.
* **Drehen**: Schaltet die Arbeitsfläche vertikal um.
* **Bildschirmgröße**: Passen Sie den Zoomgrad der Arbeitsfläche an Ihren Bildschirm an.
* **Auszoomen** / **Einzoomen**: Zoomen Sie aus oder in die Arbeitsfläche.
* **Anzeigekarte**: Öffnet eine Momentaufnahme der Arbeitsfläche, in der Sie sich befinden.

### Bereich &quot;Regeleigenschaften&quot; {#rule-properties}

Auf der rechten Seite wird die **[!UICONTROL Regeleigenschaften]** enthält Informationen zu Ihrer Abfrage. Damit können Sie verschiedene Vorgänge ausführen, um die Abfrage zu überprüfen und sicherzustellen, dass sie Ihren Anforderungen entspricht. [Erfahren Sie, wie Sie Ihre Abfrage überprüfen und validieren](build-query.md#check-and-validate-your-query)
