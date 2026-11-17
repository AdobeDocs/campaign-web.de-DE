---
audience: end-user
title: Importieren Ihrer E-Mail-Inhalte
description: Erfahren Sie, wie Sie E-Mail-Inhalte importieren
exl-id: ef9c8e6f-f422-404e-9ebb-a89d1bd45e7f
TQID: 'https://experienceleague.adobe.com/tBeOFkGoxZ-QYEt6dse2-1KSiE318onNSEtGTYzTCO8'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 88%
---
# Importieren Ihrer E-Mail-Inhalte {#existing-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_import_content"
>title="Verwenden eines vorhandenen E-Mail-Inhalts"
>abstract="Der E-Mail-Designer ermöglicht den Import vorhandener HTML-Inhalte. Dieser Inhalt kann eine HTML-Datei mit einem integrierten Stylesheet oder ein ZIP-Ordner mit der HTML-Datei, dem Stylesheet (.css) und Bildern sein."

Sie können vorhandene HTML-Inhalte in den E-Mail-Designer importieren. Dieser Inhalt kann Folgendes sein:

* Eine **HTML-Datei** mit integriertem Stylesheet,
* Ein **komprimierter Ordner** (.zip) mit HTML-Datei, Stylesheet (.css) und Bildern.

>[!NOTE]
>
>Die Struktur des komprimierten Ordners ist freigestellt. Verweise müssen jedoch relativ sein und zur Baumstruktur des ZIP-Ordners passen.

>[!IMPORTANT]
>
>Verwenden Sie das HTML `<base>`-Tag nicht in Ihrem E-Mail-Inhalt. Aus Sicherheitsgründen wird dieses Tag nicht unterstützt und kann verhindern, dass Ihre Inhalte im Inhaltseditor geladen werden. Verwenden Sie stattdessen absolute URLs für Ihre Links und externen Ressourcen.

➡️ [Entdecken Sie diese Funktion im Video](#video)

Gehen Sie wie folgt vor, um eine Datei mit HTML-Inhalten zu importieren:

1. Wählen Sie auf der Startseite des [E-Mail-Designers](get-started-email-designer.md) die Option **[!UICONTROL HTML importieren]** aus.

   ![Screenshot mit der Option „HTML importieren“ auf der Startseite des E-Mail-Designers](assets/html-import.png){zoomable="yes"}

1. Ziehen Sie die HTML- oder ZIP-Datei, die Ihren HTML-Inhalt enthält, per Drag-and-Drop und klicken Sie auf **[!UICONTROL Importieren]**.

1. Sobald der HTML-Inhalt hochgeladen wurde, befindet sich Ihr Inhalt im **[!UICONTROL Kompatibilitätsmodus]**.

   In diesem Modus können Sie Ihren Text personalisieren, Links hinzufügen oder Assets zu Ihrem Inhalt hinzufügen.

   ![Screenshot mit den hochgeladenen HTML-Inhalten im Kompatibilitätsmodus](assets/html-imported.png){zoomable="yes"}

1. Um die Inhaltskomponenten des E-Mail-Designers nutzen zu können, gehen Sie zur Registerkarte **[!UICONTROL HTML-Converter]** und klicken Sie auf **[!UICONTROL Konvertieren]**.

   ![Screenshot mit der Registerkarte „HTML-Converter“ und der Schaltfläche „Konvertieren“](assets/html-imported-2.png){zoomable="yes"}

   >[!NOTE]
   >
   >Wenn ein `<table>`-Tag als erste Ebene in einer HTML-Datei verwendet wird, kann dies zum Verlust von Stileinstellungen finden, einschließlich der Einstellungen für Hintergrund und Breite im Tag der obersten Ebene.

1. Personalisieren Sie Ihre importierte Datei nach Bedarf mit den Funktionen des E-Mail-Designers. [Weitere Informationen](content-components.md)

## Anleitungsvideo {#video}

Erfahren Sie, wie Sie eine E-Mail durch Hochladen von HTML erstellen, mit dem E-Mail-Designer kompatibel machen und in eine Vorlage umwandeln.

>[!VIDEO](https://video.tv.adobe.com/v/3427633/?quality=12)