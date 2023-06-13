---
audience: end-user
title: Erstellen von Kampagnen mit Adobe Campaign Web
description: Erfahren Sie, wie Sie mit Adobe Campaign Web Cross-Channel-Kampagnen erstellen
badge: label="Alpha" type="Positive"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: 4619cffbe2f172637357668b2b4f50cebc27af09
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 18%

---


# Erstellen von Cross-Channel-Kampagnen {#create-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Kampagnenerstellungs-Eigenschaften"
>abstract="Definieren Sie Eigenschaften und Metadaten für die Kampagne."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Eigenschaften der Kampagne"
>abstract="Definieren Sie Kampagneneinstellungen und Metadaten."

Kampagnen können Workflows und eigenständige Sendungen umfassen.

Gehen Sie wie folgt vor, um eine neue Kampagne zu erstellen:

1. Klicken Sie auf **[!UICONTROL Kampagnen]** und klicken Sie auf das **[!UICONTROL Kampagne erstellen]** Schaltfläche.
1. Wählen Sie die **Vorlage** , um die Kampagne zu verwenden und einen Titel anzugeben. Kampagnenvorlagen sind so vorkonfiguriert, dass sie zur Erstellung neuer Kampagnen wiederverwendet werden können. Sie werden über die Client-Konsole erstellt.
   [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=de)
1. Bei Bedarf können Sie Folgendes ändern: **Zusätzliche Optionen**: interner Name, Ordner, Bevollmächtigter, Beschreibung und Art.
1. Definieren Sie die **Zeitplan** Ihrer Kampagne. Die Kampagne beginnt mit Erreichen des Startdatums. Start- und Enddaten werden in der Kampagnenliste angezeigt und können als Filter verwendet werden. Weitere Informationen finden Sie in [diesem Abschnitt](gs-campaigns.md#access-campaigns).

   ![Definieren von Kampagneneigenschaften](assets/campaign-properties.png)

   >[!NOTE]
   >
   >Sie können diese Eigenschaften jederzeit ändern, indem Sie die **Kampagneneinstellungen konfigurieren** neben dem Kampagnentitel. Siehe diesen [Abschnitt](gs-campaigns.md#campaign-dashboard)

1. Wählen Sie **Erstellen** aus.
1. Fügen Sie Ihrer Kampagne Workflows und Sendungen hinzu:

   * Aus dem **Workflows** Registerkarte, klicken Sie auf **Workflow erstellen**. Beim Erstellen Ihrer Kampagne wird automatisch ein Standard-Workflow hinzugefügt. Weitere Informationen zum [Workflow erstellen](../workflows/create-workflow.md)
   * Aus dem **Sendungen** Registerkarte, klicken Sie auf **Versand erstellen**. [Weitere Informationen](../msg/gs-messages.md)

1. Verwenden Sie die **Protokolle** und **Berichterstellung** -Schaltflächen, um die Leistung Ihrer Kampagne zu analysieren.

## Monitoring- und Trackinglogs{#campaign-monitoring}

Die Überwachung von Kampagnen ist ein wichtiger Schritt zur Analyse Ihrer Kampagnen. Öffnen Sie die Kampagne und klicken Sie auf die Schaltfläche **Protokolle** Schaltfläche.

Sie können auch die entsprechenden Berichte anzeigen, indem Sie auf die **Berichte** Schaltfläche. Weitere Informationen finden Sie in [diesem Abschnitt](../reporting/campaign-reports.md).

## Kampagnen duplizieren und löschen

Sie können eine Kampagne duplizieren oder löschen:

* Klicken Sie in der Kampagnenliste auf die Suchschaltfläche und wählen Sie **Duplizieren** oder **Löschen**.
* Klicken Sie in der Kampagne selbst auf die **Mehr** Schaltfläche und wählen Sie **Duplizieren** oder **Löschen**.

>[!NOTE]
>
>Die **Sendungen** alle mit der Kampagne verknüpften Sendungen anzeigen. In einem Workflow erstellte Sendungen können jedoch nicht von dort gelöscht werden. Um einen im Rahmen eines Workflows erstellten Versand zu löschen, ist die Löschung der Versandaktivität im Workflow erforderlich.


<!--
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

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
