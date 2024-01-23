---
audience: end-user
title: Verfolgen von Nachrichten
description: Erfahren Sie, wie Sie Links hinzufügen und gesendete Nachrichten verfolgen können.
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: ht
source-wordcount: '367'
ht-degree: 100%

---

# Hinzufügen von Links und Verfolgen von Nachrichten {#tracking}

Verwenden Sie E-Mail-Designer, um Links zu Ihrem Inhalt hinzuzufügen und die gesendeten Nachrichten zu verfolgen, um das Verhalten Ihrer Empfänger zu überwachen.

## Einfügen von Links {#insert-links}

Beim Erstellen einer Nachricht können Sie Links zu Ihrem Inhalt hinzufügen.

>[!NOTE]
>
>Wenn das Tracking aktiviert ist, werden alle im Nachrichteninhalt enthaltenen Links verfolgt.

Gehen Sie wie folgt vor, um Links in Ihren E-Mail-Inhalt einzufügen:

1. Wählen Sie ein Element aus und klicken Sie in der kontextuellen Symbolleiste auf **[!UICONTROL Link einfügen]**.

   ![](assets/message-tracking-insert-link.png)

1. Fügen Sie eine **[!UICONTROL Bezeichnung]** und einen **[!UICONTROL Link]** hinzu.

1. Speichern Sie Ihre Änderungen.

1. Sobald er erstellt wurde, können Sie den Link immer noch über die Registerkarte **[!UICONTROL Einstellungen]** ändern.

   * Sie können den Link bearbeiten und seine **[!UICONTROL Zielgruppe]** ändern.
   * Sie können den Link unterstreichen oder nicht, indem Sie die entsprechende Option auswählen.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>E-Mail-Nachrichten vom Typ Marketing müssen einen Ausschluss-Link enthalten, der für Transaktionsnachrichten nicht erforderlich ist. Die Nachrichten-Kategorie (**[!UICONTROL Marketing]** oder **[!UICONTROL Transaktion]**) wird auf Ebene der Kanal-Benutzeroberfläche (d. h. der Nachrichtenvoreinstellung) und beim Erstellen der Nachricht definiert.

In allen Ihren E-Mail-Nachrichten sollte ein spezifischer Link zur Mirrorseite hinzugefügt werden. Weitere Informationen zur Mirrorseite finden Sie in [diesem Abschnitt](mirror-page.md).

## Verwalten von Tracking {#manage-tracking}

Der [E-Mail-Designer](create-email-content.md) ermöglicht Ihnen die Verwaltung der getrackten URLs, z. B. die Bearbeitung des Tracking-Typs für jeden Link.

1. Klicken Sie auf das Symbol **[!UICONTROL Links]** im linken Fensterbereich, um die Liste aller URLs Ihrer zu trackenden Inhalte anzuzeigen.

   Diese Liste bietet einen guten Überblick und ermöglicht das Auffinden aller im E-Mail-Inhalt vorhandenen URLs.

1. Um einen Link zu bearbeiten, wählen Sie das entsprechende Stiftsymbol aus.

   ![](assets/message-tracking-edit-links.png)

1. Sie können den **[!UICONTROL Tracking-Typ]** bei Bedarf ändern:

   ![](assets/message-tracking-edit-a-link.png)

   Für jede getrackte URL können Sie einen der folgenden Werte für den Tracking-Modi auswählen:

   * **[!UICONTROL Getrackt]**: aktiviert das Tracking dieser URL.
   * **[!UICONTROL Opt-out]** Diese URL wird als Opt-out- oder Abmeldungs-URL behandelt.
   * **[!UICONTROL Mirror-Seite]**: Diese URL wird als URL der Mirror-Seite behandelt.
   * **[!UICONTROL Nie]**: Das Tracking dieser URL wird nie aktiviert. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Fügen Sie eine **[!UICONTROL Kategorie]** zu Ihrem Link hinzu, um getrackte Links zu gruppieren, und klicken Sie dann auf **[!UICONTROL Speichern]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Öffnen Sie nach dem Versand den Versandbericht. Unter dem Menü **[!UICONTROL Tracking]** zeigt der Bericht **[!UICONTROL URLs und Clickstreams]** an, welche URLs aus Ihrem Versand am häufigsten besucht werden. [Weitere Informationen](../reporting/gs-reports.md)
