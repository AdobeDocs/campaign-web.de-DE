---
title: Migration von technischen Benutzerinnen und Benutzern zur Adobe Developer Console
description: Erfahren Sie, wie Sie die Benutzerzugriffsverwaltung von Campaign Standard auf Campaign v8 migrieren.
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 31befa42b04bef1a2777df9f2bd494481ccf67cd
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 5%

---

# Benutzerzugriffsverwaltung von Campaign Standard zu Campaign V8 {#user-management-acs}

Sowohl Adobe Campaign Standard als auch Adobe Campaign v8 ermöglichen es Benutzenden, Berechtigungen für verschiedene Benutzende/Benutzende zu definieren und zu verwalten. Diese Berechtigungen bestehen aus spezifischen Rechten, die Benutzern Zugriff auf verschiedene Funktionen des Produkts gewähren. Die beiden Produkte verwenden jedoch unterschiedliche Ansätze und Implementierungen für die Verwaltung des Benutzerzugriffs.

Die folgenden Konzepte werden in Adobe Campaign Standard und Campaign v8 verwendet, um die Benutzerzugriffsverwaltung zu ermöglichen:

| Campaign Standard | Campaign v8 |
|---------|----------|
| Benutzer | Operator |
| Rolle | Spezifische Berechtigung |
| Sicherheitsgruppe | Benutzergruppe |
| Organizational unit | Ordnerberechtigung |

## Migrationsansatz von der Sicherheitsgruppe zur Benutzergruppe

>[!CAUTION]
>
>Die Funktionen dieser Rollen/spezifischen Berechtigungen können in der Implementierung variieren und möglicherweise zu Autorisierungsproblemen führen (z. B. Berechtigungserweiterung oder Funktionsstörungen). Wir empfehlen Benutzern, diese Zuordnungen nach der Transition zu überprüfen, um eine ordnungsgemäße Zugriffssteuerung sicherzustellen. [Weitere Informationen zu Berechtigungen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

In der folgenden Tabelle wird der Migrationsansatz für Benutzergruppen beim Wechsel von Adobe Campaign Standard zu Campaign v8 beschrieben. In Campaign Standard wird eine **Sicherheitsgruppe** in Campaign v8 als **Benutzergruppe** bezeichnet, um einem Benutzer eine Reihe von Rollen zuzuweisen. Einige Sicherheitsgruppen/Benutzergruppen sind zwar vorkonfiguriert verfügbar, Benutzer können jedoch neue Gruppen erstellen oder bei Bedarf vorhandene ändern.

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologie**  | Sicherheitsgruppe | Benutzergruppe |

Sowohl in Adobe Campaign Standard als auch in Campaign v8 **Sicherheitsgruppen** und **Benutzergruppen** Produktprofilen in der Admin Console zugeordnet. Wenn Sie einem Benutzer eine **Sicherheitsgruppe** oder **Benutzergruppe** zuweisen möchten, können Sie das entsprechende **Produktprofil** in der Admin Console verknüpfen. Diese Zuordnung wird bei der Anmeldung des Benutzers synchronisiert. [Weitere Informationen zum Produktprofil](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Campaign Standard-Sicherheitsgruppe** | **Benutzergruppe von Campaign v8** |
|----------|---------|
| Administratoren | Administratoren |
| Versand-Verantwortliche | Administratoren |
| Workflow-Verantwortliche | Workflow-Supervisoren  |

## Migrationsansatz von Benutzerrollen zu spezifischen Berechtigungen

>[!CAUTION]
>
>Während der Migration von Adobe Campaign Standard zu Campaign v8 erhalten Benutzende mit der **Datenmodell**-Rolle, aber nicht **Administration** automatisch **Administration**-Zugriff, da für die Schemaerstellung in Campaign v8 Administratorrechte erforderlich sind. Um dies zu verhindern, entfernen Sie vor **Migration die** „Datenmodell“.

In Adobe Campaign Standard wird der Begriff **Benutzerrolle** in Campaign V8 **Spezifische Berechtigung** bezeichnet. In der folgenden Tabelle ist die Terminologie aufgeführt, die für **Spezifische Berechtigungen** in Campaign v8 verwendet wird und **Benutzerrollen** in Campaign Standard entspricht.

| **Campaign Standard-Benutzerrolle** | **Spezifische Berechtigung für Campaign v8** | **Beschreibung**  |
|----------|---------|---------|
| Administration | Administration | Ein Benutzer mit der Berechtigung Administration hat vollen Zugriff auf die Instanz. |
| Datenmodell  | Administration | Berechtigung zum Ausführen von Veröffentlichungen und Erstellen benutzerdefinierter Ressourcen. Funktion zur Schemaerstellung verfügbar für Admins in Campaign v8.  |
| Zustellbarkeit  | Administration  | Recht auf Validierung zuvor analysierter Sendungen.  |
| Exportieren | Exportieren | Recht auf Datenexport.  |
| Dateizugriff  | Dateizugriff  | Recht auf Validierung zuvor analysierter Sendungen.  |
| Allgemeiner Import  | importieren  | Recht auf allgemeinen Datenimport |
| Sendungen vorbereiten | Sendungen vorbereiten | Berechtigung zur Erstellung, Änderung, Vorbereitung und Löschung von Sendungen.  |
| Ausführung von SQL-Scripts | Ausführung von SQL-Scripts | Berechtigung zur Ausführung eines beliebigen SQL-Befehls direkt in der Datenbank. |
| Sendungen starten  | Sendungen starten  | Recht auf Validierung zuvor analysierter Sendungen.  |
| Ausführung des Systembefehls | Programmausführung | Berechtigung zur Ausführung von Systembefehlen auf dem Server. |
| Workflow | Workflow | Berechtigung zur Verwaltung der Ausführung von Workflows, Start, Stopp, Pause usw. |

## Migrationsansatz von der Organisationseinheit

>[!CAUTION]
>
>Organisationseinheiten in Adobe Campaign Standard ohne **Alle (alle)** als direkt oder indirekt übergeordnetes Element werden nicht nach Campaign V8 migriert.
></br>
>Benutzern in mehreren Sicherheitsgruppen wird die Organisationseinheit der höchsten Sicherheitsgruppe zugewiesen. Wenn mehrere Gruppen parallele Einheiten der obersten Ebene haben, ist die Anmeldung in Campaign Standard eingeschränkt, gewährt aber nach der Migration breiteren Zugriff in Campaign v8, was zu einer Eskalation der Berechtigungen führen kann. Um dies zu verhindern, vermeiden Sie die Zuweisung von Benutzern zu Sicherheitsgruppen mit parallelen Organisationseinheiten.

In Adobe Campaign Standard wird die **Organisationseinheit** dem in Campaign v8 vorhandenen **Ordner**-Hierarchiemodell zugeordnet, um eine ähnliche Zugriffssteuerung zu gewährleisten. [Weitere Informationen zur Ordnerverwaltung](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologie**  | Organizational unit | Ordner |

## Aus dem Programm stammender Migrationsansatz

In Campaign v8 werden **Programme** als **Ordner** dargestellt. Campaign v8 ermöglicht die Erstellung von Ordnern und die Einschränkung des Zugriffs darauf.

Durch die Verwendung von **Gruppen** und **spezifischen Berechtigungen** kann **Benutzern** Zugriff auf bestimmte **Ordner** innerhalb der Navigationshierarchie gewährt werden, mit der Möglichkeit, Lese-, Schreib- und Löschberechtigungen zuzuweisen. [Weitere Informationen zur Ordnerverwaltung](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Da ein **Programm** in Campaign v8 als **Ordner** behandelt wird, kann sein Zugriff auf dieselbe Weise wie für jeden anderen Ordner verwaltet werden. Nach der Migration können Campaign Standard-Administratoren die folgenden Schritte ausführen:

1. Klicken Sie im Explorer mit der rechten Maustaste auf einen beliebigen Ordner und wählen Sie **[!UICONTROL Eigenschaften…]**.

1. Navigieren Sie zur Registerkarte **[!UICONTROL Sicherheit]** .

1. Ändern Sie die Benutzergruppenberechtigungen entsprechend dem gewünschten Zugriffsmodell. 

## Produktprofilzuordnung für den Zugriff auf REST-APIs 

Für den Zugriff auf Transaktions-APIs über die Ausführungsinstanz in Campaign v8 ist **neues** Produktprofil) zusätzlich zu den Produktprofilen **Administrator** und **Message Center** erforderlich. Dieses **Produktprofil** wird bestehenden oder vorab erstellten technischen Konten in Campaign Standard hinzugefügt.

Nach der Migration sollten Campaign Standard-Benutzende ihre **Produktprofilzuordnungen** überprüfen und das entsprechende **Produktprofil** zuweisen, wenn sie ihre **technischen Konten** nicht mit dem **Administrator** Produktprofil verknüpfen möchten. Für zukünftige Integrationen empfehlen wir die Verwendung von Campaign V8 **Mandanten-ID** in der **REST-URL** anstelle der vorherigen Campaign Standard **Mandanten-ID**.

## Migration des Zugriffs auf integrierte Campaign-Ressourcen für Campaign Standard-Benutzer

Benutzende, die von Campaign Standard migriert wurden, haben Lesezugriff auf bestimmte integrierte Ressourcen in Campaign v8.

## Nicht migrierte Sicherheitsgruppen und -rollen {#non-migrated-groups-roles}

Nachfolgend finden Sie eine Liste der Campaign Standard-Rollen, die noch nicht umgestellt wurden:

* Standard-Relais-Konto 

* Message Center-Push 

Nachfolgend finden Sie eine Liste der Campaign Standard-Sicherheitsgruppenzuordnungen, die nicht übergegangen wurden.

* Message Center-Agenten

* Push-Agenten für Message Center

* Anwendungsverantwortlicher für Adobe Experience Manager

* Relais-Konto

Beachten Sie, dass benutzerdefinierte Rollen, die in Adobe Campaign Standard erstellt und Benutzenden zugewiesen wurden, nicht nach Campaign v8 migriert werden.
