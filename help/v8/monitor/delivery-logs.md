---
audience: end-user
title: Überwachen von Versandlogs
description: Erfahren Sie, wie Sie Versandlogs überwachen
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 100%

---

# Überwachen von Versandlogs {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Versandlogs"
>abstract="Die Versandlogs zeigen die Details des Versands an. Sie zeigen die Details des Versands, welche Zielgruppe ausgeschlossen wurde und warum, sowie die Tracking-Informationen wie Öffnungen und Klicks."

Nachdem der Versand vorbereitet wurde und Sie auf die Schaltfläche **Senden** geklickt haben, können Sie in den Versandlogs die Warnungen, Fehler, Status, Ausschlüsse und Tracking-Daten überprüfen. Diese Logs können direkt über das Nachrichten-Dashboard aufgerufen werden. Sie zeigen die Details des Versands, welche Zielgruppe ausgeschlossen wurde und warum, sowie die Tracking-Informationen wie Öffnungen und Klicks.

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

![](assets/logs.png)


## Sendungen {#deliveries-tab}

Der Tab **Versandlogs** zeigt die Liste der einzelnen Nachrichten eines Versands. Hier wird die Liste der gesendeten Nachrichten und deren Status gespeichert. Für jeden einzelnen Empfänger können Sie anhand des Status das Ergebnis des Versands verfolgen.

![](assets/logs2.png)

## Ausschlüsse {#exclusion-tab}

Die Registerkarte **Ausschlusslogs** zeigt die Liste aller aus der Zielgruppe ausgeschlossenen Nachrichten an und den Grund für den fehlgeschlagenen Versand.

![](assets/logs3.png)

## Ausschlussgründe {#exclusion-causes-tab}

Die Registerkarte **Ausschlussgründe** zeigt für jede mögliche Ursache die Anzahl der Nachrichten an, die von der Zielgruppe ausgeschlossen wurden.

![](assets/logs4.png)

## Getrackte URLs {#tracked-urls-tab}

Die Registerkarte **Getrackte URLs** gibt Auskunft über die in den gesendeten Nachrichten enthaltenen URLs, ihren Typ sowie ihre Quell-URLs.

![](assets/logs5.png)

## Tracking {#tracking-tab}

In der Registerkarte **Tracking** wird der Tracking-Verlauf für den jeweiligen Versand angezeigt. Hier werden die Tracking-Informationen zu allen von Adobe Campaign gesendeten Nachrichten aufgeführt, d. h. zu allen getrackten URLs.


![](assets/logs6.png)

>[!NOTE]
>
>Sollte das Tracking für einen Versand nicht aktiviert worden sein, wird diese Registerkarte nicht angezeigt.