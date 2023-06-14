---
audience: end-user
title: Senden von Angeboten
description: Senden von Angeboten
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha"
source-git-commit: 9203d2bcfbe75b584ecab65637b5ded202435d29
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 52%

---


# Senden von Angeboten {#offers-content}

Mit Adobe Campaign v8 Web können Sie Sendungen mit Ihren Versandangeboten durchführen, die in der Konsole mithilfe der **[!UICONTROL Interaction]** -Modul. Weitere Informationen zu Interaction und zur Verwaltung eines Angebotskatalogs in der Konsole finden Sie in der [Dokumentation zu Campaign V8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=de){target="_blank"}.

Gehen Sie wie folgt vor, um Angebote mit einem Versand zu versenden:

1. [Zu unterbreitende Angebote konfigurieren](#configure)
1. [Angebote in den Versand einfügen](#insert)

## Zu unterbreitende Angebote konfigurieren {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Angebotseinstellungen"
>abstract="Konfigurieren Sie, welche Angebote den Empfängerinnen und Empfängern unterbreitet werden sollen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Bietet erweiterte Einstellungen"
>abstract="Konfigurieren Sie die erweiterten Optionen für Angebote."

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Angebote einrichten]** im Bildschirm zur Inhaltsbearbeitung des Versands.

   ![](assets/setup-offers.png)

1. Konfigurieren Sie, welche Angebote den Empfängerinnen und Empfängern unterbreitet werden sollen.

   Wählen Sie zunächst die **[!UICONTROL Platzierung]** entsprechend Ihrer Angebotsumgebung. Erfahren Sie, wie Sie eine Platzierung im [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}

   ![](assets/create-content-offers.png)

1. Um die Angebotsauswahl des Moduls zu verfeinern, wählen Sie eine spezifische **[!UICONTROL Angebotskategorie]**, in der die Angebote gruppiert sind.

   Bei der Auswahl eines Ordners werden alle Unterordner automatisch eingeschlossen und können nicht entfernt werden. Beachten Sie Folgendes: [!DNL Campaign] -Schnittstelle spiegelt dieses Verhalten nicht wider.

   >[!NOTE]
   >
   >Wenn keine Kategorie spezifiziert wird, werden alle in der Umgebung enthaltenen Angebote von der Angebots-Engine berücksichtigt, es sei denn, es wurde ein **[!UICONTROL Angebotsthema]** ausgewählt.

1. (Optional) Geben Sie ein Design ein, nach dem Kategorien gefiltert werden sollen. Themen sind Schlüsselwörter, die zuvor in den Kategorien definiert wurden. Sie dienen als Filter und ermöglichen es Ihnen, die Anzahl der zu unterbreitenden Angebote durch Auswahl in einer Reihe von Kategorien zu verfeinern.

1. Verwenden Sie die **[!UICONTROL Vorschläge]** um die Anzahl der Angebote anzugeben, die Sie in den Versand einfügen möchten.

1. Wählen Sie bei Bedarf die Option **[!UICONTROL Nicht infrage kommende Empfänger ausschließen]** aus.

   Mit dieser Option können Sie den Ausschluss von Empfängern aktivieren oder deaktivieren, für die nicht genügend geeignete Angebote vorhanden sind.

   * Wenn die Option aktiviert ist, werden Empfängerinnen und Empfänger, für die nicht genügend geeignete Angebote vorhanden sind, vom Versand ausgeschlossen.
   * Wenn die Option deaktiviert ist, werden diese Empfängerinnen und Empfänger nicht vom Versand ausgeschlossen, ihnen wird aber nicht die angefragte Anzahl von Angeboten unterbreitet.

1. Wählen Sie bei Bedarf die Option **[!UICONTROL Alles ausblenden, wenn kein Angebot ausgewählt ist]**.

   Mit dieser Option können Sie festlegen, wie die Nachricht verarbeitet werden soll, wenn eine der Vorschläge nicht existiert.

   * Wenn die Option aktiviert ist, wird keine Darstellung des fehlenden Vorschlags angezeigt und es wird auch kein Inhalt für diesen Vorschlag in der Nachricht angezeigt.
   * Wenn die Option deaktiviert ist, wird die der Versand der Nachricht abgebrochen und die Empfänger und Empfängerinnen können keine Nachrichten mehr empfangen.

Nachdem Sie die für Ihren Versand vorzuschlagenden Angebote konfiguriert haben, können Sie sie mithilfe des Ausdruckseditors in den Versandinhalt einfügen.

## Angebote in den Versand einfügen {#insert}

Angebote können im Versand mit der Variablen [Ausdruckseditor](../personalization/gs-personalization.md#access). Sie können entweder in die Betreffzeile oder in den Versandtext eingefügt werden.

>[!CAUTION]
>
>Bevor Sie ein Angebot in einen Versand einfügen, stellen Sie sicher, dass Sie [konfiguriert, welche Angebote mit diesem Versand vorgeschlagen werden](#configure).

Gehen Sie wie folgt vor, um ein Angebot mit dem Ausdruckseditor einzufügen.

1. Rufen Sie die Betreffzeile oder den Inhalt eines Versands auf.

1. Platzieren Sie den Cursor an der Stelle, an der das Angebot eingefügt werden soll, und öffnen Sie den Ausdruckseditor über das Personalisierungssymbol.

1. Wählen Sie die **[!UICONTROL Vorschläge]** Menü. Die verfügbaren Vorschläge werden in der Liste angezeigt.

   >[!NOTE]
   >
   >Die Anzahl der Vorschläge wird definiert, wenn [Angebote einrichten](#configure) für den aktuellen Versand.

   ![](assets/offer-insertion.png)

1. Fügen Sie die Vorschläge mithilfe der Personalisierungsfelder, Rendering-Funktionen oder Angebotsattribute, die für jeden Vorschlag verfügbar sind, in die Betreffzeile oder den Hauptteil des Versands ein.

   ![](assets/offer-inserted.png)

   >[!NOTE]
   >
   >Die Anzahl der verfügbaren Vorschläge hängt von der Konfiguration des Angebotsmodul-Aufrufs ab und ihre Reihenfolge hängt von der Priorität der Angebote ab.

1. Speichern Sie Ihre Änderungen.

1. Schließen Sie den Inhalt ab, testen Sie Ihren Versand und führen Sie ihn aus.

Wenn nun ein Empfänger den Versand erhält, wird diesem Profil das richtige Angebot angezeigt.
