---
audience: end-user
title: Erstellen von Kampagnen mit Adobe Campaign Web
description: Erfahren Sie, wie Sie mit Adobe Campaign Web Cross-Channel-Kampagnen erstellen
badge: label="Beta"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: ef459ca97bbe327128d790f77029521ed12cc6c9
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 58%

---


# Erste Kampagne erstellen {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Kampagnenerstellungs-Eigenschaften"
>abstract="Definieren Sie in diesem Bildschirm die Kampagnenparameter: Wählen Sie eine Vorlage aus und geben Sie einen Titel für die Kampagne ein. Navigieren Sie zu den zusätzlichen Einstellungen, um den standardmäßigen internen Namen und Ordner zu ändern, eine Beschreibung hinzuzufügen und den Verantwortlichen auszuwählen."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Eigenschaften der Kampagne"
>abstract="In diesem Bildschirm können Sie Ihre Kampagneneinstellungen überprüfen und aktualisieren: Titel, interner Name, Ordner und Beschreibung. Sie können auch anzeigen, welchem Benutzer er zugewiesen ist."

Um eine neue Kampagne zu erstellen, müssen Sie deren Eigenschaften definieren, Workflows planen und Sendungen einschließen.

## Erstellen der Kampagne{#campaign-create}

Um eine neue Kampagne zu erstellen, gehen Sie folgendermaßen vor:

1. Klicken Sie auf das Menü **[!UICONTROL Kampagnen]** und dann auf die Schaltfläche **[!UICONTROL Kampagne erstellen]**.
1. Wählen Sie die zu verwendende **Vorlage** und geben Sie eine Bezeichnung für die Kampagne ein. Kampagnenvorlagen sind so vorkonfiguriert, dass sie zur Erstellung neuer Kampagnen wiederverwendet werden können. Sie werden über die Client-Konsole erstellt.
   [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=de)
1. Bei Bedarf können Sie die folgenden **zusätzlichen Optionen** ändern: interner Name, Ordner, Zuweisung, Beschreibung und Art.
1. Definieren Sie den **Zeitplan** für Ihre Kampagne. Erfahren Sie, wie Sie den Kampagnenkalender in [diesem Abschnitt](#campaign-schedule)
1. Wählen Sie **Erstellen** aus.
1. Fügen Sie Workflows und Sendungen zu Ihrer Kampagne hinzu:

   * Klicken Sie auf der Registerkarte **Workflows** auf **Workflow erstellen**. Beim Erstellen Ihrer Kampagne wird automatisch ein Standard-Workflow hinzugefügt. Weitere Informationen zum [Erstellen eines Workflows](../workflows/create-workflow.md).
   * Klicken Sie auf der Registerkarte **Sendungen** auf **Versand erstellen**. [Weitere Informationen](../msg/gs-messages.md)

1. Verwenden Sie die Schaltflächen **Protokolle** und **Berichte**, um die Leistung Ihrer Kampagne zu analysieren.

## Überwachen und Nachverfolgen Ihrer Kampagne{#campaign-monitoring}

Die Überwachung von Kampagnen ist ein wichtiger Schritt zur Analyse der Effektivität Ihrer Kampagnen. Öffnen Sie Ihre Kampagne und klicken Sie auf die Schaltfläche **Protokolle**.

Sie können auch die entsprechenden Berichte anzeigen, indem Sie auf die Schaltfläche **Berichte** klicken. Weitere Informationen finden Sie in [diesem Abschnitt](../reporting/campaign-reports.md).


## Kampagnenkalender definieren {#campaign-schedule}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Kampagnenzeitplan"
>abstract="Wählen Sie den Kampagnenkalender aus. Sie können die Kampagne erstellen, die mit Erreichen des Anfangsdatums beginnt. Standardmäßig ist das Kampagnenstartdatum das Erstellungsdatum und dauert fünf Tage. Start- und Enddatum werden in der Kampagnenliste angezeigt und können als Filter verwendet werden."


Die Kampagne beginnt, wenn das Startdatum erreicht ist. Solange das Startdatum nicht erreicht ist, verfügt die Kampagne über die **[!UICONTROL Entwurf]** -Status. Wenn das Startdatum erreicht ist, wird **[!UICONTROL Gestartet]**. Sobald das Enddatum erreicht ist, wird die Kampagne auf **[!UICONTROL Abgeschlossen]**.

Start- und Enddatum werden in der Kampagnenliste angezeigt und können als Filter verwendet werden. Weitere Informationen finden Sie in [diesem Abschnitt](manage-campaigns.md#access-campaigns).

![Definieren von Kampagneneigenschaften](assets/campaign-properties.png)

>[!NOTE]
>
>Sie können diese Eigenschaften später jederzeit über das Symbol **Kampagneneinstellungen konfigurieren** neben der Kampagnenbezeichnung ändern. Siehe diesen [Abschnitt](gs-campaigns.md#campaign-dashboard).

Sobald das Datum erreicht ist, werden in der Kampagne im Rahmen eines Workflows erstellte Sendungen, die versandbereit sind, tatsächlich gesendet. Dazu muss der Workflow gestartet worden sein.


<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}


In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
