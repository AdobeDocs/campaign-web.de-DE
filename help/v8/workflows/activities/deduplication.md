---
audience: end-user
title: Workflow-Aktivität "Deduplizierung" verwenden
description: Erfahren Sie, wie Sie die Workflow-Aktivität Deduplizierung verwenden.
badge: label="Beta"
source-git-commit: 690e2a2d17f8201c8dbb070ba936c3db513b8329
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 29%

---


# Deduplizierung {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Felder zum Identifizieren von Duplikaten"
>abstract="Im **Felder zur Identifizierung von Duplikaten** klicken Sie auf die **Attribut hinzufügen** -Schaltfläche, um die Felder anzugeben, für die die Identifizierung der Dubletten aufgrund identischer Werte möglich ist, wie z. B. E-Mail-Adresse, Vorname, Nachname etc. In der Reihenfolge der Felder können Sie angeben, welche Felder zuerst verarbeitet werden sollen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Aktivität &quot;Deduplizierung&quot;"
>abstract="Die **Deduplizierung** ermöglicht die Löschung von Dubletten in den Ergebnissen der eingehenden Aktivitäten. Sie wird hauptsächlich im Anschluss an Zielgruppenbestimmungsaktivitäten und vor Aktivitäten verwendet, die die Verwendung von Zieldaten ermöglichen."


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Komplement erzeugen"
>abstract="Sie können eine zusätzliche ausgehende Transition mit der verbleibenden Population generieren, die als Duplikat ausgeschlossen wurde. Schalten Sie dazu die Option **Komplement erzeugen** ein"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Deduplizierungseinstellungen"
>abstract="Um Duplikate in den eingehenden Daten zu löschen, definieren Sie die Deduplizierungsmethode in den unten stehenden Feldern. Standardmäßig wird nur ein Datensatz beibehalten. Sie sollten auch die Deduplizierungsmethode anhand eines Ausdrucks oder Attributs auswählen. Standardmäßig wird der Datensatz, der nicht aus den Duplikaten bestehen soll, zufällig ausgewählt."

Die **Deduplizierung** -Aktivität **Targeting** -Aktivität. Mithilfe dieser Aktivität lassen sich Dubletten in Ergebnissen aus eingehenden Aktivitäten löschen, z. B. duplizierte Profile aus der Empfängerliste. Die **Deduplizierung** -Aktivitäten werden im Allgemeinen im Anschluss an Zielgruppenbestimmungsaktivitäten und vor Aktivitäten verwendet, die die Verwendung von Zieldaten ermöglichen.

## Konfigurieren der Aktivität Deduplizierung{#deduplication-configuration}

Führen Sie die folgenden Schritte aus, um die **Deduplizierung** Aktivität:

![](../assets/workflow-deduplication.png)

1. Hinzufügen einer **Deduplizierung** -Aktivität zu Ihrem Workflow hinzu.

1. Im **Felder zur Identifizierung von Duplikaten** klicken Sie auf die **Attribut hinzufügen** -Schaltfläche, um die Felder anzugeben, für die die Identifizierung der Dubletten aufgrund identischer Werte möglich ist, wie z. B. E-Mail-Adresse, Vorname, Nachname etc. In der Reihenfolge der Felder können Sie angeben, welche Felder zuerst verarbeitet werden sollen.

1. Wählen Sie die Anzahl der eindeutigen **Beizubehaltende Duplikate**. Der Standardwert dieses Felds ist 1. Mittels des Werts 0 lassen sich alle Dubletten beibehalten.

   Nehmen wir z. B. den Fall, dass die Datensätze A und B wie Dubletten des Datensatzes Y und ein Datensatz C wie eine Dublette des Datensatzes Z angesehen werden:

   * Wenn der Wert des Felds 1 ist: nur die Datensätze Y und Z werden beibehalten.
   * Wenn der Wert des Felds 0 ist: alle Datensätze werden beibehalten.
   * Wenn der Wert des Felds 2 ist: Die Datensätze C und Z werden beibehalten und von den Datensätzen A, B und Y werden zwei entweder nach dem Zufallsprinzip oder in Abhängigkeit von der im Anschluss ausgewählten Deduplizierungsmethode beibehalten.

1. Wählen Sie die **Deduplizierungsmethode** zur Verwendung:

   * **Zufällige Auswahl**: wählt nach dem Zufallsprinzip den beizubehaltenden Datensatz aus den Duplikaten aus.
   * **Von einem Ausdruck ausgehend**: hiermit lassen sich Datensätze beibehalten, für die der angegebene Ausdruck den kleinsten oder größten Wert aufweist.
   * **Gemäß einer Werteliste**: ermöglicht die Bestimmung einer Reihenfolge nach Priorität von Werten für ein oder mehrere Felder. Um die Werte zu definieren, klicken Sie auf **Attribut** , um ein Feld auszuwählen oder einen Ausdruck zu erstellen, und fügen Sie dann die Werte zur entsprechenden Tabelle hinzu. Verwenden Sie die Schaltfläche Hinzufügen oberhalb der Werteliste, um ein neues Feld zu definieren.

1. Überprüfen Sie die **Komplement erzeugen** , wenn Sie die verbleibende Population ausnutzen möchten. Das Komplement besteht aus allen Duplikaten. Der Aktivität wird daraufhin eine zusätzliche Transition hinzugefügt.

## Beispiel{#deduplication-example}

Verwenden Sie im folgenden Beispiel eine Deduplizierungsaktivität, um vor dem Versand Duplikate aus der Zielgruppe auszuschließen. Die identifizierten duplizierten Empfänger werden einer dedizierten Audience hinzugefügt, die bei Bedarf wiederverwendet werden kann. Wählen Sie die **Email** -Adresse zur Identifizierung der Dubletten. 1 Eintrag beibehalten und die **Random** Deduplizierungsmethode.

![](../assets/workflow-deduplication-example.png)
