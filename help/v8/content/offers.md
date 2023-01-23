---
audience: end-user
title: Senden von Angeboten
description: Senden von Angeboten
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 62%

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

Adobe Campaign v8 Web ermöglicht es Ihnen, mit Ihren E-Mails Angebote zu senden, die in der Konsole mithilfe des Moduls **[!UICONTROL Interaction]** erstellt wurden. Weitere Informationen zu Interaction und zur Verwaltung eines Angebotskatalogs in der Konsole finden Sie in der [Dokumentation zu Campaign V8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=de){target="_blank"}.

Die wichtigsten Schritte zum Senden von Angeboten mit einer E-Mail sind:

1. [Zu unterbreitende Angebote konfigurieren](#configure),
1. [Angebote in E-Mail einfügen](#insert).

## Zu unterbreitende Angebote konfigurieren {#configure}

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Angebote]** im Bildschirm zur Inhaltsbearbeitung der E-Mail.

   ![](assets/setup-offers.png)

1. Konfigurieren Sie, welche Angebote den Empfängern vorgeschlagen werden sollen. Wählen Sie zuerst die **[!UICONTROL Platzierung]** die Ihrer Angebotsumgebung entspricht.

   ![](assets/create-content-offers.png)

1. Um die Angebotsauswahl des Moduls zu verfeinern, wählen Sie eine spezifische **[!UICONTROL Angebotskategorie]**, in der Angebote sortiert werden.

   Wenn keine Kategorie angegeben wird, werden alle in der Umgebung enthaltenen Angebote vom Angebotsmodul berücksichtigt, es sei denn, ein **[!UICONTROL Angebotsdesign]** ausgewählt ist.

   >[!NOTE]
   >
   >Themen sind Schlüsselwörter, die zuvor in den Kategorien definiert wurden. Sie dienen als Filter und ermöglichen es Ihnen, die Anzahl der zu unterbreitenden Angebote durch Auswahl in einer Reihe von Kategorien zu verfeinern.

1. Verwenden Sie das Feld **[!UICONTROL Vorschläge]**, um die Anzahl der Angebote anzugeben, die Sie in die E-Mail einfügen möchten.

1. Wählen Sie bei Bedarf die Option **[!UICONTROL Nicht infrage kommende Empfänger ausschließen]** aus.

   Mit dieser Option können Sie den Ausschluss von Empfängern aktivieren oder deaktivieren, für die nicht genügend geeignete Angebote vorhanden sind.

   * Wenn die Option aktiviert ist, werden Empfänger, die nicht genügend Vorschläge haben, vom Versand ausgeschlossen.
   * Wenn die Option deaktiviert ist, werden diese Empfänger nicht ausgeschlossen, können jedoch nicht über die angeforderte Anzahl von Vorschlägen verfügen.

1. Wählen Sie bei Bedarf die Option **[!UICONTROL Alles ausblenden, wenn kein Angebot ausgewählt ist]**.

   Diese Option ermöglicht die Auswahl der Art der Nachrichtenverarbeitung, falls ein Vorschlag nicht existiert.

   * Wenn die Option aktiviert ist, wird die Darstellung des fehlenden Vorschlags nicht angezeigt und es wird kein Inhalt in der Nachricht für diesen Vorschlag angezeigt.
   * Wenn die Option deaktiviert ist, wird die Nachricht selbst während des Versands abgebrochen und die Empfänger können keine Nachrichten mehr erhalten.

Nachdem Sie die Angebote konfiguriert haben, die in Ihrer E-Mail vorgeschlagen werden sollen, können Sie sie mit dem Ausdruckseditor in die E-Mail einfügen. [Erfahren Sie, wie Sie Angebote in die E-Mail einfügen](#insert)

## Einfügen von Angeboten in die E-Mail {#insert}

Angebote können mit dem Ausdruckseditor zur E-Mail hinzugefügt werden. Sie können wie folgt eingefügt werden:

* In der Betreffzeile der E-Mail:
* Im E-Mail-Textkörper durch Personalisierung in einer beliebigen Inhaltskomponente. [Erfahren Sie, wie Sie Inhaltskomponenten hinzufügen](content-components.md)

>[!NOTE]
>
>Stellen Sie vor dem Einfügen eines Angebots sicher, dass Sie [konfiguriert haben, welche Angebote mit der E-Mail vorgeschlagen werden sollen](#configure).

Gehen Sie wie folgt vor, um ein Angebot mit dem Ausdruckseditor einzufügen:

1. Öffnen Sie den Ausdruckseditor und wählen Sie dann das Menü **[!UICONTROL Vorschläge]**.

   Die verfügbaren Vorschläge werden in der Liste angezeigt. Die Anzahl der Vorschläge wird bei der Konfiguration der zu unterbreitenden Angebote bestimmt.

   ![](assets/offer-insertion.png)

1. Fügen Sie die Vorschläge mithilfe der Personalisierungsfelder, Rendering-Funktionen oder Angebotsattribute, die für jeden Vorschlag verfügbar sind, zum Betreff oder Text der E-Mail hinzu.

   ![](assets/offer-inserted.png)
