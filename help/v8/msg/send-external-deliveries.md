---
audience: end-user
title: Erste Schritte mit externen Sendungen
description: Erfahren Sie, wie Sie mit Adobe Campaign Web externe Sendungen erstellen und durchführen.
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 37%

---

# Durchführen von externen Sendungen {#gs-direct-mail}

Mit Adobe Campaign können Sie Sendungen verwalten, die außerhalb von Campaign erstellt wurden, um über ein externes System personalisierte E-Mails, SMS-Nachrichten oder Push-Benachrichtigungen (iOS und Android) in großen Mengen zu versenden.

<!--The supported channels are Email, Mobile (SMS), and Push (iOS and Android).-->

Beim Erstellen eines externen Versands generiert Adobe Campaign automatisch eine Extraktionsdatei, die alle Zielgruppenprofile und ausgewählten Daten enthält. Diese Datei wird an den Server Ihrer Wahl gesendet, der den Sendevorgang verarbeitet.

## Erstellen eines dedizierten externen Kontos {#routing-external-account}

Sie müssen ein bestimmtes externes Konto konfigurieren, das in Ihren externen Sendungen verwendet werden soll. Es muss vom Typ **[!UICONTROL Routing]** sein.

>[!NOTE]
>
>Näheres dazu, wie Sie ein externes Konto vom Typ „Routing“ erstellen, finden Sie in [diesem Abschnitt](../administration/external-account.md#routing).

Wählen Sie für das externe Konto beispielsweise den Kanal **[!UICONTROL Mobil (SMS)]** aus. **[!UICONTROL Extern]** ist standardmäßig als **[!UICONTROL Versandmodus]** ausgewählt.

![Konfiguration des Versandmodus des externen Kontos](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## Erstellen und Senden des externen Versands {#create-external-delivery}

Nachdem das spezifische externe Konto konfiguriert wurde, erstellen Sie den externen Versand. Gehen Sie dazu wie folgt vor.

1. Erstellen Sie einen Versand. [Weitere Informationen](create-deliveries.md)

   Sie haben drei Möglichkeiten:

   * **In einem Workflow**: Fügen Sie eine externe Kanalaktivität (E-Mail, SMS oder Push) zu Ihrem Workflow hinzu. Detaillierte Anweisungen zum Konfigurieren von Workflows finden Sie auf [dieser Seite](../workflows/gs-workflow-creation.md).
   * **In einer Kampagne**: Nach der Erstellung einer Kampagne können Sie einen externen E-Mail-, SMS- oder Push-Kanal-Versand erstellen. Weiterführende Informationen zum Einrichten Ihrer Kampagne finden Sie auf [dieser Seite](../campaigns/gs-campaigns.md).
   * **Eigenständiger Versand**: Binden Sie Kundinnen und Kunden direkt und sofort mit einem individuellen externen Versand ein. [Erfahren Sie, wie Sie einen Versand erstellen](../msg/gs-deliveries.md).

1. Wählen Sie in Versand oder Versandvorlage [Einstellungen](../advanced-settings/delivery-settings.md) das externe Konto aus, das für den Kanal Ihrer Wahl erstellt wurde (in diesem Beispiel den SMS-Kanal), und speichern Sie.

   ![Routing-Konfiguration für externe Sendungen](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >Wenn Sie einen Versand erstellen, stellen Sie sicher, dass Sie eine [Versandvorlage](delivery-template.md) mit einem externen Konto vom Typ **[!UICONTROL Routing]** ausgewählt haben. Andernfalls können Sie das erstellte dedizierte Konto nicht auswählen [oben](#routing-external-account).

1. Klicken Sie im Abschnitt **[!UICONTROL Inhaltsversand]** auf **[!UICONTROL Inhalt bearbeiten]**.

   ![Inhalt im externen Versand bearbeiten](assets/external-delivery-edit-content.png){zoomable="yes"}

1. Im Gegensatz zu einem Standardversand entwerfen Sie den Inhalt der Nachricht nicht selbst. Definieren Sie stattdessen die Eigenschaften und Spalten der Datei, die an das externe System gesendet werden soll.

   ![Konfiguration der Dateieigenschaften für den externen Versand](assets/external-delivery-file-properties.png){zoomable="yes"}

   Führen Sie die gleichen Schritte wie beim Entwerfen des Inhalts der von [Briefpost-Sendungen](../direct-mail/content-direct-mail.md) generierten Extraktionsdatei aus:

   * Definieren Sie die Eigenschaften der Extraktionsdatei. [Weitere Informationen](../direct-mail/content-direct-mail.md#properties)
   * Auswahl der Spalten mit den Informationen, die in die Datei exportiert werden sollen. [Weitere Informationen](../direct-mail/content-direct-mail.md#content)

1. Vorschau der Datei und Testversand<!--not in UI right now - to check-->. [Weitere Informationen](../direct-mail/send-direct-mail.md#preview-dm)

   ![Simulieren des externen Versands](assets/external-delivery-simulate.png){zoomable="yes"}

1. Senden Sie den Versand, damit die Extraktionsdatei generiert wird. [Weitere Informationen](../direct-mail/send-direct-mail.md#send-dm)

Nach dem Versand wird die Extraktionsdatei automatisch generiert und an den Speicherort exportiert, der im [externen Konto](../administration/external-account.md#create-ext-account) angegeben ist, das in den Einstellungen der Versandvorlage ausgewählt wurde.

Verfolgen Sie die KPIs auf der Versandseite und die Daten im Menü **[!UICONTROL Protokolle]**.