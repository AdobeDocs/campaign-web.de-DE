---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Erste Schritte mit Versandwarnungen {#gs-delivery-alerting}

Versandwarnung ist ein Warnhinweissystem, mit dem Benutzergruppen automatisch E-Mail-Benachrichtigungen mit Informationen zu ihren Versandausführungen erhalten können. Empfänger können laufende Sendungen, die von Adobe Campaign verarbeitet werden, überwachen und bei Problemen geeignete Maßnahmen treffen.

Benachrichtigungen können basierend auf bestimmten Warnungsbedingungen angepasst werden, die über die Adobe Campaign-Webbenutzeroberfläche definiert werden.

Weiterführende Informationen zur Verwaltung von fehlgeschlagenen Sendungen finden Sie im Abschnitt [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Inhalt der E-Mail-Benachrichtigung {#content}

E-Mail-Benachrichtigungen enthalten die folgenden Abschnitte:

* **Zusammenfassung**: Zeigt die Anzahl der Sendungen an, die Ihren definierten Kriterien entsprechen, einschließlich Titel und Farben für jede Bedingung.
* **Details**: Listet alle definierten Versandkriterien für das Dashboard und die entsprechenden Sendungen für jede Bedingung auf.

![](assets/alerting-email.png)

## Versandwarnungen einrichten {#set-up}

Um Sie bei der Einrichtung dieser Warnungen zu unterstützen, können Sie über die Campaign-Webbenutzeroberfläche Folgendes erstellen und verwalten:

* **Versandwarnungs-Dashboards**: Geben Sie Empfänger an, legen Sie Warnungsbedingungen fest, die in das Dashboard aufgenommen werden sollen, und greifen Sie auf einen Verlauf gesendeter Warnungen zu. [Erfahren Sie, wie Sie mit Dashboards arbeiten.](../msg/delivery-alerting-dashboards.md)
* **Versandwarnungsbedingungen**: Die Campaign-Webbenutzeroberfläche bietet vordefinierte Warnungsbedingungen (Sendungen mit geringem Durchsatz, Sendungen, deren Vorbereitung fehlgeschlagen ist usw.), die Sie Ihrem Dashboard hinzufügen können. Sie können auch eigene Kriterien erstellen, die Ihren Anforderungen entsprechen. [Erfahren Sie, wie Sie mit Kriterien arbeiten.](../msg/delivery-alerting-criteria.md)

Angenommen, Sie möchten Benutzer mit Administratorrechten nur über fehlgeschlagene Sendungen benachrichtigen und Marketing-Benutzer über Sendungen mit einer hohen Softbounce-Fehlerrate informieren. Erstellen Sie dazu zwei separate Dashboards mit den entsprechenden Kriterien für jede Empfängergruppe.

>[!NOTE]
>
>Um auf Dashboards und Warnungsbedingungen zugreifen und diese konfigurieren zu können, benötigen Sie **Administratorrechte** oder Teil der **Versand-Supervisoren** Sicherheitsgruppe. Standardbenutzer können nicht auf Dashboards in der Adobe Campaign-Benutzeroberfläche zugreifen, aber Warnhinweise empfangen. [Weitere Informationen zu Zugriff und Berechtigungen](../get-started/permissions.md)
