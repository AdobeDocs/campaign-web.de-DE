---
audience: end-user
title: Erste Schritte mit Adobe Campaign Web
description: Erste Schritte mit Adobe Campaign Web
exl-id: 885d7851-4e5d-4b03-ba6f-71f90ede83e8
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 99%

---

# Erste Schritte mit Adobe Campaign Web {#get-started}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_learnmore"
>title="Erste Schritte"
>abstract="Die neue Adobe Campaign Web-Schnittstelle bietet ein integriertes, intuitives und konsistentes Benutzererlebnis."

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_learnmore"
>title="Erste Schritte"
>abstract="Die neue Adobe Campaign Web-Schnittstelle bietet ein integriertes, intuitives und konsistentes Benutzererlebnis."

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Erste Schritte"
>abstract="Die neue Adobe Campaign Web-Schnittstelle bietet ein integriertes, intuitives und konsistentes Benutzererlebnis."

Adobe Campaign bietet eine Plattform für die Gestaltung kanalübergreifender Kundenerlebnisse und eine Umgebung für visuelle Kampagnenorchestrierungen, Interaktions-Management in Echtzeit und kanalübergreifende Ausführung.

Adobe Campaign v8 ist das Kampagnen-Tool der nächsten Generation und wurde für verschiedene Marketing-Kanäle wie E-Mail, Push-Benachrichtigungen, SMS und Direkt-Mail entwickelt. Adobe Campaign v8 bietet zuverlässige ETL- und Daten-Management-Funktionen, mit denen Sie die perfekte Kampagne erstellen und kuratieren können. Die Orchestrierungs-Engine ermöglicht umfassende Multi-Touch-Marketing-Programme mit einem Schwerpunkt auf Batch-gesteuerten Journeys. Darüber hinaus umfasst es einen skalierbaren Echtzeit-Messaging-Server, mit dem Marketing-Teams vordefinierte Nachrichten basierend auf einer umfassenden Payload von jedem IT-System aus versenden können, beispielsweise für das Zurücksetzen von Passwörtern, Bestellbestätigungen, elektronische Empfangsbestätigungen und vieles mehr.

Mit Campaign haben Sie folgende Möglichkeiten:

* **Fördern** von Personalisierung und Interaktion mithilfe einer umfassenden, zentralen Sicht auf Kundinnen und Kunden
* **Integrieren** von E-Mail-, Mobile-, Online- und Offline-Kanälen in die Customer Journey
* **Automatisieren** des Versands aussagekräftiger, zeitlich optimal abgestimmter Nachrichten und Angebote 

## Funktionsweise der Campaign Web-Benutzeroberfläche {#web}

Campaign war ursprünglich nur über eine umfangreiche [Client-Konsole](#ac-client) verfügbar, bietet jetzt aber eine neue Web-Benutzeroberfläche mit mehr Benutzerfreundlichkeit, Barrierefreiheit und einem neuen Design, um das Anwendererlebnis deutlich zu verbessern. Diese moderne Benutzeroberfläche vereinfacht die Gestaltung und den Versand von Marketing-Kampagnen und sorgt für Konsistenz mit anderen Adobe-Lösungen, einschließlich Adobe Experience Platform.

![Screenshot des Startbildschirms der Adobe Campaign Web-Benutzeroberfläche](assets/home.png){zoomable="yes"}

Diese neue Web-Benutzeroberfläche erfüllt in erster Linie die Anforderungen von **Business-Anwendenden**. Typische Administrationsaufgaben sind in dieser ersten Version nicht verfügbar, werden aber in nachfolgenden Versionen berücksichtigt. Beachten Sie, dass in der neuen Benutzeroberfläche derzeit nicht alle Funktionen und Optionen der Client-Konsole verfügbar sind. In zukünftigen Versionen werden neue Anwendungsfälle, Optionen und Funktionen zur Verfügung gestellt.

Wenn Admins oder erfahrene Benutzende auf Funktionen von Campaign v8 zugreifen möchten, die nicht in der Campaign Web-Benutzeroberfläche verfügbar sind, können sie sich mit der [Client-Konsole](#ac-client) verbinden.

Auf [dieser Seite](connect-to-campaign.md) finden Sie Informationen dazu, wie Sie eine Verbindung zu Adobe Campaign Web herstellen können.

➡️ [Entdecken Sie Campaign Web im Video](#video)

## Über die Campaign-Client-Konsole {#ac-client}

Die Client-Konsole ist für Admins und erfahrene Benutzende zur Ausführung ihrer Aufgaben vorgesehen. Die Campaign-Client-Konsole ist eine Browser-basierte Anwendung, die auf Ihrem System installiert ist. Sie nutzt das Web-Services-API, um eine Verbindung zu Ihrem Campaign-Anwendungs-Server herzustellen.

Kampagnendaten werden auf dem Anwendungs-Server gespeichert. Auf Daten kann sowohl über die Client-Konsole als auch über die Campaign Web-Benutzeroberfläche zugegriffen werden. Wenn Sie beispielsweise eine Versandvorlage mithilfe der Client-Konsole erstellen, ist diese ebenfalls in der Campaign Web-Benutzeroberfläche verfügbar. Ist in der Campaign Web-Benutzeroberfläche ein E-Mail-Versand eingerichtet, kann diese Versandart wiederum über die Client-Konsole aufgerufen werden.

Einige Objekte können nur in der Client-Konsole erstellt und verwaltet werden. Sie können in der Campaign Web-Benutzeroberfläche angezeigt und verwendet, aber nicht in dieser Umgebung erstellt oder geändert werden. Alle Campaign-Objekte und -Komponenten stehen in der Explorer-Ansicht zur Verfügung, auf die über den linken Navigationsbereich zugegriffen werden kann.

Weitere Informationen zur Verwendung von Campaign v8 mit der Client-Konsole finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=de){target="_blank"}.

<!--
## How-to video {#video}

Learn how to access and navigate the Campaign Web user interface and how to customize the inventory lists. Discover the AI-powered Knowledge Assistant.

>[!VIDEO](https://video.tv.adobe.com/v/3453431?quality=12&captions=ger)
-->

<!--
## Get started for marketers and administrators

>[!BEGINTABS]

>[!TAB Get started for Marketers]

**Discover the interface**

The new Adobe Campaign Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. Learn more in this section. [Learn more](user-interface.md)

**Use plans, programs, campaigns**

Adobe Campaign allows you to easily orchestrate your targeted marketing initiatives, using the built-in campaign management capability. With the ability to define a schedule, you can plan the duration and timing of your campaigns to align with strategic objectives and maximize audience engagement. [Learn more](../campaigns/gs-campaigns.md)

**Create and manage profiles and audiences**

A profile is a record stored in the database, serving as a key component to create audiences for deliveries and add personalization data to your content. Learn how to access, manage, and explore profiles using the Campaign Web User Interface in [this page](../audience/gs-audiences-recipients.md).

Audiences are sets of profiles who share similar behaviors and/or characteristics. This collection of people can either be generated, selected, or loaded. Once created, audiences can be leveraged as the target population of your deliveries. Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups. Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups in [this section](../audience/delivery-recipients.md).

**Configure workflows**

With workflows, you can orchestrate the full range of processes and tasks, improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery. Plus, you can get your channels in sync with a single, easy-to-use interface for campaign orchestration.

Understand how workflows work and how to create a targeting workflow in this how-to video:

>[!VIDEO](https://video.tv.adobe.com/v/3448373?quality=12&captions=ger)

Adobe Campaign Web user interface features a query modeler that simplifies the process of filtering the database based on various criteria. Learn how to use it in [this section](../query/query-modeler-overview.md)

**Work with deliveries**

You can create standalone deliveries from the **Deliveries** left menu, or create deliveries in the context of a workflow, included or not in a campaign. Learn how to create a delivery in [this page](../msg/gs-deliveries.md).

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns. [Learn more](../msg/delivery-template.md)

Delivery settings are technical delivery parameters that are defined in the delivery template. They can be overloaded for each delivery. These settings are available from the **Settings** button available when editing a delivery or a delivery template.

Adobe Campaign Web dynamic content capabilities allow you to customize your content based on the information you have gathered about your recipients. By utilizing dynamic content, you ensure that your marketing efforts are more relevant, avoiding marketing unwanted or unnecessary products or services. Learn more about dynamic content in [this section](../content/fragments.md).

Once your delivery content has been defined, you can use profiles and test profiles to preview and test it before sending the message. This is a crucial step to ensure that it is accurate but also free of errors both in content and personalization settings.

* **Send email** - Learn how to create an email delivery from scratch, define the audience, design the content, simulate preview, and send a proof.
    Learn how to create your first targeted email. In this use case, you schedule the sending of an email to Silver and Gold loyalty members on a specific date.

    The Email Designer enables you to create captivating, individually tailored emails through an intuitive drag-and-drop interface.

    Learn how to preview email message content and personalization, send test deliveries (proofs) to specific recipients or subscribers for testing and validation, and check the email rendering in popular desktop, mobile, and web-based clients.

* **Send SMS** - SMS deliveries provide a practical and efficient way to send text messages to your customers' mobile devices. With this feature, you can create, personalize, and preview text-based messages for effective communication.

* **Send push notifications** - Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app. They serve various purposes like providing updates, driving specific actions, and notifying about deals.

    Adobe Campaign v8 can send rich push notifications. Parameters and settings depend on the mobile operating system:
    * Android Rich push documentation
    * iOS Rich push documentation

* **Send direct mail** - Direct mail is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs. When creating a direct mail delivery, Adobe Campaign automatically generates an extraction file containing all the targeted profiles and selected data, such as postal addresses and profile attributes.<br/>

* **Create landing pages** - Adobe Campaign allows you to create, design, and share landing pages. Landing pages enable you to direct your users to online forms where they can update their data, opt-in/out from receiving your communications, or subscribe to a specific service such as a newsletter.

* **Use reporting** -  Adobe Campaign suite of reporting tools provides valuable insights into the effectiveness of your marketing efforts, allowing you to optimize your campaigns for maximum impact.

    Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city, and age in addition to functional email campaign data like opens and clicks.

>[!TAB Get started for Admins]

**Work with the client console** 

* **Install client console** - Learn how to download and install the Adobe Campaign Client Console, create and manage your connections to multiple environments, and verify access to the Adobe Campaign Client console with this tutorial video.

    Learn how to download, install, and manage the Adobe Campaign Client Console with this documentation.

* **Discover console client interface** - Learn about the Adobe Campaign v8 user interface and how to navigate the main features with this tutorial video.

    You can access Adobe Campaign via its client console or its Web user interface. You can also use APIs to manage data and perform tasks in your Campaign platform.

**Understand Campaign general architecture**

Learn about the typical Adobe Campaign solution deployment.

Adobe Campaign is a cross-channel marketing solution that automates email, mobile, social, and offline campaigns. Adobe Campaign provides a central place to access your customer data and profiles. Use Adobe Campaign to orchestrate consistent experiences for your customers, design, execute, and personalize your marketing across channels, while improving customer experiences on every device and touchpoint.

**Administrate environment**

* **Connect to your environment(s)** - Once the client console is installed, follow the steps in this documentation to create the connection to the application server.

* **Define permissions** - Adobe Campaign lets you define and manage the rights assigned to users. These permissions are defined by combining operator group permissions, named rights, and permissions on folders.

* **Use Campaign control panel** - The Adobe Campaign Control Panel allows Adobe Campaign administrators to monitor key assets and perform administrative tasks, such as managing the SFTP storage by instance, managing GPG keys, or subdomains and certificates.

    Control Panel allows you to set up new connections to your instances by adding IP address ranges to the allow list.
    Subdomain configuration allows you to configure a sub-section of your domain (technically a "DNS zone") for use with Adobe Campaign.
    In the Control Panel, you can interact with all SFTP servers that are connected to Campaign instances that you have access to.

* **Use the audit trail** - In Adobe Campaign Web User Interface, the Audit trail feature provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact a smooth operation of the instance.

**Set up user interface**

* **Customize campaign UI** - Guidelines for managing user interface settings like lists, units, or data display.

* **Add custom fields** - Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. These custom fields are displayed in various screens, for example, the details of a profile or a test profile.

**Set up the branding**

Every company has brand guidelines that define both visual elements and technical details. Adobe Campaign helps you manage these guidelines centrally, so you can present a consistent brand image to your customers in everything you do, from logos in emails to the URLs and domains used in your campaigns.

**Understand data model creation**

Adobe Campaign comes with a pre-defined data model. This section gives some details on the built-in tables of the Adobe Campaign data model and their interaction. Adobe Campaign relies on a Cloud database containing tables that are linked together.

A schema is an XML document associated with a database table. It defines data structure and describes the SQL definition of the table.
When you create or extend a schema, you need to create or modify the associated input forms to make those changes visible to end-users.
An input form lets you edit an instance associated with a data schema from the Adobe Campaign client console. The form is identified by its name and namespace.

**Understand data management**

Use Adobe Campaign workflows to improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery.

Campaign helps you add contacts to the Cloud database. You can load a file, schedule and automate multiple contact updates, collect data on the Web, or enter profile information directly into the recipient table.

You can easily export your different reports to PDF or CSV format, which enables you to share, manipulate, or print them.
Quarantine is the way to manage the invalid addresses in deliveries.

**About delivery management**

Campaign Optimization is the Adobe Campaign module which lets you control, filter, and monitor the sending of deliveries. To avoid conflicts between campaigns, Adobe Campaign can test various combinations by applying specific constraint rules. This guarantees that the messages sent meet the needs and expectations of customers and company communication policies.

All marketing campaigns are based on a template, which stores main characteristics and capabilities. Campaign comes with a built-in template to create campaigns. This template has all functionalities enabled: Documents, Seed addresses, Approvals, Delivery outlines, etc.

Learn how to set up and manage subscriptions and target subscribers.

**Work with templates**

* **Campaigns** - Campaign templates contain pre-configured settings which can be reused for creating new campaigns. A set of built-in templates is available to help you get started.

* **Delivery** - For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns.

* **Workflows** - Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows. Using a workflow template is a best practice if you need to regularly import files with the same structure.

* **Content blocks** - Learn how to create dynamic content blocks and how to use them to personalize the content of your email delivery.

* **Landing pages** - Once you design your landing page content, you can save it for future reuse.

* **Content fragments** - A content fragment is a reusable component that can be referenced in one or more messages. When modifying a fragment, every content using it is updated.

* **Triggers** - Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message.

**Use subscription services**

Use Adobe Campaign Web to manage and create your services such as newsletters, and to check the subscriptions or unsubscriptions to these services.

**Configure delivery sending**

External accounts are used by technical processes such as technical workflows or campaign workflows. For example, when setting up a file transfer in a workflow or a data exchange with any other application (Adobe Target, Experience Manager, or other tools), you need to select an external account.

**Manage Adobe Campaign integrations**

You can connect your Campaign environment with Adobe Experience Cloud solutions and apps to combine capabilities.<br/>
Adobe Campaign comes with several connectors that allow you to communicate with external applications, connect to database engines, and share and synchronize data. These connections are configured by Adobe.

Here are the possible integrations:

**Use transactional messages**

Transactional messaging (Message Center) is a Campaign module designed for managing trigger messages. These notifications are generated from events triggered from information systems, and can include: invoices, order confirmations, shipping confirmations, password changes, product unavailability notifications, account statements, website account creations, and more.

**Use reporting**

Adobe Campaign provides a set of reporting tools.

>[!ENDTABS]

-->