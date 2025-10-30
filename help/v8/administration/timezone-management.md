---
title: Zeitzonen-Management
description: Erfahren Sie, wie die Adobe Campaign Web-Benutzeroberfläche Datums- und Zeitwerte basierend auf der Zeitzone des Browsers, der Benutzerin oder des Benutzers, des Workflows und des Servers anzeigt.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 100%

---

# Zeitzonen-Management {#timezone-management}

Die Adobe Campaign Web-Benutzeroberfläche zeigt alle Datums- und Zeitwerte entsprechend der **lokalen Zeitzone des Webbrowsers der oder des Benutzenden** an. Dieses Verhalten kann zu Abweichungen führen, wenn Zeitstempel zwischen der Web-Benutzeroberfläche und der Client-Konsole verglichen werden.

In diesem Abschnitt werden die zu erwartenden Unterschiede zwischen den Zeitzonen der **Web-Benutzeroberfläche**, der **Client-Konsole** und der **Workflow-Ausführung** erklärt.

>[!NOTE]
>
>Auf dem Server gespeicherte Daten werden nicht geändert. Nur die Anzeige in der Benutzeroberfläche ändert sich.

## Schlüsselkonzepte

* **Server-Zeitzone**: Die Server-Zeitzone entspricht der im Betriebssystem des Servers konfigurierten Zeitzone. Alle Zeitstempel werden intern auf dem Server in UTC gespeichert.

* **Verhalten der Client-Konsole**: Die Client-Konsole zeigt Zeitstempel anhand der **Zeitzone der oder des Benutzenden** an, die in den Benutzereinstellungen definiert ist. Standardmäßig entspricht dies der **Zeitzone des Servers**.

* **Verhalten der Web-Benutzeroberfläche**: Die Web-Benutzeroberfläche zeigt Zeitstempel anhand der **lokalen Zeitzone des Browsers** an. Wenn Benutzende die Zeitzone des Browsers oder des Systems ändern, werden die angezeigten Datums-/Zeitwerte automatisch aktualisiert.

* **Verhalten des Workflows**: Workflows interpretieren lokale Zeitstempel basierend auf der **im Workflow konfigurierten Zeitzone**. Falls nicht anders angegeben, wird standardmäßig die **Zeitzone des Servers** verwendet.

## Beispiel

| Benutzeroberfläche | Verwendete Zeitzone | Beispielanzeige |
|------------|----------------|-----------------|
| Client-Konsole | Benutzende (Standard = Server) | `2025-10-20 14:00:00` |
| Web-Benutzeroberfläche | Lokale Zeitzone des Browsers | `2025-10-20 21:00:00` (für Browser in UTC +7) |

In diesem Beispiel verweisen beide Benutzeroberflächen auf denselben zugrunde liegenden UTC-Zeitstempel, aber jede rendert ihn in einer anderen Zeitzone.

## Auswirkung

Unterschiede in den angezeigten Zeiten können auftreten bei:

* Profil- oder Datenfeldern, die `datetime`-Werte enthalten
* Versandprotokollen oder Kontaktdaten
* Workflow-Ausführung und Import-Zeitstempeln

Die zugrunde liegenden Daten bleiben identisch. Der Unterschied besteht lediglich im **Rendern**.

>[!NOTE]
>
>Wenn Benutzende aus mehreren Regionen auf derselben Instanz zusammenarbeiten, können scheinbare Abweichungen zwischen den Zeitstempeln in der Web-Benutzeroberfläche und der Konsole auftreten.

## Empfehlungen

Um Anzeigewerte über Benutzeroberflächen hinweg anzupassen, haben Sie folgende Möglichkeiten:

* Ändern Sie die **Zeitzone Ihres Browsers**, sodass sie mit der **Zeitzone der Benutzenden oder des Servers** übereinstimmt.
* Achten Sie beim Exportieren von Daten (Exporte verwenden UTC) auf eine konsistente Konvertierung in den Reporting-Tools.
* Legen Sie beim Entwerfen von Workflows explizit die **Zeitzone des Workflows** in den Eigenschaften der Aktivität fest, um ein vorhersehbares Planungs- und Importverhalten zu gewährleisten.
* Weisen Sie Geschäftsanwendende darauf hin, dass Zeitstempelunterschiede zwischen den Ansichten der Web-Benutzeroberfläche und der Client-Konsole **normal und zu erwarten** sind.
