---
audience: end-user
title: Berechtigungsverwaltung in der Campaign Web-Benutzeroberfläche
description: Erfahren Sie mehr über Berechtigungen in der Campaign Web-Benutzeroberfläche
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f352f4e726eff50527d0b9a04d0506600c12b822
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 26%

---


# Berechtigungen {#permissions}

Jeder Benutzer in Adobe Campaign verfügt über eigene Berechtigungen und Einschränkungen in der Anwendung. Der Benutzer kann Teil der Benutzergruppe sein und erbt die Berechtigungen der Gruppe.

Je nach Berechtigung kann ein Benutzer:

* Zugriff auf bestimmte Fähigkeiten
* Zugriff auf bestimmte Daten
* Zugriff auf bestimmte Aktionen (Erstellen, Ändern, Löschen)

Ausführliche Anweisungen zum Einrichten von Berechtigungen in Adobe Campaign finden Sie in der Dokumentation zu [Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"} .

## Berechtigungen für Ordner {#folder-permissions}

Gemäß Ihren Berechtigungen können Sie die Berechtigungen für Ordner in den **[!UICONTROL Ordnereinstellungen]** anzeigen und verwalten.

Nachfolgend finden Sie ein Beispiel für einen Versandordner:

![](assets/folder_settings.png){zoomable="yes"}

Im Abschnitt **[!UICONTROL Sicherheit]** der **[!UICONTROL Ordnereinstellungen]** können Sie Benutzer oder Gruppen, die Zugriff auf den Ordner haben, anzeigen und verwalten (hinzufügen oder löschen).

![](assets/folder_security.png){zoomable="yes"}

Sie können direkt auf die Berechtigungen klicken und sie entweder **[!UICONTROL Zulässig]** oder **[!UICONTROL Verweigert]** ändern.

![](assets/folder_security_denied.png){zoomable="yes"}

Wenn die Variable **[!UICONTROL Ausdehnen]** aktiviert ist, werden alle für einen Ordner definierten Berechtigungen auf alle zugehörigen Unterordner angewendet. Diese Berechtigungen können für jeden Unterordner überschrieben werden.

Wenn die Option **[!UICONTROL Systemordner]** aktiviert ist, ist der Zugriff für alle Benutzer unabhängig von ihren Berechtigungen zulässig.

Sie können auch [die Berechtigungen für Ordner in der Adobe Campaign-Konsole verwalten](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Alle Berechtigungen in der Campaign-Web-Benutzeroberfläche werden mit den Berechtigungen der Campaign Client Console synchronisiert.
