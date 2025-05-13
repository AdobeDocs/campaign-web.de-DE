---
audience: end-user
title: Erstellen eines SMS-Versands
description: Erfahren Sie, wie Sie SMS mit Adobe Campaign Web erstellen und senden
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '511'
ht-degree: 100%

---

# Erstellen eines SMS-Versands {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Eigenschaften des SMS-Versands"
>abstract="Die Eigenschaften umfassen die gebräuchlichen Versandparameter, mit denen Sie Ihren Versand benennen und klassifizieren können. Wenn Ihr Versand ein erweitertes Schema nutzt, stehen spezifische Felder für benutzerdefinierte Optionen zur Verfügung."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definieren der SMS-Zielgruppe"
>abstract="Erstellen Sie eine neue Zielgruppe oder wählen Sie eine vorhandene aus, indem Sie auf die Schaltfläche **Zielgruppe auswählen** klicken. Bei Bedarf kann eine kontrollgruppe hinzugefügt werden, um die Wirkung des Versand zu messen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=de" text="Festlegen einer Kontrollgruppe"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Auswahl von SMS-Vorlagen"
>abstract="Wählen Sie eine vordefinierte Vorlage aus, um Ihren SMS-Versand zu starten. Versandvorlagen ermöglichen die Wiederverwendung benutzerdefinierter Inhalte und Einstellungen in allen Kampagnen und Sendungen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=de" text="Verwenden von Versandvorlagen"

Sie können einen eigenständigen SMS-Versand erstellen oder eine SMS im Kontext eines Kampagnen-Workflows erstellen. Die folgenden Schritte beschreiben die Vorgehensweise für einen eigenständigen (einmaligen) SMS-Versand. Wenn Sie im Kontext eines Kampagnen-Workflows arbeiten, finden Sie in [diesem Abschnitt](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow) detaillierte Schritte, um einen solchen Versand zu erstellen. 

Gehen Sie wie folgt vor, um einen eigenständigen SMS-Versand zu erstellen:

1. Navigieren Sie in der linken Leiste zum Menü **[!UICONTROL Sendungen]** und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

1. Wählen Sie im Abschnitt **[!UICONTROL Kanal]** den Kanal SMS aus und wählen Sie eine Vorlage aus. [Weitere Informationen zu Vorlagen](../msg/delivery-template.md)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![Screenshot mit der Schaltfläche „Versand erstellen“ und ausgewähltem SMS-Kanal](assets/sms_create_1.png){zoomable="yes"}

1. Geben Sie ein **[!UICONTROL Label]** für den Versand ein und greifen Sie auf die Dropdown-Liste **[!UICONTROL Zusätzliche Optionen]** zu. Wenn Ihr Versand ein erweitertes Schema nutzt, stehen spezifische Felder für **benutzerdefinierte Optionen** zur Verfügung.

   +++Konfigurieren Sie die folgenden Einstellungen entsprechend Ihren Anforderungen.
   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu.
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner.
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an.
   * **[!UICONTROL Art]**: Geben Sie die Art des Versands zu Klassifizierungszwecken an.
+++

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe auswählen]**, um eine vorhandene Zielgruppe anzusprechen oder eine eigene zu erstellen. [Weitere Informationen zu Zielgruppen](../audience/about-recipients.md).

   ![Screenshot mit der Schaltfläche „Zielgruppe auswählen“](assets/sms_create_2.png){zoomable="yes"}

   Weitere Informationen dazu, wie Sie eine vorhandene Zielgruppe auswählen, finden Sie auf [dieser Seite](../audience/add-audience.md).

   Weitere Informationen dazu, wie Sie eine neue Zielgruppe erstellen, finden Sie auf [dieser Seite](../audience/one-time-audience.md).

1. Aktivieren Sie die Option **[!UICONTROL Kontrollgruppe aktivieren]**, um eine Kontrollgruppe zum Messen der Wirkung Ihres Versands einzurichten. Nachrichten werden nicht an diese Kontrollgruppe gesendet, sodass Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen können, die die Nachricht nicht erhalten haben. [Weitere Informationen](../audience/control-group.md)

1. Klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**, um mit der Erstellung des Inhalts Ihrer SMS-Nachricht zu beginnen. [Weitere Informationen](content-sms.md)

   ![Screenshot mit der Schaltfläche „Inhalt bearbeiten“](assets/sms_create_4.png){zoomable="yes"}

   Auf diesem Bildschirm können Sie auch [Inhalte simulieren](../preview-test/preview-test.md) und [Angebote einrichten](../msg/offers.md).

1. Um den Versand für ein bestimmtes Datum und eine bestimmte Uhrzeit zu planen, aktivieren Sie die Option **[!UICONTROL Zeitplan aktivieren]**. Nachdem der Versand initiiert wurde, wird die Nachricht automatisch an dem Datum und zu der Uhrzeit gesendet, die Sie für die Empfängerin bzw. den Empfänger festlegen. Weitere Informationen zur Versandplanung finden Sie in [diesem Abschnitt](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Wenn ein Versand im Rahmen eines Workflows durchgeführt wird, verwenden Sie die Aktivität **Planung**. Weitere Informationen finden Sie auf [dieser Seite](../workflows/activities/scheduler.md).

1. Klicken Sie auf **[!UICONTROL Einstellungen]**, um auf die erweiterten Optionen für Ihre Versandvorlage zuzugreifen. [Weitere Informationen](../advanced-settings/delivery-settings.md)

   ![Screenshot mit der Schaltfläche „Einstellungen“](assets/sms_create_3.png){zoomable="yes"}