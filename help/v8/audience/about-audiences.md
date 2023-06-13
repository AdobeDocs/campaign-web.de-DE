---
audience: end-user
title: Erste Schritte mit Audiences
description: Erfahren Sie, wie Sie Audiences in der Web-Benutzeroberfläche von Campaign verwenden.
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: bbebd9dc462a189618cbf6e71467bb0935e1317a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Erste Schritte mit Audiences {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


Die Audience ist die Hauptzielgruppe Ihres Versands: die Empfänger, die die Nachrichten erhalten. Der Audience-Typ hängt vom in der Versandvorlage definierten Zielgruppen-Mapping ab. Versandvorlage erfahren [in diesem Abschnitt](../msg/delivery-template.md).

Zur Definition der Audience-Population haben Sie folgende Möglichkeiten:

* Wählen Sie eine vorhandene Zielgruppe aus, die als Liste in der Clientkonsole erstellt wurde. [Weitere Informationen](add-audience.md)
* Wählen Sie eine Adobe Experience Platform-Zielgruppe aus. [Weitere Informationen](aep-audience.md)
* Erstellen Sie mit dem Regel-Builder eine neue Zielgruppe, indem Sie Filterkriterien definieren und kombinieren. [Weitere Informationen](segment-builder.md)
* Verwenden Sie eine Audience aus einer externen Datei: Diese Option steht nur für eigenständige E-Mail-Sendungen zur Verfügung und kann nicht in Kampagnensendungen verwendet werden. [Weitere Informationen](file-audience.md)

Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Audience in einem bestimmten **Audience lesen** Workflow-Aktivität. In diesem Zusammenhang ist es nicht möglich, eine Audience aus einer Datei für einen E-Mail-Versand zu laden. Die Audience wird nur in dieser dedizierten Aktivität definiert. Hier erfahren Sie, wie Sie die Audience Ihres Versands in einem Kampagnen-Workflow definieren. [in diesem Abschnitt](../workflows/orchestrate-activities.md).

Darüber hinaus können Sie Kontrollgruppen definieren, um einen Teil Ihrer Audience vom Versand von Nachrichten auszuschließen und so die Wirkung Ihrer Kampagnen zu messen. [Weitere Informationen](control-group.md)

![](assets/about-audience.png)

