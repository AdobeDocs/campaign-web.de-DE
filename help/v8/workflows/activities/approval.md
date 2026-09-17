---
audience: end-user
title: Workflow-Aktivität „Validierung“
description: Weitere Informationen zur Verwendung der Workflow-Aktivität „Validierung“
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 100%
---
# Validierung {#approval}

>[!CONTEXTUALHELP]
>id="acw_orchestration_approval"
>title="Aktivität „Validierung“"
>abstract="Eine Aktivität des Typs **Validierung** erfordert die Beteiligung einer Benutzerin bzw. eines Benutzers. Weisen Sie die Aufgabe einer Gruppe oder einer einzelnen Benutzerin bzw. einem einzelnen Benutzer zu, passen Sie den Benachrichtigungstitel und die Nachricht an und definieren Sie die möglichen Antworten als Ausgabeverzweigungen."

Die Workflow-Aktivität **Validierung** ermöglicht es Ihnen, die Aufgabe einer Gruppe oder einer einzelnen Benutzerin bzw. einem einzelnen Benutzer zuzuweisen, den Titel und die Nachricht der Benachrichtigungs-E-Mail anzupassen und die möglichen Antworten (z. B. Ja/Nein) als Ausgabeverzweigungen zu definieren.

Verwenden Sie diese Aktivität, wenn ein Schritt in Ihrem Workflow zum Fortfahren eine menschliche Entscheidung erfordert, z. B. um ein Budget, eine Zielgruppe oder Inhalte genehmigen zu lassen, bevor der Workflow fortgesetzt wird.

## Funktionsweise des Validierungsprozesses {#process}

Es ist die Beteiligung von mindestens einer Benutzerin bzw. einem Benutzer erforderlich. Diese Aktivität stoppt den Workflow nicht komplett: Andere Aufgaben können ausgeführt werden, während auf eine Antwort gewartet wird.

Beim Warten auf eine Antwort wird die Aktivität auf der Arbeitsfläche als ausstehend angezeigt. Die verantwortliche Person antwortet über den Link in der Benachrichtigungsnachricht.

Der Ablauf der Validierungsaufgabe sieht wie folgt aus:

1. Erstellen Sie einen Workflow und konfigurieren Sie eine Aktivität des Typs **Validierung**.
1. Starten Sie den Workflow. Wenn die Aktivität **Validierung** erreicht wird, wird eine Aufgabe für die verantwortliche Person erstellt.
1. Die verantwortliche Person erhält die Benachrichtigungsnachricht, klickt auf den Link und wählt eine Antwort aus.
1. Sobald die verantwortliche Person antwortet, fährt der Workflow mit der Transition fort, die der Antwort entspricht.

Gehen Sie wie folgt vor, um diese Aktivität zu konfigurieren:

1. [Weitere Informationen](#assignment) zum Zuweisen einer Aufgabe
1. [Weitere Informationen](#message) zum Definieren der Benachrichtigungsnachricht
1. [Weitere Informationen](#answers) zum Definieren der möglichen Antworten
1. [Weitere Informationen](#expiration) zum optionalen Definieren eines Ablaufzeitraums

## Zuweisen der Aufgabe {#assignment}

Die Zuweisung der Aufgabe zu einer Gruppe oder einer Benutzerin bzw. einem Benutzer ist obligatorisch. Bis dies geschehen ist, wird ein Warnhinweis angezeigt.

![Screenshot des Abschnitts „Zuweisung“ der Aktivität „Validierung“](../assets/workflow-approval1.png){zoomable="yes"}

Führen Sie folgende Schritte aus:

1. Wählen Sie im Feld **[!UICONTROL Zuweisungstyp]** aus, ob die Aufgabe einer **[!UICONTROL Gruppe]** (Standard) oder **[!UICONTROL einer Benutzerin bzw. einem Benutzer]** zugewiesen wird.

1. Wählen Sie dann die **[!UICONTROL Gruppe]** (von Benutzenden) oder **[!UICONTROL eine Benutzerin bzw. einen Benutzer]** (Einzelperson) aus.

1. Aktivieren Sie **[!UICONTROL Mehrfache Validierung]**, wenn alle Verantwortlichen antworten sollen, bevor der Workflow fortgesetzt wird. Diese Option ist unabhängig vom Zuweisungstyp verfügbar. Wenn diese Option deaktiviert ist, wird der Workflow fortgesetzt, sobald eine verantwortliche Person antwortet. Diese Antwort wird berücksichtigt.

1. Klicken Sie auf **[!UICONTROL Erweiterte Parameter]**, um die Versandvorlage für die Benachrichtigung auszuwählen. Standardmäßig wird eine integrierte Vorlage verwendet, Sie können jedoch auch eine beliebige andere Versandvorlage auswählen.

   ![Screenshot der erweiterten Parameter der Aktivität „Validierung“](../assets/workflow-approval1bis.png){zoomable="yes"}

## Definieren der Benachrichtigungsnachricht {#message}

Sie können jetzt die an die verantwortliche Person gesendete Benachrichtigungsnachricht definieren.

![Screenshot des Abschnitts „Nachricht“ der Aktivität „Validierung“](../assets/workflow-approval2.png){zoomable="yes"}

Führen Sie folgende Schritte aus:

1. Definieren Sie den **[!UICONTROL Titel]** der Benachrichtigung, die an die verantwortliche Person gesendet wird.

1. Definieren Sie den **[!UICONTROL Inhalt]** der Benachrichtigung, die an die verantwortliche Person gesendet wird.

Beide Felder unterstützen Personalisierung: Klicken Sie auf das Personalisierungssymbol, um Ereignisvariablen einzufügen, z. B. **[!UICONTROL Benutzerin oder Benutzer, die/der geantwortet hat]** und **[!UICONTROL Antwort]**, die Sie an anderer Stelle in Ihrem Workflow wiederverwenden können.

![Screenshot der Personalisierung von Nachrichten](../assets/workflow-approval2bis.png){zoomable="yes"}

## Definieren der möglichen Antworten {#answers}

Es gibt zwei Standardantworten für die Aktivität: **[!UICONTROL Ja]** und **[!UICONTROL Nein]**. Jede Antwort entspricht einer Ausgabetransition auf der Arbeitsfläche.

![Screenshot des Abschnitts „Antworten“ der Aktivität „Validierung“](../assets/workflow-approval3.png){zoomable="yes"}

Klicken Sie auf **[!UICONTROL Antwort hinzufügen]**, um zusätzliche Auswahlmöglichkeiten zu definieren.

Wenn die verantwortliche Person antwortet, fährt der Workflow mit der Transition fort, die der Auswahl entspricht.

## Definieren eines Ablaufzeitraums {#expiration}

Schließlich können Sie ein Ablaufdatum für die Validierungsaufgabe definieren. Wie bei einer Antwort löst ein Ablauf eine eigene Ausgabetransition aus, wenn die verantwortliche Person nicht fristgerecht geantwortet hat.

![Screenshot des Abschnitts „Ablauf“ der Aktivität „Validierung“](../assets/workflow-approval4.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Ablauf hinzufügen]**.

1. Definieren Sie ein **[!UICONTROL Label]** für die entsprechende Ausgabetransition.

1. Wählen Sie in der Dropdown-Liste **[!UICONTROL Art des Ablaufs]** eine der folgenden Optionen aus:

   * **[!UICONTROL Nach Beginn der Aufgabe]**: Definieren Sie eine Verzögerung, die nach dem Start der Validierungsaufgabe abgewartet werden soll.
   * **[!UICONTROL Verzögerung nach einem bestimmten Datum]**: Definieren Sie eine Verzögerung, die nach einem bestimmten Datum abgewartet werden soll.
   * **[!UICONTROL Verzögerung vor einem Datum]**: Definieren Sie eine Verzögerung, die vor einem bestimmten Datum abgewartet werden soll.
   * **[!UICONTROL Durch ein Script berechnet]**: Verwenden Sie ein Skript zur Berechnung des Ablaufs.

1. Aktivieren Sie **[!UICONTROL Aufgabe nicht beenden]**, wenn die Ablauftransition aktiviert werden soll, ohne die Validierungsaufgabe zu beenden, sodass die verantwortliche Person auch danach noch antworten kann.

Sie können für dieselbe Validierungsaufgabe mehrere Ablaufdaten definieren.

Dann können Sie den Workflow starten. Sobald die verantwortliche Person antwortet, fährt der Workflow mit der Transition fort, die der Antwort entspricht. [Weitere Informationen](#process)

## Verwandte Themen {#related}

* [Über Workflow-Aktivitäten](about-activities.md)
* [Einrichten und Verwalten des Validierungsprozesses](../../campaigns/campaign-approvals.md)
