---
audience: end-user
title: Verwenden Sie die Workflow-Aktivität Warten .
description: Erfahren Sie, wie Sie die Workflow-Aktivität "Warten"verwenden
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 75%

---


# Warten {#wait}

Die **Warten**-Aktivität ermöglicht das zeitweise Aussetzen der Ausführung eines Teils eines Workflows. Die ausgehende Transition der Aktivität wird nach einer Frist aktiviert, die zwischen einigen Sekunden und mehreren Monaten liegen kann, wodurch die Ausführung der im Anschluss folgenden Aktivitäten ermöglicht wird.

Die **Warten**-Aktivität ermöglicht es, einen bestimmten Zeitraum zwischen der Ausführung zweier Aktivitäten zu definieren. Beispielsweise kann man mehrere Tage nach einer E-Mail-Versandaktivität warten, dann die während dieser Zeitspanne erfolgten Öffnungen und Klicks analysieren, bevor man andere Verarbeitungsschritte (Erinnerungs-E-Mail, Audience-Erstellung etc.) unternimmt.

Führen Sie die folgenden Schritte aus, um die **Warten** Aktivität:

1. Hinzufügen einer **Warten** in Ihren Workflow ein.

1. Bestimmen Sie die **Dauer** der Wartezeit zwischen der Aktivierung der eingehenden und der ausgehenden Transition der Aktivität.

1. Zeiteinheit auswählen **Zeitraum**: Sekunden, Minuten, Stunden.





