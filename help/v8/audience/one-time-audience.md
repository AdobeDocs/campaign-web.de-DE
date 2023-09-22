---
audience: end-user
title: Erstellen einer einmaligen Zielgruppe für einen Versand
description: Erfahren Sie, wie Sie eine einmalige Zielgruppe für einen Versand erstellen.
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 30%

---

# Erstellen einer einmaligen Zielgruppe für einen Versand {#sone-time}

In diesem Abschnitt wird beschrieben, wie Sie beim Erstellen eines neuen Versands eine Zielgruppe erstellen. In diesem Fall werden die Empfänger, die in die Versand-Audience aufgenommen werden sollen, durch Abfrage der Datenbank mit dem Regel-Builder angesprochen.

Die resultierende Audience wird für diesen Versand nur einmal verwendet. Sie wird nicht in der Zielgruppenliste gespeichert.

Bei der Bestimmung der Hauptzielgruppe eines Versands haben Sie außerdem folgende Möglichkeiten:

* [Existierende Zielgruppe auswählen](add-audience.md) aus dem **[!UICONTROL Zielgruppen]** Liste.
* [Laden einer Audience aus einer externen Datei](file-audience.md) (nur für E-Mails).

Gehen Sie wie folgt vor, um direkt aus einem Versand eine neue Zielgruppe zu erstellen:

1. Klicken Sie im Abschnitt **Audience** des Assistenten zur Versanderstellung auf die Schaltflache **[!UICONTROL Audience auswählen]** .

   ![](assets/segment-builder0.png)

1. Wählen Sie **Eigene erstellen** aus. Der Regel-Builder wird angezeigt. Sie können die Zielgruppe Ihres Versands definieren, indem Sie die in der Datenbank enthaltenen Daten filtern. [Erfahren Sie, wie Sie den Regel-Builder verwenden](segment-builder.md)

   ![](assets/segment-builder.png)

1. Sobald Ihre Abfrage fertig ist, klicken Sie auf **Bestätigen** , um die Audience als Hauptzielgruppe Ihres Versands zu verwenden.

   Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Dadurch lässt sich das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. [Weitere Informationen](control-group.md)
