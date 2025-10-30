---
title: Branding
description: Informationen zum Zuweisen Ihrer Marke
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 8f6a5255-0245-497b-880f-d91ea82ee19e
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 100%

---

# Zuweisen Ihrer Marke {#branding-assign}

## Verknüpfen von Marken mit einer Vorlage {#linking-a-brand-to-a-template}

Um die für eine Marke definierten Parameter zu nutzen, muss diese mit einer Versandvorlage verknüpft sein. Dafür ist die Erstellung oder Anpassung einer Vorlage erforderlich.

Ihre Vorlage wird mit der Marke verknüpft. Im E-Mail-Editor werden die für die Marke konfigurierten Daten in den Feldern **Standard-E-Mail-Adresse des Absenders**, **Standard-Absendername** oder **Logo** verwendet.

>[!BEGINTABS]

>[!TAB Adobe Campaign Web]

Um eine Versandvorlage zu erstellen, können Sie eine integrierte Vorlage duplizieren, einen bestehenden Versand in eine Vorlage konvertieren oder eine Versandvorlage von Grund auf erstellen. [Weitere Informationen](../../msg/delivery-template.md)

Nach der Erstellung Ihrer Vorlage können Sie sie mit einer Marke verknüpfen. Gehen Sie wie folgt vor:

1. Navigieren Sie im linken Menü **[!UICONTROL Sendungen]** zur Registerkarte **[!UICONTROL Vorlagen]** und wählen Sie eine Versandvorlage aus.

   ![](assets/branding_assign_web_1.png)

1. Klicken Sie auf **[!UICONTROL Einstellungen]**. 

   ![](assets/branding_assign_web_2.png)

1. Greifen Sie auf der Registerkarte **[!UICONTROL Versand]** auf das Feld **[!UICONTROL Branding]** zu und wählen Sie die Marke aus, die Sie mit der Vorlage verknüpfen möchten.

   ![](assets/branding_assign_web_3.png)

1. Bestätigen Sie Ihre Auswahl und speichern Sie die Vorlage.

Sie können diese Vorlage jetzt zum Durchführen Ihrer Sendungen verwenden.

>[!TAB Adobe Campaign V8]

Um eine Versandvorlage zu erstellen, können Sie eine integrierte Vorlage duplizieren, einen bestehenden Versand in eine Vorlage konvertieren oder eine Versandvorlage von Grund auf erstellen. [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/create-templates.html?lang=de)

Nach der Erstellung Ihrer Vorlage können Sie sie mit einer Marke verknüpfen. Gehen Sie wie folgt vor:

1. Navigieren Sie im Adobe Campaign-Explorer zu **[!UICONTROL Ressourcen]** `>` **[!UICONTROL Vorlagen]** `>` **[!UICONTROL Versandvorlagen]**.

1. Wählen Sie eine Versandvorlage aus oder duplizieren Sie eine vorhandene. 

   ![](assets/branding_assign_V8_1.png)

1. Rufen Sie die **[!UICONTROL Eigenschaften]** der ausgewählten Versandvorlage auf.

   ![](assets/branding_assign_V8_2.png)

1. Wählen Sie auf der Registerkarte **[!UICONTROL Allgemein]** aus der Dropdown-Liste **[!UICONTROL Branding]** Ihre Marke aus.

   ![](assets/branding_assign_V8_3.png)

1. Wählen Sie nach der Konfiguration **OK** aus.

Sie können diese Vorlage jetzt zum Durchführen Ihrer Sendungen verwenden.

>[!ENDTABS]

## Zuweisen einer Marke zu Ihrem Versand {#assigning-a-brand-to-an-email}

>[!BEGINTABS]

>[!TAB Adobe Campaign Web]

Gehen Sie wie folgt vor, um einen neuen eigenständigen Versand zu erstellen.

1. Navigieren Sie in der linken Leiste zum Menü **[!UICONTROL Sendungen]** und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

   ![](assets/branding_assign_web_4.png)

1. Wählen Sie als Kanal „E-Mail“ oder „Push-Benachrichtigung“ aus und wählen Sie eine Versandvorlage aus der Liste.

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

1. Klicken Sie auf der Seite **[!UICONTROL Eigenschaften]** auf **[!UICONTROL Einstellungen]**.

   ![](assets/branding_assign_web_5.png)

1. Greifen Sie auf der Registerkarte **[!UICONTROL Versand]** auf das Feld **[!UICONTROL Branding]** zu.

   ![](assets/branding_assign_web_6.png)

1. Wählen Sie die Marke aus, die Sie mit der Vorlage verknüpfen möchten.

   ![](assets/branding_assign_web_7.png)

1. Personalisieren Sie Ihre Sendungen weiter. Weitere Informationen zum Erstellen einer E-Mail finden Sie im Abschnitt [Erstellen Ihrer ersten E-Mail](../../email/create-email.md).

>[!TAB Adobe Campaign V8]

Gehen Sie wie folgt vor, um einen neuen eigenständigen Versand zu erstellen.

1. Um einen neuen Versand zu erstellen, navigieren Sie zur Registerkarte **[!UICONTROL Kampagnen]**.

1. Klicken Sie auf **[!UICONTROL Sendungen]** und anschließend auf die Schaltfläche **[!UICONTROL Erstellen]** oberhalb der Liste der vorhandenen Sendungen.

   ![](assets/branding_assign_V8_4.png)

1. Wählen Sie eine Versandvorlage aus. 

1. Rufen Sie die **[!UICONTROL Eigenschaften]** der ausgewählten Versandvorlage auf.

   ![](assets/branding_assign_V8_5.png)

1. Wählen Sie auf der Registerkarte **[!UICONTROL Allgemein]** aus der Dropdown-Liste **[!UICONTROL Branding]** Ihre Marke aus.

   ![](assets/branding_assign_V8_6.png)

1. Wählen Sie nach der Konfiguration **OK** aus.

1. Personalisieren Sie Ihre Sendungen weiter. Weitere Informationen zum Erstellen einer E-Mail finden Sie im Abschnitt [Entwerfen und Senden von E-Mails](../../email/create-email.md).

>[!ENDTABS]

## Überprüfen des mit Transaktionsnachrichten verknüpften Brandings {#check-branding-transactional}

>[!IMPORTANT]
>
>Dieser Abschnitt gilt nur für Transaktionsnachrichten (Message Center).
>
>Auch wenn in der Campaign Web-Benutzeroberfläche Transaktionsfunktionen verfügbar sind, müssen die nachfolgenden Verifizierungsschritte in der Client-Konsole von Campaign v8 (Kontrollinstanz) ausgeführt werden.

Transaktionssendungen, die von Real Time (RT)-Ausführungsinstanzen mit der Kontrollinstanz synchronisiert wurden, replizieren keine Eigenschaften wie Routing oder Branding. Diese synchronisierten Sendungen werden wöchentlich aus derselben Vorlage generiert, um die Versandindikatoren in die Kontrollinstanz zurückzuführen.

Aus diesem Grund zeigt die Kontrollinstanz die Standardmarke an. Die tatsächlichen Marken- und Routing-Einstellungen, die während der Nachrichtenausführung verwendet werden, sind in der Transaktionsnachrichtenvorlage auf der Kontrollinstanz definiert.

So überprüfen Sie, welche Marke für eine Transaktionsnachricht verwendet wurde:

1. Identifizieren Sie den internen Namen der in Real-Time veröffentlichten Transaktionsvorlage (z. B. „`TransactionalMessaging4768`“).

   ![](assets/branding-transactional.png)

1. Suchen Sie in der Kontrollinstanz unter **Transaktionsnachrichtenvorlagen** nach diesem internen Namen.

   ![](assets/branding-transactional2.png)

1. Öffnen Sie die Vorlage, um die Marke und andere zugehörige Eigenschaften anzuzeigen.
