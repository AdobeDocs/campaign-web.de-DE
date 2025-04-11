---
audience: end-user
title: Berechtigungsverwaltung in der Campaign Web-Benutzeroberfläche
description: Erfahren Sie mehr über Berechtigungen in der Campaign Web-Benutzeroberfläche
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 14%

---

# Berechtigungen {#permissions}

Jeder Anwender in Adobe Campaign verfügt über bestimmte Berechtigungen und Einschränkungen in der Anwendung. Der Benutzer kann einer Benutzergruppe angehören und die Berechtigungen der Gruppe übernehmen.

Basierend auf ihren Berechtigungen kann ein Benutzer:

* Zugriff auf bestimmte Funktionen
* Zugriff auf bestimmte Daten
* Zugriff auf bestimmte Aktionen (Erstellen, Ändern, Löschen)

Eine ausführliche Anleitung zum Einrichten von Berechtigungen in Adobe Campaign finden Sie in der Dokumentation zu [Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Berechtigungen für Ordner {#folder-permissions}

Basierend auf Ihren Rechten können Sie Berechtigungen für Ordner in den **[!UICONTROL Ordnereinstellungen“ anzeigen und]**.

Nachfolgend finden Sie ein Beispiel für einen Versandordner:

![Beispiel für Ordnereinstellungen in Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

Im Abschnitt **[!UICONTROL Sicherheit]** der **[!UICONTROL Ordnereinstellungen]** können Sie Benutzer oder Gruppen anzeigen und verwalten (hinzufügen oder löschen), die auf den Ordner zugreifen können.

![Beispiel für Ordnersicherheitseinstellungen in Adobe Campaign](assets/folder_security.png){zoomable="yes"}

Sie können direkt auf die Berechtigungen klicken und sie entweder in &quot;**[!UICONTROL &quot;]** &quot;**[!UICONTROL &quot;]**.

![Beispiel für verweigerte Berechtigungen in Ordnersicherheitseinstellungen](assets/folder_security_denied.png){zoomable="yes"}

Wenn die **[!UICONTROL Propagieren]**-Option aktiviert ist, gelten alle für einen Ordner definierten Berechtigungen für alle zugehörigen Unterordner. Diese Berechtigungen können für jeden Unterordner überschrieben werden.

Wenn die Option **[!UICONTROL Systemordner]** ausgewählt ist, wird der Zugriff allen Benutzern unabhängig von ihren Berechtigungen gewährt.

Sie können auch [die Berechtigungen für Ordner in der Adobe Campaign-Konsole verwalten](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Alle Berechtigungen in der Web-Benutzeroberfläche von Campaign werden mit den Berechtigungen der Campaign-Client-Konsole synchronisiert.