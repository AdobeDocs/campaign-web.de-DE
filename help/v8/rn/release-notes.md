---
audience: end-user
title: Versionshinweise zu Campaign Web v8
description: Versionshinweise zu Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
source-git-commit: 54bcb9b0ba8704cde8beaf1b0400eaa01bba0b15
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 100%

---

# Versionshinweise  {#release-notes}

![](../assets/do-not-localize/badge.png)

Auf dieser Seite sind die neuesten Funktionen und Verbesserungen für Campaign Web v8 aufgeführt.

## Alpha-Version{#alpha-release}

Diese moderne Web-Benutzeroberfläche von Campaign ist derzeit nur für **Alpha-Anwendende** verfügbar und enthält die folgenden Funktionen:

**Modernes, intuitives und einheitliches Erlebnis**

Die neue Web-Benutzeroberfläche von Campaign bietet ein neues Benutzererlebnis, das mit allen Adobe Experience Cloud-Lösungen und -Programmen abgestimmt ist. Sie bietet:

* Zugriff auf die neue Benutzeroberfläche und andere Adobe-Lösungen über eine einzige, gemeinsam genutzte Benutzersitzung
* Neues Navigationserlebnis mit Zugriff auf alle Menüs und Ordner in der linken Leiste
* Umschalter für Lösungen und Organisationen in der oberen Leiste
* Unified Shell-Integration mit direktem Zugriff auf die Community, die Hilfe und den Support
<!--
No search and pulse notifications in Alpha
-->

Weitere Informationen über die neue Benutzeroberfläche finden Sie auf [dieser Seite](../get-started/user-interface.md).

**Erstellen, Starten und Messen Ihrer E-Mail-Kampagne**

Verwenden Sie die neue Web-Benutzeroberfläche von Campaign für Folgendes:

* Erstellen personalisierter E-Mail-Inhalte mit dem E-Mail-Designer – [Weitere Informationen](../content/edit-content.md)
* Definieren von Audiences mit dem Regel-Builder – [Weitere Informationen](../audience/about-audiences.md)
* Vorschau, Testen und Senden Ihrer E-Mail-Nachrichten – [Weitere Informationen](../monitor/prepare-send.md)
* Überwachen, Senden und Messen von Ergebnissen mit integrierten Berichten – [Weitere Informationen](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->

>[!NOTE]
>
>Beachten Sie, dass Cross-Channel-Kampagnen und Workflow-Management-Funktionen als Teil des Beta-Programms verfügbar sein werden.

## Aktualisierungen der Terminologie

Bestehende Campaign-Benutzende sollten beachten, dass einige Konzepte entsprechend den aktuellen Terminologiestandards umbenannt wurden. Diese Änderungen gelten nur für die Web-Benutzeroberfläche von Campaign und werden nicht in der Client-Konsole übernommen. Sie sind unten zusammengefasst.

* Testsendungen heißen jetzt **Test-E-Mails**: verwenden Sie zum Testversand die Schaltfläche **Test** in der Benutzeroberfläche des E-Mail-Versands. Die Zielgruppe des Testversands wird jetzt als **Testprofile** bezeichnet
* Testadressen werden jetzt als **Testprofile** verwendet: Senden Sie die Test-E-Mail an Testadressen, bei denen es sich um zusätzliche, fiktive Empfänger in der Datenbank handelt
* Die Versandanalyse heißt jetzt **Versandvorbereitung**. Wenn Sie die Analyse starten möchten, klicken Sie auf die Schaltfläche **Vorbereiten**
* Die E-Mail-Vorschau ist jetzt über die Schaltfläche **Inhalt simulieren** verfügbar
* Listen heißen jetzt **Audiences**
