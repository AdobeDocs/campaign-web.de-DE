---
audience: end-user
title: Hinzufügen eines Links zur Mirrorseite
description: Erfahren Sie, wie Sie den Link zur Mirrorseite hinzufügen und verwalten
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 00a612513bcb649d23b2c5b4d5ed05b06a6a80ef
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 81%

---

# Mirrorseite {#mirror-page}

Die Mirrorseite ist eine Online-Version Ihrer E-Mail. Es empfiehlt sich, einen Link zur Mirrorseite hinzuzufügen, um E-Mail-Marketing zu ermöglichen. Benutzerinnen und Benutzer können die Mirrorseite einer E-Mail aufrufen, etwa wenn bei der Anzeige in ihrem Posteingang Rendering-Probleme auftreten oder Bilder beschädigt sind. Es wird außerdem empfohlen, aus Gründen der Barrierefreiheit oder um zum Social Sharing zu ermutigen, eine Online-Version bereitzustellen.

Die von Adobe Campaign erzeugte Mirrorseite enthält alle Personalisierungsdaten.

![Beispiel für einen Mirrorlink](assets/mirror-page-link.png){width="600" align="left"}

## Hinzufügen eines Links zur Mirrorseite{#link-to-mirror-page}

In Adobe Campaign können Sie einen Link zur Mirrorseite in den E-Mail-Inhalt einfügen, indem Sie den dedizierten **Gestaltungsbaustein** verwenden. Der integrierte Gestaltungsbaustein **Link zur Mirrorseite** fügt den folgenden Code in Ihren E-Mail-Inhalt ein: `<%@ include view='MirrorPage' %>`.

Gehen Sie wie folgt vor, um Ihrer E-Mail einen Link zu einer Mirrorseite hinzuzufügen:

1. Wählen Sie ein Element (Text oder Bild) aus und klicken Sie **[!UICONTROL der kontextuellen Symbolleiste auf]** Link einfügen“.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Wählen Sie das Symbol **[!UICONTROL Personalisierung hinzufügen]** aus, um auf das Personalisierungsmenü zuzugreifen.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Wählen Sie im Menü **[!UICONTROL Fragmente]** die Option **[!UICONTROL URL der Mirrorseite]** und klicken Sie auf **[!UICONTROL Hinzufügen]**. [Erfahren Sie, wie Sie Ausdrucksfragmente verwenden](../content/use-expression-fragments.md)

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

Die Mirrorseite wird automatisch erstellt.

Wenn die Empfänger nach dem Versand der E-Mail auf den Link zur Mirrorseite klicken, wird der Inhalt der E-Mail in ihrem Standard-Webbrowser angezeigt.

Standardmäßig beträgt die Beibehaltungsdauer für eine Mirrorseite **60 Tage**. Nach dieser Verzögerung ist die Mirrorseite nicht mehr verfügbar.

>[!CAUTION]
>
>* Links zu Mirrorseiten werden automatisch generiert und können nicht bearbeitet werden. Sie enthalten alle verschlüsselten personalisierten Daten, die zum Rendern der ursprünglichen E-Mail erforderlich sind. Daher kann die Verwendung personalisierter Attribute mit großen Werten zu langen Mirrorseiten-URLs führen, wodurch der Link in Webbrowsern mit einer maximalen URL-Länge eventuell nicht funktioniert.
>
>* Im Testversand an die Testprofile ist der Link zur Mirrorseite nicht aktiv. Er ist nur in den endgültigen Nachrichten aktiv.


## Erzeugung der Mirrorseite {#mirror-page-generation}

Standardmäßig wird die Mirrorseite von Adobe Campaign automatisch erzeugt, wenn der E-Mail-Inhalt nicht leer ist und einen Link zur Mirrorseite enthält (auch Mirrorlink genannt).

Sie können den Erzeugungsmodus der E-Mail-Mirrorseite steuern. Optionen sind in den Versandeigenschaften verfügbar. [Weitere Informationen](../advanced-settings/delivery-settings.md#mirror)
