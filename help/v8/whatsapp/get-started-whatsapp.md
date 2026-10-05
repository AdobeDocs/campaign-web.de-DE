---
audience: end-user
title: Erste Schritte mit WhatsApp-Nachrichten
description: Erfahren Sie, wie Sie WhatsApp-Nachrichten mit der Adobe Campaign Web-Benutzeroberfläche erstellen und senden
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 100%
---
# Erste Schritte mit WhatsApp-Nachrichten {#get-started-whatsapp}

Sie können WhatsApp-Nachrichten über die **Adobe Campaign Web-Benutzeroberfläche** mithilfe der [Cloud-API](https://developers.facebook.com/docs/whatsapp/cloud-api/) von Meta senden. Verwenden Sie WhatsApp in eigenständigen Sendungen, in Kampagnen-Workflows oder innerhalb von Marketing-Kampagnen zusammen mit Ihren anderen Kanälen.

* **[!UICONTROL Sendungen:]** Erstellen Sie in der Adobe Campaign Web-Benutzeroberfläche einen eigenständigen WhatsApp-Versand über das Menü **[!UICONTROL Sendungen]** in der linken Leiste – ähnlich wie bei SMS oder Push. [Weitere Informationen](create-whatsapp.md).

* **[!UICONTROL Kampagnen:]** Öffnen Sie in der Adobe Campaign Web-Benutzeroberfläche eine Kampagne und fügen Sie einen WhatsApp-Versand über die Registerkarte **[!UICONTROL Sendungen]** hinzu oder koordinieren Sie Sendungen mit einem an die Kampagne angehängten Workflow. [Weitere Informationen](../campaigns/create-campaigns.md).

* **[!UICONTROL Workflows:]** Fügen Sie in der Workflow-Arbeitsfläche der Adobe Campaign Web-Benutzeroberfläche die Kanalaktivität **[!UICONTROL WhatsApp]** hinzu, wählen Sie eine Versandvorlage aus und definieren Sie dann Inhalt und Einstellungen im Versand-Dashboard. Weitere Informationen zu Kanalaktivitäten finden Sie in [diesem Abschnitt](../workflows/activities/channels.md).

## Voraussetzungen: {#prereq}

Die Integration von WhatsApp erfordert Folgendes:

* Meta Business Manager-Konto
* [WhatsApp Business-Konto mit verifiziertem Absendernamen und Telefonnummer](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [Benutzerautorisierungs-Token mit entsprechenden Berechtigungen](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Genehmigte Meta-Vorlagen](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

Sie müssen außerdem Folgendes bestätigen, bevor Sie fortfahren:

* [WhatsApp-Inhaltsregeln](https://www.whatsapp.com/legal/messaging-guidelines)
* [Konformität mit den Meta-Richtlinien](https://www.whatsapp.com/legal)
* [24-Stunden-Dialogbegrenzungen](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


