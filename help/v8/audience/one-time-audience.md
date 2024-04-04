---
audience: end-user
title: Erstellen einer einmaligen Zielgruppe für einen Versand
description: Erfahren Sie, wie Sie eine einmalige Zielgruppe für einen Versand erstellen.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: b166d06215e06d6426ab9ce9a757fcc041810df9
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 66%

---

# Erstellen einer einmaligen Zielgruppe {#one-time}

In diesem Abschnitt wird beschrieben, wie Sie beim Entwerfen eines neuen Versands eine Zielgruppe erstellen. In diesem Fall werden die Profile, die in die Versand-Audience eingeschlossen werden sollen, durch Abfrage der Datenbank mit dem Abfragemodell abgefragt. Die resultierende Zielgruppe wird nur ein einziges Mal für diesen Versand verwendet. Sie wird nicht in der Zielgruppenliste gespeichert.

Bei der Bestimmung der Hauptzielgruppe eines Versands haben Sie außerdem folgende Möglichkeiten:
* [Wählen Sie eine vorhandene Zielgruppe](add-audience.md) aus der Liste **[!UICONTROL Zielgruppen]** aus.
* [Laden Sie eine Zielgruppe aus einer externen Datei](file-audience.md) (nur für E-Mails).

Gehen Sie wie folgt vor, um eine einmalige neue Zielgruppe für einen Versand zu erstellen:

1. Klicken Sie im Abschnitt **Zielgruppe** des Assistenten zur Versanderstellung auf die Schaltflache **[!UICONTROL Zielgruppe auswählen]**.

   ![](assets/segment-builder0.png){zoomable=&quot;yes&quot;}

1. Auswählen **Erstellen eigener** , um das Abfragemodell zu öffnen, mit dem Sie die Zielpopulation definieren können, indem Sie Daten aus der Datenbank filtern. [So verwenden Sie den Abfrage-Modeler](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable=&quot;yes&quot;}

1. Sobald Ihre Abfrage fertig ist, klicken Sie auf **Bestätigen** , um die resultierende Audience als Hauptzielgruppe Ihres Versands zu verwenden.

   Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Dadurch lässt sich das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. [Weitere Informationen](control-group.md)
