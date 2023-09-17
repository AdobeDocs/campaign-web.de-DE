---
audience: end-user
title: Arbeiten mit Abonnementdiensten
description: Erfahren Sie, wie Sie Dienste im Adobe Campaign Web erstellen
badge: label="Beta"
source-git-commit: dd8e8acb37cf9a68768c5da48335275c09d67cc8
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Arbeiten mit Abonnementdiensten {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Erstellen und Verwalten Ihrer Dienste"
>abstract="Verwenden Sie Adobe Campaign, um Ihre Dienste wie z. B. Newsletter zu erstellen und zu überwachen und die An- und Abmeldungen dieser Dienste zu überprüfen. Abonnements gelten nur für E-Mail- und SMS-Sendungen."

Verwenden Sie das Adobe Campaign-Web, um Ihre Dienste wie z. B. Newsletter zu verwalten und zu erstellen und die An- und Abmeldungen für diese Dienste zu überprüfen.

>[!NOTE]
>
>Abonnements gelten nur für E-Mail- und SMS-Sendungen.

Es können mehrere Dienste parallel definiert werden, z. B. Newsletter für bestimmte Produktkategorien, Themen oder Bereiche einer Website, Abonnements für verschiedene Arten von Warnhinweisen und Echtzeit-Benachrichtigungen.

Weiterführende Informationen zur Verwaltung von An- und Abmeldungen finden Sie im Abschnitt [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Anmeldedienste aufrufen {#access-services}

Um auf die für Ihre Plattform verfügbaren Anmeldedienste zuzugreifen, navigieren Sie zu **[!UICONTROL Abonnementdienste]** in der linken Navigationsleiste.

![](assets/service-list.png)

Die Liste aller vorhandenen Anmeldedienste wird angezeigt. Sie können die Dienste durchsuchen und nach Kanal, Ordner oder erweiterten Filtern filtern.

![](assets/service-filters.png)

Um einen vorhandenen Dienst zu bearbeiten, klicken Sie auf seinen Namen.

## Erstellen des ersten Abonnementdienstes {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Eigenschaften des Anmeldedienstes"
>abstract="Geben Sie den Titel des Anmeldedienstes ein und definieren Sie zusätzliche Optionen."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Bestätigungsnachrichten für den Abonnementdienst"
>abstract="Wenn sich ein Benutzer für einen Dienst anmeldet oder sich von einem Dienst abmeldet, können Sie eine Bestätigungsnachricht senden. Wählen Sie die für diese Nachrichten zu verwendenden Vorlagen aus."


Gehen Sie wie folgt vor, um einen Abonnementdienst zu erstellen:

1. Wählen Sie die **[!UICONTROL Abonnement-Dienst erstellen]** Schaltfläche.

   ![](assets/service-create-button.png)

1. Kanal auswählen: **[!UICONTROL Email]** oder **[!UICONTROL SMS]**.

1. Geben Sie in den Diensteigenschaften einen Titel ein und definieren Sie nach Bedarf zusätzliche Optionen.

   ![](assets/service-create-properties.png)

1. Standardmäßig sind Abonnements unbegrenzt. Sie können die **[!UICONTROL Unbegrenzte Gültigkeitsdauer]** -Option, um eine Gültigkeitsdauer für den Dienst festzulegen. <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. Wenn sich ein Benutzer für einen Dienst anmeldet oder diesen abmeldet, können Sie eine Bestätigungsnachricht senden. Wählen Sie je nach Anwendungsfall die Vorlagen aus, die für diese Nachricht verwendet werden sollen.

   ![](assets/service-create-confirmation-msg.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**. Der neue Dienst wird zum **[!UICONTROL Abonnementdienste]** Liste.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


