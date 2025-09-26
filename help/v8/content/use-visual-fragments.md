---
audience: end-user
title: Hinzufügen visueller Fragmente zu E-Mails
description: Erfahren Sie, wie Sie visuelle Fragmente zu Ihren E-Mails hinzufügen
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: ht
source-wordcount: '609'
ht-degree: 100%

---

# Hinzufügen visueller Fragmente zu E-Mails {#use-visual-fragments}

>[!AVAILABILITY]
>
>Diese Funktion erfordert ein Update auf Campaign v8.6.4. Weitere Informationen finden Sie in den [Versionshinweisen zur Client Console von Campaign v8](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/releases/release-notes).

In der Campaign Web-Benutzeroberfläche sind **visuelle Fragmente** vordefinierte visuelle Bausteine, die Sie in mehreren [E-Mail-Sendungen](../email/get-started-email-designer.md) oder in [Inhaltsvorlagen](../content/use-email-templates.md) wiederverwenden können. Weitere Informationen zur Erstellung und Verwaltung von Inhaltsfragmenten finden Sie in [diesem Abschnitt](fragments.md).

![Visuelle Darstellung verwendeter visueller Fragmente](assets/do-not-localize/fragments.gif)

## Verwenden eines visuellen Fragments {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentoptionen"
>abstract="Dieser Bereich enthält Optionen für das ausgewählte Fragment. Damit können Sie die Geräte auswählen, auf denen das Fragment angezeigt werden soll, und den Inhalt dieses Fragments öffnen. Verwenden Sie die Registerkarte **[!UICONTROL Stile]** , um Ihr Fragment weiter anzupassen. Sie können die Vererbung auch mit dem ursprünglichen visuellen Fragment unterbrechen."

<!-- pas vu dans l'UI-->

Gehen Sie wie folgt vor, um ein visuelles Fragment in den Inhalt einer E-Mail einzufügen:

1. Öffnen Sie eine E-Mail oder eine Inhaltsvorlage mit [E-Mail-Designer](../email/get-started-email-designer.md).

1. Wählen Sie in der linken Leiste das Symbol **[!UICONTROL Fragmente]** aus.

   ![Screenshot mit dem Symbol „Fragmente“ in der Benutzeroberfläche des E-Mail-Designers](assets/fragments-in-designer.png)

1. Es wird eine Liste mit allen in der aktuellen Sandbox erstellten visuellen Fragmente angezeigt. Sie haben folgende Möglichkeiten:

   * Suchen Sie nach einem bestimmten Fragment, indem Sie sein Label eingeben.
   * Sortieren Sie Fragmente in auf- oder absteigender Reihenfolge.
   * Ändern Sie die Anzeige der Fragmente (Karten- oder Listenansicht).

   >[!NOTE]
   >
   >Fragmente werden nach ihrem Erstellungsdatum sortiert. Zuletzt hinzugefügte Fragmente werden in der Liste zuerst angezeigt.

   Wenn visuelle Fragmente beim Bearbeiten von Inhalten geändert oder hinzugefügt werden, klicken Sie auf das Symbol **Aktualisieren**, um die Liste mit den neuesten Änderungen zu aktualisieren.

1. Ziehen Sie ein beliebiges visuelles Fragment aus der Liste in den Bereich, in den es eingefügt werden soll. Wie jede andere Komponente können Sie das Fragment innerhalb Ihres Inhalts verschieben.

1. Wählen Sie das Fragment aus, um die zugehörigen Optionen im rechten Bereich anzuzeigen.

   ![Screenshot mit den Fragmentoptionen im rechten Bereich](assets/fragment-right-pane.png)

   Auf der Registerkarten **[!UICONTROL Einstellungen]** haben Sie folgende Möglichkeiten:

   * Wählen Sie die Geräte aus, auf denen das Fragment angezeigt werden soll.
   * Klicken Sie auf die Schaltfläche **Inhalt bearbeiten**, um den Inhalt dieses Fragments zu öffnen. [Weitere Informationen](../content/fragments.md#edit-fragments)

     Sie können Ihr Fragment mit der Registerkarte **[!UICONTROL Stile]** weiter anpassen.

1. Unterbrechen Sie bei Bedarf die Vererbung mit dem ursprünglichen visuellen Fragment. [Weitere Informationen](#break-inheritance)

   Sie können das Fragment auch aus dem Inhalt löschen oder duplizieren. Diese Aktionen werden direkt über das Kontextmenü ausgeführt, das über dem Fragment angezeigt wird.

1. Fügen Sie so viele visuelle Fragmente wie erforderlich hinzu und **[!UICONTROL speichern]** Sie Ihre Änderungen.

### Visuelles Fragment im schreibgeschützten Modus {#fragment-readonly}

Visuelle Fragmente können Zugriffsberechtigungen unterliegen.

Wenn keine Berechtigungen zur Bearbeitung eines bestimmten visuellen Fragments vorliegen, wird die Inhaltsvorlage im **schreibgeschützten Modus** angezeigt. In diesem Fall wird die Schaltfläche **[!UICONTROL Inhalt bearbeiten]** durch die Schaltfläche **[!UICONTROL Inhalt anzeigen]** ersetzt, sodass Sie das Fragment anzeigen, aber keine Änderungen vornehmen können.

![Screenshot mit einem visuellen Fragment im schreibgeschützten Modus](assets/fragment-readonly.png){zoomable="yes"}

Wie unten dargestellt, werden alle Funktionssymbole deaktiviert, wodurch die Interaktion auf das Anzeigen beschränkt bleibt.

![Screenshot mit deaktivierten Funktionssymbolen im schreibgeschützten Modus](assets/fragment-readonly-view.png){zoomable="yes"}

## Unterbrechen der Vererbung {#break-inheritance}

Wenn Sie ein visuelles Fragment bearbeiten, werden die Änderungen synchronisiert und automatisch auf alle E-Mail-Sendungen und Inhaltsvorlagen übertragen, die dieses Fragment enthalten.

Standardmäßig werden Fragmente synchronisiert, wenn sie einer E-Mail oder Inhaltsvorlage hinzugefügt werden.

Sie können jedoch die Vererbung vom ursprünglichen Fragment unterbrechen. In diesem Fall wird der Inhalt des Fragments in den aktuellen Entwurf kopiert und die Änderungen werden nicht mehr synchronisiert.

Gehen Sie wie folgt vor, um die Vererbung zu unterbrechen:

1. Wählen Sie das visuelle Fragment aus.

1. Klicken Sie in der kontextbezogene Symbolleiste auf das Entsperrsymbol.

   ![Screenshot mit dem Entsperrsymbol zum Unterbrechen der Vererbung](assets/fragment-break-inheritance.png)

1. Das Fragment wird dann zu einem eigenständigen Element, das nicht mehr mit dem ursprünglichen Fragment verknüpft ist. Bearbeiten Sie es wie jede andere Inhaltskomponente in Ihrem Inhalt. [Weitere Informationen](../email/content-components.md)