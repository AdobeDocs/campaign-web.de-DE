---
audience: end-user
title: Erstellen und Veröffentlichen eines Angebots
description: Erfahren Sie, wie Sie ein Angebot in Campaign Web erstellen, konfigurieren, genehmigen und bereitstellen.
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7bd09b83112efb99c90884b7da21a5e9a5c76b6c
workflow-type: tm+mt
source-wordcount: 1057
ht-degree: 3%

---

# Erstellen und Veröffentlichen eines Angebots {#create-offer}

Ein **Angebot** ist ein individueller Vorschlag mit eigenem Eignungszeitraum, Zielgruppenfilter, Gewichtung und Inhalt. Angebote sind im Angebotskatalog über **Kategorien** organisiert und werden Empfängerinnen und Empfängern über eine **Platzierung“**.

Bevor Sie ein Angebot erstellen, stellen Sie sicher, dass die Angebotsumgebung konfiguriert und mindestens eine Platzierung veröffentlicht wurde. Weitere Informationen finden [ unter „Konfigurieren einer ](offer-environment.md)&quot; und [Erstellen und Verwalten von Platzierungen](offer-space.md).

## Zugriff auf den Angebotskatalog {#access}

Um Angebote zu durchsuchen und zu erstellen, wählen **[!UICONTROL Angebote]** in der linken Navigationsleiste aus. Die Liste zeigt die vorhandenen Angebote an. Verwenden Sie das Suchfeld, den Ordnerselektor oder den [Abfrage-Modellierer](../query/query-modeler-overview.md), um die Liste zu filtern.

![Screenshot mit dem Angebotskatalog.](assets/offers-offer.png){zoomable="yes"}

Klicken Sie auf einen Angebotsnamen, um ihn zur Bearbeitung zu öffnen, oder verwenden Sie die drei Punkte daneben, um ihn zu **[!UICONTROL Duplizieren]** oder **[!UICONTROL Löschen]**.

## Angebot erstellen {#create}

So erstellen Sie ein neues Angebot:

1. Klicken Sie in der Liste der Angebote auf **[!UICONTROL Angebot erstellen]**.

1. Wählen Sie **[!UICONTROL Vorlage]** aus, aus der das Angebot erstellt werden soll (z. B. ein leeres Angebot oder eine anonyme Angebotsvorlage).

   ![Screenshot zur Angebotserstellung.](assets/offers-offer-1.png){zoomable="yes"}

1. Geben Sie einen **[!UICONTROL Titel]** ein und weisen Sie das Angebot optional einem Benutzer zu, indem Sie **[!UICONTROL Zugewiesen an]** und/oder geben Sie einen **[!UICONTROL Angebotscode]** ein.

1. Erweitern Sie **[!UICONTROL Zusätzliche Optionen]**, um den automatisch generierten **[!UICONTROL internen Namen]** zu bearbeiten, wählen Sie die **[!UICONTROL Kategorie]**, in der das Angebot gespeichert ist, oder fügen Sie eine Beschreibung hinzu. Dieser Schritt ist optional.

1. Erweitern Sie **[!UICONTROL Genehmigungen]**, um Genehmigende den Gruppen **[!UICONTROL Eignungsvalidierung]** und **[!UICONTROL Inhaltsvalidierung]** zuzuweisen. Dieser Schritt ist optional.

1. Erweitern Sie **[!UICONTROL Benutzerdefinierte Optionen]** um alle zusätzlichen Felder auszufüllen, die Ihr Unternehmen zum Angebotsschema hinzugefügt hat. Die in diesem Abschnitt angezeigten Felder variieren von einer Campaign-Instanz zur anderen. Dieser Schritt ist optional.

1. Wählen Sie **[!UICONTROL Erstellen]** aus. Der Bildschirm mit den vollständigen Einstellungen wird angezeigt.

   ![Screenshot mit dem Bildschirm mit den Angebotseinstellungen.](assets/offers-offer-2.png){zoomable="yes"}

### Definieren der Eignung {#eligibility}

In diesem Abschnitt können Sie steuern, wann und wem das Angebot unterbreitet werden kann. Folgende Optionen stehen zur Verfügung:

* **[!UICONTROL Zeitplan]** - Legen Sie das Start- und Enddatum fest, zwischen denen das Angebot unterbreitet werden kann.

  >[!NOTE]
  >
  >Schnittmengen aus Eignungszeiträumen mit der übergeordneten Kategorie werden berücksichtigt: Selbst wenn der eigene Zeitplan des Angebots breiter ist, wird das Angebot nur angezeigt, während seine übergeordnete Kategorie ebenfalls geeignet ist.

* **[!UICONTROL Filter für die Zielgruppe]** — Klicken Sie auf **[!UICONTROL Filter erstellen]**, um den Regel-Builder zu öffnen und das Angebot auf eine bestimmte Zielgruppe zu beschränken. Lassen Sie den Filter leer, damit das Angebot für die gesamte Umgebung und Zielgruppe geeignet ist. Informationen zur Wiederverwendung eines **vordefinierten Filters** der auf Plattformebene deklariert wurde, finden Sie in der [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}. Vordefinierte Filter werden über die Client-Konsole erstellt.

* **[!UICONTROL Verwaltung der Angebotsgewichtung]** - Klicken Sie auf **[!UICONTROL Angebotsgewichtung anzeigen]** und dann auf **[!UICONTROL Gewichtung hinzufügen]**, um die Priorität des Angebots zu beeinflussen, wenn mehrere Angebote gleichzeitig geeignet sind. Jede Gewichtung hat ein Startdatum, ein Enddatum und einen optionalen Filter.

>[!NOTE]
>
>Das Angebotsmodul sortiert geeignete Angebote nach abnehmender Gewichtung und gibt zuerst die höchsten gewichteten Vorschläge zurück. Die Auswahllogik - auch als **bezeichnet** - berücksichtigt auch die Eignungsregeln und Gewichtungen, die für die übergeordnete Kategorie und die Umgebung konfiguriert sind. Weitere Informationen zum Schlichtungsprinzip finden Sie in der [ zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=de){target="_blank"}.

### Inhalt des Berichts definieren {#content}

Wählen Sie im Angebot die Registerkarte **[!UICONTROL Inhalt]** aus. Auf dieser Registerkarte werden die Werte definiert, die von der Rendering-Funktion verfügbar gemacht werden.

1. Füllen Sie die vordefinierten Attribute - **[!UICONTROL Titel]**, **[!UICONTROL Ziel-URL]**, **[!UICONTROL Bild-URL]** und alle benutzerdefinierten Attribute aus, die im Angebotsschema deklariert wurden.

1. Verwenden Sie den [Ausdruckseditor](../query/expression-editor.md) um die Werte mit Profildaten, Angebotsattributen oder Vorschlagsfeldern zu personalisieren.

1. Klicken Sie für die HTML- und Text-Payloads **[!UICONTROL Inhalt bearbeiten]**, um den Inhaltseditor zu öffnen. Sie können Inhalte von Grund auf neu entwerfen, Ihre eigene HTML codieren oder vorhandene HTML importieren, optional ausgehend von einer Beispielvorlage.

>[!IMPORTANT]
>
>Die im Abschnitt **[!UICONTROL Inhalt]** verfügbaren Attribute hängen vom [!DNL nms:offer] Schema ab. Um benutzerdefinierte Attribute verfügbar zu machen, erweitern Sie das Schema und wählen Sie sie im Abschnitt **[!UICONTROL Angebotsinhalt]** aus. Weitere Informationen finden Sie unter [Arbeiten mit Schemata](../administration/schemas.md).

## Erstellen einer Vorschau des Angebots {#preview}

Sie können das Angebot vor dem Absenden in der Vorschau anzeigen.

1. Wählen Sie im Angebot die Registerkarte **[!UICONTROL Vorschau]** neben **[!UICONTROL Übersicht]** aus.

   ![Screenshot der Angebotsvorschau.](assets/offers-offer-3.png){zoomable="yes"}

1. Wählen Sie ein Zielprofil und gegebenenfalls die Platzierung aus, für die die Vorschau ausgeführt werden soll.

   Die in der Platzierung definierte Rendering-Funktion wird auf den Angebotsinhalt angewendet, und die daraus resultierende Darstellung wird angezeigt.

>[!NOTE]
>
>Wenn die Vorschau einen Fehler oder keinen Inhalt zurückgibt, überprüfen Sie die Rendering-Funktion der Platzierung, die Eignungsregeln des Angebots und ob alle erforderlichen Inhaltsfelder ausgefüllt sind.

## Genehmigen und Bereitstellen des Angebots {#approve-deploy}

Angebote sind in Sendungen nicht sofort verfügbar: Sie durchlaufen einen Genehmigungs- und Bereitstellungszyklus.

1. Klicken Sie in der Angebotsübersicht auf **[!UICONTROL Genehmigung]**.

   ![Screenshot der Angebotsvalidierung.](assets/offers-offer-4.png){zoomable="yes"}

1. Genehmigen Sie **[!UICONTROL Eignung]** und den **[!UICONTROL Inhalt]**. Inhalte können pro Platzierung genehmigt werden, sodass Sie sie für eine Platzierung genehmigen können, während andere ausstehen.

1. Sobald beide Genehmigungen erteilt wurden, klicken Sie auf **[!UICONTROL Bereitstellen]**, um das Angebot in der Live-Umgebung zu veröffentlichen.

1. Aktualisieren Sie die Angebotsansicht, um zu bestätigen **[!UICONTROL dass die]**-Darstellung auf dem neuesten Stand ist.

<!--
>[!NOTE]
>
>Once deployed, the design offer's status resets to **[!UICONTROL Being edited]** — its normal draft status, not a sign that someone is actively editing it. This just means the design offer is ready to accept further changes, which would then need to go through a new approval and deployment cycle. The live representation itself remains untouched until that happens.
-->

>[!CAUTION]
>
>Die Validierung der Eignung und des Inhalts eines Angebots sind zwei unterschiedliche Aktionen. Ein Angebot kann teilweise genehmigt werden (z. B. nur Inhalt) und so lange nicht verfügbar sein, bis auch die Eignungsvalidierung erteilt wird.

## Überwachen des Angebots-Dashboard {#dashboard}

Die Registerkarte **[!UICONTROL Überblick]** fasst den Angebotsstatus in den Karten **[!UICONTROL Eigenschaften]**, **[!UICONTROL Inhalt]** und **[!UICONTROL Eignung]** zusammen, wobei jeweils ein Stiftsymbol angezeigt wird, um zur Bearbeitung zurückzukehren. Eine **[!UICONTROL Darstellung]**-Karte listet jede Platzierung auf, mit der das Angebot verknüpft ist, zusammen mit ihrem aktuellen Design-Status.

![Screenshot mit dem Angebots-Dashboard.](assets/offers-offer-5.png){zoomable="yes"}

Klicken Sie auf **[!UICONTROL Protokolle]**, um auf die Bereitstellungsprotokolle zuzugreifen, oder auf das Menü **・・** (**[!UICONTROL Mehr]**), um das Angebot **[!UICONTROL zu duplizieren]** oder **[!UICONTROL Löschen]**.

Sobald ein Angebot live ist, wird durch Ändern einer beliebigen Einstellung das Design-Angebot wieder in einen bearbeitbaren Status versetzt. Die Live-Darstellung bleibt bis zum nächsten Genehmigungs- und Bereitstellungszyklus unberührt.

## Verwenden des Angebots in einem Versand {#use-in-delivery}

Wenn das Angebot live ist, kann es aus jedem Versand ausgewählt werden, der auf die passende Platzierung abzielt. Erfahren Sie in [Hinzufügen von Angeboten zu Ihren Nachrichten](../msg/offers.md), wie Sie Angebote für einen Versand einrichten.

Die vollständige Integration des ausgehenden Versands, einschließlich der Art und Weise, wie der Modulaufruf aufgebaut ist und wie das Tracking auf Angebotslinks angewendet wird, finden Sie in der [Campaign v8-Dokumentation Angebote in ausgehenden Sendungen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html){target="_blank"}.

