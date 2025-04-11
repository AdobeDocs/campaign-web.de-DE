---
audience: end-user
title: Transaktionsnachrichten
description: Informationen zu Transaktionsnachrichten mit Adobe Campaign Web
exl-id: 90830dca-acff-4aa3-a88b-1005e349cf52
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 44%

---

# Informationen zu Transaktionsnachrichten {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="Transaktionsnachrichten"
>abstract="Transaktionsnachrichten sind ein spezielles Modul in Adobe Campaign, das für die Verarbeitung ausgelöster Nachrichten entwickelt wurde."

<!-- >>[!CONTEXTUALHELP]
>id="acw_transacmessages_exclusionlogs"
>title="Transactional messaging exclusion logs"
>abstract="Transactional messaging exclusion logs" -->

Transaktionsnachrichten sind ein spezielles Modul in Adobe Campaign, das für die Verarbeitung ausgelöster Nachrichten entwickelt wurde. Diese Nachrichten werden automatisch als Reaktion auf Ereignisse generiert, die aus Informationssystemen stammen. Häufige Beispiele für solche Ereignisse sind das Klicken auf Schaltflächen oder Links, der Warenkorbabbruch, das Anfordern von Warnhinweisen zur Produktverfügbarkeit, die Erstellung oder Änderung eines Kontos.

Transaktionsnachrichten dienen zum Senden von:

* wichtigen Benachrichtigungen, z. B. Bestellbestätigungen oder Rücksetzungen von Passwörtern,
* Echtzeit-Reaktionen auf Kundenaktionen, wie z. B. Kontoerstellung oder Kaufabschluss,
* Inhalten, bei denen es sich nicht um Werbung handelt und die für Kundeninteraktionen wichtig sind.

Das Transaktionsnachrichten-Modul lässt sich nahtlos in Ihre Informationssysteme integrieren. Ereignisse, z. B. Kundenaktionen, werden an Adobe Campaign gepusht, das die entsprechende personalisierte Nachricht sendet. Diese Nachrichten können einzeln oder in Batches über verschiedene Kanäle wie E-Mail, SMS oder Push-Benachrichtigungen gesendet werden.

Sie finden das Modul für **[!UICONTROL Transaktionsnachrichten]** im Abschnitt **[!UICONTROL Ausgelöste Nachrichten]**.

![Schnittstelle für Transaktionsnachrichten mit ausgelösten Nachrichten und deren Status](assets/transactional.png){zoomable="yes"}

Die Seite „Transaktionsnachricht **[!UICONTROL enthält drei Registerkarten]**:

* **[!UICONTROL Durchsuchen]**, wobei Sie die Liste der Transaktionsnachrichten mit ihrem Status haben,
* **[!UICONTROL Vorlagen]**, in denen Sie die Transaktionsnachrichtenvorlagen finden und erstellen,
* **[!UICONTROL History]**, wo Sie die Details zu allen ausgeführten Transaktionsnachrichten haben.

In dieser Dokumentation erhalten Sie weitere Informationen zu folgenden Themen:

* [Erstellen von Transaktionsnachrichten](create-transactional.md) mithilfe einer Vorlage und Kennenlernen der dafür erforderlichen Einstellungen,
* [Validieren des Inhalts Ihrer Transaktionsnachrichten ](validate-transactional.md) Simulieren der Personalisierung,
* [Überwachen von Transaktionsnachrichten](monitor-transactional.md).