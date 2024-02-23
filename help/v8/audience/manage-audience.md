---
audience: end-user
title: Überwachen und Verwalten von Zielgruppen
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Campaign Web überwachen und verwalten können.
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: ht
source-wordcount: '541'
ht-degree: 100%

---

# Überwachen und Verwalten von Zielgruppen {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Eigenschaften"
>abstract="Hier finden Sie eine Zusammenfassung der Zielgruppen-Eigenschaften wie Herkunft, Speicherordner oder Status. Klicken Sie auf den Link im Abschnitt **Letzter Workflow**, um den Workflow zu öffnen, der zur Erstellung der Zielgruppe verwendet wurde."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Zielgruppengröße"
>abstract="Hier finden Sie die Gesamtzahl der Profile innerhalb der Zielgruppe. Klicken Sie auf die Schaltfläche „Berechnen“, um die Zielgruppengebnisse zu aktualisieren und neu zu berechnen."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Zielgruppenfehler"
>abstract="Zielgruppendaten sind nicht verfügbar. Warten Sie bis zum Ende der Workflow-Ausführung."

Die Zielgruppe ist das wichtigste Ziel Ihres Versands: die Empfängerinnen und Empfänger, die die Nachrichten erhalten. Der Zielgruppentyp hängt vom in der Versandvorlage definierten Zielgruppen-Mapping ab. Weiterführende Informationen zu Versandvorlagen finden Sie auf [dieser Seite](../msg/delivery-template.md).

Um die Population Ihrer Zielgruppe zu bestimmen, können Sie:

* [neue Zielgruppen erstellen](create-audience.md) über das Menü **[!UICONTROL Zielgruppen]**,
* [eine vorhandene Zielgruppe auswählen](add-audience.md), die als Liste in der Client-Konsole erstellt wurde oder aus Adobe Experience Platform stammt,
* Mit dem Abfrage-Builder [eine neue Zielgruppe erstellen](../query/query-modeler-overview.md), indem Sie Filterkriterien definieren und kombinieren,
* [eine Zielgruppe aus einer externen Datei verwenden](file-audience.md). Diese Option steht nur für eigenständige E-Mail-Sendungen zur Verfügung und kann nicht in Kampagnensendungen verwendet werden.

Wenn Sie eine Zielgruppe ansprechen, können Sie außerdem **Kontrollgruppen** definieren, um einen Teil Ihrer Zielgruppe vom Versand von Nachrichten auszuschließen und so die Wirkung Ihrer Kampagnen zu messen. [Erfahren Sie, wie Sie eine Kontrollgruppe festlegen](control-group.md)

>[!NOTE]
>
>Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Zielgruppe in der speziellen Workflow-Aktivität **Zielgruppe erstellen** definiert. In diesem Zusammenhang ist es nicht möglich, eine Zielgruppe aus einer Datei für einen E-Mail-Versand zu laden. Die Zielgruppe wird nur in dieser dedizierten Aktivität definiert. In [diesem Abschnitt](../workflows/activities/build-audience.md) erfahren Sie, wie Sie die Zielgruppe Ihres Versands in einem Kampagnen-Workflow definieren

Die Liste der Zielgruppen, die in Campaign Web verwendet werden können, ist über das Menü **[!UICONTROL Zielgruppen]** verfügbar.

![](assets/audiences-list.png){zoomable=&quot;yes&quot;}

Zielgruppen können aus mehreren Quellen stammen. Die Spalte **[!UICONTROL Herkunft]** gibt an, wo eine bestimmte Zielgruppe erstellt wurde:

* **[!UICONTROL Adobe Campaign]**: Diese Zielgruppen werden in der Adobe Campaign v8-Konsole erstellt. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=de){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Diese Zielgruppen werden in Adobe Experience Platform erstellt und mithilfe der Integration von Adobe-Quellen- und Zielen in Campaign Web integriert. Erfahren Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=de){target="_blank"}, wie Sie diese Integration einrichten.

>[!NOTE]
>
>Um Adobe Experience Platform-Zielgruppen in Campaign verwenden zu können, müssen Sie die Integration mit Adobe-Quellen und -Zielen konfigurieren. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=de){target="_blank"}.

* **[!UICONTROL Adobe Campaign WebUI]**: Diese Zielgruppen werden mithilfe von Zielgruppen-Workflows von Campaign Web erstellt. [Erfahren Sie, wie Sie Zielgruppen erstellen](create-audience.md)

Um weitere Informationen zu einer Zielgruppe zu erhalten, öffnen Sie sie in der Liste. Die Eigenschaften der Zielgruppe werden zusammen mit der Anzahl der in der Zielgruppe enthaltenen Profile angezeigt. Sie können die Anzahl der Zielgruppen jederzeit mit der Schaltfläche **[!UICONTROL Berechnen]** aktualisieren.

Die Registerkarte **[!UICONTROL Daten]** ermöglicht die Visualisierung der Profile, die Teil der Zielgruppe sind. Sie können diese Ansicht anpassen, indem Sie weitere Spalten hinzufügen oder erweiterte Filter nutzen, um die angezeigten Daten zu präzisieren.

![](assets/audiences-details.png){zoomable=&quot;yes&quot;}

Um eine Zielgruppe zu duplizieren oder zu löschen, klicken Sie auf die Schaltfläche **[!UICONTROL Mehr Aktionen]** in der Zielgruppenliste neben dem Zielgruppennamen oder in einem Bildschirm mit Zielgruppendetails.
