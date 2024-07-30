---
audience: end-user
title: Hinzufügen visueller Fragmente zu E-Mails
description: Erfahren Sie, wie Sie visuelle Fragmente zu Ihren E-Mails hinzufügen
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 64%

---

# Hinzufügen visueller Fragmente zu E-Mails {#use-visual-fragments}

>[!AVAILABILITY]
>
>Diese Funktion ist nur eingeschränkt verfügbar. Sie ist Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und kann nicht in anderen Umgebungen bereitgestellt werden.

Sie können ein visuelles Fragment in einem [E-Mail-Versand](../email/get-started-email-designer.md) oder in einer [Inhaltsvorlage](../email/use-email-templates.md) verwenden. Die einzelnen Schritte werden nachfolgend beschrieben. [Erfahren Sie, wie Sie Inhaltsfragmente erstellen und verwalten](fragments.md).

![](assets/fragments.gif)

## Verwenden eines visuellen Fragments {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentoptionen"
>abstract="Dieser Bereich enthält Optionen für das ausgewählte Fragment. Damit können Sie die Geräte auswählen, auf denen das Fragment angezeigt werden soll, und den Inhalt dieses Fragments öffnen. Verwenden Sie die Registerkarte **[!UICONTROL Stile]** , um Ihr Fragment weiter anzupassen. Sie können die Vererbung auch mit dem ursprünglichen visuellen Fragment aufheben."

<!-- pas vu dans l'UI-->

Gehen Sie wie folgt vor, um ein visuelles Fragment in einen E-Mail-Inhalt einzufügen:

1. Öffnen Sie eine E-Mail oder eine Inhaltsvorlage mit [E-Mail-Designer](../email/get-started-email-designer.md).

1. Wählen Sie in der linken Leiste das Symbol **[!UICONTROL Fragmente]** aus.

   ![](assets/fragments-in-designer.png)

1. Es wird eine Liste mit allen in der aktuellen Sandbox erstellten visuellen Fragmente angezeigt. Sie haben folgende Möglichkeiten:

   * Suchen Sie nach einem bestimmten Fragment, indem Sie mit der Eingabe seines Titels beginnen.
   * Sortieren Sie Fragmente in auf- oder absteigender Reihenfolge.
   * Ändern Sie die Anzeige der Fragmente (Karten- oder Listenansicht).

   >[!NOTE]
   >
   >Fragmente werden nach Erstellungsdatum sortiert: Kürzlich hinzugefügte Fragmente werden zuerst in der Liste angezeigt.

   Wenn einige visuelle Fragmente während der Bearbeitung des Inhalts geändert oder hinzugefügt wurden, klicken Sie auf das Symbol **Aktualisieren** , um die Liste mit den neuesten Änderungen zu aktualisieren.

1. Ziehen Sie ein beliebiges visuelles Fragment aus der Liste in den Bereich, in den Sie es einfügen möchten. Wie jede andere Komponente können Sie das Fragment innerhalb Ihres Inhalts verschieben.

1. Wählen Sie das Fragment aus, um die zugehörigen Optionen im rechten Bereich anzuzeigen.

   ![](assets/fragment-right-pane.png)

   Auf der Registerkarten **[!UICONTROL Einstellungen]** haben Sie folgende Möglichkeiten:

   * Wählen Sie die Geräte aus, auf denen das Fragment angezeigt werden soll.
   * Klicken Sie auf die Schaltfläche **Inhalt bearbeiten**, um den Inhalt dieses Fragments zu öffnen. [Weitere Informationen](../content/fragments.md#edit-fragments)

     Sie können Ihr Fragment mit der Registerkarte **[!UICONTROL Stile]** weiter anpassen.

1. Bei Bedarf können Sie die Vererbung mit dem ursprünglichen visuellen Fragment aufheben. [Weitere Informationen](#break-inheritance)

   Sie können das Fragment auch aus dem Inhalt löschen oder duplizieren. Diese Aktionen können direkt über das Kontextmenü ausgeführt werden, das über dem Fragment angezeigt wird.

1. Fügen Sie beliebig viele visuelle Fragmente hinzu und **[!UICONTROL Speichern]** Sie Ihre Änderungen.

## Unterbrechen der Vererbung {#break-inheritance}

Wenn Sie ein visuelles Fragment bearbeiten, werden die Änderungen synchronisiert. Sie werden automatisch in alle E-Mail-Sendungen und Inhaltsvorlagen übernommen, die dieses Fragment enthalten.

Wenn Fragmente zu einer E-Mail oder einer Inhaltsvorlage hinzugefügt werden, werden sie standardmäßig synchronisiert.

Sie können jedoch die Vererbung vom ursprünglichen Fragment unterbrechen. In diesem Fall wird der Inhalt des Fragments in den aktuellen Entwurf kopiert und die Änderungen werden nicht mehr synchronisiert.

Gehen Sie wie folgt vor, um die Vererbung zu unterbrechen:

1. Wählen Sie das visuelle Fragment aus.

1. Klicken Sie in der kontextbezogene Symbolleiste auf das Entsperrsymbol.

   ![](assets/fragment-break-inheritance.png)

1. Dieses Fragment wird dann zu einem eigenständigen Element, die nicht mehr mit dem ursprünglichen Fragment verknüpft ist. Bearbeiten Sie es wie jede andere Inhaltskomponente in Ihrem Inhalt. [Weitere Informationen](../email/content-components.md)
