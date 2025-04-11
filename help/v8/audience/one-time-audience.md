---
audience: end-user
title: Erstellen einer einmaligen Zielgruppe für einen Versand
description: Erfahren Sie, wie Sie eine einmalige Zielgruppe für einen Versand erstellen.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 44%

---

# Erstellen einer einmaligen Zielgruppe {#one-time}

In diesem Abschnitt wird beschrieben, wie Sie beim Erstellen eines neuen Versands eine Audience erstellen. In diesem Szenario werden die in der Versandzielgruppe enthaltenen Profile durch die Abfrage der Datenbank mithilfe des Abfrage-Modellierers angesprochen. Die resultierende Audience wird nur einmal für diesen Versand verwendet und nicht in der Liste der Audiences gespeichert.

Bei der Bestimmung der Hauptzielgruppe eines Versands haben Sie außerdem folgende Möglichkeiten:
* [Wählen Sie eine vorhandene Zielgruppe](add-audience.md) aus der Liste **[!UICONTROL Zielgruppen]** aus.
* [Laden Sie eine Zielgruppe aus einer externen Datei](file-audience.md) (nur für E-Mails).

Gehen Sie wie folgt vor, um eine neue einmalige Zielgruppe für einen Versand zu erstellen:

1. Klicken Sie im Abschnitt **Zielgruppe** des Assistenten zur Versanderstellung auf die Schaltflache **[!UICONTROL Zielgruppe auswählen]**.

   [Screenshot mit dem Abschnitt Audience des Assistenten zur Versanderstellung mit hervorgehobener Schaltfläche „Audience auswählen“](assets/segment-builder0.png){zoomable="yes"}

1. Wählen Sie **Eigene erstellen** aus, um den Abfrage-Modellierer zu öffnen. Mit dem Abfrage-Modellierer können Sie die Zielpopulation definieren, indem Sie in der Datenbank enthaltene Daten filtern. [Erfahren Sie, wie Sie den Abfrage-Modellierer ](../query/query-modeler-overview.md).

   [Screenshot der Benutzeroberfläche von Query Modeler](assets/query-modeler.png){zoomable="yes"}

1. Wenn Ihre Abfrage bereit ist, klicken Sie auf **Bestätigen**, um die resultierende Zielgruppe als Hauptzielgruppe Ihres Versands zu verwenden.

   Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Auf diese Weise können Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. [Weitere Informationen](control-group.md).