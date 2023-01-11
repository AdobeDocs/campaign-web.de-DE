---
audience: end-user
title: Senden von Angeboten
description: Senden von Angeboten
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 94%

---

# Senden von Angeboten {#offers-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Angebotseinstellungen"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Erweiterte Einstellungen für Angebote"
>abstract="TBC"

Mit Adobe Campaign v8 Web können Sie mit Ihren E-Mail-Angeboten, die in der Konsole mit der **[!UICONTROL Interaction]** -Modul. Weiterführende Informationen zu Interaction und zur Verwaltung eines Angebotskatalogs in der Konsole finden Sie im Abschnitt [Dokumentation zu Campaign V8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html).

Die wichtigsten Schritte zum Senden von Angeboten mit einer E-Mail sind:

1. [Zu unterbreitende Angebote konfigurieren](#configure),
1. [Angebote in E-Mail einfügen](#insert).

## Zu unterbreitende Angebote konfigurieren {#configure}

Klicken Sie auf die Schaltfläche **[!UICONTROL Angebote]** im Bildschirm zur Inhaltsbearbeitung der E-Mail und konfigurieren Sie dann die zu unterbreitenden Angebote.

![](assets/create-content-offers.png)

1. Wählen Sie die Ihrer Angebotsumgebung entsprechende **[!UICONTROL Platzierung]** aus.

1. Um die Angebotsauswahl des Moduls zu verfeinern, wählen Sie eine spezifische **[!UICONTROL Angebotskategorie]**, in der Angebote sortiert werden.

   Wenn keine Kategorie angegeben wird, werden alle in der Umgebung enthaltenen Angebote vom Angebotsmodul berücksichtigt, es sei denn, ein **[!UICONTROL Angebots-Design]** wird ausgewählt.

   >[!NOTE]
   >
   >Themen sind Schlüsselwörter, die zuvor in den Kategorien definiert wurden. Sie dienen als Filter und ermöglichen es Ihnen, die Anzahl der zu unterbreitenden Angebote durch Auswahl in einer Reihe von Kategorien zu verfeinern.

1. Verwenden Sie das Feld **[!UICONTROL Vorschläge]**, um die Anzahl der Angebote anzugeben, die Sie in die E-Mail einfügen möchten.

1. Wählen Sie bei Bedarf die Option **[!UICONTROL Nicht infrage kommende Empfänger ausschließen]** aus.

   Mit dieser Option können Sie den Ausschluss von Empfängern aktivieren oder deaktivieren, für die nicht genügend geeignete Angebote vorhanden sind.

   * Wenn die Option aktiviert ist, werden Empfänger, die nicht genügend Vorschläge haben, vom Versand ausgeschlossen.
   * Wenn die Option deaktiviert ist, werden diese Empfänger nicht ausgeschlossen, erhalten jedoch nicht die angefragte Anzahl an Vorschlägen.

1. Wählen Sie bei Bedarf die Option **[!UICONTROL Alles ausblenden, wenn kein Angebot ausgewählt ist]**.

   Mit dieser Option können Sie festlegen, wie die Nachricht verarbeitet werden soll, falls einer der Vorschläge nicht existiert.

   * Wenn die Option aktiviert ist, wird die Darstellung des fehlenden Vorschlags nicht angezeigt, und es wird auch kein Inhalt in der Nachricht für diesen Vorschlag angezeigt.
   * Wenn die Option deaktiviert ist, wird die Nachricht selbst während des Versands abgebrochen, und die Empfänger erhalten keine Nachrichten mehr.

Nachdem Sie die Angebote konfiguriert haben, die in Ihrer E-Mail vorgeschlagen werden sollen, können Sie sie mit dem Ausdruckseditor in die E-Mail einfügen. [Erfahren Sie, wie Sie Angebote in die E-Mail einfügen](#insert)

## Einfügen von Angeboten in die E-Mail {#insert}

Angebote werden mit dem Ausdruckseditor in eine E-Mail eingefügt. Sie können wie folgt eingefügt werden:

* in der Betreffzeile der E-Mail,
* im Textkörper der E-Mail durch Personalisierung in einer beliebigen Inhaltskomponente. [Erfahren Sie, wie Sie Inhaltskomponenten hinzufügen](content-components.md)

>[!NOTE]
>
>Stellen Sie vor dem Einfügen eines Angebots sicher, dass Sie [konfiguriert haben, welche Angebote mit der E-Mail vorgeschlagen werden sollen](#configure).

Gehen Sie wie folgt vor, um ein Angebot mit dem Ausdruckseditor einzufügen:

1. Öffnen Sie den Ausdruckseditor und wählen Sie dann das Menü **[!UICONTROL Vorschläge]**.

   Die verfügbaren Vorschläge werden in der Liste angezeigt. Die Anzahl der Vorschläge wird bei der Konfiguration der zu unterbreitenden Angebote bestimmt.

   ![](assets/offer-insertion.png)

1. Fügen Sie die Vorschläge mithilfe der Personalisierungsfelder, Rendering-Funktionen oder Angebotsattribute, die für jeden Vorschlag verfügbar sind, zum Betreff oder Text der E-Mail hinzu.

   ![](assets/offer-inserted.png)
