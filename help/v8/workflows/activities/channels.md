---
audience: end-user
title: Verwenden der Workflow-Aktivität „Versand“
description: Erfahren Sie, wie Sie eine Workflow-Aktivität „Versand“ hinzufügen (E-Mail, Push-Benachrichtigung, SMS).
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: 0f420559fa49efbe7eea79474d2db7341e51fca8
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 70%

---

# E-Mail-, SMS- und Push-Aktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketing-Kampagnen über E-Mail-, SMS- oder Push-Kanäle automatisieren und durchführen. Sie können Kanalaktivitäten in die Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Aktionen ausgelöst werden können.

Sie können beispielsweise eine Begrüßungs-E-Mail-Kampagne erstellen, die eine Reihe von Nachrichten über verschiedene Kanäle wie E-Mail, SMS und Push-Benachrichtigungen enthält. Sie können auch eine Folge-E-Mail senden, nachdem eine Kundin oder ein Kunde einen Kauf getätigt hat, oder eine personalisierte Geburtstagsnachricht per SMS an eine Kundin bzw. einen Kunden senden.

Mithilfe von Kanalaktivitäten können Sie umfassende und personalisierte Kampagnen erstellen, die Kundinnen und Kunden über mehrere Touchpoints hinweg ansprechen, und Konversionen fördern.

>[!NOTE]
>
>Sie können auch einen eigenständigen Versand außerhalb des Kampagnen-Workflows erstellen. Weitere Informationen finden Sie in den folgenden Abschnitten:
>* [Erstellen eines eigenständigen E-Mail-Versands](../../email/create-email.md)
>* [Erstellen eines eigenständigen SMS-Versands](../../sms/create-sms.md)
>* [Erstellen eines eigenständigen Push-Versands](../../push/create-push.md)

## Erstellen eines Workflows {#build-your-workflow}

Beginnen Sie mit der Erstellung Ihres Workflows mit den relevanten Aktivitäten, bevor Sie die Kanalaktivität einfügen:

* Bevor Sie eine Versandaktivität einfügen, müssen Sie die Zielgruppe definieren. Die Audience ist die Hauptzielgruppe Ihres Versands: die Profile, an die die Nachrichten gesendet werden. Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Nachrichtenzielgruppe nicht in der Kanalaktivität, sondern in einer dedizierten Aktivität definiert, z. B.:

   * A **Audience erstellen** -Aktivität. [Weitere Informationen](build-audience.md).

  ![](../../msg/assets/add-delivery-in-wf.png)

   * A **Datei laden** -Aktivität und **Abstimmung** -Aktivität. [Weitere Informationen](load-file.md).


* Um einen wiederkehrenden Versand zu senden, starten Sie Ihren Workflow mit einem **Planung** -Aktivität. Sie können auch eine **Planung** -Aktivität für einmalige Sendungen, um das Kontaktdatum für diesen Versand festzulegen. Dieses Kontaktdatum kann auch in den Versandeinstellungen festgelegt werden. Weitere Informationen finden Sie in [diesem Abschnitt](scheduler.md).


## Konfigurieren der Kanalaktivität {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="E-Mail-Aktivität"
>abstract="Die E-Mail-Aktivität erleichtert den E-Mail-Versand innerhalb Ihres Workflows und ermöglicht sowohl einmalige als auch wiederkehrende Nachrichten. Damit wird der Versand von E-Mails an eine innerhalb desselben Workflows berechnete Zielgruppe automatisiert. Sie können Kanalaktivitäten in die Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Aktionen ausgelöst werden können."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS-Aktivität"
>abstract="Die SMS-Aktivität erleichtert den SMS-Versand innerhalb Ihres Workflows und ermöglicht sowohl einmalige als auch wiederkehrende Nachrichten. Damit wird der SMS-Versand an eine innerhalb desselben Workflows berechnete Zielgruppe automatisiert. Sie können Kanalaktivitäten in die Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Aktionen ausgelöst werden können."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Push-iOS-Aktivität"
>abstract="Die Push-iOS-Aktivität optimiert den Versand von iOS-Push-Benachrichtigungen im Rahmen Ihres Workflows. Dies ermöglicht den Versand einmaliger und wiederkehrender Nachrichten und automatisiert den Versand von iOS-Push-Benachrichtigungen an eine vordefinierte Zielgruppe innerhalb desselben Workflows. Sie können Kanalaktivitäten in die Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Aktionen ausgelöst werden können."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Push-Android-Aktivität"
>abstract="Die Push-Android-Aktivität vereinheitlicht den Versandprozess für Android-Push-Benachrichtigungen im Rahmen Ihres Workflows. Dadurch wird der Versand einmaliger und wiederkehrender Nachrichten ermöglicht, wodurch der Versand von Android-Push-Benachrichtigungen an eine vordefinierte Zielgruppe innerhalb desselben Workflows automatisiert wird. Sie können Kanalaktivitäten in die Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Aktionen ausgelöst werden können."

Gehen Sie wie folgt vor, um einen Versand im Kontext eines Workflows einzurichten:

1. Fügen Sie eine Kanalaktivität hinzu: **[!UICONTROL E-Mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Push-Benachrichtigung (Android)]** oder **[!UICONTROL Push-Benachrichtigung (iOS)]**.

1. Wählen Sie den **Versandtyp** aus: einmalig oder wiederkehrend.

   * A **Einzelversand** ist ein einmaliger Versand, der nur einmal gesendet wird, beispielsweise eine Black Friday-E-Mail.
   * A **Wiederkehrender Versand** wird mehrmals gesendet, je nachdem, welche Ausführungshäufigkeit in einer [Planungsaktivität](scheduler.md). Bei jeder Ausführung des Workflows wird die Audience neu berechnet und der Versand an die aktualisierte Audience mit dem aktualisierten Inhalt gesendet. Dies kann beispielsweise ein wöchentlicher Newsletter oder eine wiederkehrende Geburtstags-E-Mail sein.

1. Wählen Sie eine **Versandvorlage** aus. Vorlagen sind vorkonfigurierte, kanalspezifische Versandeinstellungen. Für jeden Kanal ist eine integrierte Vorlage verfügbar, die standardmäßig vorausgefüllt ist. [Weitere Informationen](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)

   Sie können die Vorlage im linken Bereich der Konfiguration der Kanalaktivität auswählen. Wenn die zuvor ausgewählte Zielgruppe nicht mit dem Kanal kompatibel ist, können Sie keine Vorlage auswählen. Um dies zu beheben, aktualisieren Sie die Aktivität **Zielgruppe erstellen**, um eine Zielgruppe mit dem richtigen Zielgruppen-Mapping auszuwählen. Weitere Informationen zu Zielgruppen-Mappings finden Sie unter [diesem Abschnitt](../../audience/targeting-dimensions.md)

1. Klicken Sie auf **Versand erstellen**. Sie können dann Ihre Nachrichteneinstellungen und Inhalte auf die gleiche Weise wie einen eigenständigen Versand definieren. Sie können den Inhalt auch testen und simulieren. [Weitere Informationen](../../msg/gs-messages.md)

1. Navigieren Sie zurück zu Ihrem Workflow. Wenn Sie mit dem Workflow fortfahren möchten, können Sie die **Ausgehende Transition erzeugen** -Option, um eine Transition nach der Kanalaktivität hinzuzufügen.

1. Klicken Sie auf **Starten**, um Ihren Workflow zu starten.

   Standardmäßig wird durch Starten eines Workflows die Vorbereitungsphase der Nachricht ausgelöst, ohne dass die Nachricht sofort versendet wird.

1. Öffnen Sie Ihre Kanalaktivität, um den Versand über die **Überprüfen und Senden** Schaltfläche.

1. Klicken Sie im Versand-Dashboard auf **Senden**.

## Beispiele {#cross-channel-workflow-sample}

Im Folgenden finden Sie ein Beispiel eines Cross-Channel-Workflows mit einer Segmentierung und zwei Sendungen. Der Workflow richtet sich an alle Kundinnen und Kunden, die in Paris leben und an Kaffeemaschinen interessiert sind. Innerhalb dieser Population wird eine E-Mail an die regulären Kundinnen und Kunden und eine SMS an diejenigen mit VIP-Status gesendet.

![](../assets/workflow-channel-example.png)

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->

Sie können auch einen wiederkehrenden Workflow erstellen, um jeden ersten Tag des Monats um 20 Uhr eine personalisierte SMS an alle in Paris lebenden Kundinnen und Kunden zu senden.

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
