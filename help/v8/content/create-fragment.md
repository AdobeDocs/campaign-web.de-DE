---
audience: end-user
title: Erstellen von Inhaltsfragmenten
description: Erfahren Sie, wie Sie Inhaltsfragmente erstellen
exl-id: 8f37e9e6-3085-4a68-9746-8ca34cfa4242
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1026'
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
>abstract="Geben Sie das Label des Fragments ein. Bei Bedarf können Sie weitere Optionen definieren, z. B. den internen Namen des Fragments, dessen Ordner und eine Beschreibung."

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Typ des Inhaltsfragments"
>abstract="Wählen Sie den Fragmenttyp aus, den Sie erstellen möchten. **Visuelle Fragmente** sind vordefinierte visuelle Bausteine, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. **Ausdrucksfragmente** sind vordefinierte Ausdrücke, die über einen dedizierten Eintrag im Ausdruckseditor verfügbar sind."

Es gibt zwei Möglichkeiten, Inhaltsfragmente zu erstellen:

* Erstellen Sie ein Fragment mithilfe des dediziertes Menüs **[!UICONTROL Fragmente]** von Grund auf neu. [Weitere Informationen dazu](#create-from-scratch)
* Speichern Sie beim Entwerfen von Inhalten einen Teil des Inhalts als Fragment. [Weitere Informationen](#save-as-fragment)

  >[!NOTE]
  >
  >Diese Funktion ist nur für visuelle Fragmente verfügbar. Ausdrucksfragmente werden ausschließlich über das Menü **Fragmente** erstellt.

Nach dem Speichern kann Ihr Inhaltsfragment in beliebigen Versand- oder Inhaltsvorlagen verwendet werden.

## Erstellen eines Inhaltsfragments von Grund auf {#create-from-scratch}

Gehen Sie wie folgt vor, um ein Inhaltsfragment von Grund auf neu zu erstellen.

1. [Rufen Sie die Fragmentliste](#access-manage-fragments) über das linke Menü unter **[!UICONTROL Content-Management]** > **[!UICONTROL Fragmente]** auf und wählen Sie **[!UICONTROL Fragment erstellen]** aus.

   ![Bildschirm der Fragmentliste mit der Option „Fragment erstellen“](assets/fragments-list.png)

1. Geben Sie das Label des Fragments ein. Definieren Sie bei Bedarf weitere Optionen, z. B. den internen Namen des Fragments, dessen Ordner und eine Beschreibung.

1. Wählen Sie den zu erstellenden Fragmenttyp aus: **Visuelles Fragment** oder **Ausdrucksfragment**. [Lernen Sie die Unterschiede zwischen visuellen und Ausdrucksfragmenten kennen](fragments.md)

   ![Bildschirm zur Fragmenterstellung mit Typauswahl](assets/fragment-create.png)

   >[!AVAILABILITY]
   >
   >Für visuelle Fragmente ist eine Aktualisierung auf Campaign v8.6.4 erforderlich. Weitere Informationen finden Sie in den [Versionshinweisen zur Client Console von Campaign v8](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/releases/release-notes).

1. Klicken Sie auf die Schaltfläche **Erstellen**.

   * Für **visuelle Fragmente** wird der [E-Mail-Designer](../email/get-started-email-designer.md) angezeigt. Bearbeiten Sie den Inhalt nach Bedarf, so wie bei jeder anderen E-Mail in einer Kampagne. Klicken Sie anschließend auf die Schaltfläche **Speichern und schließen**. Fügen Sie Bilder, Links, Personalisierungsfelder und dynamische Inhalte hinzu.

     ![Bildschirm des E-Mail-Designers für visuelle Fragmente](assets/fragment-designer.png)

   * Für **Ausdrucksfragmente** wird der Ausdruckseditor geöffnet. Nutzen Sie die Personalisierungs- und Authoring-Funktionen, um den Inhalt zu erstellen, und klicken Sie dann auf **Bestätigen**. [Erfahren Sie mehr über die Arbeit mit dem Ausdruckseditor](../personalization/personalize.md)

     ![Bildschirm des Ausdruckseditors für Ausdrucksfragmente](assets/fragment-expression.png)

1. Wenn der Inhalt bereit ist, klicken Sie auf **Speichern**.

Das Inhaltsfragment kann nun beim Erstellen eines beliebigen Versands oder [Inhaltsvorlagen](../email/use-email-templates.md) in Campaign verwendet werden. In diesem Abschnitt erfahren Sie, wie Sie visuelle und Ausdrucksfragmente verwenden:
* [Hinzufügen visueller Fragmente zu E-Mails](use-visual-fragments.md)
* [Hinzufügen von Ausdrucksfragmenten zum Ausdruckseditor](use-expression-fragments.md)

## Speichern von Inhalt als visuelles Fragment {#save-as-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Als Fragment speichern"
>abstract="Um Inhalt als visuelles Fragment zu speichern, wählen Sie die Elemente aus, die in das Fragment aufgenommen werden sollen, einschließlich Personalisierungsfeldern und dynamischer Inhalte. Es können nur benachbarte Abschnitte ausgewählt werden. Leere Strukturen oder andere Inhaltsfragmente können nicht ausgewählt werden. Der Inhalt wird dann zu einem eigenständigen Fragment, das zur Fragmentliste hinzugefügt wurde und das über das dedizierte Menü aufgerufen werden kann. Dieses Fragment kann beim Erstellen einer E-Mail oder Inhaltsvorlage in Campaign verwendet werden."

<!--pas vu dans l'UI-->

Jeder E-Mail-Inhalt kann zur späteren Wiederverwendung als visuelles Fragment gespeichert werden. Speichern Sie beim Entwerfen einer [Inhaltsvorlage](../email/use-email-templates.md) oder eines [E-Mail-Versands](../email/get-started-email-designer.md) einen Teil des Inhalts als visuelles Fragment. Gehen Sie dazu wie folgt vor:

1. Klicken Sie oben rechts auf dem Bildschirm im [E-Mail-Designer](../email/get-started-email-designer.md) auf **Mehr**.

1. Wählen Sie im Dropdown-Menü die Option **[!UICONTROL Als Fragment speichern]** aus.

   ![Option „Als Fragment speichern“ im E-Mail-Designer](assets/fragment-save-as.png)

1. Der Bildschirm **[!UICONTROL Als Fragment speichern]** wird angezeigt. Wählen Sie die Elemente aus, die in das Fragment aufgenommen werden sollen, z. B. Personalisierungsfelder und dynamische Inhalte.

   >[!CAUTION]
   >
   >Es können nur benachbarte Abschnitte ausgewählt werden. Leere Strukturen oder andere Inhaltsfragmente können nicht ausgewählt werden.

   ![Bildschirm „Als Fragment speichern“ mit Elementauswahl](assets/fragment-save-as-screen.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Geben Sie den Fragmentnamen an und speichern Sie es.

   ![Bestätigungsbildschirm zum Speichern visueller Fragmente](assets/fragment-save-confirm.png)

   Dieser Inhalt ist jetzt ein eigenständiges Fragment, das zur [Fragmentliste](#manage-fragments) hinzugefügt wurde und das über das dedizierte Menü aufgerufen werden kann. Verwenden Sie dieses Fragment beim Erstellen von [E-Mails](../email/get-started-email-designer.md) oder [Inhaltsvorlagen](../email/use-email-templates.md) in Campaign. [Weitere Informationen](../content/use-visual-fragments.md)

>[!NOTE]
>
>Änderungen an diesem neuen Fragment werden nicht in der E-Mail oder Vorlage übernommen, aus der es stammt. Wenn der ursprüngliche Inhalt in dieser E-Mail oder Vorlage bearbeitet wird, wird das neue Fragment gleichermaßen nicht geändert.

## Verwalten Ihrer Inhaltsfragmente {#manage-fragments}

Sie können ein Inhaltsfragment in der Fragmentliste bearbeiten, aktualisieren, duplizieren oder daraus löschen.

### Bearbeiten und Aktualisieren eines Inhaltsfragments {#edit-fragments}

Gehen Sie wie folgt vor, um ein Inhaltsfragment zu bearbeiten:

1. Klicken Sie in der Liste **[!UICONTROL Fragmente]** auf den Namen des zu bearbeitenden Fragments.
1. Klicken Sie auf die Schaltfläche **Inhalt bearbeiten**, um den Inhalt des Fragments zu öffnen.

   ![Schaltfläche „Inhalt bearbeiten“ für Fragmente](assets/fragment-edit-content.png)

1. Nehmen Sie die erforderlichen Änderungen vor und speichern Sie diese.

>[!CAUTION]
>
>Änderungen an einem Fragment werden an die Sendungen oder Vorlagen weitergegeben, die es verwenden.

### Löschen eines Inhaltsfragments {#delete-fragments}

Gehen Sie wie folgt vor, um ein Inhaltsfragment zu löschen:

1. Navigieren Sie zur Fragmentliste und klicken Sie neben dem zu löschenden Fragment auf die Schaltfläche **[!UICONTROL Mehr Aktionen]**.
1. Klicken Sie auf **Löschen** und bestätigen Sie den Vorgang.

   ![Option „Löschen“ in der Fragmentliste](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Beim Löschen eines Fragments werden Sendungen und Vorlagen, in denen es verwendet wird, aktualisiert. Das Fragment wird aus dem Inhalt entfernt, aber nach wie vor referenziert. Um den Fragmentinhalt in diesen Sendungen und Vorlagen zu behalten, unterbrechen Sie die Vererbung, bevor Sie das Fragment löschen, [wie in diesem Abschnitt beschrieben](use-visual-fragments.md#break-inheritance).

### Archivieren eines Inhaltsfragments {#archive}

Sie können die Fragmentliste bereinigen, indem Sie die Fragmente archivieren, die für Ihre Marke nicht mehr relevant sind. Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Mehr Aktionen]** neben dem gewünschten Fragment und wählen Sie **[!UICONTROL Archivieren]** aus. Das Fragment wird aus der Fragmentliste entfernt. Dadurch wird verhindert, dass es in zukünftigen E-Mails oder Vorlagen von Benutzenden verwendet wird.

Verwenden Sie für den Zugriff auf archivierte Fragmente das Filterfenster, um sie anzuzeigen. Um die Archivierung eines Fragments aufzuheben, klicken Sie auf die Schaltfläche **[!UICONTROL Mehr Aktionen]** und wählen Sie **[!UICONTROL Archivierung aufheben]** aus.

![Option „Archivierung aufheben“ für Fragmente](assets/fragment-unarchive.png)

>[!NOTE]
>
>Wenn Sie ein Fragment archivieren, das in einem Inhalt verwendet wird, wirkt sich dies nicht auf diesen Inhalt aus.

### Duplizieren eines Inhaltsfragments {#duplicate-fragments}

Sie können ein Inhaltsfragment einfach duplizieren, um ein neues zu erstellen. Gehen Sie wie folgt vor, um ein vorhandenes Fragment zu duplizieren:

1. Navigieren Sie zur Fragmentliste und klicken Sie neben dem zu duplizierenden Fragment auf die Schaltfläche **[!UICONTROL Mehr Aktionen]**.
1. Klicken Sie auf **Duplizieren** und bestätigen Sie den Vorgang.
1. Geben Sie das Label des neuen Fragments ein und speichern Sie die Änderungen.

   Das Fragment wird der Liste der Inhaltsfragmente hinzugefügt. Bearbeiten und konfigurieren Sie es nach Bedarf.