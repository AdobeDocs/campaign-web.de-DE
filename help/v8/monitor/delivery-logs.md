---
audience: end-user
title: Überwachen von Versandlogs
description: Erfahren Sie, wie Sie Versandlogs überwachen
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Überwachen von Versandlogs {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Versandlogs"
>abstract="Die Versandlogs zeigen die Details des Versands an. Sie zeigen die Details des Versands, welche Zielgruppe ausgeschlossen wurde und warum, sowie die Tracking-Informationen wie Öffnungen und Klicks."

Nachdem der Versand vorbereitet wurde und Sie auf die Schaltfläche **Senden** geklickt haben, navigieren Sie zu den Versandlogs, um die Warnungen, Fehler, Status, Ausschlüsse und Tracking-Daten zu überprüfen. Diese Logs können direkt über das Nachrichten-Dashboard aufgerufen werden. Sie zeigen die Details des Versands, welche Zielgruppe ausgeschlossen wurde und warum, sowie die Tracking-Informationen wie Öffnungen und Klicks.

Um die Logs anzuzeigen, rufen Sie Ihr Versand-Dashboard auf und klicken Sie auf die Schaltfläche **Protokolle**.

Folgende Registerkarten stehen zur Verfügung:

* [Logs](#logs-tab)
* [Sendungen](#deliveries-tab)
* [Ausschlüsse](#exclusion-tab)
* [Ausschlussgründe](#exclusion-causes)
* [Getrackte URLs](#tracked-urls)
* [Tracking](#tracking)

## Logs {#logs-tab}

Die Registerkarte **Protokolle** enthält alle mit dem Versand und den Testsendungen verbundenen Nachrichten. Eventuelle Fehler oder Warnmeldungen werden durch spezifische Symbole hervorgehoben.

Alle Validierungsschritte, Warnungen und Fehler werden aufgelistet. Farbige Symbole zeigen den Nachrichtentyp an:

* Das blaue Symbol steht für eine informative Nachricht.
* Das gelbe Symbol steht für einen nicht kritischen Verarbeitungsfehler.
* Das rote Symbol steht für einen kritischen Fehler, der die Durchführung des Versands verhindert. Kritische Fehler müssen behoben sein, damit der Versand durchgeführt werden kann.

![&#x200B; Registerkarte „Logs“ mit Validierungsschritten, Warnungen und Fehlern mit farbigen Symbolen, die auf Nachrichtentypen hinweisen.](assets/logs.png){zoomable="yes"}

## Sendungen {#deliveries-tab}

Der Tab **Versandlogs** zeigt die Liste der einzelnen Nachrichten eines Versands. Hier wird die Liste der gesendeten Nachrichten und deren Status gespeichert. Für jeden einzelnen Empfänger können Sie anhand des Status das Ergebnis des Versands verfolgen.

![&#x200B; Registerkarte „Sendungen“ mit dem Verlauf der gesendeten Nachrichten und ihren Status.](assets/logs2.png){zoomable="yes"}

## Ausschlüsse {#exclusion-tab}

Die Registerkarte **Ausschlusslogs** zeigt die Liste aller aus der Zielgruppe ausgeschlossenen Nachrichten an und den Grund für den fehlgeschlagenen Versand.

![Registerkarte „Ausschlüsse“ mit den ausgeschlossenen Nachrichten und den Gründen für fehlgeschlagene Sendungen](assets/logs3.png){zoomable="yes"}

## Ausschlussgründe {#exclusion-causes-tab}

Die Registerkarte **Ausschlussgründe** zeigt für jede mögliche Ursache die Anzahl der Nachrichten an, die von der Zielgruppe ausgeschlossen wurden.

![Registerkarte „Ausschlussgründe“ mit der Anzahl der ausgeschlossenen Nachrichten für jeden Grund](assets/logs4.png){zoomable="yes"}

## Getrackte URLs {#tracked-urls-tab}

Die Registerkarte **Getrackte URLs** gruppiert die in den gesendeten Nachrichten enthaltenen URLs, ihren URL-Typ sowie ihre Quell-URL.

![Registerkarte „Getrackte URLs“ mit den in gesendeten Nachrichten enthaltenen URLs, ihre Typen und Quell-URLs.](assets/logs5.png){zoomable="yes"}

## Tracking {#tracking-tab}

Auf der Registerkarte **Tracking** wird der Tracking-Verlauf für den vorliegenden Versand angezeigt. Auf dieser Registerkarte werden Tracking-Daten zu den gesendeten Nachrichten angezeigt, einschließlich aller URLs, die von Adobe Campaign getrackt werden.

![Registerkarte „Tracking“ mit Tracking-Verlauf und -Daten für gesendete Nachrichten](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>Wenn das Tracking für einen Versand nicht aktiviert ist, wird diese Registerkarte nicht angezeigt.