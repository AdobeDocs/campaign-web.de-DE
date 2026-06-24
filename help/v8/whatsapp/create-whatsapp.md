---
audience: end-user
title: Erstellen eines WhatsApp-Versands
description: Erfahren Sie, wie Sie in der Adobe Campaign Web-Benutzeroberfläche einen WhatsApp-Versand erstellen
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
hide: true
source-git-commit: aa1a7c48d1708e73e4d6c6bbe4decd2e5ca69102
workflow-type: ht
source-wordcount: '472'
ht-degree: 100%

---


# Erstellen einer WhatsApp-Nachricht {#create-whatsapp}

Mit der **Adobe Campaign Web-Benutzeroberfläche** können Sie WhatsApp-Nachrichten erstellen, die von Meta genehmigte Vorlagen verwenden, sie für jedes Profil personalisieren und vor dem Versand testen.


+++ Weitere Informationen zu unterstützten Nachrichtenelementen und Aktionsaufrufen

Die folgenden Nachrichtentypen werden in WhatsApp unterstützt:

| Nachrichtenfunktion | Beschreibung |
|-|-|
| Kopfzeilen | Optionaler Text, der über dem Nachrichtentext angezeigt wird. |
| Text | Unterstützt dynamische Inhalte durch Parameter. |
| Kopfzeilenbild | Optionales Bild, das über dem Nachrichtentext angezeigt wird. |
| Textkörper | Unterstützt dynamische Inhalte durch Parameter. |
| Fußzeilentext | Unterstützt dynamische Inhalte durch Parameter. |

+++


## Erstellen eines WhatsApp-Versands {#create-whatsapp-journey-campaign}

>[!IMPORTANT]
>
>Feedback zu WhatsApp-Nachrichten wird derzeit nicht unterstützt.

Gehen Sie in der Web-Benutzeroberfläche von Adobe Campaign wie folgt vor, um einen eigenständigen WhatsApp-Versand zu erstellen.

1. Wählen Sie das Menü **[!UICONTROL Sendungen]** aus und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

   ![](assets/whatsapp-create-1.png)

1. Wählen Sie **[!UICONTROL WhatsApp]** und wählen Sie eine Versandvorlage aus. [Weitere Informationen zu Vorlagen](../msg/delivery-template.md).

   ![](assets/whatsapp-create-2.png)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

1. Klicken Sie auf **[!UICONTROL Einstellungen]**, um auf die erweiterten Optionen für Ihre Versandvorlage zuzugreifen. [Weitere Informationen](../advanced-settings/delivery-settings.md)

   ![](assets/whatsapp-create-3.png)

1. Geben Sie einen **[!UICONTROL Titel]** für den Versand ein. Verwenden Sie **[!UICONTROL Zusätzliche Optionen]** wenn Sie internen Namen, Ordner, Versand-Code, Beschreibung oder Art nach dem gleichen Muster wie andere Kanäle benötigen.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe auswählen]**, um eine vorhandene Zielgruppe anzusprechen oder eine eigene zu erstellen. [Weitere Informationen zu Zielgruppen](../audience/about-recipients.md).

1. Klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**, um den WhatsApp-Inhalts-Editor zu öffnen, siehe [Definieren Ihres WhatsApp-Inhalts](#whatsapp-content)).

   ![](assets/whatsapp-create-4.png)

1. Sie können **[!UICONTROL Zeitplanung aktivieren]** aktivieren, um die Nachrichten an einem bestimmten Datum und zu einer bestimmten Uhrzeit zu senden. [Weitere Informationen](../msg/gs-deliveries.md#gs-schedule).


## Definieren Ihres WhatsApp-Inhalts{#whatsapp-content}

>[!BEGINSHADEBOX]

Bevor Sie Ihre WhatsApp-Nachricht in der Web-Benutzeroberfläche von Adobe Campaign entwerfen, erstellen Sie Ihre Vorlage in Meta und senden Sie sie dort. [Weitere Informationen](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

Ihre WhatsApp-Vorlage muss vor der Verwendung von Meta genehmigt werden. Die Genehmigung dauert häufig wenige Stunden, kann aber bis zu 24 Stunden dauern. [Weitere Informationen](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. Klicken Sie in der Adobe Campaign Web-Benutzeroberfläche auf der Seite mit der Versandkonfiguration auf **[!UICONTROL Inhalt bearbeiten]**, um die WhatsApp-Nachricht zu konfigurieren.

1. Wählen Sie „Marketing“ als **Vorlagenkategorie**:

   [Weitere Informationen zu Vorlagenkategorien](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

   ![](assets/whatsapp-design-1.png)

1. Wählen Sie aus dem Dropdown-Menü **WhatsApp-Vorlage** Ihre von Meta genehmigte Vorlage aus.

   [Weitere Informationen zum Erstellen von WhatsApp-Vorlagen](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

   ![](assets/whatsapp-design-2.png)

1. Wenn Ihre von Meta genehmigte Vorlage ein Bild enthält, geben Sie die **[!UICONTROL Bild-URL]** an.

   ![](assets/whatsapp-design-3.png)

1. Verwenden Sie im Feld **Platzhalter für Personalisierung** den Personalisierungs-Editor, um den Vorlagenparametern Profilfelder und Ausdrücke zuzuordnen. [Weitere Informationen](../personalization/personalize.md).

   ![](assets/whatsapp-design-4.png)

Wenn die Nachricht fertig ist:

* **Eigenständiger oder Kampagnen-Versand**: Verwenden Sie **[!UICONTROL Überprüfen und Senden]** und **[!UICONTROL Senden]** im Versand-Dashboard.

* **Workflow**: Öffnen Sie den Versand über die Workflow-Aktivität, wenn die Ausführung ihn verfügbar macht, und verwenden Sie dann das Versand-Dashboard auf die gleiche Weise. [Weitere Informationen](../workflows/start-monitor-workflows.md)

Sie können dann die Ergebnisse der Versandeinstiegspunkte **[!UICONTROL Berichte]** und [Versandberichte](../reporting/delivery-reports.md) verfolgen.
