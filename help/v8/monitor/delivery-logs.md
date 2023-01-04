---
audience: end-user
title: Versandlogs überwachen
description: Web-Dokumentation zu Campaign v8
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 13765b02288ec4682c5d55603c68f8ea1a5758f8
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 64%

---

# Versandlogs überwachen {#delivery-logs}

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Versandlogs"
>abstract="TBC"

Nach der Vorbereitung und dem Versand einer E-Mail können Sie mithilfe der Versandlogs überprüfen, ob kein Fehler vorliegt. Auf diese Protokolle kann direkt über das Nachrichten-Dashboard zugegriffen werden. In ihnen werden Details zum Versand dargestellt und Sie erfahren, welche Zielgruppe warum ausgeschlossen wurde sowie Tracking-Informationen wie z. B. Öffnungen und Klicks.

Um die Logs anzuzeigen, rufen Sie Ihr Versand-Dashboard auf und klicken Sie auf die Schaltfläche **Protokolle** Schaltfläche.

Es stehen mehrere Registerkarten zur Verfügung:

## Logs

Die **Protokolle** enthält alle Nachrichten bezüglich des Versands und der Testsendungen. Eventuelle Fehler oder Warnmeldungen werden durch spezifische Symbole hervorgehoben.

Alle Validierungsschritte, Warnungen und Fehler werden aufgelistet. Farbige Symbole zeigen den Nachrichtentyp an:

* Das graue Symbol zeigt eine informative Nachricht an.
* Das gelbe Symbol steht für einen nicht kritischen Verarbeitungsfehler.
* Das rote Symbol steht für einen kritischen Fehler, der die Durchführung des Versands verhindert.

![](assets/logs.png)

## Sendungen

Die **Sendungen** -Tab zeigt einen Verlauf aller Vorkommen dieses Versands an. sowie deren Status an. Für jeden einzelnen Empfänger können Sie anhand des Status das Ergebnis des Versands verfolgen.

![](assets/logs2.png)

## Ausschlüsse

Der Tab **Ausschlusslogs** zeigt die Liste der vom Versand ausgeschlossenen Empfänger und den jeweiligen Ausschlussgrund an.

![](assets/logs3.png)

## Ausschlussgründe

Der Tab **Ausschlussgründe** zeigt die Anzahl an ausgeschlossenen Empfängern pro Ausschlussgrund an.

![](assets/logs4.png)

## Getrackte URLs

Der Tab **Getrackte URLs** gibt Auskunft über die in der gesendeten Nachricht enthaltenen URLs, ihren Typ sowie ihre Quell-URLs.

![](assets/logs5.png)

## Tracking

Die **Tracking** enthält den Verlauf des Trackings für diesen Versand. Auf diesem Tab werden Tracking-Daten zu den gesendeten Nachrichten angezeigt, d. h. alle URLs, die der Verfolgung durch Adobe Campaign unterliegen.

>[!NOTE]
>
>Sollte das Tracking für einen Versand nicht aktiviert worden sein, wird dieser Tab nicht angezeigt.

![](assets/logs6.png)
