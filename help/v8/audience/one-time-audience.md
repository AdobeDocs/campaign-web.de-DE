---
audience: end-user
title: Erstellen einer einmaligen Zielgruppe für einen Versand
description: Erfahren Sie, wie Sie eine einmalige Zielgruppe für einen Versand erstellen.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 100%

---

# Erstellen einer einmaligen Zielgruppe {#one-time}

In diesem Abschnitt wird beschrieben, wie Sie beim Entwerfen eines neuen Versands eine Zielgruppe erstellen. In diesem Fall werden die Profile, die in die Versandzielgruppe aufgenommen werden sollen, durch Abfragen der Datenbank mit dem Abfrage-Modeler ermittelt. Die resultierende Zielgruppe wird nur ein einziges Mal für diesen Versand verwendet. Sie wird nicht in der Zielgruppenliste gespeichert.

Bei der Bestimmung der Hauptzielgruppe eines Versands haben Sie außerdem folgende Möglichkeiten:
* [Wählen Sie eine vorhandene Zielgruppe](add-audience.md) aus der Liste **[!UICONTROL Zielgruppen]** aus.
* [Laden Sie eine Zielgruppe aus einer externen Datei](file-audience.md) (nur für E-Mails).

Gehen Sie wie folgt vor, um eine neue einmalige Zielgruppe für einen Versand zu erstellen:

1. Klicken Sie im Abschnitt **Zielgruppe** des Assistenten zur Versanderstellung auf die Schaltflache **[!UICONTROL Zielgruppe auswählen]**.

   ![](assets/segment-builder0.png){zoomable="yes"}

1. Wählen Sie **Eigene erstellen**, um den Abfrage-Modeler zu öffnen, mit dem Sie die Zielpopulation durch Filtern der in der Datenbank enthaltenen Daten definieren können. [So verwenden Sie den Abfrage-Modeler](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable="yes"}

1. Wenn Ihre Abfrage bereit ist, klicken Sie auf **Bestätigen**, um die resultierende Zielgruppe als Hauptzielgruppe Ihres Versands zu verwenden.

   Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Dadurch lässt sich das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. [Weitere Informationen](control-group.md)
