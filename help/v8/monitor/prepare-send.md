---
audience: end-user
title: E-Mail vorbereiten und senden
description: Web-Dokumentation zu Campaign v8
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 15%

---

# E-Mail vorbereiten und senden {#prepare-send}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="E-Mail vorbereiten und senden"
>abstract="Erfahren Sie, wie Sie Ihre E-Mail vorbereiten und mehr über das Senden von KPIs erfahren."

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Versandvorbereitung{#prepare}

Wenn Sie Inhalt, Zielgruppe und Zeitplan definiert haben, können Sie Ihre Nachricht vorbereiten. Während der Vorbereitung wird die Zielpopulation berechnet und der Nachrichteninhalt für jedes Profil in der Zielgruppe erzeugt. Sobald die Vorbereitung abgeschlossen ist, können die Nachrichten entweder sofort oder zu dem geplanten Datum und der geplanten Uhrzeit gesendet werden. Die bei der Analyse verwendeten Validierungsregeln werden in diesem Abschnitt beschrieben. [Abschnitt](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies).

Gehen Sie dazu wie folgt vor:

1. Klicken Sie im Versand-Dashboard auf die **Vorbereiten** -Schaltfläche oben rechts klicken und bestätigen.

   ![](assets/prepare.png)

   Der Vorbereitungsfortschritt wird angezeigt. Abhängig von der Größe der Ziel-Population kann dieser Vorgang einige Zeit in Anspruch nehmen.

   >[!NOTE]
   >
   >Sie können die Vorbereitung jederzeit mit dem **Vorbereitung stoppen** Schaltfläche. Dies ist mit keinerlei Risiko verbunden, da in dieser Phase keine Nachrichten gesendet werden. Je nach Größe der Zielgruppe kann die Dauer der Versandvorbereitung variieren.

1. Wenn die Vorbereitung abgeschlossen ist, überprüfen Sie die KPIs. Wenn die Anzahl zu sendender Nachrichten nicht Ihren Erwartungen entspricht, ändern Sie Ihre Audience und starten Sie die Vorbereitung neu.

   ![](assets/prepare2.png)

   Im Folgenden werden die verschiedenen KPIs angezeigt:

   * **Targeting**: Anzahl der Zielgruppenempfänger
   * **Zu liefern**: die Anzahl der zu sendenden Nachrichten,
   * **Ausschließen**: Anzahl der Nachrichten, die durch eine Typologieregel ausgeschlossen sind

1. Klicken Sie auf **Protokolle** und vergewissern Sie sich, dass kein Fehler vorliegt. Der letzte Logeintrag zeigt eventuelle Fehler und deren Anzahl an. Weiterführende Informationen hierzu finden Sie in [diesem Abschnitt](delivery-logs.md).

   ![](assets/prepare-logs.png)

Wenn die Vorbereitung einen kritischen Fehler erkennt, der den Versand verhindert, wird der Vorbereitungsstatus im Versand-Dashboard als fehlgeschlagen angezeigt.

![](assets/prepare-error.png)

Wenn Sie nach der Vorbereitung Änderungen an Ihrem Versand vornehmen müssen, müssen Sie die Vorbereitung neu starten, damit diese Änderungen berücksichtigt werden.

Sobald die Vorbereitung ohne Fehler abgeschlossen ist, kann Ihre Nachricht gesendet werden. Weiterführende Informationen hierzu finden Sie in [diesem Abschnitt](#send).

## Senden der Nachricht{#send}

Sobald die Vorbereitung abgeschlossen ist, können Sie Ihre Nachricht senden. Dieser Schritt ist nur für Nachrichten erforderlich, die sofort gesendet werden. Wenn die Nachricht terminiert ist, wird sie zum definierten Datum gesendet.

Führen Sie folgende Schritte aus:

1. Klicken Sie im Versand-Dashboard auf die **Senden** oben rechts klicken und bestätigen.

   ![](assets/send.png)

1. Der Versandfortschritt wird angezeigt. Überprüfen Sie die angezeigten KPIs. Sie können auch die Protokolle überprüfen. Weiterführende Informationen hierzu finden Sie in [diesem Abschnitt](delivery-logs.md).

   ![](assets/send2.png)

   Im Folgenden werden die verschiedenen KPIs angezeigt:

   * **Zugestellt**: die Anzahl der erfolgreich gesendeten Nachrichten. Der Prozentsatz basiert auf der Gesamtzahl der Zielgruppenempfänger.
   * **Öffnungen**: die Anzahl der geöffneten Nachrichten. Der Prozentsatz basiert auf der Anzahl der zugestellten Nachrichten.
   * **Klicks**: die Anzahl der Empfänger, die mindestens einmal in der E-Mail geklickt haben. Der Prozentsatz basiert auf der Anzahl der zugestellten Nachrichten.

   >[!NOTE]
   >
   >Die **Öffnungen** und **Klicks** werden in Echtzeit aktualisiert.

   Sie können den Versand jederzeit anhalten und dann fortsetzen. Wenn Sie den Versand stoppen, während er gesendet wird, können Sie den Versand nicht fortsetzen.
