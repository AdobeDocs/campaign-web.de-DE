---
title: Zeitzonen-Management
description: Erfahren Sie, wie die Adobe Campaign-Web-Benutzeroberfläche Datums- und Zeitwerte basierend auf Browser, Operator, Workflow und Server-Zeitzonen anzeigt.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 4%

---

# Zeitzonen-Management {#timezone-management}

Die Adobe Campaign-Web-Benutzeroberfläche zeigt alle Datums- und Zeitwerte entsprechend **lokalen Zeitzone des Webbrowsers des Benutzers** an. Dieses Verhalten kann beim Vergleich von Zeitstempeln zwischen der Web-Benutzeroberfläche und der Client-Konsole zu Unterschieden führen.

In diesem Abschnitt werden die erwarteten Unterschiede zwischen den Zeitzonen **Web**, **Client-**) und **Workflow-Ausführung** erläutert.

>[!NOTE]
>
>Auf dem Server gespeicherte Daten werden nicht geändert. Nur die Anzeige in der Benutzeroberfläche ändert sich.

## Schlüsselkonzepte

* **Zeitzone des Servers**: Die Zeitzone des Servers entspricht der Zeitzone, die auf dem Betriebssystem des Servers konfiguriert ist. Alle Zeitstempel werden intern in UTC auf dem Server gespeichert.

* **Verhalten der Client** Konsole: Die Client-Konsole zeigt Zeitstempel anhand der **Zeitzone des Benutzers** an, die in den Benutzereinstellungen definiert ist. Standardmäßig entspricht dies der **Zeitzone des Servers**.

* **Verhalten der Web** Benutzeroberfläche: Die Web-Benutzeroberfläche zeigt Zeitstempel mithilfe der **lokalen Zeitzone des Browsers**. Wenn ein(e) Benutzende(r) den Browser oder die Systemzeitzone ändert, werden die angezeigten Datums-/Zeitwerte automatisch aktualisiert.

* **Workflow-**: Workflows interpretieren lokale Zeitstempel basierend auf der konfigurierten **des Workflows**. Wenn kein Wert angegeben ist **wird standardmäßig die Zeitzone** Servers verwendet.

## Beispiel

| Benutzeroberfläche | Verwendete Zeitzone | Beispiel-Anzeige |
|------------|----------------|-----------------|
| Client-Konsole | Benutzer des Benutzers (Standard = Server) | `2025-10-20 14:00:00` |
| Web-Benutzeroberfläche | Lokale Zeitzone des Browsers | `2025-10-20 21:00:00` (für Browser in UTC +7) |

In diesem Beispiel verweisen beide Schnittstellen auf denselben zugrunde liegenden UTC-Zeitstempel, aber jede rendert ihn mit einer anderen Zeitzone.

## Auswirkung

Unterschiede in den angezeigten Zeiten können auftreten bei:

* Profil- oder Datenfelder, die `datetime` enthalten
* Versandlogs oder Kontaktdaten
* Workflow-Ausführung und Zeitstempel importieren

Die zugrunde liegenden Daten bleiben identisch. Der Unterschied besteht nur in **Rendering**.

>[!NOTE]
>
>Wenn Benutzende aus mehreren Regionen an derselben Instanz zusammenarbeiten, können offensichtliche Diskrepanzen zwischen den Zeitstempeln der Web-Benutzeroberfläche und der Konsole auftreten.

## Empfehlungen

Um Anzeigewerte über Schnittstellen hinweg auszurichten, haben Sie folgende Möglichkeiten:

* Ändern Sie **Zeitzone des Browsers** entsprechend der **Zeitzone des Benutzers oder Servers**.
* Stellen Sie beim Exportieren von Daten (Exporte verwenden UTC) in den Reporting-Tools eine konsistente Konvertierung sicher.
* Legen Sie beim Entwerfen von Workflows explizit die **Workflow-Zeitzone** in den Aktivitätseigenschaften fest, um ein vorhersehbares Planungs- und Importverhalten zu erzielen.
* Kommunizieren Sie Geschäftsbenutzern, dass die Zeitstempelunterschiede zwischen den Ansichten der Web-Benutzeroberfläche und der Client-Konsole **normal und erwartet** sind.
