---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 2%

---

# Erste Schritte mit Versandwarnungen {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Versandwarnung"
>abstract="Versandwarnung ist jetzt in Campaign verfügbar. Diese Funktion ist ein Warnhinweissystem, mit dem Benutzergruppen automatisch E-Mail-Benachrichtigungen mit Informationen zu ihren Versandausführungen erhalten können."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

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
