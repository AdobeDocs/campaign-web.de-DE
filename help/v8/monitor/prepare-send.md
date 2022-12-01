---
audience: end-user
title: E-Mail vorbereiten und senden
description: Webdokumentation zu Campaign v8
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 33%

---

# E-Mail vorbereiten und senden {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="E-Mail vorbereiten und senden"
>abstract="Erfahren Sie, wie Sie Ihre E-Mail vorbereiten und mehr über das Senden von KPIs erfahren."

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Versandvorbereitung

Während der Vorbereitung wird die Zielpopulation berechnet und der Nachrichteninhalt für jedes Profil in der Zielgruppe erzeugt. Sobald die Vorbereitung abgeschlossen ist, können die Nachrichten entweder sofort oder zu dem geplanten Datum und der geplanten Uhrzeit gesendet werden. Die bei der Analyse verwendeten Validierungsregeln werden in diesem Abschnitt beschrieben. [Abschnitt](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Klicken Sie auf **Vorbereiten** -Schaltfläche oben rechts.

1. Der Vorbereitungsfortschritt wird angezeigt. Abhängig von der Größe der Ziel-Population kann dieser Vorgang einige Zeit in Anspruch nehmen.

   >[!NOTE]
   >
   >Sie können die Vorbereitung jederzeit mit dem **Vorbereitung stoppen** Schaltfläche. Dies ist mit keinerlei Risiko verbunden, da in dieser Phase keine Nachrichten gesendet werden. Je nach Größe der Zielgruppe kann die Dauer der Versandvorbereitung variieren.

1. Wenn die Vorbereitung abgeschlossen ist, überprüfen Sie die **Targeting**, **Zu liefern** und **Ausschließen** KPIs. Wenn die Anzahl zu sendender Nachrichten nicht Ihren Erwartungen entspricht, ändern Sie Ihre Audience und starten Sie die Vorbereitung neu.

1. Klicken Sie auf **Protokolle** und vergewissern Sie sich, dass kein Fehler vorliegt. Alle Validierungsschritte, Warnungen und Fehler werden aufgelistet. Farbige Symbole zeigen den Nachrichtentyp an:

   * Das graue Symbol zeigt eine informative Nachricht an.
   * Das gelbe Symbol steht für einen nicht kritischen Verarbeitungsfehler.
   * Das rote Symbol steht für einen kritischen Fehler, der die Durchführung des Versands verhindert.

1. Nachdem Sie die Änderungen vorgenommen haben, starten Sie die Vorbereitung neu.

Nach Abschluss der Vorbereitung ist die Nachricht versandbereit. Weiterführende Informationen dazu finden Sie im Abschnitt Versand bestätigen.


## Senden der Nachricht

Nachdem die Vorbereitung abgeschlossen ist, führen Sie die folgenden Schritte aus, um Ihre Nachricht zu senden.

1. Klicken Sie auf **Schaltfläche Senden** in der oberen rechten Ecke und bestätigen Sie.

1. Der Versandfortschritt wird zusammen mit drei KPIs angezeigt: Zugestellt, Öffnungen, Klicks.

1. Schließen Sie den Sendevorgang ab, indem Sie auf die Schaltfläche OK klicken.

PROTOKOLLE

>[!NOTE]
>
>Wenn die Meldung geplant ist, wird sie gesendet, sobald die Sendezeit erreicht ist. Weiterführende Informationen zum Planen von Nachrichten finden Sie in diesem Abschnitt.

