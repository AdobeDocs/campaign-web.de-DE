---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten können.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
TQID: https://experienceleague.adobe.com/EGP8dJLZGnGqQDiDfeal6wv5UL0ygtw9Y6F9SKLGrC8
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
subfeature_v2: id: e3988c18-3cfa-4f16-b812-ac2d2b1056fa
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 326
ht-degree: 100%

---

# Erste Schritte mit Versandwarnungen {#gs-delivery-alerting}

Bei Versandwarnungen handelt es sich um ein System zum Warnungs-Management, über das Benutzergruppen automatisch E-Mail-Benachrichtigungen mit Informationen zu ihren Versandausführungen erhalten. Empfängerinnen und Empfänger überwachen die von Adobe Campaign verarbeiteten Sendungen und ergreifen entsprechende Maßnahmen, wenn Fehler auftreten.

Benachrichtigungen werden basierend auf bestimmten Warnungskriterien angepasst, die über die Adobe Campaign Web-Benutzeroberfläche definiert werden.

Weitere Informationen zum Verwalten von Versandfehlern finden Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Inhalt der E-Mail-Benachrichtigung {#content}

E-Mail-Benachrichtigungen enthalten die folgenden Abschnitte:

* **Zusammenfassung**: Zeigt die Anzahl der Sendungen an, die den von Ihnen definierten Kriterien entsprechen, mit den Titeln und Farben für jedes Kriterium.
* **Details**: Führt alle für das Dashboard definierten Versandkriterien und die entsprechenden Sendungen für jedes Kriterium auf.

![Beschreibung: Dieser Screenshot zeigt das Layout der E-Mail-Benachrichtigung, einschließlich der Abschnitte „Zusammenfassung“ und „Details“.](assets/alerting-email.png)

## Einrichten von Versandwarnungen {#set-up}

Für die Einrichtung dieser Warnungen können Sie über die Campaign Web-Benutzeroberfläche Folgendes erstellen und verwalten:

* **Versandwarnungs-Dashboards**: Geben Sie Empfängerinnen und Empfänger an, legen Sie Warnungskriterien fest, die in das Dashboard aufgenommen werden sollen, und greifen Sie auf den Verlauf der gesendeten Warnungen zu. [Erfahren Sie, wie Sie mit Dashboards arbeiten](../msg/delivery-alerting-dashboards.md).
* **Versandwarnungskriterien**: Die Campaign Web-Benutzeroberfläche bietet vordefinierte Warnungskriterien wie Sendungen mit geringem Durchsatz oder Sendungen, deren Vorbereitung fehlgeschlagen ist. Sie können diese Kriterien zu Ihrem Dashboard hinzufügen oder eigene Kriterien erstellen, die Ihren Anforderungen entsprechen. [Erfahren Sie, wie Sie mit Kriterien arbeiten](../msg/delivery-alerting-criteria.md).

Sie können beispielsweise Benutzende mit Administratorrechten nur über fehlgeschlagene Sendungen benachrichtigen und Marketing-Benutzende über Sendungen mit einer hohen Softbounce-Fehlerrate informieren. Erstellen Sie dazu zwei separate Dashboards mit den entsprechenden Kriterien für jede Empfängergruppe.

>[!NOTE]
>
>Um Dashboards und Warnungskriterien öffnen und konfigurieren zu können, müssen Sie über **Administratorrechte** verfügen oder der Sicherheitsgruppe **Versand-Supervisoren** angehören. Standardmäßige Benutzerinnen und Benutzer können nicht auf Dashboards in der Adobe Campaign-Benutzeroberfläche zugreifen, aber Benachrichtigungen zu Warnungen empfangen. [Erfahren Sie mehr über Zugriff und Berechtigungen](../get-started/permissions.md).