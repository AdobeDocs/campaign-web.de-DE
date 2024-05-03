---
audience: end-user
title: Hinzufügen visueller Fragmente zu E-Mails
description: Erfahren Sie, wie Sie Ihren E-Mails visuelle Fragmente hinzufügen
hide: true
source-git-commit: 2abbe837197980b4eacb0b5171dc29637fd19dfc
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# Hinzufügen visueller Fragmente zu E-Mails {#use-visual-fragments}

Sie können ein visuelles Fragment in einem [Email-Versand](get-started-email-designer.md)oder in einer [Inhaltsvorlage](use-email-templates.md).



>[!NOTE]
>
>Erfahren Sie, wie Sie Fragmente in erstellen und verwalten [diesem Abschnitt](fragments.md).


## Fragmente verwenden {#use-fragment}

Gehen Sie wie folgt vor, um ein Fragment in einen E-Mail-Inhalt einzufügen:

1. Öffnen Sie eine E-Mail oder einen Vorlageninhalt mit dem [Email Designer](get-started-email-designer.md).

1. Wählen Sie die **[!UICONTROL Fragmente]** in der linken Leiste.

   ![](assets/fragments-in-designer.png)

1. Die Liste aller in der aktuellen Sandbox erstellten visuellen Fragmente wird angezeigt. Sie haben folgende Möglichkeiten:

   * Suchen Sie nach einem bestimmten Fragment, indem Sie mit der Eingabe des Titels beginnen.
   * Sortieren Sie Fragmente in auf- oder absteigender Reihenfolge.
   * Ändern Sie die Anzeige der Fragmente (Karten- oder Listenansicht).

   >[!NOTE]
   >
   >Fragmente werden nach Erstellungsdatum sortiert: Kürzlich hinzugefügte visuelle Fragmente werden zuerst in der Liste angezeigt.

   Wenn einige Fragmente während der Bearbeitung des Inhalts geändert oder hinzugefügt wurden, klicken Sie auf die Schaltfläche **Aktualisieren** -Symbol, um die Liste mit den neuesten Änderungen zu aktualisieren.

1. Ziehen Sie ein beliebiges Fragment aus der Liste in den Bereich, in den Sie es einfügen möchten. Wie jede andere Komponente können Sie das Fragment in Ihrem Inhalt verschieben.

1. Wählen Sie das Fragment aus, um seine Optionen im rechten Bereich anzuzeigen.

   ![](assets/fragment-right-pane.png)

   Aus dem **[!UICONTROL Einstellungen]** können Sie:

   * Wählen Sie die Geräte aus, auf denen das Fragment angezeigt werden soll.
   * Öffnen Sie das Fragment in einer neuen Registerkarte, um es bei Bedarf zu bearbeiten. [Weitere Informationen](../email/fragments.md#edit-fragments)

   Sie können Ihr Fragment mit dem **[!UICONTROL Stile]** Registerkarte.

1. Bei Bedarf können Sie die Vererbung mit dem ursprünglichen Fragment aufheben. [Weitere Infos](#break-inheritance)
Sie können das Fragment auch aus dem Inhalt löschen oder duplizieren. Diese Aktionen können direkt über das Kontextmenü ausgeführt werden, das über dem Fragment angezeigt wird.

1. Fügen Sie beliebig viele Fragmente hinzu und **[!UICONTROL Speichern]** Ihre Änderungen.

## Vererbung unterbrechen {#break-inheritance}

Wenn Sie ein visuelles Fragment bearbeiten, werden die Änderungen synchronisiert. Sie werden automatisch in alle E-Mail-Sendungen und Inhaltsvorlagen übernommen, die dieses Fragment enthalten.

Wenn Fragmente zu einer E-Mail oder einer Inhaltsvorlage hinzugefügt werden, werden sie standardmäßig synchronisiert.

Sie können die Vererbung jedoch vom ursprünglichen Fragment abbrechen. In diesem Fall wird der Inhalt des Fragments in den aktuellen Entwurf kopiert und die Änderungen werden nicht mehr synchronisiert.

Gehen Sie wie folgt vor, um die Vererbung zu unterbrechen:

1. Wählen Sie das Fragment aus.

1. Klicken Sie in der dedizierten Symbolleiste auf das Symbol Entsperren .

   ![](assets/fragment-break-inheritance.png)

1. Dieses Fragment wird zu einem eigenständigen Element, das nicht mehr mit dem ursprünglichen Fragment verknüpft ist. Bearbeiten Sie sie wie jede andere Inhaltskomponente in Ihrem Inhalt. [Weitere Informationen](content-components.md)
