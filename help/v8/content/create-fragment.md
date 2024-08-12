---
audience: end-user
title: Erstellen von Inhaltsfragmenten
description: Erfahren Sie, wie Sie Inhaltsfragmente erstellen
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: ht
source-wordcount: '918'
ht-degree: 100%

---


# Erstellen von Inhaltsfragmenten {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Definieren Ihrer eigenen Inhaltsfragmente"
>abstract="Definieren Sie die Fragmenteigenschaften und den Fragmenttyp, den Sie erstellen möchten. Anschließend können Sie den E-Mail-Designer oder den Ausdruckseditor verwenden, um den Inhalt Ihres Fragments zu konfigurieren."

<!-- pas vu dans l'UI-->

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragmenteigenschaften"
>abstract="Geben Sie den Titel des Fragments ein. Bei Bedarf können Sie weitere Optionen definieren, z. B. den internen Namen des Fragments, dessen Ordner und eine Beschreibung."

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Typ des Inhaltsfragments"
>abstract="Wählen Sie den Fragmenttyp aus, den Sie erstellen möchten. **Visuelle Fragmente** sind vordefinierte visuelle Bausteine, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. **Ausdrucksfragmente** sind vordefinierte Ausdrücke, die über einen dedizierten Eintrag im Ausdruckseditor verfügbar sind."

Es gibt zwei Möglichkeiten, Inhaltsfragmente zu erstellen:

* Erstellen Sie ein Fragment mithilfe des dediziertes Menüs **[!UICONTROL Fragmente]** von Grund auf neu. [Weitere Informationen dazu](#create-from-scratch)
* Speichern Sie beim Entwerfen von Inhalten einen Teil des Inhalts als Fragment. [Weitere Informationen dazu](#save-as-fragment)

  >[!NOTE]
  >
  >Diese Funktion ist nur für visuelle Fragmente verfügbar. Ausdrucksfragmente werden ausschließlich über das Menü **Fragmente** erstellt.

Nach dem Speichern kann Ihr Inhaltsfragment in beliebigen Versand- oder Inhaltsvorlagen verwendet werden.

## Erstellen eines Inhaltsfragments von Grund auf {#create-from-scratch}

Gehen Sie wie folgt vor, um ein Inhaltsfragment von Grund auf neu zu erstellen.

1. [Rufen Sie die Fragmentliste](#access-manage-fragments) über das linke Menü unter **[!UICONTROL Content-Management]** > **[!UICONTROL Fragmente]** auf und wählen Sie **[!UICONTROL Fragment erstellen]** aus.

   ![](assets/fragments-list.png)

1. Geben Sie den Titel des Fragments ein. Bei Bedarf können Sie weitere Optionen definieren, z. B. den internen Namen des Fragments, dessen Ordner und eine Beschreibung.

1. Wählen Sie den zu erstellenden Fragmenttyp aus: **Visuelles Fragment** oder **Ausdrucksfragment**. [Lernen Sie die Unterschiede zwischen visuellen und Ausdrucksfragmenten kennen](fragments.md)

   ![](assets/fragment-create.png)

   >[!AVAILABILITY]
   >
   >Visuelle Fragmente sind eingeschränkt verfügbar (LA, Limited Availability). Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.

1. Klicken Sie auf die Schaltfläche **Erstellen**.

   * Für **visuelle Fragmente** wird der [E-Mail-Designer](../email/get-started-email-designer.md) angezeigt. Bearbeiten Sie Ihren Inhalt nach Bedarf, so wie bei jeder anderen E-Mail in einer Kampagne. Klicken Sie anschließend auf die Schaltfläche **Speichern und schließen**. Sie können Bilder, Links, Personalisierungsfelder und dynamische Inhalte hinzufügen.

     ![](assets/fragment-designer.png)

   * Für **Ausdrucksfragmente** wird der Ausdruckseditor geöffnet. Nutzen Sie die Personalisierungs- und Authoring-Funktionen, um Ihren Inhalt zu erstellen, und klicken Sie dann auf **Bestätigen**. [Erfahren Sie mehr über die Arbeit mit dem Ausdruckseditor](../personalization/personalize.md)

     ![](assets/fragment-expression.png)

1. Wenn Ihr Inhalt bereit ist, klicken Sie auf **Speichern**.

Dieses Inhaltsfragment kann nun beim Erstellen von Sendungen oder [Inhaltsvorlagen](../email/use-email-templates.md) in Campaign verwendet werden. In diesem Abschnitt erfahren Sie, wie Sie visuelle und Ausdrucksfragmente verwenden:
* [Hinzufügen visueller Fragmente zu E-Mails](use-visual-fragments.md)
* [Hinzufügen eines Ausdrucksfragments zum Ausdruckseditor](use-expression-fragments.md)

## Speichern von Inhalt als visuelles Fragment {#save-as-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Als Fragment speichern"
>abstract="Um Inhalt als visuelles Fragment zu speichern, wählen Sie die Elemente aus, die in das Fragment aufgenommen werden sollen, einschließlich Personalisierungsfeldern und dynamischer Inhalte. Sie können nur Abschnitte auswählen, die nebeneinander liegen. Sie können weder eine leere Struktur noch ein anderes Inhaltsfragment auswählen. Dieser Inhalt ist dann ein eigenständiges Fragment, das zur Fragmentliste hinzugefügt wurde und das über das dedizierte Menü aufgerufen werden kann. Sie können dieses Fragment nun beim Erstellen einer E-Mail oder Inhaltsvorlage in Campaign verwenden."

<!--pas vu dans l'UI-->

Jeder E-Mail-Inhalt kann zur späteren Wiederverwendung als visuelles Fragment gespeichert werden. Beim Entwerfen einer [Inhaltsvorlage](../email/use-email-templates.md) oder eines [E-Mail-Versands](../email/get-started-email-designer.md) können Sie einen Teil des Inhalts als visuelles Fragment speichern. Gehen Sie dazu wie folgt vor:

1. Klicken Sie in [E-Mail-Designer](../email/get-started-email-designer.md) oben rechts auf dem Bildschirm auf **Mehr**.

1. Wählen Sie im Dropdown-Menü die Option **[!UICONTROL Als Fragment speichern]** aus.

   ![](assets/fragment-save-as.png)

1. Der Bildschirm **[!UICONTROL Als Fragment speichern]** wird angezeigt. Hier können Sie die Elemente auswählen, die in das Fragment aufgenommen werden sollen, einschließlich Personalisierungsfelder und dynamischer Inhalte.

   >[!CAUTION]
   >
   >Sie können nur Abschnitte auswählen, die nebeneinander liegen. Sie können weder eine leere Struktur noch ein anderes Inhaltsfragment auswählen.

   ![](assets/fragment-save-as-screen.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Geben Sie den Fragmentnamen an und speichern Sie es.

   ![](assets/fragment-save-confirm.png)

   Dieser Inhalt ist jetzt ein eigenständiges Fragment, das zur [Fragmentliste](#manage-fragments) hinzugefügt wurde und das über das dedizierte Menü aufgerufen werden kann. Sie können dieses Fragment nun beim Erstellen von [E-Mails](../email/get-started-email-designer.md) oder [Inhaltsvorlagen](../email/use-email-templates.md) in Campaign verwenden. [Weitere Informationen dazu](../content/use-visual-fragments.md)

>[!NOTE]
>
>Änderungen an diesem neuen Fragment werden nicht in der E-Mail oder Vorlage übernommen, aus der es stammt. Wenn der ursprüngliche Inhalt in dieser E-Mail oder Vorlage bearbeitet wird, wird das neue Fragment nicht gleichermaßen geändert.-->

## Verwalten Ihrer Inhaltsfragmente {#manage-fragments}

Sie können ein Inhaltsfragment in der Fragmentliste bearbeiten, aktualisieren, duplizieren oder löschen.

### Bearbeiten und Aktualisieren eines Inhaltsfragments {#edit-fragments}

Gehen Sie wie folgt vor, um ein Inhaltsfragment zu bearbeiten:

1. Klicken Sie in der Liste **[!UICONTROL Fragmente]** auf den Namen des zu bearbeitenden Fragments.
1. Klicken Sie auf die Schaltfläche **Inhalt bearbeiten**, um den Inhalt dieses Fragments zu öffnen.

   ![](assets/fragment-edit-content.png)

1. Nehmen Sie die erforderlichen Änderungen vor und speichern Sie diese.

>[!CAUTION]
>
>Jede Änderung an einem Fragment wird an die Sendungen oder Vorlagen weitergegeben, die es verwenden.

### Löschen eines Inhaltsfragments {#delete-fragments}

Gehen Sie wie folgt vor, um ein Inhaltsfragment zu löschen:

1. Navigieren Sie zur Fragmentliste und klicken Sie neben dem zu löschenden Fragment auf die Schaltfläche **[!UICONTROL Mehr Aktionen]**.
1. Klicken Sie auf **Löschen** und bestätigen Sie den Vorgang.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Beim Löschen eines Fragments werden die Sendungen und Vorlagen, die dieses Fragment verwenden, aktualisiert: Das Fragment wird aus dem Inhalt entfernt, wird aber trotzdem noch referenziert. Um den Fragmentinhalt in diesen Sendungen und Vorlagen zu behalten, müssen Sie die Vererbung aufheben, bevor Sie das Fragment löschen, [wie in diesem Abschnitt beschrieben](use-visual-fragments.md#break-inheritance).

### Duplizieren eines Inhaltsfragments {#duplicate-fragments}

Sie können ein Inhaltsfragment einfach duplizieren, um ein neues zu erstellen. Gehen Sie wie folgt vor, um ein vorhandenes Fragment zu duplizieren:

1. Navigieren Sie zur Fragmentliste und klicken Sie neben dem zu duplizierenden Fragment auf die Schaltfläche **[!UICONTROL Mehr Aktionen]**.
1. Klicken Sie auf **Duplizieren** und bestätigen Sie den Vorgang.
1. Geben Sie den Titel des neuen Fragments ein und speichern Sie die Änderungen.

   Das Fragment wird der Liste der Inhaltsfragmente hinzugefügt. Sie können sie bearbeiten und nach Bedarf konfigurieren.
