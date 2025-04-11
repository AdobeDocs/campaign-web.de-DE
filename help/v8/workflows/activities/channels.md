---
audience: end-user
title: Verwenden einer Workflow-Aktivität „Versand“
description: Erfahren Sie, wie Sie eine Workflow-Aktivität „Versand“ hinzufügen (E-Mail, Push-Benachrichtigung, SMS, Briefpost).
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 38%

---

# E-Mail-, SMS-, Push- und Briefpost-Aktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketing-Kampagnen für E-Mail-, SMS-, Briefpost- und Push-Kanäle automatisieren und ausführen. Sie können Kanalaktivitäten in der Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Trigger-Aktionen erstellt werden.

Erstellen Sie beispielsweise eine Begrüßungs-E-Mail-Kampagne, die eine Reihe von Nachrichten über verschiedene Kanäle wie E-Mail, SMS, Push und Briefpost enthält. Sie können auch eine Folgenachricht senden, nachdem eine Kundin oder ein Kunde einen Kauf getätigt hat, oder eine personalisierte Geburtstagsnachricht per SMS an eine Kundin bzw. einen Kunden senden.

Erstellen Sie mithilfe von Kanalaktivitäten umfassende und personalisierte Kampagnen, die Kundinnen und Kunden über mehrere Touchpoints hinweg ansprechen und Konversionen fördern.

>[!NOTE]
>
>Sie können auch einen einmaligen Versand außerhalb eines Kampagnen-Workflows erstellen. Weitere Informationen finden Sie in den folgenden Abschnitten:
>* [Erstellen eines eigenständigen E-Mail-Versands](../../email/create-email.md)
>* [Erstellen eines eigenständigen SMS-Versands](../../sms/create-sms.md)
>* [Erstellen eines eigenständigen Push-Versands](../../push/create-push.md)
>* [Erstellen eines eigenständigen Briefpost-Versands](../../direct-mail/create-direct-mail.md)

## Voraussetzungen {#channel-activity-prereq}

Beginnen Sie, Ihren Workflow mit den entsprechenden Aktivitäten aufzubauen:

* Bevor Sie eine Kanalaktivität einfügen, definieren Sie die Audience. Die Zielgruppe ist das hauptsächliche Ziel Ihres Versands: die Profile, die die Nachrichten erhalten. Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Nachrichtenzielgruppe nicht in der Kanalaktivität definiert, sondern in einer dedizierten Aktivität, z. B.:

   * Eine Aktivität **Zielgruppe erstellen**. [Weitere Informationen](build-audience.md).

     ![Screenshot zum Hinzufügen eines Versands in einem Workflow](../../msg/assets/add-delivery-in-wf.png)

   * Eine Aktivität **Datei laden** gefolgt von einer Aktivität **Abstimmung**. [Weitere Informationen](load-file.md).

     ![Screenshot mit Workflow-Abstimmkriterien](../assets/workflow-reconciliation-criteria.png)

* Um einen wiederkehrenden Versand durchzuführen, starten Sie Ihren Workflow mit der Aktivität **Planung**. Verwenden **Aktivität „Planung** für einmalige Sendungen, um das Kontaktdatum für diesen Versand festzulegen. Dieses Kontaktdatum kann auch in den Versandeinstellungen festgelegt werden. Weitere Informationen finden Sie in diesem [Abschnitt](scheduler.md).

## Konfigurieren der Kanalaktivität {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="E-Mail-Aktivität"
>abstract="Die E-Mail-Aktivität erleichtert den E-Mail-Versand innerhalb Ihres Workflows und ermöglicht sowohl einmalige als auch wiederkehrende Nachrichten. Es automatisiert den Prozess des E-Mail-Versands an eine Zielgruppe, die innerhalb desselben Workflows berechnet wird. Sie können Kanalaktivitäten in der Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Trigger-Aktionen erstellt werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS-Aktivität"
>abstract="Die SMS-Aktivität erleichtert den SMS-Versand innerhalb Ihres Workflows und ermöglicht sowohl einmalige als auch wiederkehrende Nachrichten. Es automatisiert den Prozess des Versands von SMS an eine Zielgruppe, die innerhalb desselben Workflows berechnet wird. Sie können Kanalaktivitäten in der Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Trigger-Aktionen erstellt werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Push-iOS-Aktivität"
>abstract="Die Push-iOS-Aktivität optimiert den Versand von iOS-Push-Benachrichtigungen im Rahmen Ihres Workflows. Sie ermöglicht den Versand sowohl einmaliger als auch wiederkehrender Nachrichten und automatisiert so den Versand von iOS-Push-Benachrichtigungen an eine vordefinierte Zielgruppe innerhalb desselben Workflows. Sie können Kanalaktivitäten in der Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Trigger-Aktionen erstellt werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Push-Android-Aktivität"
>abstract="Die Push-Android-Aktivität vereinheitlicht den Versandprozess für Android-Push-Benachrichtigungen im Rahmen Ihres Workflows. Sie ermöglicht den Versand sowohl einmaliger als auch wiederkehrender Nachrichten und automatisiert so den Versand von Android-Push-Benachrichtigungen an eine vordefinierte Zielgruppe innerhalb desselben Workflows. Sie können Kanalaktivitäten in der Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Trigger-Aktionen erstellt werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Briefpost-Aktivität"
>abstract="Die Briefpost-Aktivität erleichtert den Briefpostversand innerhalb Ihres Workflows und ermöglicht sowohl einmalige als auch wiederkehrende Nachrichten. Es automatisiert den Prozess der Generierung der Extraktionsdatei, die von Briefpostanbietern benötigt wird. Sie können Kanalaktivitäten in der Workflow-Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf Kundenverhalten und Daten Trigger-Aktionen erstellt werden."

Gehen Sie wie folgt vor, um einen Versand im Kontext eines Workflows einzurichten:

1. Fügen Sie eine Kanalaktivität hinzu: **[!UICONTROL E]**, **[!UICONTROL SMS]**, **[!UICONTROL Push-Benachrichtigung (Android)]**, **[!UICONTROL Push-Benachrichtigung (iOS)]** oder **[!UICONTROL Briefpost]**.

1. Wählen Sie den **Versandtyp** aus: einmalig oder wiederkehrend.

   * Ein **Einzelversand** ist ein einmaliger Versand, der nur einmal gesendet wird, z. B. eine Black Friday-E-Mail.
   * Ein **Wiederkehrender Versand** wird entsprechend der Ausführungshäufigkeit, die in der Aktivität [Planung](scheduler.md) definiert ist, mehrfach verschickt. Bei jeder Ausführung des Workflows wird die Zielgruppe neu berechnet, und der Versand wird mit den aktualisierten Inhalten an die aktualisierte Zielgruppe gesendet. Dabei kann es sich etwa um einen wöchentlichen Newsletter oder eine wiederkehrende Geburtstags-E-Mail handeln.

1. Wählen Sie eine **Versandvorlage** aus. Vorlagen sind vorkonfigurierte Versandeinstellungen, die speziell für einen Kanal gelten. Für jeden Kanal ist eine integrierte Vorlage verfügbar, die standardmäßig vorausgefüllt ist. [Weitere Informationen](../../msg/delivery-template.md)

   ![Screenshot der Versandaktivität in einem Workflow](../assets/delivery-activity-in-wf.png)

   Wählen Sie die Vorlage aus dem linken Bereich Konfiguration der Kanalaktivität aus. Wenn die zuvor ausgewählte Zielgruppe nicht mit dem Kanal kompatibel ist, können Sie keine Vorlage auswählen. Um dies zu beheben, aktualisieren Sie die Aktivität **Zielgruppe erstellen**, um eine Zielgruppe mit dem richtigen Zielgruppen-Mapping auszuwählen. Weitere Informationen über Zielgruppen-Mapping finden Sie in [diesem Abschnitt](../../audience/targeting-dimensions.md).

1. Klicken Sie auf **Versand erstellen**. Definieren Sie Ihre Nachrichteneinstellungen und den Inhalt so wie einen eigenständigen Versand. Testen und simulieren Sie den Inhalt. [Weitere Informationen](../../msg/gs-messages.md)

1. Navigieren Sie zurück zu Ihrem Workflow. Um Ihren Workflow fortzusetzen, aktivieren Sie die Option **Ausgehende Transition erzeugen**, um nach der Kanalaktivität eine Transition hinzuzufügen.

1. Klicken Sie auf **Starten**, um Ihren Workflow zu starten.

   Trigger Standardmäßig erfolgt beim Starten eines Workflows die Vorbereitung der Nachricht, ohne dass die Nachricht sofort gesendet wird.

1. Öffnen Sie die Kanalaktivität, um den Versand über die Schaltfläche **Überprüfen und senden** zu bestätigen.

1. Klicken Sie im Versand-Dashboard auf **Senden**.

## Beispiele {#cross-channel-workflow-sample}

Im Folgenden finden Sie ein Beispiel für einen Cross-Channel-Workflow mit Segmentierung und zwei Sendungen. Der Workflow richtet sich an alle Kunden, die in Paris leben und an Kaffeemaschinen interessiert sind. In dieser Population wird eine E-Mail an Standardkunden und eine SMS an VIP-Kunden gesendet.

![Screenshot mit einem Beispiel für einen Cross-Channel-Workflow](../assets/workflow-channel-example.png)

Sie können auch einen wiederkehrenden Workflow erstellen, um jeden ersten Tag des Monats um 20 Uhr eine personalisierte SMS an alle in Paris lebenden Kundinnen und Kunden zu senden.

![Screenshot mit einem Beispiel für einen wiederkehrenden Workflow](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->