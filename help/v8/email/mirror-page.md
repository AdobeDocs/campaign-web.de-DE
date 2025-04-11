---
audience: end-user
title: Hinzufügen eines Links zur Mirrorseite
description: Erfahren Sie, wie Sie den Link zur Mirrorseite hinzufügen und verwalten
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 29%

---

# Mirrorseite {#mirror-page}

Die Mirrorseite ist eine Online-Version Ihrer E-Mail. Es empfiehlt sich, im E-Mail-Marketing einen Link zur Mirrorseite hinzuzufügen. Benutzer können auf die Mirrorseite einer E-Mail zugreifen, wenn sie beispielsweise beim Anzeigen in ihrem Posteingang Rendering-Probleme oder beschädigte Bilder feststellen. Die Bereitstellung einer Online-Version wird auch aus Gründen der Barrierefreiheit oder zur Förderung des Social Sharing empfohlen.

Die von Adobe Campaign generierte Mirrorseite enthält alle Personalisierungsdaten.

![Beispiel für einen Mirror-Link in einer E-Mail](assets/mirror-page-link.png){width="600" align="left"}

## Hinzufügen eines Links zur Mirrorseite {#link-to-mirror-page}

Fügen Sie in Adobe Campaign einen Link zur Mirrorseite in den E-Mail-Inhalt ein, indem Sie den dedizierten **Gestaltungsbaustein“**. Der integrierte Gestaltungsbaustein **Link zur Mirrorseite** fügt den folgenden Code in Ihren E-Mail-Inhalt ein: `<%@ include view='MirrorPage' %>`.

Gehen Sie wie folgt vor, um Ihrer E-Mail einen Link zu einer Mirrorseite hinzuzufügen:

1. Wählen Sie ein Element (Text oder Bild) aus und klicken Sie **[!UICONTROL der kontextuellen Symbolleiste auf]** Link einfügen“.

   ![Kontextuelle Symbolleiste mit der Option „Link einfügen“](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Wählen Sie das Symbol **[!UICONTROL Personalisierung hinzufügen]** aus, um auf das Personalisierungsmenü zuzugreifen.

   ![Personalization-Menü in Adobe Campaign](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Wählen Sie **[!UICONTROL Menü]** Fragmente“ die Option **[!UICONTROL URL der Mirrorseite]** und klicken Sie auf **[!UICONTROL Hinzufügen]**. [Erfahren Sie, wie Sie Ausdrucksfragmente verwenden](../content/use-expression-fragments.md)

   ![Option URL der Mirrorseite im Menü „Fragmente“](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

Die Mirrorseite wird automatisch erstellt.

Wenn die E-Mail gesendet wird, sehen Empfängerinnen und Empfänger, die auf den Link zur Mirrorseite klicken, den E-Mail-Inhalt in ihrem Standard-Webbrowser.

Standardmäßig beträgt die Beibehaltungsdauer für eine Mirrorseite **60 Tage**. Nach diesem Zeitraum ist die Mirrorseite nicht mehr verfügbar.

>[!CAUTION]
>
>* Mirrorseiten-Links werden automatisch generiert und können nicht bearbeitet werden. Sie enthalten alle verschlüsselten personalisierten Daten, die zum Rendern der ursprünglichen E-Mail erforderlich sind. Die Verwendung personalisierter Attribute mit großen Werten kann zu langen Mirror-Seiten-URLs führen, wodurch der Link in Webbrowsern mit einer maximalen URL-Länge möglicherweise nicht funktioniert.
>
>* Im Testversand an Testprofile ist der Link zur Mirrorseite nicht aktiv. Er wird erst in den endgültigen Nachrichten aktiv.

## Erzeugung der Mirrorseite {#mirror-page-generation}

Standardmäßig generiert Adobe Campaign automatisch die Mirrorseite, wenn der E-Mail-Inhalt nicht leer ist und einen Link zur Mirrorseite enthält (auch als Mirrorlink bezeichnet).

Den Erzeugungsmodus der E-Mail-Mirrorseite über die in den Versandeigenschaften verfügbaren Optionen steuern. [Weitere Informationen](../advanced-settings/delivery-settings.md#mirror)