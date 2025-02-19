---
audience: end-user
title: Erste Schritte mit externen Sendungen
description: Erfahren Sie, wie Sie mit Adobe Campaign Web externe Sendungen erstellen und senden
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 10%

---

# Durchführen von externen Sendungen {#gs-direct-mail}


Adobe Campaign ermöglicht die Verarbeitung von Sendungen, die außerhalb von Campaign erstellt wurden, um über ein externes System massenweise personalisierte E-Mails, SMS-Nachrichten oder Push-Benachrichtigungen (iOS und Android) zu versenden.

<!--The supported channels are Email, Mobile (SMS), and Push (iOs and Android).-->

Beim Erstellen eines externen Versands generiert Adobe Campaign automatisch eine Extraktionsdatei, die alle Zielgruppenprofile und ausgewählten Daten enthält. Diese Datei wird an den Server Ihrer Wahl gesendet, der den Versandprozess für Sie übernimmt.

## Erstellen eines dedizierten externen Kontos {#routing-external-account}

Zunächst müssen Sie ein spezielles externes Konto konfigurieren, das in Ihren externen Sendungen verwendet wird. Sie muss vom Typ **[!UICONTROL Routing]** sein.

>[!NOTE]
>
>Erfahren Sie in ([ Abschnitt), wie Sie ein externes Konto vom Typ „Routing“ ](../administration/external-account.md#routing).

Wählen Sie beispielsweise den Kanal **[!UICONTROL Mobil (SMS)]** für das externe Konto aus. **[!UICONTROL Extern]** ist standardmäßig als **[!UICONTROL Versandmodus]** ausgewählt.

![](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## Externen Versand erstellen und senden {#create-external-delivery}

Nachdem das spezifische externe Konto konfiguriert wurde, erstellen Sie den externen Versand. Gehen Sie dazu wie folgt vor.

1. Erstellen Sie einen Versand. [Weitere Informationen](create-deliveries.md)

   Sie haben drei Möglichkeiten:

   * **In einem Workflow**: Fügen Sie eine externe Kanalaktivität (E-Mail, SMS oder Push) zu Ihrem Workflow hinzu. Detaillierte Anweisungen zum Konfigurieren eines Workflows finden Sie auf [dieser Seite](../workflows/gs-workflow-creation.md).
   * **In einer Kampagne**: Nachdem Sie eine Kampagne erstellt haben, können Sie einen externen E-Mail-, SMS- oder Push-Kanal-Versand erstellen. Weiterführende Informationen zum Einrichten Ihrer Kampagne finden Sie auf [dieser Seite](../campaigns/gs-campaigns.md).
   * **Eigenständiger Versand**: Wenden Sie sich mit einem individuellen externen Versand direkt und sofort an Ihre Kunden. [Erfahren Sie, wie Sie einen Versand erstellen](../msg/gs-deliveries.md).

1. Wählen Sie in Versand oder Versandvorlage [Einstellungen](../advanced-settings/delivery-settings.md) das externe Konto aus, das Sie für den Kanal Ihrer Wahl (in diesem Beispiel den SMS-Kanal) erstellt haben, und speichern Sie es.

   ![](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >Vergewissern Sie sich beim Erstellen eines Versands, dass Sie eine [Versandvorlage](delivery-template.md) mit einem externen Konto vom Typ **[!UICONTROL Routing]** ausgewählt haben. Andernfalls können Sie das von Ihnen erstellte dedizierte Konto nicht auswählen [oben](#routing-external-account).

1. Klicken Sie im Abschnitt **[!UICONTROL Inhalt]** auf **[!UICONTROL Inhalt bearbeiten]**.

   ![](assets/external-delivery-edit-content.png){zoomable="yes"}

1. Im Gegensatz zu einem Standardversand gestalten Sie den Inhalt der Nachricht nicht selbst. Stattdessen müssen Sie die Eigenschaften und Spalten der Datei definieren, die an das externe System gesendet wird.

   ![](assets/external-delivery-file-properties.png){zoomable="yes"}

   Führen Sie die gleichen Schritte wie beim Entwerfen des Inhalts der von (Briefpost[Sendungen) generierten Extraktionsdatei ](../direct-mail/content-direct-mail.md):

   * Definieren Sie die Eigenschaften der Extraktionsdatei. [Weitere Informationen](../direct-mail/content-direct-mail.md#properties)
   * Wählen Sie die Spalten mit den Informationen aus, die in diese Datei exportiert werden sollen. [Weitere Informationen](../direct-mail/content-direct-mail.md#content)

1. Sie können eine Vorschau der Datei anzeigen und einen Testversand durchführen<!--not in UI right now - to check-->. [Weitere Informationen](../direct-mail/send-direct-mail.md#preview-dm)

   ![](assets/external-delivery-simulate.png){zoomable="yes"}

1. Versand durchführen, um die Extraktionsdatei zu erzeugen. [Weitere Informationen](../direct-mail/send-direct-mail.md#send-dm)

Nach dem Versand wird die Extraktionsdatei automatisch generiert und an den Speicherort exportiert, der im [externen Konto](../administration/external-account.md#create-ext-account) angegeben ist, das in den Einstellungen der Versandvorlage ausgewählt wurde.

Sie können die KPIs auf der Versandseite und die Daten im Menü **[!UICONTROL Protokolle]** verfolgen.
