---
title: Erstellen und Veröffentlichen von Schemata
description: Erfahren Sie, wie Sie Schemata erstellen, erweitern und veröffentlichen.
exl-id: 1da53fe0-1d64-4907-ba06-206f69e83d7c
source-git-commit: 0cc09a983d412889f2b734a5bfb30bf422247ec0
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# Erstellen und Veröffentlichen von Schemata {#create-publish}

## Erstellen und Verwalten von Schemata {#create-schemas}

Sie können neue Schemata erstellen, vorhandene Schemata erweitern und auf externe Datenbanken zugreifen.

### Erstellen oder Erweitern eines Schemas {#create-new}

So erstellen oder erweitern Sie ein Schema:

1. Navigieren Sie zu **[!UICONTROL Administration]** > **[!UICONTROL Schemata]**.
1. Klicken Sie auf **[!UICONTROL Schema erstellen]**.

   ![Dialog „Schemaerstellung“](assets/schemas-create1.png)

1. Geben Sie einen Namespace für Ihr Schema ein (z. B. `cus` für benutzerdefinierte Schemata).
1. Geben Sie einen eindeutigen Namen und ein eindeutiges Label ein und wählen Sie aus, ob Sie ein neues Schema erstellen oder ein vorhandenes erweitern möchten.

1. Wählen Sie **[!UICONTROL Erstellen]** aus.
   ![Dialog „Schemaerstellung“](assets/schemas-create2.png)

Das Schema wird erstellt und die generierte Schemastruktur wird angezeigt.

Standardmäßig ist das Schema leer. Jetzt müssen Sie die Felder, die Sie in Ihr Schema einbeziehen möchten, mit dem Schema-Editor hinzufügen:

1. Klicken Sie auf das Stiftsymbol im Abschnitt **[!UICONTROL Inhalt]** des Bildschirms mit den Schemadetails.
2. Fügen Sie die erforderlichen Elemente hinzu und speichern Sie sie. Im Folgenden finden Sie ein Beispiel für eine benutzerdefinierte Schemastruktur:

   ![Dialog „Schemaerstellung“](assets/schemas-create3.png)

Das System validiert automatisch die XML-Struktur und generiert das Schema.

### Definieren der Bildschirmbearbeitung {#define-attributes}

Nachdem Sie das Schema erstellt haben, müssen Sie die Bildschirmbearbeitung definieren.

Weitere Informationen zum Bildschirm „Bildschirmdefinition“ und zum Zugriff darauf finden Sie im Abschnitt [Zugreifen auf die Bildschirmdefinition](schemas-browse-access.md#screen-def).

In unserem Beispiel fügen wir einfach zwei benutzerdefinierte Felder hinzu:

1. Klicken Sie in der Detailansicht des Schemas auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**, um auf die Bildschirmdefinition zuzugreifen.

1. Klicken Sie oberhalb der Tabelle **[!UICONTROL Liste der benutzerdefinierten Felder]** auf das Symbol mit den Auslassungspunkten und wählen Sie **[!UICONTROL Attribute auswählen]**.
1. Wählen Sie die benutzerdefinierten Felder aus, die Sie hinzufügen möchten, und bestätigen Sie die Auswahl.

   ![Dialog „Schemaerstellung“](assets/schemas-create4.png)

## Veröffentlichen und Synchronisieren von Schemata {#publish}

Nachdem Sie ein Schema erstellt oder geändert haben, müssen Sie es veröffentlichen, um das logische Schema mit der physischen Datenbankstruktur zu synchronisieren.

### Veröffentlichen von Schemaänderungen {#publish-changes}

>[!CAUTION]
>
>Durch das Veröffentlichen von Schemaänderungen wird die Datenbankstruktur geändert. Seien Sie sich der Auswirkungen dieser Änderungen bewusst, bevor Sie die Veröffentlichung bestätigen.

So veröffentlichen Sie Ihre Schemaänderungen:

1. Navigieren Sie zu **[!UICONTROL Administration]** > **[!UICONTROL Schemata]**, um auf die Schemaliste zuzugreifen.
1. Klicken Sie auf **[!UICONTROL Veröffentlichung]** und bestätigen Sie den Vorgang.

   ![Dialogfeld für die Schemaveröffentlichung mit den anzuwendenden Änderungen](assets/schemas-publish1.png)

1. Wählen Sie in der Liste das Schema aus, das Sie synchronisieren möchten.

   ![Dialogfeld für die Schemaveröffentlichung mit den anzuwendenden Änderungen](assets/schemas-publish2.png)

1. Prüfen Sie das SQL-Skript, das zur Aktualisierung der Datenbankstruktur ausgeführt wird.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Veröffentlichen]**, um mit der Veröffentlichung fortzufahren.

>[!NOTE]
>
>Der Vorgang kann je nach Größe der Datenbank und Komplexität der Änderungen einige Zeit in Anspruch nehmen.

### Erstellen eines Navigationseintrags {#navigation}

Nach dem Veröffentlichen eines benutzerdefinierten Schemas können Sie im Explorer einen Navigationseintrag erstellen, um auf Ihre benutzerdefinierten Daten zuzugreifen:

1. Navigieren Sie zum **[!UICONTROL Explorer]**-Menü und wählen Sie einen Ordner aus, in dem Sie Ihr benutzerdefiniertes Schema platzieren möchten.
1. Klicken Sie auf das Symbol mit den Auslassungspunkten und dann auf **[!UICONTROL Neuen Ordner erstellen]**.
   ![Erstellen von Navigationseinträgen für ein benutzerdefiniertes Schema](assets/schemas-publish3.png)
1. Fügen Sie ein Label hinzu und wählen Sie Ihr Schema im Feld **[!UICONTROL Ordnertyp]** aus.
   ![Erstellen von Navigationseinträgen für ein benutzerdefiniertes Schema](assets/schemas-publish5.png)
1. Auf das benutzerdefinierte Schema kann jetzt über die Ansicht **[!UICONTROL Explorer]** zugegriffen werden.

Im neuen Ordner haben Sie folgende Möglichkeiten:

* Anzeigen der Liste der Einträge in Ihrem benutzerdefinierten Schema.
* Erstellen neuer Einträge.
* Bearbeiten und Löschen vorhandener Einträge.
* Anpassen, welche Spalten standardmäßig in der Listenansicht angezeigt werden.
