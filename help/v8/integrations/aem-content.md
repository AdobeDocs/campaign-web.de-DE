---
audience: end-user
title: Verwalten von Assets mit Adobe Experience Manager as a Cloud Service
description: Erfahren Sie, wie Sie Inhalte mit Adobe Experience Manager as a Cloud Service verwalten können
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 97%

---

# Verwalten von Vorlagen mit [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Erste Schritte mit [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

Die Integration der Adobe Campaign Web-Oberfläche in Adobe Experience Manager ermöglicht eine optimierte Verwaltung von E-Mail-Versandinhalten und Formularen direkt auf der Adobe Experience Manager-Plattform.

![](assets/do-not-localize/book.png) [Erfahren Sie mehr über Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=de)

## Erstellen einer Vorlage in [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Navigieren Sie zu Ihrer [!DNL Adobe Experience Manager]-Autoreninstanz und klicken Sie oben links auf der Seite auf „Adobe Experience“. Wählen im Menü die Option **[!UICONTROL Sites]** aus.

1. Rufen Sie **[!UICONTROL Kampagnen > Name Ihrer Marke > Hauptbereich > Name Ihrer Seite]** auf.

1. Klicken Sie auf **[!UICONTROL Erstellen]** und wählen Sie im Dropdown-Menü die Option **[!UICONTROL Seite]** aus.

   ![Screenshot mit der Schaltfläche „Erstellen“ und der Option „Seite“ im Dropdown-Menü](assets/aem_1.png)

1. Wählen Sie die Vorlage **[!UICONTROL Adobe Campaign-E-Mail]** aus und benennen Sie Ihren Newsletter.

   ![[Screenshot mit der Auswahl der Vorlage „Adobe Campaign-E-Mail“ und dem Feld für die Benennung]](assets/aem_2.png)

1. Passen Sie den E-Mail-Inhalt an, indem Sie Komponenten hinzufügen, z. B. Personalisierungsfelder aus Adobe Campaign. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=de#editing-email-content)

1. Wenn Ihre E-Mail fertig ist, navigieren Sie zum Menü **[!UICONTROL Seiteninformationen]** und klicken Sie auf **[!UICONTROL Workflow starten]**.

   ![Screenshot mit dem Menü „Seiteninformationen“ und der Option „Bericht Workflow starten“](assets/aem_3.png)

1. Wählen Sie in der ersten Dropdown-Liste als Workflow-Modell **[!UICONTROL Adobe Campaign genehmigen]** aus und klicken Sie auf **[!UICONTROL Workflow starten]**.

1. Oben auf Ihrer Seite erscheint ein Haftungsausschluss mit folgendem Inhalt: `This page is subject to the workflow Approve for Adobe Campaign`. Klicken Sie neben dem Haftungsausschluss auf **[!UICONTROL Beendet]**, um die Überprüfung zu bestätigen. Klicken Sie dann auf **[!UICONTROL Ok]**.

   ![Screenshot mit dem Haftungsausschluss und der Schaltfläche „Beendet“](assets/aem_4.png)

1. Klicken Sie erneut auf **[!UICONTROL Beendet]** und wählen Sie **[!UICONTROL Newsletter-Genehmigung]** in der Dropdown-Liste **[!UICONTROL Nächster Schritt]** aus.

Ihr Newsletter ist jetzt fertig und in Adobe Campaign synchronisiert.

## Importieren einer Adobe Experience Manager as a Cloud Service-Vorlage{#aem-templates-perso}

Sobald die Experience Manager-Vorlage im Adobe Campaign Web als Inhaltsvorlage verfügbar ist, können Sie den für die E-Mail erforderlichen Inhalt einschließlich Personalisierung identifizieren und integrieren.

1. Klicken Sie im Menü **[!UICONTROL Sendungen]** auf **[!UICONTROL Versand erstellen]**. 

1. Wählen Sie im Fenster der E-Mail-Vorlage die integrierte Vorlage **[!UICONTROL E-Mail-Versand mit AEM Inhalt]** aus.

   ![Screenshot der Vorlagenauswahl „E-Mail-Versand mit AEM-Inhalt“](assets/aem_5.png)

1. Geben Sie ein **[!UICONTROL Label]** für den Versand ein und konfigurieren Sie zusätzliche Optionen entsprechend Ihren Anforderungen:

   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu.
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner.
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an.
   * **[!UICONTROL Art]**: Geben Sie zu Klassifizierungszwecken die Art der E-Mail an.

1. Definieren Sie eine **[!UICONTROL Zielgruppe]** für Ihre E-Mail. [Weitere Informationen](../email/create-email.md#define-audience)

1. Klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**.

1. Klicken Sie im Menü **[!UICONTROL Inhalt bearbeiten]** auf **[!UICONTROL AEM-Inhalt auswählen]**.

   ![Screenshot mit der Option „AEM-Inhalt auswählen“ im Menü „Inhalt bearbeiten“](assets/aem_6.png)

1. Durchsuchen Sie Ihre AEM-Vorlagen und wählen Sie diejenige aus, die Sie in Campaign Web importieren möchten.

   ![Screenshot mit der Benutzeroberfläche zur Auswahl der AEM-Vorlage](assets/aem_8.png)

1. Beachten Sie, dass Inhalte nicht automatisch synchronisiert werden. Wenn Änderungen an Ihren Vorlagen direkt in Adobe Experience Manager vorgenommen werden, wählen Sie **[!UICONTROL AEM-Inhalt aktualisieren]**, um auf die neueste Version Ihrer Vorlage zu aktualisieren.

1. Um die Verknüpfung zwischen Experience Manager und Campaign zu entfernen oder Ihre Experience Manager-Vorlage in E-Mail-Designer weiter zu personalisieren, klicken Sie auf **[!UICONTROL Verknüpfung von AEM-Inhalt aufheben]**.

   ![Screenshot mit der Option „Verknüpfung von AEM-Inhalt aufheben“](assets/aem_9.png)

1. Wenn Sie Ihrer Experience Manager-Vorlage personalisierten Inhalt hinzugefügt haben, klicken Sie auf **[!UICONTROL Inhalt simulieren]**, um mithilfe von Testprofilen eine Vorschau des Nachrichteninhalts anzuzeigen.

[Weitere Informationen zu Vorschau und Testprofilen](../preview-test/preview-content.md)

1. Bei der Anzeige der Nachrichtenvorschau werden alle personalisierten Elemente automatisch durch die entsprechenden Daten aus dem ausgewählten Testprofil ersetzt.

   Fügen Sie bei Bedarf zusätzliche Testprofile über die Schaltfläche **[!UICONTROL Testprofile verwalten]** hinzu.

Ihre Nachricht ist jetzt bereit für den Versand.