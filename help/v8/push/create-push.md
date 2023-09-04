---
audience: end-user
title: Erstellen eines Push-Benachrichtigungs-Versands
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Push-Benachrichtigungs-Versand erstellen
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 100%

---

# Erstellen eines Push-Benachrichtigungs-Versands {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definieren der Push-Zielgruppe"
>abstract="Wählen Sie die beste Zielgruppe für Ihre Push-Nachricht aus."

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Vorlage für Push-Benachrichtigungen"
>abstract="Wählen Sie eine Vorlage für Push-Benachrichtigungen aus, um Ihren Push-Versand zu starten."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Eigenschaften des Push-Versands"
>abstract="Verwalten Sie die Eigenschaften eines Push-Versands."

1. Klicken Sie auf der **[!UICONTROL Sendungen]**-Startseite auf **[!UICONTROL Versand erstellen]**.

1. Wählen Sie im Abschnitt **[!UICONTROL Kanal]** die Push-Benachrichtigung als Kanal und wählen Sie eine Vorlage je nach dem gewählten Betriebssystem: Android oder iOS. [Weitere Informationen zu Vorlagen](../msg/delivery-template.md)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![](assets/push_create_1.png)

1. Geben Sie eine **[!UICONTROL Kennzeichnung]** für den Versand ein und greifen Sie auf die Dropdown-Liste **[!UICONTROL Zusätzliche Optionen]** zu.

   +++Konfigurieren Sie die folgenden Einstellungen entsprechend Ihren Anforderungen.
   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu.
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner.
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an.
   * **[!UICONTROL Art]**: Geben Sie die Art der E-Mail zu Klassifizierungszwecken an.
+++

1. Wählen Sie im Menü **[!UICONTROL Zielgruppe]** die Anwendung aus, die Sie für diesen Versand verwenden möchten.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe auswählen]**, um eine vorhandene Zielgruppe anzusprechen oder eine eigene zu erstellen. [Weitere Informationen](../audience/about-audiences.md)

   Beachten Sie, dass Ihre Push-Benachrichtigung standardmäßig an alle Abonnentinnen und Abonnenten der Anwendung gesendet wird.

   ![](assets/push_create_2.png)

1. Schalten Sie die Gruppenoption **[!UICONTROL Kontrollgruppe aktivieren]** ein, um zur Messung der Wirkung Ihres Versands eine Kontrollgruppe einzurichten, durch die Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen können, die sie nicht erhalten haben. [Weitere Informationen](../audience/control-group.md)

1. Klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**, um mit der Gestaltung des Inhalts Ihrer Push-Benachrichtigung zu beginnen. [Weitere Informationen](content-push.md)

   ![](assets/push_create_5.png)

   Auf diesem Bildschirm können Sie auch [Inhalte simulieren](../preview-test/preview-test.md) und [Angebote einrichten](../content/offers.md).

1. Um den Versand für ein bestimmtes Datum und eine bestimmte Uhrzeit zu planen, aktivieren Sie die Option **[!UICONTROL Zeitplan aktivieren]**. Nachdem der Versand initiiert wurde, wird die Nachricht automatisch an dem Datum und zu der Uhrzeit gesendet, die Sie für die Empfängerin bzw. den Empfänger festgelegt haben.

   ![](assets/push_create_3.png)

1. Klicken Sie auf **[!UICONTROL Versandeinstellungen konfigurieren]**, um auf erweiterte Optionen in Bezug auf Ihre Versandvorlage zuzugreifen. [Weitere Informationen](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
