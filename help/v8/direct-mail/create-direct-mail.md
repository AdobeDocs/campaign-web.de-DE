---
audience: end-user
title: Erstellen eines Briefpostversands
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Briefpost-Versand erstellen
exl-id: 9b5172b2-1880-4768-a33b-8a20ec5a30ab
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 50%

---

# Erstellen eines Briefpostversands {#create-direct-mail}

Sie können einen eigenständigen Briefpost-Versand erstellen oder im Rahmen eines Kampagnen-Workflows einen Briefpost-Versand erstellen. Die folgenden Schritte beschreiben das Verfahren für einen eigenständigen (einmaligen) Briefpost-Versand. Wenn Sie im Rahmen eines Kampagnen-Workflows arbeiten, werden die Erstellungsschritte im Abschnitt [diesem Abschnitt](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Gehen Sie wie folgt vor, um einen neuen eigenständigen Briefpost-Versand zu erstellen:

1. Gehen Sie zum Menü **[!UICONTROL Sendungen]** in der linken Leiste, und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

1. Unter dem **[!UICONTROL Kanal]** auswählen **[!UICONTROL Briefpost]** als Kanal verwenden und eine Vorlage auswählen. [Weitere Informationen zu Vorlagen](../msg/delivery-template.md)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![](assets/dm-create.png){zoomable=&quot;yes&quot;}

1. Geben Sie einen **[!UICONTROL Titel]** für den Versand ein und greifen Sie auf die Dropdown-Liste **[!UICONTROL Zusätzliche Optionen]** zu. Wenn Ihr Versand auf einem erweiterten Schema basiert, stehen spezifische Felder für **Benutzerdefinierte Optionen** zur Verfügung.

   ![](assets/dm-properties.png){zoomable=&quot;yes&quot;}

   +++Konfigurieren Sie die folgenden Einstellungen entsprechend Ihren Anforderungen.
   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu.
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner.
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an.
   * **[!UICONTROL Art]**: Geben Sie die Art des Versands zu Klassifizierungszwecken an.
+++

1. Klicken Sie auf **[!UICONTROL Zielgruppe auswählen]** -Schaltfläche, um eine vorhandene Zielgruppe anzusprechen oder eine eigene zu erstellen.

   * [Erfahren Sie, wie Sie eine vorhandene Zielgruppe auswählen](../audience/add-audience.md)
   * [Erfahren Sie, wie Sie eine neue Zielgruppe erstellen](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Briefpost-Empfänger müssen mindestens ihren Namen und ihre Anschrift enthalten. Eine Anschrift gilt als vollständig angegeben, wenn die Felder Name, Postleitzahl und Ort nicht leer sind. Empfängerinnen und Empfänger mit unvollständigen Adressen werden von Direkt-Mail-Sendungen ausgeschlossen.

1. Aktivieren Sie die Option **[!UICONTROL Kontrollgruppe aktivieren]**, um eine Kontrollgruppe zum Messen der Wirkung Ihres Versands einzurichten. Nachrichten werden nicht an diese Kontrollgruppe gesendet, sodass Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen können, die die Nachricht erhalten haben. [Erfahren Sie, wie Sie mit Kontrollgruppen arbeiten](../audience/control-group.md)

1. Klicks **[!UICONTROL Inhalt bearbeiten]** um die Informationen (Spalten) zu definieren, die in die Extraktionsdatei exportiert werden sollen. [Weitere Informationen](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable=&quot;yes&quot;}

1. Um den Versand für ein bestimmtes Datum und eine bestimmte Uhrzeit zu planen, aktivieren Sie die Option **[!UICONTROL Zeitplan aktivieren]**. Nach dem Start des Versands wird die Extraktionsdatei automatisch zu dem von Ihnen definierten Zeitpunkt generiert. [Erfahren Sie, wie Sie Sendungen planen](../msg/gs-messages.md#gs-schedule).

   >[!NOTE]
   >
   >Wenn ein Versand im Rahmen eines Workflows durchgeführt wird, müssen Sie die Aktivität **Planung** verwenden. Weitere Informationen finden Sie auf [dieser Seite](../workflows/activities/scheduler.md).

1. Klicken Sie auf **[!UICONTROL Einstellungen]**, um auf die erweiterten Optionen für Ihre Versandvorlage zuzugreifen. [Weitere Informationen](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable=&quot;yes&quot;}

1. Sobald Ihr Briefpost-Versand fertig ist, klicken Sie auf **[!UICONTROL Überprüfen und Senden]** -Schaltfläche, um Ihren Versand zu validieren und zu versenden und die Extraktionsdatei zu erstellen. [Erfahren Sie, wie Sie einen Briefpost-Versand in der Vorschau anzeigen und senden.](send-direct-mail.md)
