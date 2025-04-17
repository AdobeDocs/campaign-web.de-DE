---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten können.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 42%

---

# Erste Schritte mit Versandwarnungen {#gs-delivery-alerting}

Versandwarnungen sind ein System zur Verwaltung von Warnhinweisen, mit dem Benutzergruppen automatisch E-Mail-Benachrichtigungen mit Informationen zu ihren Versandausführungen erhalten können. Empfänger und Empfängerinnen überwachen die von Adobe Campaign verarbeiteten Sendungen und ergreifen geeignete Maßnahmen, wenn Probleme auftreten.

Benachrichtigungen werden anhand spezifischer Warnkriterien angepasst, die in der Web-Benutzeroberfläche von Adobe Campaign definiert sind.

Weitere Informationen zur Verwaltung von fehlgeschlagenen Sendungen finden Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

## Inhalt der E-Mail-Benachrichtigung {#content}

E-Mail-Benachrichtigungen enthalten die folgenden Abschnitte:

* **Zusammenfassung**: Zeigt die Anzahl der Sendungen an, die den von Ihnen definierten Kriterien entsprechen, mit den Titeln und Farben für jedes Kriterium.
* **Details**: Führt alle für das Dashboard definierten Versandkriterien und die entsprechenden Sendungen für jedes Kriterium auf.

![Beschreibung: Dieser Screenshot zeigt das Layout der E-Mail-Benachrichtigung, einschließlich der Abschnitte Zusammenfassung und Details.](assets/alerting-email.png)

## Einrichten von Versandwarnungen {#set-up}

Um diese Warnhinweise einzurichten, können Sie in der Web-Benutzeroberfläche von Campaign folgende Elemente erstellen und verwalten:

* **Versandwarnungs-Dashboards**: Geben Sie Empfängerinnen und Empfänger an, legen Sie Warnungskriterien fest, die in das Dashboard aufgenommen werden sollen, und greifen Sie auf den Verlauf der gesendeten Warnungen zu. [Erfahren Sie, wie Sie mit Dashboards arbeiten](../msg/delivery-alerting-dashboards.md).
* **Kriterien für Versandwarnungen**: Die Web-Benutzeroberfläche von Campaign bietet vordefinierte Warnkriterien, wie Sendungen mit geringem Durchsatz oder Sendungen, deren Vorbereitung fehlgeschlagen ist. Sie können diese Kriterien zu Ihrem Dashboard hinzufügen oder eigene Kriterien erstellen, die Ihren Anforderungen entsprechen. [Erfahren Sie, wie Sie mit Kriterien arbeiten](../msg/delivery-alerting-criteria.md).

Benachrichtigen Sie beispielsweise Benutzende mit Administratorrechten nur über fehlgeschlagene Sendungen und Marketing-Benutzende über Sendungen mit einer hohen Softbounce-Fehlerquote. Erstellen Sie dazu zwei separate Dashboards mit den entsprechenden Kriterien für jede Empfängergruppe.

>[!NOTE]
>
>Um Dashboards und Warnungskriterien öffnen und konfigurieren zu können, müssen Sie über **Administratorrechte** verfügen oder der Sicherheitsgruppe **Versand-Supervisoren** angehören. Standardmäßige Benutzerinnen und Benutzer können nicht auf Dashboards in der Adobe Campaign-Benutzeroberfläche zugreifen, aber Benachrichtigungen zu Warnungen empfangen. [Weitere Informationen zu Zugriff und Berechtigungen](../get-started/permissions.md).