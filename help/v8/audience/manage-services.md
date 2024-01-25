---
audience: end-user
title: Arbeiten mit Anmeldediensten
description: Erfahren Sie, wie Sie in Adobe Campaign Web auf Anmeldedienste zugreifen, diese erstellen und sie verwalten können.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: cbfd821173466c51e9073f01e8792cbdc069c6a2
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 71%

---

# Abonnement-Dienste erstellen und verwalten {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Erstellen und Verwalten von Diensten"
>abstract="Adobe Campaign verwenden, um Dienste wie z. B. Newsletter zu erstellen und zu überwachen und die An- und Abmeldungen für diese Dienste zu überprüfen. Abonnements gelten nur für den E-Mail- und SMS-Versand."

Verwenden Sie Adobe Campaign Web, um Ihre Dienste wie z. B. Newsletter zu verwalten und zu erstellen und die An- und Abmeldungen für diese Dienste zu überprüfen.

>[!NOTE]
>
>Abonnements gelten nur für den E-Mail- und SMS-Versand.

Dabei können mehrere Dienste parallel definiert werden, z. B. Newsletter für bestimmte Produktkategorien, Themen oder Bereiche einer Website, Abonnements zu verschiedenen Arten von Warnmeldungen und Echtzeitbenachrichtigungen.

Weiterführende Informationen zur Verwaltung von Abonnements und Abmeldungen finden Sie im Abschnitt [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html?lang=de){target="_blank"}.

## Zugreifen auf Anmeldedienste {#access-services}

Gehen Sie wie folgt vor, um auf die für Ihre Plattform verfügbaren Anmeldedienste zuzugreifen.

1. Navigieren Sie zum Menü **[!UICONTROL Anmeldedienste]** in der linken Navigationsleiste.

   ![](assets/service-list.png)

1. Die Liste aller vorhandenen Anmeldedienste wird angezeigt. Sie können die Dienste durchsuchen und nach Kanal, Ordner oder Regeln filtern, indem Sie die [Abfragemodellierung](../query/query-modeler-overview.md).

   ![](assets/service-filters.png)

1. Um einen vorhandenen Dienst zu bearbeiten, klicken Sie auf seinen Namen.

1. Sie können jeden Dienst löschen oder duplizieren, indem Sie das Symbol mit den drei Punkten neben dem Dienstnamen verwenden.<!--so all subscribers are unsubscribed - need to mention?-->

## Erstellen Ihres ersten Anmeldedienstes {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Definieren der Diensteigenschaften"
>abstract="Geben Sie den Titel des Anmeldedienstes ein und definieren Sie zusätzliche Optionen, z. B. einen Gültigkeitszeitraum für Ihren Dienst."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Auswählen einer Bestätigungsnachricht"
>abstract="Wenn sich eine Benutzerin bzw. ein Benutzer für einen Dienst anmeldet oder sich von ihm abmeldet, können Sie eine Bestätigungsnachricht senden. Wählen Sie die Vorlagen aus, die für diese Nachricht verwendet werden sollen."

Gehen Sie wie folgt vor, um einen Anmeldedienst zu erstellen.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Anmeldedienst erstellen]**.

   ![](assets/service-create-button.png)

1. Wählen Sie einen Kanal aus: **[!UICONTROL E-Mail]** oder **[!UICONTROL SMS]**.

1. Geben Sie in den Diensteigenschaften einen Titel ein und definieren Sie **[!UICONTROL Zusätzliche Optionen]** wie gewünscht.

   ![](assets/service-create-properties.png)

1. Dienste werden standardmäßig im **[!UICONTROL Dienste und Abonnements]** Ordner. Sie können ihn ändern, indem Sie zum gewünschten Speicherort navigieren. [Erfahren Sie mehr über die Arbeit mit Ordnern](../get-started/permissions.md#folders)

1. Standardmäßig sind Abonnements unbegrenzt. Sie können die Option **[!UICONTROL Unbegrenzter Gültigkeitszeitraum]** deaktivieren, um einen Gültigkeitszeitraum für den Dienst festzulegen.

   Im folgenden Beispiel wäre nach 20 Tagen Folgendes der Fall:
   * Empfängerinnen und Empfänger können sich nicht mehr für einen Dienst anmelden.
   * Alle Abonnentinnen und Abonnenten dieses Dienstes werden nach 20 Tagen automatisch abgemeldet. [Weitere Informationen](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. Wenn sich eine Benutzerin bzw. ein Benutzer für einen Dienst anmeldet oder sich von ihm abmeldet, können Sie eine Bestätigungsnachricht senden. Wählen Sie je nach Anwendungsfall die Vorlagen aus, die für diese Nachricht verwendet werden sollen. Diese Vorlagen müssen mit dem Zielgruppen-Mapping für die  **[!UICONTROL Abonnements]** konfiguriert werden. [Weitere Informationen](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. Klicken Sie auf **[!UICONTROL Speichern und überprüfen]**. Der neue Dienst wird zur Liste **[!UICONTROL Anmeldedienste]** hinzugefügt.

Sie können jetzt:

* Fügen Sie Abonnenten zu diesem Dienst hinzu und melden Sie Empfänger ab. [Weitere Informationen](../msg/send-to-subscribers.md)

* Senden Sie Nachrichten an die Abonnenten dieses Dienstes. [Weitere Informationen dazu](../msg/send-to-subscribers.md)

## Erstellen einer Bestätigungsnachricht {#create-confirmation-message}

Um den Benutzerinnen und Benutzern, die sich für Ihren Dienst angemeldet haben oder sich von ihm abmelden, Bestätigungsnachrichten zu senden, müssen Sie eine Versandvorlage mit dem Zielgruppen-Mapping für die **[!UICONTROL Abonnements]** erstellen, und zwar ohne eine definierte Zielgruppe. Gehen Sie dazu wie folgt vor.

1. Erstellen Sie eine Versandvorlage für die Abonnementbestätigung. [Erfahren Sie, wie Sie eine Vorlage erstellen](../msg/delivery-template.md)

1. Wählen Sie für diesen Versand keine Zielgruppe aus. Rufen Sie stattdessen den Versand auf. **[!UICONTROL Einstellungen]**, navigieren Sie zu [Zielgruppe](../advanced-settings/delivery-settings.md#audience) und wählen Sie die **[!UICONTROL Abonnements]** Zielgruppen-Mapping aus der Liste.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >Wenn Sie das Zielgruppen-Mapping für **[!UICONTROL Abonnements]** nicht auswählen, erhalten Ihre Abonnentinnen und Abonnenten keine Bestätigungsnachricht. Zielgruppen-Mappings werden in der Campaign v8-Konsole definiert. Weitere Informationen finden Sie unter [Dokumentation zu Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=de){target="_blank"}.

1. Bearbeiten Sie den Inhalt Ihrer Versandvorlage, speichern und schließen Sie sie.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >Erfahren Sie in den Abschnitten [E-Mail-Kanal](../email/create-email.md) und [SMS-Kanal](../sms/create-sms.md) mehr über Versandkanäle und darüber, wie Sie Versandinhalte definieren.

1. Wiederholen Sie die obigen Schritte, um eine Versandvorlage für die Abmeldebestätigung zu erstellen.

Sie können diese Nachrichten jetzt auswählen, wenn Sie einen [Anmeldedienst erstellen](#create-service). Benutzende, die diesen Dienst abonnieren oder sich von ihm abmelden, erhalten die ausgewählten Bestätigungsnachrichten.

## Überwachen von Anmeldediensten {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Abonnierende insgesamt"
>abstract="Klicks **berechnen** die Gesamtzahl der Abonnenten für diesen Dienst."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Anzahl Anmeldungen im Zeitraum"
>abstract="Verwenden Sie die Dropdown-Liste, um den Zeitraum zu ändern und die Anzahl der Anmeldungen und Abmeldungen im ausgewählten Zeitraum anzuzeigen."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Abonnements – Gesamtentwicklung"
>abstract="Dieses Diagramm zeigt die Aufschlüsselung nach Zeitraum, einschließlich Anmeldungen, Abmeldungen, die Entwicklung der Zahlen und des Treueprozentsatzes."

Um die Effektivität Ihrer Anmeldedienste für die Kanäle SMS und E-Mail zu messen, können Sie auf die Protokolle und Berichte für einen bestimmten Dienst zugreifen.

1. Wählen Sie einen vorhandenen Dienst aus der Liste **[!UICONTROL Anmeldedienste]** aus. Klicks **[!UICONTROL berechnen]** Rufen Sie die Gesamtzahl der Abonnenten ab.

   ![](assets/service-logs-subscribers-count.png)

1. Wählen Sie im Dienst-Dashboard **[!UICONTROL Protokolle]** um die Liste der Abonnenten dieses Dienstes anzuzeigen.

   Sie können die Gesamtzahl der Abonnenten, den Namen und die Adresse jedes Empfängers sowie den Zeitpunkt seiner An- oder Abmeldung überprüfen. Sie können auch danach filtern.

   ![](assets/service-logs.png)

1. Wählen Sie im Dashboard des Dienstes die Option **[!UICONTROL Berichte]** aus. Überprüfen Sie die folgenden Indikatoren:

   * Die **[!UICONTROL Gesamtzahl der Abonnentinnen und Abonnenten]** wird angezeigt.

   * Sie können die Anzahl der Abonnierungen und Abmeldungen in einem ausgewählten Zeitraum anzeigen. Verwenden Sie die Dropdown-Liste, um den Zeitraum zu ändern.

     ![](assets/service-reports.png)

   * Der Graph **[!UICONTROL Gesamtentwicklung der Abonnements]** zeigt die Aufschlüsselung nach Zeitraum, einschließlich Abonnierungen, Abmeldungen, Entwicklung der Zahlen und Prozentsatz der Kundentreue.<!--what is Registered?-->

1. Klicken Sie auf **[!UICONTROL Neu laden]**, um die letzten Werte aus der Ausführung und Planung des Tracking-Workflow abzurufen.
