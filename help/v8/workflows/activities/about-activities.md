---
audience: end-user
title: Arbeiten mit Workflow-Aktivitäten
description: Erfahren Sie, wie Workflow-Aktivitäten ausgeführt werden
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 6af0b460a3c81f063a855b2fabba221b43e4ebb9
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 51%

---


# Über Workflow-Aktivitäten {#workflow-activities}

Workflow-Aktivitäten sind in drei Kategorien unterteilt. Je nach Kontext können die verfügbaren Aktivitäten unterschiedlich sein.

Alle Aktivitäten werden in den folgenden Abschnitten beschrieben:

* [Zielgruppenaktivitäten](#targeting)
* [Kanalaktivitäten](#channel)
* [Flusssteuerungsaktivitäten](#flow-control)

## Zielgruppenbestimmungsaktivitäten {#targeting}

Diese Aktivitäten dienen der Zielgruppenbestimmung, Manipulation und Anreicherung von Populationsdaten. Damit können Sie eine oder mehrere Zielgruppen erstellen, indem Sie eine Zielgruppe definieren und diese mithilfe von Schnittmengen-, Vereinigungs- oder Ausschlussvorgängen teilen oder kombinieren.

* Die [Audience erstellen](build-audience.md) ermöglicht die Bestimmung der Zielpopulation. Sie können entweder eine vorhandene Zielgruppe auswählen oder den Regel-Builder verwenden, um Ihre eigene Abfrage zu definieren.
* Die [Kombinieren](combine.md) -Aktivität ermöglicht die Segmentierung Ihrer eingehenden Population. Sie können eine Vereinigung, eine Schnittmenge oder einen Ausschluss verwenden.
* Die [Anreicherung](enrichment.md) -Aktivität können Sie zusätzliche Daten definieren, die in Ihrem Workflow verarbeitet werden sollen. Mit dieser Aktivität können Sie die eingehende Transition nutzen und die Aktivität so konfigurieren, dass die ausgehende Transition mit zusätzlichen Daten ergänzt wird.

## Kanalaktivitäten {#channel}

Mit Adobe Campaign Web können Sie Marketing-Kampagnen über mehrere Kanäle hinweg automatisieren und ausführen, z. B. E-Mail, SMS oder Push-Benachrichtigungen. Mit Adobe Campaign-Workflows können Sie Kanalaktivitäten in der Arbeitsfläche kombinieren, um kanalübergreifende Workflows zu erstellen, mit denen basierend auf dem Kundenverhalten Aktionen ausgelöst werden können.

Sie können beispielsweise eine Begrüßungs-E-Mail-Kampagne erstellen, die eine Reihe von Nachrichten über verschiedene Kanäle wie E-Mail, SMS und Push-Benachrichtigungen enthält. Sie können auch eine Folgenachricht senden, nachdem eine Kundin oder ein Kunde einen Kauf getätigt hat, oder eine personalisierte Geburtstagsnachricht per SMS an eine Kundin bzw. einen Kunden senden.

Mithilfe von Kanalaktivitäten können Sie umfassende, personalisierte Kampagnen erstellen, die Kundinnen und Kunden über mehrere Touchpoints hinweg ansprechen und Konversionen fördern.

* [E-Mail](email.md)
* [Push-Benachrichtigung](push.md)
* [SMS](sms.md)

## Flusssteuerungsaktivitäten {#flow-control}

Die folgenden Aktivitäten dienen der Anordnung und Ausführung von Workflows. Sie ermöglichen die Koordinierung der anderen Aktivitäten:

* Die [Und-Verknüpfung](and-join.md) ermöglicht die Synchronisation mehrerer Ausführungszweige eines Workflows.
* Die [Ende](end.md) -Aktivität können Sie das Ende eines Workflows grafisch markieren. Diese Tätigkeiten haben keine funktionalen Auswirkungen und sind daher optional.
* Eine [Verzweigung](fork.md) erzeugt ausgehende Transitionen, um mehrere Workflow-Aktivitäten parallel zu starten.
* Die [Warten](wait.md)-Aktivität ermöglicht das zeitweise Aussetzen der Ausführung eines Teils eines Workflows.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

