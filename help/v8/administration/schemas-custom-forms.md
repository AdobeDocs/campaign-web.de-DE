---
title: Arbeiten mit benutzerdefinierten Formularen
description: Erfahren Sie, wie Sie Einträge in benutzerdefinierten Schemata mithilfe von Dateneingabeformularen erstellen, bearbeiten und verwalten.
exl-id: c997d676-bfe1-4e28-9e11-41e902a782c1
source-git-commit: 9d7ff3bc648567640ef501bff2228e5c6cff25bc
workflow-type: ht
source-wordcount: '416'
ht-degree: 100%

---

# Arbeiten mit benutzerdefinierten Formularen {#custom-forms}

Benutzerdefinierte Formulare sind Dateneingabeschnittstellen, mit denen Sie Einträge in benutzerdefinierten Schemata direkt über die Web-Benutzeroberfläche verwalten können. Jedes benutzerdefinierte Formular entspricht einem bestimmten benutzerdefinierten Schema und bietet eine Listenansicht zum Durchsuchen von Einträgen und eine Detailansicht zum Erstellen, Bearbeiten und Löschen von Einträgen.

Benutzerdefinierte Formulare basieren auf der Formulardefinition (Bildschirmdefinition) des Schemas, die konfiguriert, welche Felder angezeigt werden und wie sie organisiert sind.

>[!NOTE]
>
>Benutzerdefinierte Formulare sind nur für Schemata verfügbar, für die eine Formulardefinition konfiguriert ist.

## Erstellen und Veröffentlichen der benutzerdefinierten Schemata {#form-schema}

Zunächst müssen Sie Ihre benutzerdefinierten Schemata erstellen und veröffentlichen. Ausführliche Informationen finden Sie in [diesem Abschnitt](schemas-create-publish.md).

Im Folgenden finden Sie das für dieses Beispiel verwendete Datenmodell:

* Eine Empfängerin bzw. ein Empfänger tätigt mehrere Käufe
* Ein Kauf wird mit einem Produkt verknüpft
* Ein Produkt wird mit einer Marke verknüpft

Für diesen Anwendungsfall werden drei Schemata erstellt: die Schemata „Käufe“, „Produkte“ und „Marke“. Hier ein Beispiel:

![Benutzerdefinierte Formulare](assets/schemas-forms.png)

## Konfigurieren der Bildschirmdefinition {#form-screen-schema}

Legen Sie fest, welche Felder angezeigt und wie sie organisiert werden. Ausführliche Informationen finden Sie in [diesem Abschnitt](schemas-browse-access.md#screen-def).

Im Folgenden finden Sie ein Beispiel für das Markenschema, bei dem die benutzerdefinierte Liste „Produkte“ hinzugefügt wird. Das Formular zeigt dann die Liste der mit der Marke verknüpften Produkte an.

![Benutzerdefinierte Formulare](assets/schemas-forms2.png)

Für das Schema „Produkte“ fügen wir die benutzerdefinierte Liste „Käufe“ hinzu. Und für das Schema „Käufe“ die Felder „Produkt“ und „Empfänger“.

## Erstellen von Navigationseinträgen {#form-screen-entries}

Erstellen Sie Ordner im Explorer, um auf Ihr benutzerdefiniertes Formular zuzugreifen. Ausführliche Informationen finden Sie in [diesem Abschnitt](schemas-create-publish.md#navigation).

![Benutzerdefinierte Formulare](assets/schemas-forms3.png)

Die Listenansicht zeigt alle Einträge für dieses Schema an. Wenn für das Schema eine Formulardefinition konfiguriert ist, kann die Liste bearbeitet werden und Sie können Einträge erstellen, bearbeiten und löschen.
![Benutzerdefinierte Formulare](assets/schemas-forms4.png)

Anschließend können Sie:

* **Einträge anzeigen und bearbeiten:** Klicken Sie in der Listenansicht auf einen Eintrag, um ihn in der Detailansicht zu öffnen und Felder direkt zu bearbeiten.
* **Neue Einträge erstellen:** Klicken Sie auf die Schaltfläche **[!UICONTROL Erstellen]** und füllen Sie die erforderlichen Felder aus. Verwenden Sie für verknüpfte Felder das Suchsymbol, um aus verfügbaren verknüpften Einträgen auszuwählen.
* **Einträge löschen:** Wählen Sie einen Eintrag aus und verwenden Sie die Löschaktion, die in der Eintragsdetails- oder Listenansicht verfügbar ist.
* **Verwandte Daten in Registerkarten anzeigen:** Greifen Sie über spezielle Registerkarten in der Detailansicht auf verwandte Einträge zu (zeigen Sie beispielsweise alle mit einer Marke verknüpften Produkte oder alle mit einem Produkt verknüpften Käufe an).
* **Filter anwenden:** Verwenden Sie das Panel „Filter“, um die Listenansicht zu verfeinern und spezifische Einträge basierend auf einem beliebigen Feld in Ihrem Schema zu finden.
* **Listenspalten anpassen:** Mit dieser Option können Sie über die Bildschirmdefinition konfigurieren, welche Spalten in Listenansichten standardmäßig angezeigt werden.
