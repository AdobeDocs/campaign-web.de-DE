---
audience: end-user
title: Erstellen eines Callcenter-Versands
description: Weitere Informationen zum Erstellen eines Callcenter-Versands mit Adobe Campaign Web
exl-id: fe8d4773-2271-46ec-9b2e-f50311a4ccf3
source-git-commit: 1581943b0f13cbd4296e1f42fae8560626b61bdf
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 100%

---

# Erstellen und Durchführen eines Callcenter-Versands {#create-call-center}

Sie können einen eigenständigen Callcenter-Versand oder einen Callcenter-Versand im Kontext eines Kampagnen-Workflows erstellen. Die folgenden Schritte beschreiben die Vorgehensweise beim Erstellen eines eigenständigen (einmaligen) Versands. Wenn Sie im Kontext eines Kampagnen-Workflows arbeiten, werden die Erstellungsschritte in [diesem Abschnitt](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow) beschrieben.

Gehen Sie wie folgt vor, um einen neuen eigenständigen Callcenter-Versand zu erstellen und zu senden:

1. [Weitere Informationen](#create-delivery) zum Erstellen eines Versands
1. [Weitere Informationen](#select-audience) zum Definieren einer Zielgruppe
1. [Weitere Informationen](#edit-content) zum Bearbeiten des Inhalts
1. [Weitere Informationen](#preview-send) zum Anzeigen einer Vorschau und zum Senden eines Versands

## Erstellen des Versands{#create-delivery}

Führen Sie die folgenden Schritte aus, um den Versand zu erstellen und seine Eigenschaften zu konfigurieren:

1. Wählen Sie das Menü **[!UICONTROL Sendungen]** aus und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

1. Wählen Sie als Kanal **[!UICONTROL Callcenter]** aus und klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![Screenshot der Erstellung eines Callcenter-Versands](assets/cc-create.png){zoomable="yes"}

   >[!NOTE]
   >
   >Informationen zum Auswählen einer anderen Vorlage finden Sie auf dieser [Seite](../msg/delivery-template.md).

1. Geben Sie unter **[!UICONTROL Eigenschaften]** ein **[!UICONTROL Label]** für den Versand ein. Zusätzliche Optionen werden in diesem [Abschnitt](../email/create-email.md#create-email) beschrieben.

   ![Screenshot der Konfiguration der Eigenschaften für einen Callcenter-Versand](assets/cc-properties.png){zoomable="yes"}

>[!NOTE]
>
>Sie können den Versand so planen, dass er zu einem bestimmten Datum erfolgt. Weitere Informationen hierzu finden Sie in diesem [Abschnitt](../msg/gs-deliveries.md#gs-schedule).

## Definieren der Zielgruppe{#select-audience}

Definieren Sie nun die Zielgruppe für die Extraktionsdatei.

1. Klicken Sie im Abschnitt **[!UICONTROL Zielgruppe]** der Versandseite auf **[!UICONTROL Zielgruppe auswählen]**.

   ![Screenshot der Zielgruppenauswahl für einen Callcenter-Versand](assets/cc-audience.png){zoomable="yes"}

1. Wählen Sie eine vorhandene Zielgruppe oder erstellen Sie eine eigene.

   * [Erfahren Sie, wie Sie eine vorhandene Zielgruppe auswählen.](../audience/add-audience.md)
   * [Erfahren Sie, wie Sie eine neue Zielgruppe erstellen.](../audience/one-time-audience.md)

   ![Screenshot der Zielgruppenauswahl für einen Callcenter-Versand](assets/cc-audience2.png){zoomable="yes"}

>[!NOTE]
>
>Für die Empfängerinnen und Empfänger des Callcenter-Versands müssen mindestens Name und Telefonnummer angegeben sein. Empfängerinnen und Empfänger mit unvollständigen Informationen werden von Callcenter-Sendungen ausgeschlossen.
>
>Weitere Informationen zur Konfiguration von Kontrollgruppen finden Sie auf dieser [Seite](../audience/control-group.md).

## Bearbeiten des Inhalts{#edit-content}

Nun wird der Inhalt der Extraktionsdatei bearbeitet, die vom Callcenter-Versand generiert wird.

1. Klicken Sie auf der Versandseite auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]**.

   ![Screenshot der Inhaltsbearbeitung für einen Callcenter-Versand](assets/cc-content0.png){zoomable="yes"}

1. Füllen Sie das Feld **[!UICONTROL Dateiname]** aus. Weitere Informationen zur Personalisierung des Dateinamens finden Sie auf dieser [Seite](../personalization/personalize.md).

1. Wählen Sie ein **[!UICONTROL Dateiformat]** aus: **Text**, **Text in Spalten mit fester Breite**, **CSV (Excel)** oder **XML**.

   ![Screenshot der Inhaltsbearbeitung für einen Callcenter-Versand](assets/cc-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >Mögliche Formatoptionen werden auf dieser [Seite](../direct-mail/content-direct-mail.md#properties) beschrieben.

1. Schalten Sie die Option **[!UICONTROL Anz. abzurufender Datensätze]** ein, wenn Sie die Anzahl der Empfängerinnen und Empfänger für Ihren Versand zu begrenzen möchten.

1. Klicken Sie im Abschnitt **[!UICONTROL Inhalt]** auf die Schaltfläche **[!UICONTROL Attribut hinzufügen]**, um eine neue Spalte zu erstellen, die in der Extraktionsdatei angezeigt wird.

1. Wählen Sie das Attribut aus, das in der Spalte angezeigt werden soll, und bestätigen Sie dann die Auswahl. Weitere Informationen zum Auswählen von Attributen und zum Hinzufügen dieser zu den Favoriten finden Sie auf dieser [Seite](../get-started/attributes.md).

   ![Screenshot mit der Schaltfläche „Attribut hinzufügen“ und Optionen zum Hinzufügen von Attributen zur Extraktionsdatei.](assets/cc-add-attribute.png)

1. Wiederholen Sie diese Schritte, um so viele Spalten hinzuzufügen, wie Sie für Ihre Extraktionsdatei benötigen.

   Anschließend können Sie die Attribute bearbeiten, die Extraktionsdatei sortieren oder die Position der Spalten ändern. Weiterführende Informationen hierzu finden Sie auf [dieser Seite](../direct-mail/content-direct-mail.md#content).

   ![Screenshot mit den Konfigurationsoptionen für Attribute für die Extraktionsdatei](assets/cc-content-attributes.png)

## Vorschau und Durchführen des Versands{#preview-send}

Wenn der Versandinhalt fertig ist, können Sie ihn mithilfe von Testprofilen in der Vorschau anzeigen und einen Testversand durchführen. Sie können dann den Callcenter-Versand durchführen, um die Extraktionsdatei zu generieren.

Nachfolgend werden die wichtigsten Schritte beschrieben, um die Extraktionsdatei in einer Vorschau anzuzeigen und zu senden. Weitere Details finden Sie auf [dieser Seite](../direct-mail/send-direct-mail.md).

1. Klicken Sie auf der Seite des Versandinhalts auf die Schaltfläche **[!UICONTROL Inhalte simulieren]**.

   ![Screenshot mit der Option „Inhalte simulieren“ auf der Seite für den Versandinhalt](assets/cc-simulate0.png){zoomable="yes"}

1. Wählen Sie mindestens ein Testprofil aus, um eine Vorschau des personalisierten Inhalts anzuzeigen. Sie können auch Testsendungen durchführen. [Weitere Informationen](../direct-mail/send-direct-mail.md#preview-dm)

   ![Screenshot mit der Option „Inhalte simulieren“ auf der Seite für den Versandinhalt](assets/cc-simulate.png){zoomable="yes"}

1. Klicken Sie auf der Versandseite auf **[!UICONTROL Überprüfen und senden]**.

   ![Screenshot der Option „Überprüfen und senden“ auf der Versandseite](assets/cc-review-send.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Vorbereiten]** und überwachen Sie den Fortschritt und die bereitgestellten Statistiken. Bestätigen Sie anschließend.

   ![Screenshot mit der Option „Vorbereiten“ und dem Menü „Logs“](assets/cc-prepare.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Senden]**, um mit dem endgültigen Sendevorgang fortzufahren, und bestätigen Sie dann.

Nach dem Versand wird die Extraktionsdatei automatisch generiert und an den Speicherort exportiert, der im in den [erweiterten Einstellungen](../advanced-settings/delivery-settings.md) in der Versandvorlage ausgewählten externen Konto **[!UICONTROL Routing]** angegeben ist. Sie können die Datei auch in der Vorschau anzeigen, indem Sie im Abschnitt **Inhalt** des Bildschirms auf die Schaltfläche **Datei in Vorschau anzeigen** klicken.

Verfolgen Sie die Daten Ihrer KPIs (Key Performance Indicators) über Ihre Versandseite und weitere Daten über das Menü **[!UICONTROL Logs]**.

Messen Sie die Wirkung Ihrer Nachricht mit integrierten Berichten. [Weitere Informationen](../reporting/direct-mail.md)
