---
audience: end-user
title: Verfolgen von Nachrichten
description: Erfahren Sie, wie Sie Links hinzufügen und gesendete Nachrichten verfolgen können.
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: ht
source-wordcount: '607'
ht-degree: 100%

---

# Hinzufügen von Links und Verfolgen von Nachrichten {#tracking}

Verwenden Sie den E-Mail-Designer, um Links zu Ihrem Inhalt hinzuzufügen und die gesendeten Nachrichten zu verfolgen und so das Verhalten Ihrer Empfängerinnen und Empfänger überwachen zu können.

## Einfügen von Links {#insert-links}

Beim Erstellen einer Nachricht können Sie Links zu Ihrem Inhalt hinzufügen.

>[!NOTE]
>
>Wenn das Tracking aktiviert ist, werden alle im Nachrichteninhalt enthaltenen Links verfolgt.

Gehen Sie wie folgt vor, um Links in Ihren E-Mail-Inhalt einzufügen:

1. Wählen Sie ein Element aus und klicken Sie in der kontextuellen Symbolleiste auf **[!UICONTROL Link einfügen]**.

1. Wählen Sie den gewünschten Link-Typ aus.

   ![Screenshot der Benutzeroberfläche zum Einfügen von Links im Nachrichten-Tracking-Tool](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL Externer Link]**: Fügen Sie einen Link zu einer externen URL ein.

     >[!AVAILABILITY]
     >
     >Die folgenden Funktionen (Link zu **[!UICONTROL Landingpage]**, **[!UICONTROL Anmelde-Link]** und **[!UICONTROL Abmelde-Link]**) sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.

   * **[!UICONTROL Landingpage]**: Fügen Sie einen Link zu einer Landingpage ein. Wenn Sie eine dynamische Landingpage auswählen (und die Option **[!UICONTROL Dienst über URL]** ausgewählt ist), können Sie einen beliebigen Dienst aus der Liste auswählen. [Weitere Informationen](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![Screenshot der Benutzeroberfläche zum Verknüpfen mit einer Landingpage im E-Mail-Designer](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL Anmelde-Link]**: Fügen Sie einen Link zu einem Anmelde-Dienst ein.  Wenn Benutzende auf den Link klicken, werden sie zur Abonnement-Landingpage weitergeleitet, auf die im ausgewählten Dienst verwiesen wird. [Weitere Informationen](../audience/manage-services.md#create-service)

     ![Screenshot der Benutzeroberfläche zum Erstellen eines standardmäßigen Abonnement-Links im Dienst-Tool](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL Abmelde-Link]**: Fügen Sie einen Link zu einem Abmelde-Dienst ein.  Wenn Abonnentinnen und Abonnenten auf den Link klicken, werden sie zur Abmeldungs-Landingpage weitergeleitet, auf die im ausgewählten Dienst verwiesen wird. [Weitere Informationen](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Geben Sie die gewünschte URL in das entsprechende Feld ein oder wählen Sie eine Landingpage oder einen Dienst aus und definieren Sie die Link-Einstellungen und -Stile.

1. Fügen Sie eine **[!UICONTROL Bezeichnung]** und einen **[!UICONTROL Link]** hinzu.

1. Speichern Sie Ihre Änderungen.

1. Nachdem Sie den Link erstellt haben, ändern Sie ihn bei Bedarf auf der Registerkarte **[!UICONTROL Einstellungen]**.

   * Bearbeiten Sie den Link und ändern Sie seine **[!UICONTROL Zielgruppe]**.
   * Wählen Sie, ob der Link unterstrichen werden soll, indem Sie die entsprechende Option aktivieren.

   ![Screenshot der Benutzeroberfläche mit den Einstellungen zum Ändern von Link-Eigenschaften im Nachrichten-Tracking-Tool](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>E-Mail-Nachrichten vom Typ Marketing müssen einen Ausschluss-Link enthalten, was für Transaktionsnachrichten nicht erforderlich ist. Die Kategorie der Nachricht (**[!UICONTROL Marketing]** oder **[!UICONTROL Transaktion]**) wird auf Ebene der Kanaloberfläche und beim Erstellen der Nachricht definiert.

Schließen Sie in allen Ihren E-Mail-Nachrichten einen spezifischen Link zur Mirrorseite ein. Weitere Informationen zur Mirrorseite finden Sie in [diesem Abschnitt](mirror-page.md).

## Verwalten von Tracking {#manage-tracking}

Der [E-Mail-Designer](create-email-content.md) ermöglicht Ihnen die Verwaltung verfolgter URLs, z. B. die Bearbeitung des Tracking-Typs für jeden Link.

1. Klicken Sie im linken Bereich auf das Symbol **[!UICONTROL Links]**, um die Liste aller URLs in Ihren zu verfolgenden Inhalten anzuzeigen.

   Diese Liste bietet einen guten Überblick und ermöglicht das Auffinden aller im E-Mail-Inhalt vorhandenen URLs. 

1. Um einen Link zu bearbeiten, wählen Sie das entsprechende Stiftsymbol aus.

   ![Screenshot der Benutzeroberfläche zum Bearbeiten von Links im Nachrichten-Tracking-Tool](assets/message-tracking-edit-links.png){zoomable="yes"}

1. Ändern Sie den **[!UICONTROL Tracking-Typ]** bei Bedarf:

   ![Screenshot der Benutzeroberfläche zum Bearbeiten von Tracking-Typen im Nachrichten-Tracking-Tool](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   Wählen Sie für jede verfolgte URL einen der folgenden Werte für den Tracking-Modus aus:

   * **[!UICONTROL Getrackt]**: Aktiviert das Tracking für diese URL.
   * **[!UICONTROL Opt-out]**: Markiert diese URL als Opt-out- oder Abmelde-URL.
   * **[!UICONTROL Mirrorseite]**: Markiert diese URL als URL der Mirrorseite.
   * **[!UICONTROL Nie]**: Verhindert das Tracking dieser URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Fügen Sie Ihrem Link eine **[!UICONTROL Kategorie]** hinzu, um verfolgte Links zu gruppieren, und klicken Sie dann auf **[!UICONTROL Speichern]**.

   ![Screenshot der Oberfläche zum Hinzufügen von Kategorien zu verfolgten Links im Nachrichten-Tracking-Tool](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. Öffnen Sie nach dem Versand den Versandbericht. Unter dem Menü **[!UICONTROL Tracking]** zeigt der Bericht **[!UICONTROL URLs und Clickstreams]** an, welche URLs aus Ihrem Versand am häufigsten besucht werden. [Weitere Informationen](../reporting/gs-reports.md)