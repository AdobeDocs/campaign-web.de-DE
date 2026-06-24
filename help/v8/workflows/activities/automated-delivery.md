---
audience: end-user
title: Workflow-Aktivität „Automatischer Versand“
description: Erfahren Sie, wie Sie die Workflow-Aktivität für automatischen Versand verwenden
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '643'
ht-degree: 100%

---

# Automatischer Versand {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Aktivität „Automatischer Versand“"
>abstract="Die Workflow-Aktivität „Automatisierter Versand“ ist jetzt in der Workflow-Palette verfügbar. Sie können damit Versandaktionen (vorbereiten, einen Testversand durchführen, vorbereiten und starten) direkt in Ihrem Workflow erstellen und ausführen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="Aktivität „Automatischer Versand“"
>abstract="Die Aktivität **Automatisierter Versand** wird für die Automatisierung verwendet: Erstellen oder führen Sie einen Versand in Ihrem Workflow erneut aus und wählen Sie dann die auszuführende Aktion aus (vorbereiten, vorbereiten und starten, Testversand durchführen). Sie können einen außerhalb des Workflows erstellten bestehenden expliziten Versand auswählen oder bei jeder Ausführung der Aktivität einen neuen Versand aus einer Vorlage erstellen."

Die Aktivität **Automatisierter Versand** ermöglicht die Erstellung, Konfiguration und Ausführung von Versandaktionen direkt in Ihrem Workflow. Verwenden Sie diese Option, wenn Sie einen vordefinierten Versand nach einem Zeitplan oder als Teil eines automatisierten Flusses ausführen möchten oder wenn Sie bei jeder Ausführung der Aktivität einen neuen Versand aus einer Vorlage generieren möchten.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. 
-->

Gehen Sie wie folgt vor, um diese Aktivität zu konfigurieren:

1. Definieren Sie die Versandeinstellungen ([weitere Informationen](#delivery-settings))
1. Wählen Sie die auszuführende Aktion aus ([weitere Informationen](#action-to-execute))
1. Konfigurieren Sie die Transition ([weitere Informationen](#transition-to-execute))
1. Definieren Sie ein Änderungsskripts ([weitere Informationen](#script))

## Definieren der Versandeinstellungen {#delivery-settings}

Wenn Sie die Aktivität konfigurieren, wählen Sie aus, woher der Versand kommen soll. In diesem Abschnitt stehen zwei Optionen zur Verfügung:

![Screenshot des automatischen Versands](../assets/automated-delivery.png){zoomable="yes"}

* Wählen Sie **Expliziter Versand** aus, wenn Sie einen vorhandenen Versand bearbeiten möchten, z. B. einen eigenständigen Versand oder einen Versand, der aus einer Kampagne erstellt wurde. Wählen Sie den Versand mit der Schaltfläche **Versand auswählen** aus. Bei jeder Ausführung des Workflows und beim Erreichen dieser Aktivität wird **derselbe** Versand bearbeitet. Es wird kein neuer Versand bei jeder Ausführung erstellt. Die Aktivität verwendet denselben Versand erneut. Dies ist nützlich, wenn Sie einen einzelnen Versand haben, den Sie vorbereiten oder wiederholt senden möchten, z. B. im Rahmen eines Zeitplans oder nach einem Validierungsschritt.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* Wählen Sie **Neu, basierend auf einer Vorlage erstellt** aus, wenn bei jeder Ausführung der Aktivität ein **neuer** Versand erstellt werden soll. Wählen Sie mit der Schaltfläche **Vorlage auswählen** die Versandvorlage aus. Jede Ausführung generiert einen neuen auf dieser Vorlage basierenden Versand. Verwenden Sie dies, wenn jede Workflow-Ausführung zu einem eigenen Versand führen soll (z. B. eine E-Mail pro Ausführung).

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>Die Optionen **Wird durch die Transition angegeben** und **Wird durch Skript berechnet** für erweiterte Anwendungsfälle können nur in der Client-Konsole konfiguriert werden. Weiterführende Informationen dazu finden Sie in der [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/de/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}.

## Auswählen der auszuführenden Aktion {#action-to-execute}

Wählen Sie in diesem Abschnitt aus, wie die Aktivität mit dem Versand vorgehen soll. Folgende Optionen stehen zur Verfügung:

![Screenshot der Aktionen, die im automatischen Versand ausgeführt werden sollen](../assets/automated-delivery2.png){zoomable="yes"}

* **Speichern**: Erstellt und speichert den Versand, ohne ihn zu analysieren oder zu versenden.
* **Zielgruppe schätzen**: Die Versand-Zielgruppe wird berechnet, um das Potenzial der Kampagne einschätzen zu können (erste Phase der Analyse).
* **Vorbereiten**: Führt die vollständige Analyse durch (Zielgruppenberechnung und Inhaltsvorbereitung). Der Versand wird nicht gesendet.
* **Testversand**: Sendet einen Testversand.
* **Vorbereiten und Starten**: Startet den gesamten Analyseprozess (Zielgruppenberechnung und Inhaltsvorbereitung) und sendet den Versand.

## Einrichten der Transition {#transition-to-execute}

In diesem Abschnitt können Sie auswählen, ob Sie nach der Aktivität Transitionen generieren möchten. Folgende Optionen stehen zur Verfügung:

![Screenshot der Transitionen im automatischen Versand](../assets/automated-delivery3.png){zoomable="yes"}

* **Ausgehende Transition erzeugen**: Generiert eine ausgehende Transition, wenn die Aktivität abgeschlossen ist.
* **Transitionstitel**: Ermöglicht die Anpassung des Labels, das in der Arbeitsfläche auf der Transition angezeigt wird.
* **Fehler verarbeiten**: Fügt eine zusätzliche Transition für die Fehlerbehandlung hinzu.

## Definieren eines Änderungsskripts {#script}

Sie können ein Skript verwenden, um das Verhalten der Aktivität zu ändern, z. B. Versandparameter wie das Aktivitäts-Label. Verwenden Sie dies, wenn Sie benutzerdefinierte Logik für diese Aktivität benötigen.

Klicken Sie auf **Skript erstellen** und schreiben Sie Ihre Änderungslogik im Editor.

## Verwandte Themen {#related}

* [Über Workflow-Aktivitäten](about-activities.md)
* [Versand (fortlaufend)](continuous-delivery.md)
* [E-Mail-, SMS-, Push- und Briefpost-Aktivitäten](channels.md)
* [Versandvorlagen](../../msg/delivery-template.md)
