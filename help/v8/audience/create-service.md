---
audience: end-user
title: Arbeiten mit Abonnementdiensten
description: Erfahren Sie, wie Sie Dienste im Adobe Campaign Web erstellen und verwalten
badge: label="Beta"
source-git-commit: 47c00b3520ea38d4afa173f8a221ae5e127dd7a9
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 4%

---


# Arbeiten mit Abonnementdiensten {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Erstellen und Verwalten Ihrer Dienste"
>abstract="Verwenden Sie Adobe Campaign, um Ihre Dienste wie z. B. Newsletter zu erstellen und zu überwachen und die An- und Abmeldungen für diese Dienste zu überprüfen. Abonnements gelten nur für E-Mail- und SMS-Sendungen."

Verwenden Sie das Adobe Campaign-Web, um Ihre Dienste wie z. B. Newsletter zu verwalten und zu erstellen und die An- und Abmeldungen für diese Dienste zu überprüfen.

>[!NOTE]
>
>Abonnements gelten nur für E-Mail- und SMS-Sendungen.

Es können mehrere Dienste parallel definiert werden, z. B. Newsletter für bestimmte Produktkategorien, Themen oder Bereiche einer Website, Abonnements für verschiedene Arten von Warnhinweisen und Echtzeit-Benachrichtigungen.

Weiterführende Informationen zur Verwaltung von An- und Abmeldungen finden Sie im Abschnitt [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Anmeldedienste aufrufen {#access-services}

Gehen Sie wie folgt vor, um auf die für Ihre Plattform verfügbaren Anmeldedienste zuzugreifen.

1. Navigieren Sie zum **[!UICONTROL Abonnementdienste]** in der linken Navigationsleiste.

   ![](assets/service-list.png)

1. Die Liste aller vorhandenen Anmeldedienste wird angezeigt. Sie können die Dienste durchsuchen und nach Kanal, Ordner oder erweiterten Filtern filtern.

   ![](assets/service-filters.png)

1. Um einen vorhandenen Dienst zu bearbeiten, klicken Sie auf seinen Namen.

1. Sie können jeden Dienst löschen oder duplizieren, indem Sie das Symbol mit den drei Punkten neben diesem Dienstnamen verwenden.

## Erstellen des ersten Abonnementdienstes {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Diensteigenschaften definieren"
>abstract="Geben Sie den Titel des Anmeldedienstes ein und definieren Sie zusätzliche Optionen, z. B. einen Gültigkeitszeitraum für Ihren Dienst."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Bestätigungsnachricht auswählen"
>abstract="Wenn sich ein Benutzer für einen Dienst anmeldet oder diesen abmeldet, können Sie eine Bestätigungsnachricht senden. Wählen Sie die für diese Nachricht zu verwendenden Vorlagen aus."

Gehen Sie wie folgt vor, um einen Abonnementdienst zu erstellen.

1. Wählen Sie die **[!UICONTROL Abonnement-Dienst erstellen]** Schaltfläche.

   ![](assets/service-create-button.png)

1. Kanal auswählen: **[!UICONTROL Email]** oder **[!UICONTROL SMS]**.

1. Geben Sie in den Diensteigenschaften einen Titel ein und definieren Sie nach Bedarf zusätzliche Optionen.

   ![](assets/service-create-properties.png)

1. Standardmäßig sind Abonnements unbegrenzt. Sie können die **[!UICONTROL Unbegrenzte Gültigkeitsdauer]** -Option, um eine Gültigkeitsdauer für den Dienst festzulegen. Im folgenden Beispiel können sich nach 20 Tagen keine Benutzer mehr für diesen Dienst anmelden.

   ![](assets/service-create-validity-period.png)

1. Wenn sich ein Benutzer für einen Dienst anmeldet oder diesen abmeldet, können Sie eine Bestätigungsnachricht senden. Wählen Sie je nach Anwendungsfall die Vorlagen aus, die für diese Nachricht verwendet werden sollen. Diese Vorlagen müssen mit dem **[!UICONTROL Abonnements]** Zielgruppen-Mapping. [Weitere Informationen](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. Klicks **[!UICONTROL Speichern und überprüfen]**. Der neue Dienst wird zum **[!UICONTROL Abonnementdienste]** Liste.

## Bestätigungsnachricht erstellen {#create-confirmation-message}

Um den Benutzern, die sich für Ihren Dienst anmelden oder von ihm abmelden, eine Bestätigungsnachricht zu senden, müssen Sie eine Versandvorlage mit dem **[!UICONTROL Abonnements]** Zielgruppen-Mapping ohne definierte Zielgruppe. Gehen Sie dazu wie folgt vor.

1. Erstellen Sie eine Versandvorlage für die Anmeldebestätigung. [Weitere Informationen dazu](../msg/delivery-template.md)

1. Wählen Sie keine Zielgruppe für diesen Versand aus. Greifen Sie stattdessen auf die **[!UICONTROL Versandeinstellungen]**, navigieren Sie zu [Zielgruppe](../advanced-settings/delivery-settings.md#audience) und wählen Sie die **[!UICONTROL Abonnements]** Zielgruppen-Mapping aus der Liste.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >Wenn Sie die  **[!UICONTROL Abonnements]** Zielgruppen-Mapping verwenden, erhalten Ihre Abonnenten keine Bestätigungsnachricht. Zielgruppen-Mappings sind in der Campaign v8-Konsole definiert. Weitere Informationen finden Sie unter [Dokumentation zu Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=de){target="_blank"}.

1. Bearbeiten Sie den Inhalt Ihrer Versandvorlage, speichern und schließen Sie sie.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >Erfahren Sie mehr über Versandkanäle und wie Sie Versandinhalte im Abschnitt [Email-Kanal](../email/create-email.md) und [SMS Kanal](../sms/create-sms.md) Abschnitte.

1. Wiederholen Sie die obigen Schritte, um eine Versandvorlage für die Abmeldebestätigung zu erstellen.

Sie können diese Nachrichten jetzt auswählen, wenn [Abonnement-Dienst erstellen](#create-service). Benutzer, die diesen Dienst abonnieren oder sich von ihm abmelden, erhalten die ausgewählte Bestätigungsnachricht.

## Abonnenten zu Ihrem Dienst hinzufügen {#add-subscribers}

Nachdem Sie einen Dienst erstellt haben, können Sie Abonnenten manuell hinzufügen. Gehen Sie dazu wie folgt vor.

1. Wählen Sie einen vorhandenen Dienst aus der **[!UICONTROL Abonnementdienste]** Liste.

1. Wählen Sie die **[!UICONTROL Abonnenten]** Registerkarte und klicken Sie auf **[!UICONTROL Profile hinzufügen]**.

   ![](assets/service-subscribers-tab.png)

1. Wählen Sie die hinzuzufügenden Profile aus der Liste aus und klicken Sie auf **[!UICONTROL Bestätigen]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Klicks **[!UICONTROL Senden]**. Die ausgewählten Empfänger erhalten das Abonnement [Bestätigungsnachricht](#create-confirmation-message) die Sie beim [Erstellen des Dienstes](#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

Die hinzugefügten Profile werden im Abschnitt **[!UICONTROL Abonnenten]** Liste. Sie haben jetzt Ihren Dienst abonniert.

## Entfernen von Abonnenten aus Ihrem Dienst {#remove-subscribers}

Nachdem Sie Abonnenten zu Ihrem Dienst hinzugefügt haben, können Sie sie entfernen. Gehen Sie dazu wie folgt vor.

1. Wählen Sie einen vorhandenen Dienst aus der **[!UICONTROL Abonnementdienste]** Liste.

1. Klicken Sie auf das Drei-Punkte-Symbol neben dem gewünschten Empfängernamen und wählen Sie **[!UICONTROL Löschen]**.

   ![](assets/service-subscribers-delete.png)

1. Löschen bestätigen und auf **[!UICONTROL Senden]**. Die ausgewählten Empfänger erhalten die Abmeldung [Bestätigungsnachricht](#create-confirmation-message) die Sie beim [Erstellen des Dienstes](#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

Der Empfänger wird aus der **[!UICONTROL Abonnenten]** und Ihr Dienst nicht mehr abonniert hat.

## Protokolle und Berichte des Abonnementdienstes {#logs-and-reports}

Um die Effektivität Ihrer Abonnementdienste für SMS- und E-Mail-Kanäle zu messen, können Sie auf die Protokolle und Berichte für einen bestimmten Dienst zugreifen.

1. Wählen Sie einen vorhandenen Dienst aus der **[!UICONTROL Abonnementdienste]** Liste. Klicks **[!UICONTROL berechnen]** Rufen Sie die Anzahl der Abonnenten insgesamt ab.

   ![](assets/service-logs-reports-buttons.png)

1. Wählen Sie im Dienst-Dashboard **[!UICONTROL Protokolle]** um die Liste der Abonnenten dieses Dienstes anzuzeigen. Sie können die Gesamtzahl der Abonnenten, den Namen und die Adresse jedes Empfängers sowie den Zeitpunkt seiner An- oder Abmeldung überprüfen. Sie können auch danach filtern.

   ![](assets/service-logs.png)

1. Wählen Sie im Dienst-Dashboard **[!UICONTROL Berichte]**. Überprüfen Sie die folgenden Indikatoren:

   * Die **[!UICONTROL Gesamtzahl der Abonnenten]** angezeigt.

   * Sie können die Anzahl der An- und Abmeldungen in einem ausgewählten Zeitraum anzeigen. Verwenden Sie die Dropdownliste, um den Zeitraum zu ändern.

     ![](assets/service-reports.png)

   * Die **[!UICONTROL Gesamtentwicklung der Anmeldungen]** Das Diagramm zeigt die Aufschlüsselung nach Zeitraum, einschließlich Anmeldungen, Abmeldungen, die Entwicklung der Zahlen und des Treueprozentsatzes.<!--what is Registered?-->

   * Verwenden Sie die **[!UICONTROL Neu laden]** -Schaltfläche, um die letzten Werte aus der Ausführung und Planung des Tracking-Workflows abzurufen.

## An Abonnenten eines Dienstes versenden

Einmal [Abonnement-Dienst erstellt](#create-service), können Sie die Abonnenten in einem Versand gezielt ansprechen. Gehen Sie dazu wie folgt vor.

1. [Erstellen einer Zielgruppe](../audience/create-audience.md) einschließlich der Abonnenten des von Ihnen erstellten Dienstes:

   * Im **[!UICONTROL Audience erstellen]** Aktivität, erweiterte Attribute anzeigen und **[!UICONTROL Empfänger]** > **[!UICONTROL Abonnements]** > **[!UICONTROL Dienst]**.

   * Wählen Sie in diesem Beispiel die Benutzer aus, die den Dienst abonniert haben, der über die **Luma-Newsletter** Beschriftung.

   ![](assets/service-audience-subscribers.png)

1. [Versand erstellen](../msg/gs-messages.md) und wählen Sie die zuvor erstellte Audience aus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Bearbeiten Sie den Inhalt Ihrer Nachricht nach Bedarf und senden Sie ihn.

   ![](assets/service-delivery-ready.png)

Ihre Nachricht wird nur an die Abonnenten dieses Dienstes gesendet.







