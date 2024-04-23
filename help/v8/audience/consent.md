---
audience: end-user
title: Einverständnis
description: Informationen zur Einwilligung im Adobe Campaign Web
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 9a184d7558ca39be3afed4a7217a5e5687799c0d
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%

---

# Einverständnisverwaltung {#manage-consent}

## Allgemeine Empfehlungen {#general-recommendations}

Mit Adobe Campaign können Sie Daten, einschließlich personenbezogener und vertraulicher Daten, erfassen. Daher ist es wichtig, dass Sie die Zustimmung Ihrer Empfänger gemäß den Datenschutzbestimmungen wie der DSGVO (Datenschutz-Grundverordnung) und anderen geltenden Datenschutzgesetzen einholen und überwachen.

* Senden Sie zunächst keine unerwünschten E-Mails, Push-Benachrichtigungen und SMS-Nachrichten (&quot;Spam&quot;). Adobe glaubt fest an die Prinzipien des Permission Marketing, um den Lebenszeitwert und die Treue von Kunden zu fördern, und verbietet daher strikt die Verwendung von Adobe Campaign zum Versand unerwünschter Nachrichten. [Weitere Informationen](#denylisted-profiles)

* Lassen Sie Empfänger immer dem Empfang von Nachrichten zustimmen, indem Sie ihnen die Möglichkeit geben, sich von Ihren Sendungen abzumelden.<!-- and keep honoring opt-out requests as quickly as possible-->. [Weitere Informationen](#opt-out)

* Mithilfe der Abonnementverwaltung können Sie die Voreinstellungen Ihrer Empfänger verwalten und verfolgen, welche Empfänger sich für welche Art von Abonnements entschieden haben. [Weitere Informationen](../../delivery/using/about-services-and-subscriptions.md)

## Opt-out verwalten {#opt-out}

Es ist gesetzlich vorgeschrieben, den Empfängern die Möglichkeit zu geben, sich vom Erhalt von Nachrichten einer Marke abzumelden, und sicherzustellen, dass diese Entscheidung respektiert wird. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Warum ist es wichtig?**

* Die Nichteinhaltung dieser Vorschriften führt zu rechtlichen Risiken für Ihre Marke.
* Auf diese Weise können Sie vermeiden, unerwünschte Nachrichten an Ihre Empfänger zu senden, wodurch diese Ihre Nachrichten als Spam markieren und Ihrer Reputation schaden könnten.

Beim Versand von Nachrichten über Adobe Campaign Web müssen Sie stets sicherstellen, dass sich Kunden von künftigen Nachrichten abmelden können. Nach der Abmeldung werden die Profile automatisch aus der Audience künftiger Marketing-Nachrichten entfernt.

### E-Mail-Opt-out {#email-opt-out}

Um Empfängern die Möglichkeit zu geben, sich vom Erhalt von E-Mail-Nachrichten abzumelden, müssen Sie stets eine **Abmelde-Link** in jeder E-Mail, die an Empfänger gesendet wird.

Gehen Sie dazu wie folgt vor:

1. Erstellen Sie eine externe Landingpage und hosten Sie sie auf dem Drittanbietersystem Ihrer Wahl.

1. Erstellen Sie einen E-Mail-Versand. [Weitere Informationen dazu](../email/create-email.md)

1. Fügen Sie einen Link zu Ihrem E-Mail-Inhalt ein. [Weitere Informationen dazu](../email/message-tracking.md#insert-links)

   ![](../email/assets/message-tracking-insert-link.png)

1. Im **[!UICONTROL URL]** den Link zu Ihrer Drittanbieter-Landingpage einfügen.

1. Klicken Sie auf das Symbol **[!UICONTROL Links]** im linken Fensterbereich, um die Liste aller URLs Ihrer zu trackenden Inhalte anzuzeigen.

1. Klicken Sie auf das Stiftsymbol neben dem neuen Link, um ihn zu bearbeiten.

1. Ändern Sie die **[!UICONTROL Tracking-Typ]** und legen Sie **[!UICONTROL Opt-out]**.

   ![](../email/assets/message-tracking-edit-a-link.png)

1. Klicks **[!UICONTROL Speichern]** und senden Sie die Nachricht. [Weitere Informationen](../monitor/prepare-send.md)

1. Wenn der Empfänger nach Erhalt der Nachricht auf den Abmelde-Link klickt, wird Ihre Landingpage angezeigt.

1. Wenn der Empfänger das Landingpage-Formular sendet, werden die Profildaten aktualisiert. [Weitere Informationen](#denylisted-profiles)

<!--Any other option availabe such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Auf die Blockierungsliste gesetzt Profile {#denylisted-profiles}

Nach einer Abmeldung (Opt-out) befinden sich die Profile im **Blockierungsliste** für einen bestimmten Kanal: Dies bedeutet, dass er von keinem Versand mehr als Zielgruppe ausgewählt wird.

>[!NOTE]
>
>Wenn ein Profil auf der Blockierungsliste für den E-Mail-Kanal zwei E-Mail-Adressen hat, werden beide Adressen vom Versand ausgeschlossen.

Sie können für einen oder mehrere Kanäle in der **[!UICONTROL No longer contact]** des Profils **[!UICONTROL Details]** Registerkarte. [Weitere Informationen](../audience/about-recipients.md#access)

![](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->



