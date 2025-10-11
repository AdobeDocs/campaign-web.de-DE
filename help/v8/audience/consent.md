---
audience: end-user
title: Einverständnis
description: Informationen zum Einverständnis in Campaign Web
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 100%

---

# Einverständnisverwaltung {#manage-consent}

## Allgemeine Empfehlungen {#general-recommendations}

Mit Adobe Campaign können Sie Daten, einschließlich personenbezogener und vertraulicher Daten, erfassen. Es ist wichtig, dass Sie das Einverständnis Ihrer Empfängerinnen und Empfänger gemäß den Datenschutzbestimmungen wie der DSGVO (Datenschutz-Grundverordnung) und anderen geltenden Datenschutzgesetzen einholen und überwachen.

* Senden Sie vor allem keine unerwünschten E-Mails, Push-Benachrichtigungen und SMS-Nachrichten („Spam“). Adobe steht fest hinter den Grundsätzen des Permission Marketing, um den Kundenlebenszeitwert und die Treue zu fördern. Adobe verbietet daher strikt die Verwendung von Adobe Campaign zum Versenden von unerbetenen Nachrichten. [Weitere Informationen](#denylisted-profiles)

* Stellen Sie stets sicher, dass Empfängerinnen und Empfänger dem Empfang von Nachrichten zustimmen, indem Sie ihnen die Möglichkeit geben, sich von Ihren Sendungen abzumelden<!-- and keep honoring opt-out requests as quickly as possible-->. [Weitere Informationen](#opt-out)

* Verwenden Sie die Abonnementverwaltung, um die Voreinstellungen Ihrer Empfängerinnen und Empfänger zu verwalten und nachzuverfolgen, welche von ihnen sich für welche Art von Abonnements entschieden haben. [Weitere Informationen](../../delivery/using/about-services-and-subscriptions.md)

## Verwalten des Opt-out {#opt-out}

Es ist gesetzlich vorgeschrieben, Empfängerinnen und Empfängern die Möglichkeit zu geben, sich vom Erhalt von Nachrichten einer Marke abzumelden. Außerdem muss sichergestellt werden, dass diese Entscheidung respektiert wird. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html?lang=de#privacy-regulations){target="_blank"}.-->

**Warum ist das wichtig?**

* Die Nichteinhaltung dieser Vorschriften führt zu rechtlichen Risiken für Ihre Marke.
* Auf diese Weise können Sie vermeiden, unerwünschte Nachrichten an Ihre Empfängerinnen und Empfänger zu senden, wodurch diese Ihre Nachrichten als Spam markieren und Ihrem Ruf schaden könnten.

Stellen Sie beim Versand von Sendungen mit Adobe Campaign Web stets sicher, dass sich Kundinnen und Kunden von künftigen Nachrichten abmelden können.  Nach der Kündigung des Abos werden die Profile automatisch aus der Zielgruppe künftiger Marketing-Nachrichten entfernt.

### E-Mail-Opt-out {#email-opt-out}

Damit sich Empfängerinnen und Empfänger vom Erhalt von E-Mail-Nachrichten abmelden können, muss jede E-Mail, die an sie gesendet wird, einen **Abmelde-Link** enthalten. 

Führen Sie folgende Schritte aus:

1. Erstellen Sie eine externe Landingpage und hosten Sie sie auf dem Drittanbietersystem Ihrer Wahl.

1. Erstellen Sie einen E-Mail-Versand.  [Weitere Informationen dazu](../email/create-email.md)

1. Fügen Sie einen Link in Ihren E-Mail-Inhalt ein. [Weitere Informationen](../email/message-tracking.md#insert-links)

   ![Link in E-Mail-Inhalt einfügen](../email/assets/message-tracking-insert-link.png)

1. Fügen Sie den Link zu Ihrer Drittanbieter-Landingpage im Feld **[!UICONTROL URL]** ein.

1. Klicken Sie auf das Symbol **[!UICONTROL Links]** im linken Bereich, um die Liste aller URLs Ihrer zu trackenden Inhalte anzuzeigen.

1. Klicken Sie auf das Stiftsymbol neben dem neuen Link, um ihn zu bearbeiten.

1. Ändern Sie den **[!UICONTROL Tracking-Typ]** und setzen Sie ihn auf **[!UICONTROL Opt-out]**.

   ![Tracking-Typ für Opt-out bearbeiten](../email/assets/message-tracking-edit-a-link.png)

1. Klicken Sie auf **[!UICONTROL Speichern]** und senden Sie die Nachricht ab. [Weitere Informationen](../monitor/prepare-send.md)

1. Wenn die Empfängerin bzw. der Empfänger nach Erhalt der Nachricht auf den Abmelde-Link klickt, wird die Landingpage angezeigt.

1. Wenn die Empfängerin bzw. der Empfänger das Landingpage-Formular sendet, werden die Profildaten aktualisiert. [Weitere Informationen](#denylisted-profiles)

<!--Any other option available such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Profile, die auf die Blockierungsliste gesetzt wurden {#denylisted-profiles}

Nach einer Abmeldung (Opt-out) werden die Profile der **Blockierungsliste** für einen bestimmten Kanal hinzugefügt. Dies bedeutet, dass sie von keinem Versand mehr als Zielgruppe ausgewählt werden.

>[!NOTE]
>
>Wenn ein Profil, das auf der Blockierungsliste für den E-Mail-Kanal steht, zwei E-Mail-Adressen hat, werden beide Adressen vom Versand ausgeschlossen.

Im Abschnitt **[!UICONTROL Nicht mehr kontaktieren]** auf der Registerkarte **[!UICONTROL Details]** des Profils können Sie überprüfen, ob sich ein Profil für einen oder mehrere Kanäle auf der Blockierungsliste befindet. [Weitere Informationen](../audience/about-recipients.md#access)

![Überprüfen des Status der Blockierungsliste in den Profildetails](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html?lang=de#feedback-loops){target="_blank"}.

Learn more about quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=de#non-deliverable-bounces){target="_blank"}.-->