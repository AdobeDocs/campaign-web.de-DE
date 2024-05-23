---
audience: end-user
product: campaign
title: Arbeiten mit Inhaltsvorlagen
description: Erfahren Sie, wie Sie Vorlagen erstellen, um Inhalte in Adobe Campaign-E-Mails wiederzuverwenden
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 100%

---

# Arbeiten mit Inhaltsvorlagen {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Inhaltsvorlagen "
>abstract="Um den Design-Prozess zu beschleunigen und zu verbessern, können Sie eigenständige E-Mail-Vorlagen erstellen, um benutzerdefinierte Inhalte in Adobe Campaign einfach wiederzuverwenden. Diese Inhaltsvorlagen können von Grund auf neu erstellt werden, basierend auf integrierten oder benutzerdefinierten Vorlagen, die aus einem vorhandenen Inhalt erstellt oder in den Inhaltsvorlagen-Editor importiert werden."

Um den Design-Prozess zu beschleunigen und zu verbessern, können Sie eigenständige Vorlagen erstellen, um benutzerdefinierte Inhalte in [!DNL Adobe Campaign] einfach wiederzuverwenden. Diese Inhaltsvorlagen können von Grund auf neu erstellt werden, basierend auf integrierten oder benutzerdefinierten Vorlagen, die aus einem vorhandenen Inhalt erstellt oder in den Inhaltsvorlagen-Editor importiert werden.

Diese Funktion ermöglicht es inhaltsorientierten Benutzenden, an eigenständigen Vorlagen zu arbeiten, sodass Marketing-Benutzende diese in ihren E-Mail-Kampagnen wiederverwenden und anpassen können.

>[!NOTE]
>
>Derzeit werden nur **E-Mail**-Inhaltsvorlagen unterstützt.

## Zugreifen auf Inhaltsvorlagen {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Bearbeiten des Vorlageninhalts"
>abstract="Klicken Sie auf die Schaltfläche **Inhalt bearbeiten**, um Ihre Inhalte mit dem E-Mail-Designer zu aktualisieren."

Um auf die Liste der Inhaltsvorlagen zuzugreifen, navigieren Sie über die linke Leiste zum Menü **[!UICONTROL Content-Management]** > **[!UICONTROL Inhaltsvorlagen]**.

![](assets/content-template-list.png){zoomable="yes"}

In diesem Dashboard werden alle verfügbaren Inhaltsvorlagen als Liste angezeigt. Über die Dropdown-Liste können Sie nach einem bestimmten [Ordner](../get-started/permissions.md#folders) filtern oder mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzufügen.

![](assets/content-template-list-filters.png){zoomable="yes"}

In der Liste können Sie vorhandene Inhaltsvorlagen bearbeiten, duplizieren oder löschen. Verwenden Sie die Schaltfläche im oberen Bereich, um eine Inhaltsvorlage zu erstellen.


## Erstellen von Inhaltsvorlagen {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Inhaltsvorlage – Design"
>abstract="Entwerfen Sie Ihre E-Mail-Inhaltsvorlage."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Inhaltsvorlage – Auswahl"
>abstract="Wählen Sie Ihre E-Mail-Inhaltsvorlage aus."

Inhaltsvorlagen können durch das [Speichern einer vorhandenen E-Mail als Vorlage](#save-as-template) oder aus der Liste der E-Mail-Vorlagen über die Schaltfläche **Inhaltsvorlage erstellen** erstellt werden, [wie unten dargestellt](#create-template-from-scratch).

Nachdem Sie diese Vorlage gespeichert haben, können Sie sie beim Erstellen eine [E-Mail](../email/create-email.md) in [!DNL Adobe Campaign] verwenden. [Weitere Informationen dazu](use-email-templates.md)

>[!NOTE]
>
>* Änderungen an Inhaltsvorlagen werden nicht in E-Mails übernommen.
>
>* Wenn Vorlagen in einer E-Mail verwendet werden, wirken sich Änderungen an Ihrem E-Mail-Inhalt nicht auf die zuvor verwendete Inhaltsvorlage aus.

### Erstellen einer neuen Inhaltsvorlage {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Definieren von Eigenschaften für Vorlagen"
>abstract="Definieren Sie die Eigenschaften Ihrer E-Mail-Inhaltsvorlage, um sie bei Bedarf ganz einfach abrufen zu können."

Gehen Sie wie folgt vor, um im Dashboard für Inhaltsvorlagen eine neue Inhaltsvorlage zu erstellen:

1. Navigieren Sie über die linke Leiste **[!UICONTROL Content-Management]** > **[!UICONTROL Inhaltsvorlagen]** zu der Liste mit den Inhaltsvorlagen.

1. Wählen Sie **[!UICONTROL Vorlage erstellen]** aus.

   ![](assets/content-template-create.png){zoomable="yes"}

1. Geben Sie den Titel und die Eigenschaften der Vorlage ein. Sie können den Ordner auswählen, in dem Sie Ihre Vorlage speichern möchten. Standardmäßig werden Inhaltsvorlagen in einem dedizierten Ordner der Adobe Campaign-Hierarchie gespeichert: **[!UICONTROL Explorer]** > **[!UICONTROL Ressourcen]** > **[!UICONTROL Vorlagen]** > **[!UICONTROL Inhaltsvorlagen]**. Weitere Informationen über Ordner finden Sie auf [dieser Seite](../get-started/permissions.md#folders).

   ![](assets/content-template-details.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Erstellen]** und wählen Sie aus den verschiedenen Optionen aus, wie Sie Ihre Vorlage entwerfen möchten:

   * [E-Mail von Grund auf neu erstellen](create-email-content.md) über die Benutzeroberfläche des E-Mail-Designers.

   * [Rohes HTML kodieren oder einfügen](code-content.md) direkt im E-Mail-Designer.

   * [Vorhandenen HTML-Inhalt importieren](existing-content.md) aus einer Datei oder einem ZIP-Ordner.

   * Verwenden Sie vorhandenen Inhalt aus einer Liste integrierter oder benutzerdefinierter Vorlagen. Die Schritte zur Verwendung einer Inhaltsvorlage in einer E-Mail werden in [diesem Abschnitt](use-email-templates.md) beschrieben.

   ![](assets/email_designer-templates.png){zoomable="yes"}

1. Der E-Mail-Designer wird angezeigt. Bearbeiten Sie Ihren Inhalt nach Bedarf, so wie Sie es bei jeder anderen E-Mail auch tun würden, je nach der von Ihnen gewählten Option. Mehr über die Arbeit mit dem E-Mail-Designer erfahren Sie in [diesem Abschnitt](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Wenn die Vorlage fertig ist, klicken Sie auf **[!UICONTROL Speichern]**.

   Klicken Sie bei Bedarf auf den Pfeil neben dem Vorlagennamen, um zum Bildschirm **[!UICONTROL Details]** zurückzukehren und die Vorlage zu bearbeiten.

   ![](assets/content-template-save-back.png){zoomable="yes"}

Die Vorlage ist in der Liste **[!UICONTROL Inhaltsvorlagen]** verfügbar. [Weitere Informationen](#access-templates)

Anhand dieser Vorlage können Sie nun einen neuen Inhalt erstellen: Sie finden ihn in der Registerkarte **[!UICONTROL Gespeicherte Vorlagen]** des E-Mail-Designers. [Weitere Informationen dazu](use-email-templates.md)

### Speichern von E-Mail-Inhalten als Vorlage {#save-as-template}

Sobald Sie [eine E-Mail gestaltet haben](create-email-content.md), können Sie diesen Inhalt als Vorlage speichern, um ihn später wiederzuverwenden. Gespeicherte Vorlagen stehen allen in Ihrer Adobe Campaign-Umgebung zur Verfügung.

Gehen Sie wie folgt vor, um E-Mail-Inhalte als Vorlage zu speichern:

1. Klicken Sie im E-Mail-Designer oben rechts im Bildschirm auf **[!UICONTROL Mehr]**.

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Als Inhaltsvorlage speichern]** aus.

   ![](assets/email_designer-save-template.png){zoomable="yes"}

1. Geben Sie einen Namen für diese Vorlage ein und speichern Sie sie.

   ![](assets/email_designer-template-name.png){zoomable="yes"}

Die Vorlage wird gespeichert und in der Liste **[!UICONTROL Inhaltsvorlagen]** angezeigt. Sie wird zu einer eigenständigen Inhaltsvorlage, die Sie wie jedes andere Element in der Liste öffnen, bearbeiten und löschen können. [Weitere Informationen](#access-manage-templates)

Anhand dieser Vorlage können Sie nun einen neuen Inhalt erstellen: Sie finden ihn in der Registerkarte **[!UICONTROL Gespeicherte Vorlagen]** des E-Mail-Designers. [Weitere Informationen dazu](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable="yes"}


>[!NOTE]
>
>Änderungen an dieser neuen Vorlage werden nicht an die E-Mail-Adresse weitergeleitet, von der sie stammen. Wenn der ursprüngliche Inhalt in dieser E-Mail bearbeitet wird, wird die neue Vorlage ebenfalls nicht geändert.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## Ändern einer Inhaltsvorlage {#modify-delete}

Gehen Sie wie folgt vor, um eine vorhandene Inhaltsvorlage zu aktualisieren:

1. Wählen Sie in der Liste der Inhaltsvorlagen den Titel der zu ändernden Vorlage aus, um sie zu bearbeiten.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]**, um den Inhalt mit dem [E-Mail-Designer](get-started-email-designer.md) zu aktualisieren.

![](assets/content-template-edition.png){zoomable="yes"}

>[!NOTE]
>
>Änderungen an Inhaltsvorlagen werden bei Verwendung dieser Inhaltsvorlage nicht in E-Mails übernommen.

## Löschen einer Inhaltsvorlage {#content-delete}

Sie haben zwei Möglichkeiten, eine Inhaltsvorlage zu löschen:

* Klicken Sie in der Liste der Inhaltsvorlagen auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Löschen** aus.

  ![Löschen einer Inhaltsvorlage aus dem Dashboard](assets/content-template-list-delete.png)

* Klicken Sie in der Inhaltsvorlage selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Löschen** aus.


>[!NOTE]
>
>Das Löschen einer Inhaltsvorlage hat keine Auswirkungen auf Sendungen, die bereits mit dieser Vorlage erstellt wurden.


## Duplizieren einer Inhaltsvorlage {#content-duplicate}

Sie haben zwei Möglichkeiten, eine Inhaltsvorlage zu duplizieren:

* Klicken Sie in der Liste der Inhaltsvorlagen auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Duplizieren** aus.

* Klicken Sie in der Inhaltsvorlage selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Duplizieren** aus.

Bestätigen Sie in beiden Fällen die Duplizierung, um die neue Inhaltsvorlage zu erstellen. Der Titel der neuen Inhaltsvorlage lautet **Kopie von`<label of the initial campaign`**. Gehen Sie zu den Vorlageneinstellungen, um diesen Titel zu aktualisieren.

