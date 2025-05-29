---
audience: end-user
title: Berechtigungsverwaltung in der Campaign Web-Benutzeroberfläche
description: Erfahren Sie mehr über Berechtigungen in der Campaign Web-Benutzeroberfläche
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: 692a9badf72e465791e6f964d02753e7f1a25713
workflow-type: ht
source-wordcount: '296'
ht-degree: 100%

---

# Berechtigungen {#permissions}

Jede Benutzerin und jeder Benutzer in Adobe Campaign hat spezifische Berechtigungen und Einschränkungen in der Anwendung. Benutzerinnen und Benutzer können zu einer Benutzergruppe gehören und die Berechtigungen der Gruppe erben.

Benutzerinnen und Benutzer haben je nach Berechtigung:

* Zugriff auf bestimmte Fähigkeiten
* Zugriff auf bestimmte Daten
* Zugriff auf bestimmte Aktionen (Erstellen, Ändern, Löschen)

Detaillierte Anweisungen zum Festlegen von Berechtigungen in Adobe Campaign sind in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"} verfügbar.

## Berechtigungen für Ordner {#folder-permissions}

Basierend auf Ihren Berechtigungen können Sie die Berechtigungen für Ordner in den **[!UICONTROL Ordnereinstellungen]** anzeigen und verwalten.

Hier ist ein Beispiel für einen Versandordner:

![Beispiel für Ordnereinstellungen in Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

Unter **[!UICONTROL Ordnereinstellungen]** können Sie im Abschnitt **[!UICONTROL Sicherheit]** Benutzende oder Gruppen, die Zugriff auf den Ordner haben, anzeigen und verwalten (hinzufügen oder löschen).

![Beispiel für die Sicherheitseinstellungen eines Ordners in Adobe Campaign](assets/folder_security.png){zoomable="yes"}

Sie können direkt auf die Berechtigungen klicken und sie entweder in **[!UICONTROL Zulässig]** oder **[!UICONTROL Abgelehnt]** ändern.

![Beispiel für abgelehnte Berechtigungen in den Sicherheitseinstellungen eines Ordners](assets/folder_security_denied.png){zoomable="yes"}

>[!NOTE]
>
>Sie sollten kein Objekt erstellen können, für das Sie nicht über mindestens einen Ordner mit Schreibrechten verfügen.
>
>Sie müssen nicht Teil des Admin-Teams sein, um Fragmente zu erstellen, benötigen aber Schreibrechte für mindestens einen Ordner „Inhalt – Visuelle Fragmente“. Andernfalls können Sie kein visuelles Fragment erstellen.

Wenn die Option **[!UICONTROL Ausdehnen]** aktiviert ist, werden alle für einen Ordner definierten Berechtigungen auf alle zugehörigen Unterordner angewendet. Diese Berechtigungen können für jeden Unterordner überschrieben werden.

Wenn die Option **[!UICONTROL Systemordner]** aktiviert ist, haben alle Benutzenden unabhängig von ihren Berechtigungen Zugriff.

Sie können auch [die Berechtigungen für Ordner in der Adobe Campaign-Konsole verwalten](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Alle Berechtigungen in der Benutzeroberfläche von Campaign Web werden mit den Berechtigungen der Campaign-Client-Konsole synchronisiert.