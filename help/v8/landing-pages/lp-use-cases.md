---
solution: Journey Optimizer
product: journey optimizer
title: Landingpage – Anwendungsfälle
description: Erkunden Sie die häufigsten Anwendungsfälle für Landingpages in Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: Landing, Landingpage, Anwendungsfall
exl-id: 8c00d783-54a3-45d9-bd8f-4dc58804d922
source-git-commit: 601cc62c5640069ce9e6ee4830f924c610e0915f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 30%

---

# Landingpage verwenden {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="URL mit Vorsicht kopieren"
>abstract="Um Ihre Landingpage vollständig zu testen oder zu nutzen, können Sie diesen Link nicht direkt in einen Webbrowser oder in Ihre Sendungen kopieren und einfügen. Verwenden Sie stattdessen die **Inhalt simulieren** , um sie zu testen, und führen Sie die in der Dokumentation beschriebenen Schritte aus, um Ihre Landingpage ordnungsgemäß zu nutzen."

Um Ihre Landingpage richtig zu nutzen, sollten Sie sie als Link in einem Versand mit der entsprechenden Option referenzieren.

>[!CAUTION]
>
>Um Ihre Landingpage vollständig zu nutzen, können Sie den im Dashboard des veröffentlichten Versands angezeigten Link nicht direkt in Ihre Sendungen oder auf eine Webseite kopieren und einfügen.

Im [!DNL Adobe Campaign Web] In der Benutzeroberfläche stehen Ihnen vier vordefinierte Vorlagen zur Verfügung, mit denen Sie verschiedene Anwendungsfälle implementieren können. Die wichtigsten Schritte bleiben jedoch gleich und werden im Folgenden beschrieben.

1. [Landingpage erstellen](create-lp.md#create-landing-page) und wählen Sie je nach Anwendungsfall die gewünschte Vorlage aus:

   * [Akquise](#lp-acquisition)
   * [Anmeldung](#lp-subscription)
   * [Abmeldung](#lp-unsubscription)
   * [Blockierungsliste](#lp-denylist)

1. Definieren Sie die Eigenschaften und Einstellungen der Landingpage.

   ![](assets/lp-uc-properties.png)

1. Wählen Sie je nach Fall die **[!UICONTROL Akquise]**, **[!UICONTROL Abonnement]**, **[!UICONTROL Abmeldung]** oder **[!UICONTROL Blockierungsliste]** Seite.

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den dem Landingpage-Formular entsprechenden Teil aus.

   ![](assets/lp-uc-form.png)

1. Nehmen Sie bei Bedarf weitere Änderungen an den Landingpage-Bezeichnungen und -Feldern vor. Bearbeiten Sie den Rest Ihres Inhalts nach Bedarf, speichern Sie Ihre Änderungen und schließen Sie sie.

1. Gehen Sie für jeden Anwendungsfall wie folgt vor:

1. Bearbeiten Sie die **[!UICONTROL Bestätigung]** sowie die **[!UICONTROL Fehler]** und **[!UICONTROL Ablauf]** Seiten. Sie wird Ihren Empfängern angezeigt, sobald sie das Registrierungsformular einreichen.

   ![](assets/lp-uc-confirmation-page.png)

1. Testen und [publish](create-lp.md#publish-landing-page) Ihre Landingpage.

1. Erstellen Sie eine [email](../email/create-email.md) -Versand, um den Traffic zur Landingpage zu lenken.

1. [Fügen Sie einen Link](../email/message-tracking.md#insert-links) in Ihren Nachrichteninhalt ein. Auswählen **[!UICONTROL Landingpage]** als **[!UICONTROL Link-Typ]** und wählen Sie [Landingpage](create-lp.md#configure-primary-page) die Sie erstellt haben.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Um Ihre Nachricht senden zu können, darf die ausgewählte Landingpage noch nicht abgelaufen sein. [In diesem Abschnitt](create-lp.md#create-landing-page) erfahren Sie, wie Sie das Ablaufdatum aktualisieren können.

Wenn Ihre Empfänger nach dem Erhalt der E-Mail auf den Link zur Landingpage klicken und das Landingpage-Formular übermitteln, werden sie zur Bestätigungsseite weitergeleitet und jede andere auf der Landingpage definierte Aktion wird angewendet (z. B. werden die Benutzer bei Ihrem Dienst angemeldet oder erhalten von Ihnen keine Nachrichten mehr).

Im Folgenden finden Sie einige Beispiele für die Verwendung von Landingpages in [!DNL Adobe Campaign], damit sich Ihre Kundinnen und Kunden für den Empfang bestimmter oder aller Ihrer Nachrichten an- bzw. abmelden können.

## Profilakquise {#lp-acquisition}

1. [Landingpage erstellen](create-lp.md#create-landing-page). Wählen Sie die **[!UICONTROL Akquise]** Vorlage.

1. Definieren Sie die Eigenschaften und Einstellungen der Landingpage.

   ![](assets/lp-uc-properties.png)

1. Wählen Sie die **[!UICONTROL Akquise]** Seite, um den Inhalt zu bearbeiten.

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den dem Landingpage-Formular entsprechenden Teil aus.

## Abonnement für einen Dienst {#lp-subscription}

Einer der häufigsten Anwendungsfälle besteht darin, über eine Landingpage Ihre Kundinnen und Kunden einzuladen, einen [Dienst zu abonnieren](../audience/manage-services.md) (z. B. einen Newsletter oder eine Veranstaltung). Gehen Sie dazu wie folgt vor.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Erstellen Sie zunächst eine Bestätigungsvorlage für Benutzer, die Ihr Ereignis abonnieren, damit Sie diese bei der Erstellung des Dienstes einfach auswählen können. [Weitere Informationen](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. Erstellen Sie einen Anmeldedienst, der die registrierten Benutzer für Ihr Ereignis speichert. [Erfahren Sie, wie Sie einen Dienst erstellen](../audience/manage-services.md)

1. Wählen Sie die Vorlage aus, die Sie als Bestätigungs-E-Mail erstellt haben, die die Benutzer beim Abonnieren erhalten.

   ![](assets/lp-uc-subscription-service.png)

1. [Landingpage erstellen](create-lp.md#create-landing-page) , damit sich Ihre Empfänger für Ihr Ereignis registrieren können. Wählen Sie die **[!UICONTROL Abonnement]** Vorlage.

   <!--![](assets/lp-uc-subscription-template.png)-->

1. Definieren Sie die Eigenschaften und Einstellungen der Landingpage.

   <!--![](assets/lp-uc-properties.png)-->

1. Wählen Sie die **[!UICONTROL Abonnement]** Seite, um den Inhalt zu bearbeiten.

   ![](assets/lp-uc-subscription-page-edit.png)

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den dem Landingpage-Formular entsprechenden Teil aus und erweitern Sie die **[!UICONTROL Kontrollkästchen 1]** Abschnitt.

   Im **[!UICONTROL Abonnements und Dienste]** auswählen, wählen Sie den Dienst aus, den Sie für Ihr Ereignis erstellt haben. Lassen Sie die **[!UICONTROL Abonnieren, wenn aktiviert]** aktiviert ist.

   ![](assets/lp-uc-subscription-checkbox-1.png)

1. Sie können ein zusätzliches Kontrollkästchen hinzufügen, um beispielsweise ein Abonnement für Ihren Newsletter anzubieten.

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. Nehmen Sie bei Bedarf weitere Änderungen an den Landingpage-Bezeichnungen und -Feldern vor. Bearbeiten Sie den Rest Ihres Inhalts nach Bedarf, speichern Sie Ihre Änderungen und schließen Sie sie.

1. Bearbeiten Sie die **[!UICONTROL Bestätigung]** sowie die **[!UICONTROL Fehler]** und **[!UICONTROL Ablauf]** Seiten. Sie wird Ihren Empfängern angezeigt, sobald sie das Registrierungsformular einreichen.

   ![](assets/lp-uc-confirmation-page.png)

1. Testen und [publish](create-lp.md#publish-landing-page) Ihre Landingpage.

1. Erstellen Sie eine **Email** -Versand, um den Traffic zur Anmelde-Landingpage zu leiten. Gestalten Sie die E-Mail so, dass die Registrierung jetzt für Ihr Ereignis geöffnet ist.

1. [Fügen Sie einen Link](../email/message-tracking.md#insert-links) in Ihren Nachrichteninhalt ein. Wählen Sie **[!UICONTROL Landingpage]** als **[!UICONTROL Link-Typ]** aus und wählen Sie die [Landingpage](create-lp.md#configure-primary-page) aus, die Sie für die Registrierung erstellt haben.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Um Ihre Nachricht senden zu können, darf die ausgewählte Landingpage noch nicht abgelaufen sein. [In diesem Abschnitt](create-lp.md#create-landing-page) erfahren Sie, wie Sie das Ablaufdatum aktualisieren können.

Wenn Ihre Empfänger nach dem Erhalt der E-Mail auf den Link zur Landingpage klicken und das Landingpage-Formular übermitteln, werden sie zur Bestätigungsseite weitergeleitet und auf die Abonnementliste gesetzt.

## Abmeldung {#lp-unsubscription}

1. [Landingpage erstellen](create-lp.md#create-landing-page). Wählen Sie die **[!UICONTROL Abmeldung]** Vorlage.

1. Definieren Sie die Eigenschaften und Einstellungen der Landingpage.

1. Wählen Sie die **[!UICONTROL Abmeldung]** Seite, um den Inhalt zu bearbeiten.

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den dem Landingpage-Formular entsprechenden Teil aus.

## Opt-out-Landingpages einrichten {#lp-denylist}

Es ist gesetzlich vorgeschrieben, Empfängerinnen und Empfängern die Möglichkeit zu geben, sich vom Erhalt von Nachrichten einer Marke abzumelden. Weitere Informationen zu den geltenden Rechtsvorschriften finden Sie in der [Experience Platform-Dokumentation](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html?lang=de#regulations){target="_blank"}.

Daher müssen Sie immer einen **Abmelde-Link** in jede an Empfängerinnen und Empfänger gesendete E-Mail aufnehmen:

* Durch Klicken auf diesen Link werden die Empfängerinnen und Empfänger zu einer Landingpage weitergeleitet, die eine Schaltfläche enthält, über die sich die Abbestellung bestätigen lässt.
* Wenn jemand auf die Schaltfläche zum Abbestellen klickt, werden die Profildaten mit diesen Informationen aktualisiert.

Sie können eine **[!UICONTROL Blockierungsliste]** Landingpage, über die sich Benutzer von allen Sendungen abmelden können.

Damit Benutzer sich von allen Sendungen abmelden können, müssen Sie eine **[!UICONTROL Blockierungsliste]** Landingpage.

Sobald ein Empfänger den Link in der Landingpage auswählt, wird automatisch die Option **[!UICONTROL Nicht mehr kontaktieren (alle Kanäle)]** im Profil des Empfängers aktiviert.

![](assets/blocklisting_allchannels.png)

definieren **[!UICONTROL Opt-out]** und wählen Sie die Option **[!UICONTROL Kanal (E-Mail)]**: Das Profil, das das Opt-out-Feld auf Ihrer Landingpage aktiviert, wird von all Ihrer Kommunikation ausgeschlossen.

Wenn Empfängerinnen und Empfänger nach Erhalt der Nachricht auf den Abbestellungs-Link in der E-Mail klicken, wird Ihre Landingpage angezeigt.

![](assets/lp_opt-out-submit-form.png)

Wenn Empfängerinnen und Empfänger das Kästchen aktivieren und das Formular senden:

* Die abgemeldeten Empfängerinnen und Empfänger werden zum Bestätigungsbildschirm weitergeleitet.

* Die Profildaten werden aktualisiert und sie erhalten keine Nachrichten mehr von Ihrer Marke, es sei denn, sie melden sich erneut an.

Um zu überprüfen, ob die Auswahl des entsprechenden Profils aktualisiert wurde, gehen Sie zu Profile und wählen Sie das Profil aus.







