---
title: Arbeiten mit GenStudio for Performance Marketing in Adobe Campaign
description: Informationen zum Arbeiten mit GenStudio for Performance Marketing in Adobe Campaign
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 100%

---

# Arbeiten mit GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Verwenden einer mit GenStudio erstellten Vorlage"
>abstract="Dank der nahtlosen Integration mit Adobe GenStudio for Performance Marketing können Sie eine mit KI-Technologie von Adobe erweiterte GenStudio-Vorlage einfach importieren."

## Erste Schritte mit GenStudio {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} ist eine auf generative KI ausgerichtete Anwendung, mit der Marketing-Teams ihre eigenen Anzeigen und E-Mails erstellen können, um wirkungsvolle, personalisierte Marketing-Kampagnen zu gestalten, die Ihren Markenstandards und Unternehmensrichtlinien entsprechen. Auf Grundlage der KI-Technologie von Adobe wird eine umfassende Palette an Tools angeboten, die die komplexe Erstellung und Verwaltung von Inhalten vereinfachen, sodass sich Kreative auf Innovationen konzentrieren können.

>[!AVAILABILITY]
>
>Diese Funktion ist nur für den E-Mail-Kanal verfügbar.

Um die Marketing-Effizienz zu steigern und die Markenkonsistenz zu wahren, können Sie Erlebnisse aus [!DNL **GenStudio for Performance Marketing**] nahtlos mit [!DNL **Adobe Campaign**] integrieren. Auf diese Weise können Sie die KI-gestützte Content-Erstellung von [!DNL GenStudio] zusammen mit den erweiterten Orchestrierungsfunktionen von [!DNL Adobe Campaign] nutzen.

>[!INFO]
>
>Weitere Informationen finden Sie in diesem [Überblick](https://business.adobe.com/de/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} und einer [Demo](https://business.adobe.com/de/products/genstudio-for-performance-marketing.html#demo){target="_blank"} von [!DNL Adobe GenStudio for Performance Marketing].

## Verwenden von GenStudio-Funktionen in Adobe Campaign {#use-genstudio}

Die Integration von [!DNL GenStudio for Performance Marketing] und [!DNL Adobe Campaign] ermöglicht eine bessere Zusammenarbeit der Marketing-Fachleute in Ihrem Unternehmen und optimiert so Prozesse.

Beispielsweise kann eine technische Marketing-Fachkraft, die [!DNL Adobe Campaign] zum Entwickeln und Automatisieren von E-Mail-Kampagnen verwendet, mit einer Fachkraft für Performance-Marketing zusammenarbeiten, die Inhalte mithilfe von [!DNL GenStudio] erstellt.

Mit dieser Integration können beide gemeinsam markenkonforme Inhalte von [!DNL GenStudio] einfach in [!DNL Adobe Campaign] integrieren und ansprechende E-Mails versenden, die auf bestimmte Kundensegmente zugeschnitten sind und den Umsatz steigern.

### Exportieren einer HTML-Vorlage von Adobe Campaign nach GenStudio {#export-from-campaign-to-genstudio}

Zunächst können Sie eine HTML-Vorlage mit den Richtlinien Ihrer Marke von [!DNL Adobe Campaign] nach [!DNL GenStudio for Performance Marketing] exportieren. Gehen Sie dazu wie folgt vor.

1. Greifen Sie in [!DNL Adobe Campaign] auf den Inhalt Ihrer E-Mail zu. [Weitere Informationen](../email/create-email.md#create-content)

1. Wählen Sie im E-Mail-Designer über die Schaltfläche **[!UICONTROL Mehr]** die Option **[!UICONTROL HTML exportieren]** aus.

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Laden Sie diese exportierte HTML-Vorlage in [!DNL GenStudio for Performance Marketing] hoch. <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >Im entsprechenden Abschnitt im [Benutzerhandbuch zu Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"} erfahren Sie, wie Sie eine HTML-Vorlage in [!DNL GenStudio] hochladen.<!--GenStudio doc to be updated with Campaign-->

1. Verwenden Sie diese Vorlage in GenStudio, um mehrere E-Mail-Varianten mit KI-Prompts zu erstellen und zu speichern.

   >[!NOTE]
   >
   >Im entsprechenden [Abschnitt](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} zu GenStudio erfahren Sie, wie Sie E-Mail-Erlebnisse erstellen.

### Nutzen von GenStudio-Erlebnissen in Adobe Campaign {#leverage-genstudio-experiences}

Gehen Sie wie folgt vor, um die [!DNL GenStudio]-E-Mail-Varianten zu nutzen, die Sie soeben durch Importieren in [!DNL Adobe Campaign] erstellt haben.

1. Erstellen Sie in [!DNL Adobe Campaign] [einen E-Mail-Versand](../email/create-email.md).

1. Klicken Sie im Dashboard des E-Mail-Versands auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]**. [Weitere Informationen](../email/create-email.md#create-content)

1. Wählen Sie auf der Startseite des E-Mail-Designers **[!UICONTROL HTML importieren]** aus und klicken Sie auf die Schaltfläche **[!UICONTROL Adobe GenStudio for Performance Marketing]**.

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Durchsuchen Sie die GenStudio-Erlebnisse, um mit der Erstellung Ihrer Inhalte zu beginnen. Sie können die Erlebnisse nach verschiedenen Kriterien filtern, z. B. nach Produkten, Rollen, Marken oder sogar Farben.

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Wählen Sie ein Erlebnis aus und klicken Sie auf **[!UICONTROL Verwenden]**.

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Wählen Sie den Ordner aus, in den Sie das GenStudio-Erlebnis importieren möchten.

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. Der ausgewählte Inhalt wird im E-Mail-Designer angezeigt.

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >[Aus einer  [!DNL Adobe Campaign] -Vorlage](#export-from-ajo-to-genstudio) erstellte GenStudio-Erlebnisse werden direkt in den E-Mail-Designer importiert. Ohne [!DNL Adobe Campaign]-Vorlage erstellte GenStudio-Erlebnisse werden in den [Kompatibilitätsmodus](../email/existing-content.md) importiert.

   Verwenden Sie die [Tools zur Bearbeitung von E-Mail-Inhalten](../email/create-email-content.md) und [Personalisierungsfelder](../personalization/personalize.md), um Ihre E-Mail nach Bedarf zu bearbeiten. Speichern Sie Ihren Inhalt.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456058/?captions=ger&quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->