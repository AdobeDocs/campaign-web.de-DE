---
audience: end-user
title: Berechtigungsverwaltung in Campaign Web
description: Erfahren Sie mehr über Berechtigungen in Campaign Web v8
badge: label="Beta"
source-git-commit: 3cd540af6ccccdecc4d41983d4d11ffb1ea72c43
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 33%

---


# Zugriff und Berechtigungen {#access-and-permissions}


>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="Berechtigung erforderlich"
>abstract="Ihr Administrator muss Ihnen die Berechtigung erteilen, bevor Sie dieses Objekt erstellen können."



Die Zugriffskontrolle kann den Zugriff auf Objekte und Daten aus Hauptlisten, wie Sendungen, Empfängerinnen bzw. Empfänger oder Workflows, einschränken. Diese Einschränkungen gelten auch für die Navigationsstruktur des Explorers. Darüber hinaus benötigen Sie Berechtigungen zum Erstellen, Löschen, Duplizieren und Bearbeiten von Objekten über die Benutzeroberfläche.

Die Zugriffskontrolle wird in der Client-Konsole verwaltet. Alle Berechtigungen in Campaign Web werden mit den Berechtigungen der Campaign-Client-Konsole synchronisiert. Nur Campaign-Admins können Benutzerberechtigungen definieren und ändern. Weitere Informationen zu Benutzerberechtigungen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=de){target="_blank"}.

Wenn Sie die Campaign-Webbenutzeroberfläche durchsuchen, können Sie abhängig von Ihren Berechtigungen auf Daten, Objekte und Funktionen zugreifen. Wenn Sie beispielsweise keine Zugriffsberechtigungen für einen Ordner haben, können Sie ihn nicht sehen. Ihre Berechtigungen wirken sich auch auf die Objekte- und Datenverwaltung aus. Ohne Schreibberechtigungen für einen bestimmten Ordner können Sie einen Versand nicht in diesem Ordner erstellen, selbst wenn er in der Benutzeroberfläche angezeigt wird.

## Berechtigungen anzeigen {#view-permissions}

Aus dem **Explorer** können Sie die Berechtigungen für die einzelnen Ordner durchsuchen. Diese Berechtigungen werden in der Clientkonsole festgelegt und zum Organisieren und Steuern des Zugriffs auf Campaign-Daten verwendet.


Gehen Sie wie folgt vor, um Berechtigungen für einen Ordner anzuzeigen:

1. Aus dem **Explorer** Wählen Sie im linken Navigationsmenü einen Ordner aus.
1. Klicken Sie auf die drei Punkte oben rechts und wählen Sie **Ordnerberechtigungen**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. Überprüfen Sie die Details im Bildschirm wie unten gezeigt:

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   Eine Gruppe oder ein Benutzer kann Lese-, Schreib- und/oder Löschberechtigungen für Daten erhalten, die im ausgewählten Ordner gespeichert sind.

   Wenn die Variable **Propagat** aktiviert ist, werden alle für einen Ordner definierten Berechtigungen auf alle zugehörigen Unterordner angewendet. Diese Berechtigungen können für jeden Unterordner überschrieben werden.

   Wenn die Variable **Systemordner** aktiviert ist, ist der Zugriff für alle Benutzer unabhängig von deren Berechtigungen zulässig.

Erfahren Sie mehr über die Ordnerberechtigungen in [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## Arbeiten mit Ordnern {#folders}

Sie können Ordner erstellen, umbenennen, neu anordnen und verschieben, um Ihre Komponenten und Daten zu organisieren. Sie können Ordner auch aus demselben Menü löschen.

>[!CAUTION]
>
>Beim Löschen eines Ordners werden auch alle im Ordner gespeicherten Daten gelöscht.

Gehen Sie wie folgt vor, um einen Ordner zu erstellen:

1. Aus dem **Explorer** Wählen Sie im linken Navigationsmenü einen Ordner aus.
1. Klicken Sie auf die drei Punkte oben rechts und wählen Sie **Erstellen neuer Unterordner**.
1. Geben Sie den Namen des Ordners ein und speichern Sie ihn.

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   Der Ordner wird als Unterordner des aktuellen Ordners hinzugefügt. Navigieren Sie zu diesem neuen Ordner, um Komponenten direkt darin zu erstellen. Sie können eine Komponente auch aus einem beliebigen Ordner erstellen und in diesem neuen Ordner speichern, indem Sie die **Zusätzliche Optionen** -Abschnitt der Eigenschaften, wie unten für einen Versand dargestellt:

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}
