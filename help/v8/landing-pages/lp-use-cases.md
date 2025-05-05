---
solution: Campaign, Campaign v8 Web User Interface
title: Landingpage – Anwendungsfälle
description: Informationen zu den häufigsten Anwendungsfällen für Landingpages in der Campaign Web-Benutzeroberfläche
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: Landing, Landingpage, Anwendungsfall
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: a9ce4fd103c4af8f47ba887031e8d6d53e8d5f0b
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 66%

---

# Verwenden einer Landingpage {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Vorsicht beim Kopieren der URL"
>abstract="Sie können diesen Link nicht direkt in einen Webbrowser oder in Ihre Sendungen kopieren und einfügen, um Ihre Landingpage vollständig zu testen oder zu nutzen. Verwenden Sie stattdessen die Funktion **Inhalt simulieren**, um sie zu testen, und führen Sie die in der Dokumentation beschriebenen Schritte aus, um Ihre Landingpage richtig zu nutzen."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="Vorsicht beim Kopieren der URL"
>abstract="Bei der Erstellung einer Landingpage können Sie mit vier nativen Vorlagen verschiedene Anwendungsfälle implementieren: Hinzufügen oder Aktualisieren eines Profils zur Campaign-Datenbank, Abonnieren eines Dienstes, Abmelden von einem Dienst oder Abmelden von Benutzenden."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?lang=de#create-landing-page" text="Erstellen einer Landingpage"

Um Ihre Landingpage ordnungsgemäß zu verwenden, referenzieren Sie sie mithilfe der entsprechenden Option als Link in einer Nachricht. Sie können den im Dashboard des veröffentlichten Versands angezeigten Link nicht direkt in Ihre Sendungen kopieren oder auf eine Web-Seite einfügen. Verwenden Sie stattdessen die Funktion **Inhalt simulieren**, um ihn zu testen.

In der [!DNL Adobe Campaign Web] können Sie mit vier vordefinierten Vorlagen verschiedene Anwendungsfälle implementieren. Die wichtigsten Schritte sind jedoch identisch und werden im Folgenden beschrieben.

1. [Erstellen Sie eine Landingpage](create-lp.md#create-landing-page) und wählen Sie je nach Anwendungsfall die gewünschte Vorlage aus.

1. Definieren der Eigenschaften und Einstellungen der Landingpage

   ![Screenshot mit den Eigenschaften und Einstellungen der Landingpage.](assets/lp-uc-properties.png){zoomable="yes"}

1. Auf die Blockierungsliste setzen Wählen Sie je nach Fall die Seite **[!UICONTROL Akquise]**, **[!UICONTROL Abonnement]**, **[!UICONTROL Abmeldung]** oder **&#x200B;**&#x200B;aus.

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den dem Landingpage-Formular entsprechenden Teil aus.

   ![Screenshot der Formularschnittstelle für Landingpages.](assets/lp-uc-form.png){zoomable="yes"}

1. Bearbeiten Sie den Inhalt entsprechend der ausgewählten Vorlage:

   * [Akquise](#lp-acquisition)
   * [Anmeldung](#lp-subscription)
   * [Abmeldung](#lp-unsubscription)
   * [Blockierungsliste](#lp-denylist)

1. Ändern Sie den Rest Ihres Inhalts nach Bedarf, speichern Sie Ihre Änderungen und schließen Sie ihn.

1. Bearbeiten Sie nach Bedarf die Seite **[!UICONTROL Bestätigung]** sowie die Seiten **[!UICONTROL Fehler]** und **[!UICONTROL Ablauf]**. Die Seite **[!UICONTROL Bestätigung]** wird Ihren Empfängerinnen und Empfängern angezeigt, sobald sie das Formular übermitteln.

   ![Screenshot der Benutzeroberfläche der Bestätigungsseite.](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [Testen](create-lp.md#test-landing-page) und [veröffentlichen](create-lp.md#publish-landing-page) Sie Ihre Landingpage.

1. Erstellen Sie einen [E-Mail-Versand](../email/create-email.md), um den Traffic auf die Landingpage zu lenken.

1. [Fügen Sie einen Link](../email/message-tracking.md#insert-links) in Ihren Nachrichteninhalt ein. Wählen Sie **[!UICONTROL Landingpage]** als **[!UICONTROL Link-Typ]** und dann die von Ihnen erstellte Landingpage aus.

   ![Screenshot der Einfügeoberfläche für E-Mail-Links.](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >Um Ihre Nachricht senden zu können, darf die ausgewählte Landingpage noch nicht abgelaufen sein. [Weitere Informationen](create-lp.md#create-landing-page)

Wenn Ihre Empfängerinnen und Empfänger die E-Mail erhalten und auf den Link zur Landingpage klicken und das Formular übermitteln, geschieht Folgendes:

* Sie werden zur Bestätigungsseite weitergeleitet.
* Jede andere Aktion, die auf Ihrer Landingpage definiert ist, wird angewendet. Beispielsweise werden Benutzende für Ihren Dienst angemeldet oder sie erhalten keine weiteren Nachrichten mehr von Ihnen.

Im Folgenden finden Sie einige Beispiele für die Verwendung von [!DNL Adobe Campaign]-Landingpages in den verschiedenen Anwendungsfällen.

## Profilakquise {#lp-acquisition}

Mit der ersten Vorlage können Sie ein Profil zur Campaign-Datenbank hinzufügen oder darin aktualisieren.

1. Wählen Sie beim [Erstellen einer Landingpage](create-lp.md#create-landing-page) die Vorlage **[!UICONTROL Akquise]** aus.

1. Wählen Sie in den Eigenschaften der Landingpage die Option **[!UICONTROL Vorbefüllen mit den im Formular referenzierten Daten]** aus, um alle vorhandenen Informationen aus dem Profil vorab auszufüllen und das Erstellen von Duplikaten zu vermeiden.

1. Wählen Sie die Seite **[!UICONTROL Akquise]** aus, um ihren Inhalt zu bearbeiten.

1. Bearbeiten Sie die Textfelder nach Bedarf entsprechend den Informationen, die zu Ihren Profilen gesammelt werden sollen.

1. Fügen Sie ein Kontrollkästchen hinzu, mit dem Ihre Kunden aufgefordert werden, Ihren Newsletter-Dienst zu abonnieren. [Erfahren Sie, wie Sie einen Dienst erstellen](../audience/manage-services.md)

   ![Screenshot der Oberfläche der Akquise-Seite mit dem Kontrollkästchen für ein Newsletter-Abonnement.](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. Passen Sie den Inhalt nach Bedarf an und speichern Sie Ihre Änderungen.

1. Überprüfen und [veröffentlichen](create-lp.md#publish-landing-page) Sie Ihre Landingpage.

1. Erstellen Sie eine [E-Mail](../email/create-email.md) und fügen Sie einen [Link](../email/message-tracking.md#insert-links) zu Ihrer Landingpage hinzu.

Wenn Ihre Empfänger nach Erhalt der E-Mail auf den Link zur Landingpage klicken und das Formular senden, wird ihr Profil zur Campaign-Datenbank hinzugefügt oder mit den von ihnen bereitgestellten Informationen aktualisiert.

![Screenshot mit einem in der Campaign-Datenbank aktualisierten Profil.](assets/lp-uc-profile-updated.png){zoomable="yes"}

Wenn sie sich für den Erhalt Ihres Newsletters entschieden haben, werden sie für den entsprechenden Dienst angemeldet.

![Screenshot mit einer Newsletter-Anmeldebestätigung.](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## Abonnement für einen Dienst {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Festlegen der Anmelde-Landingpage"
>abstract="Über eine Anmeldeseite können Ihre Kundinnen und Kunden einen Dienst abonnieren."

Einer der häufigsten Anwendungsfälle besteht darin, Ihre Kunden über eine Landingpage zum [Abonnieren eines Services](../audience/manage-services.md) (z. B. eines Newsletters oder einer Veranstaltung) aufzufordern. Gehen Sie dazu wie folgt vor.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Erstellen Sie eine Bestätigungsvorlage für Benutzer, die Ihr Ereignis abonnieren, damit Sie sie beim Erstellen des Service einfach auswählen können. [Weitere Informationen](../audience/manage-services.md#create-confirmation-message)

   ![Screenshot der Oberfläche der E-Mail-Bestätigungsvorlage.](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. Erstellen Sie einen Abonnement-Service, in dem die registrierten Benutzer für Ihre Veranstaltung gespeichert werden. [Erfahren Sie, wie Sie einen Dienst erstellen](../audience/manage-services.md)

1. Wählen Sie die Vorlage aus, die Sie als Bestätigungs-E-Mail erstellt haben und die die Benutzenden beim Abonnieren erhalten sollen.

   ![Screenshot der Benutzeroberfläche des Abonnement-Services.](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [Erstellen Sie eine Landingpage](create-lp.md#create-landing-page), damit sich Ihre Empfängerinnen und Empfänger für Ihr Ereignis registrieren können. Wählen Sie die **[!UICONTROL Abonnement-Vorlage]** aus.

1. Wählen Sie die Seite **[!UICONTROL Abonnement]** aus, um den Inhalt zu bearbeiten.

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den Teil aus, der dem Landingpage-Formular entspricht und erweitern Sie den Abschnitt **[!UICONTROL Kontrollkästchen 1]**.

1. Wählen Sie im Feld **[!UICONTROL Abonnements und Dienste]** den Dienst aus, den Sie für Ihr Ereignis erstellt haben. Lassen Sie die Option **[!UICONTROL Anmelden wenn aktiviert]** aktiviert.

   ![Screenshot der Benutzeroberfläche für das Abonnement-Kontrollkästchen.](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Passen Sie den Inhalt nach Bedarf an und speichern Sie Ihre Änderungen.

1. Überprüfen und [veröffentlichen](create-lp.md#publish-landing-page) Sie Ihre Landingpage.

1. Erstellen Sie eine [E-Mail](../email/create-email.md) und fügen Sie einen [Link](../email/message-tracking.md#insert-links) hinzu, um den Traffic zur Landingpage für die Registrierung zu leiten.

1. Entwerfen Sie eine E-Mail, um anzukündigen, dass die Registrierung für Ihr Ereignis jetzt geöffnet ist.

Wenn Ihre Empfänger nach Erhalt der E-Mail auf den Link zur Landingpage klicken und das Formular senden, werden sie zur Bestätigungsseite weitergeleitet und auf die Abonnement-Liste gesetzt.

## Abmeldung {#lp-unsubscription}

Sie können Ihren Kunden und Kundinnen über eine Landingpage die Möglichkeit geben, sich von einem Dienst abzumelden.

1. Erstellen Sie eine Bestätigungsvorlage für Benutzer, die sich von Ihrem Service abmelden möchten, damit Sie sie bei der Erstellung des Services einfach auswählen können. [Weitere Informationen](../audience/manage-services.md#create-confirmation-message)

1. Wählen Sie im [Abonnement-Dienst](../audience/manage-services.md) die Vorlage aus, die Sie als Bestätigungs-E-Mail erstellt haben, die die Benutzenden bei der Abmeldung erhalten sollen.

1. [Erstellen Sie eine Landingpage](create-lp.md#create-landing-page). Wählen Sie die Vorlage für die **[!UICONTROL Abmeldung]** aus.

1. Wählen Sie die Seite **[!UICONTROL Abmeldung]** aus, um den Inhalt zu bearbeiten.

1. Der Inhalt der Seite wird angezeigt. Wählen Sie den dem Landingpage-Formular entsprechenden Teil aus.

1. Fügen Sie einen Abschnitt **[!UICONTROL Kontrollkästchen]** hinzu, wählen Sie den Service aus und wählen Sie die Option **[!UICONTROL Abmelden, falls aktiviert]** aus.

   ![Screenshot mit der Benutzeroberfläche des Kontrollkästchen für die Abmeldung.](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. Erweitern Sie den Abschnitt **[!UICONTROL Aktionsaufruf]** und wählen Sie die Option **[!UICONTROL Zusätzliche Aktualisierungen]** aus. Wählen Sie den Dienst aus und aktivieren Sie die Option **[!UICONTROL Opt-out]**.

   ![Screenshot der call-to-action-Benutzeroberfläche für die Abmeldung.](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. Passen Sie den Inhalt nach Bedarf an und speichern Sie Ihre Änderungen.

1. Überprüfen und [veröffentlichen](create-lp.md#publish-landing-page) Sie Ihre Landingpage.

1. Erstellen Sie eine [E-Mail](../email/create-email.md) und fügen Sie einen [Link](../email/message-tracking.md#insert-links) zur Landingpage hinzu.

Wenn Ihre Empfänger nach Erhalt der E-Mail auf den Link zur Landingpage klicken und das Formular senden, werden sie zur Bestätigungsseite zur Abmeldung weitergeleitet und vom entsprechenden Abonnement-Service entfernt.

## Blockierungsliste {#lp-denylist}

Es ist gesetzlich vorgeschrieben, Empfängerinnen und Empfängern die Möglichkeit zu geben, sich vom Erhalt von Nachrichten einer Marke abzumelden. Daher müssen Sie immer einen **Abmelde-Link** in jede an Empfängerinnen und Empfänger gesendete E-Mail aufnehmen: Durch Klicken auf diesen Link werden die Empfängerinnen und Empfänger zu einer Landingpage weitergeleitet, die eine Schaltfläche enthält, über die sich die Abbestellung bestätigen lässt.

Sie können auch eine Landingpage vom Typ **[!UICONTROL Blockierungsliste]** einrichten, über die sich Empfängerinnen und Empfänger von allen Sendungen abmelden können.

1. Wählen Sie beim [Erstellen einer Landingpage](create-lp.md#create-landing-page) die Vorlage **[!UICONTROL Blockierungsliste]** aus.

1. Wählen Sie die Seite **[!UICONTROL Blockierungsliste]**, um den Inhalt zu bearbeiten.

1. Erweitern Sie den Abschnitt **[!UICONTROL Aktionsaufruf]** und wählen Sie die Option **[!UICONTROL Zusätzliche Aktualisierungen]** aus.

1. Wählen Sie aus der entsprechenden Dropdown-Liste **[!UICONTROL Kanal (E-Mail)]** aus, damit sich Ihre Empfängerinnen und Empfänger nur von der E-Mail-Kommunikation abmelden können. Sie können auch **[!UICONTROL Nach allen Kanälen]** auswählen, um sie von allen Kommunikationen auf allen Kanälen abzumelden.

   auf die Blockierungsliste setzen ![Screenshot der call-to-action-Benutzeroberfläche.](assets/lp-uc-denylist.png){zoomable="yes"}

1. Passen Sie den Inhalt nach Bedarf an und speichern Sie Ihre Änderungen.

1. Überprüfen und [veröffentlichen](create-lp.md#publish-landing-page) Sie Ihre Landingpage.

1. Erstellen Sie eine [E](../email/create-email.md)Mail[ und fügen Sie einen Link ](../email/message-tracking.md#insert-links) Ihrer Landingpage hinzu, damit Benutzer sich vom Erhalt von Nachrichten abmelden können.

Wenn Ihre Empfängerinnen und Empfänger nach dem Erhalt der E-Mail auf den Link zur Landingpage klicken und das Formular absenden, werden sie zur Bestätigungsseite für die Blockierungsliste weitergeleitet und ihr Profil wird mit den von ihnen angegebenen Informationen aktualisiert.

Um zu überprüfen, ob die Auswahl des entsprechenden Profils aktualisiert wurde, navigieren Sie zum Menü **[!UICONTROL Profile]** und wählen Sie dieses Profil aus.

Wenn Sie beispielsweise die Option **[!UICONTROL Kanal (E-Mail)]** auf Ihrer Landingpage aktualisieren, wird die Option **[!UICONTROL Nicht länger per E-Mail kontaktieren]** aktiviert.

auf die Blockierungsliste setzen ![Screenshot mit einem Profil, das mit den Profilvoreinstellungen aktualisiert wurde.](assets/lp-uc-denylist-profile.png){zoomable="yes"}

Dieses Profil erhält keine E-Mail-Nachrichten mehr von Ihrer Marke, es sei denn, es wird erneut angemeldet.