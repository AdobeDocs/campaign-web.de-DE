---
audience: end-user
title: Verwenden der Workflow-Aktivität „Deduplizierung“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Deduplizierung“ verwenden.
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 100%

---

# Deduplizierung {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Felder zum Identifizieren von Duplikaten"
>abstract="Klicken Sie im Abschnitt **Felder zum Identifizieren von Duplikaten** auf die Schaltfläche **Attribut hinzufügen**, um die Felder anzugeben, für die die Identifizierung von Duplikaten aufgrund identischer Werte möglich ist, wie z. B. E-Mail-Adresse, Vorname und Nachname. Die Reihenfolge der Felder gibt an, welche Felder zuerst verarbeitet werden sollen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Aktivität „Deduplizierung“"
>abstract="Die Aktivität **Deduplizierung** löscht Duplikate in den Ergebnissen eingehender Aktivitäten. Sie wird hauptsächlich nach Zielgruppenbestimmungsaktivitäten und vor Aktivitäten verwendet, die Zielgruppendaten verwenden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Erzeugen eines Komplements"
>abstract="Sie können eine zusätzliche ausgehende Transition mit der verbleibenden Population generieren, die als Duplikat ausgeschlossen wurde. Schalten Sie dazu die Option **Komplement erzeugen** ein."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Deduplizierungseinstellungen"
>abstract="Um Duplikate in den eingehenden Daten zu löschen, definieren Sie die Deduplizierungsmethode in den folgenden Feldern. Standardmäßig wird nur ein Eintrag beibehalten. Wählen Sie die Deduplizierungsmethode anhand eines Ausdrucks oder Attributs aus. Standardmäßig wird der Eintrag, der von den Duplikaten ausgenommen sein soll, zufällig ausgewählt."

Die **Deduplizierungsaktivität** ist eine **Zielgruppenbestimmungsaktivität**. Diese Aktivität löscht Duplikate in den Ergebnissen eingehender Aktivitäten, z. B. doppelte Profile in der Empfängerliste. Die Aktivität **Deduplizierung** wird im Allgemeinen im Anschluss an Zielgruppenbestimmungsaktivitäten und vor Aktivitäten verwendet, die Zielgruppendatum verwenden.

## Konfigurieren der Deduplizierungsaktivität {#deduplication-configuration}

Gehen Sie folgendermaßen vor, um die **Deduplizierungsaktivität** zu konfigurieren:

![Konfigurationsprozess für die Workflow-Deduplizierung](../assets/workflow-deduplication.png)

1. Fügen Sie eine **Deduplizierungsaktivität** zu Ihrem Workflow hinzu.

1. Klicken Sie im Abschnitt **Felder zum Identifizieren von Duplikaten** auf die Schaltfläche **Attribut hinzufügen**, um die Felder anzugeben, für die die Identifizierung von Duplikaten aufgrund identischer Werte möglich ist, wie z. B. E-Mail-Adresse, Vorname und Nachname. Die Reihenfolge der Felder gibt an, welche Felder zuerst verarbeitet werden sollen. [Erfahren Sie, wie Sie Attribute auswählen und zu den Favoriten hinzufügen](../../get-started/attributes.md).

1. Wählen Sie im Abschnitt **Deduplizierungseinstellungen** die Anzahl der eindeutigen **beizubehaltenden Duplikate** aus. Der Standardwert dieses Felds ist 1. Beim Wert 0 werden alle Duplikate beibehalten.

   Nehmen wir z. B. den Fall, dass die Einträge A und B wie Duplikate des Datensatzes Y und ein Datensatz C wie ein Duplikat des Datensatzes Z angesehen werden:

   * Wenn der Wert des Felds 1 ist: nur die Datensätze Y und Z werden beibehalten.
   * Wenn der Wert des Felds 0 ist: alle Datensätze werden beibehalten.
   * Wenn der Wert des Felds 2 ist: Die Einträge C und Z werden beibehalten und von den Einträgen A, B und Y werden zwei entweder nach dem Zufallsprinzip oder in Abhängigkeit von der ausgewählten Deduplizierungsmethode beibehalten.

1. Wählen Sie die **Deduplizierungsmethode** aus, die verwendet werden soll:

   * **Zufällige Auswahl**: Wählt nach dem Zufallsprinzip unter den Duplikaten den Eintrag aus, der beibehalten werden soll.
   * **Von einem Ausdruck ausgehend**: Behält Einträge bei, für die der angegebene Ausdruck den kleinsten oder größten Wert aufweist.
   * **Wert nicht leer**: Behält Einträge bei, für die der Ausdruck nicht leer ist.
   * **Gemäß einer Werteliste**: Definiert eine Priorität nach Wert für ein oder mehrere Felder. Klicken Sie zur Bestimmung dieser Werte auf **Attribute**, um ein Feld auszuwählen, oder erstellen Sie einen Ausdruck und fügen Sie dann die Werte der entsprechenden Tabelle hinzu. Verwenden Sie die Schaltfläche **Hinzufügen** oberhalb der Werteliste, um ein neues Feld zu definieren.

1. Kreuzen Sie die Option **Komplement erzeugen** an, um die verbleibende Population zu verwenden. Das Komplement besteht aus allen Duplikaten. Der Aktivität wird daraufhin eine zusätzliche Transition hinzugefügt.

## Beispiel {#deduplication-example}

Verwenden Sie im folgenden Beispiel eine Deduplizierungsaktivität, um vor dem Versand Duplikate aus der Zielgruppe auszuschließen. Die identifizierten duplizierten Profile werden einer dedizierten Zielgruppe hinzugefügt, die bei Bedarf wiederverwendet werden kann. Wählen Sie die **E-Mail-Adresse** zur Identifizierung der Duplikate. Behalten Sie einen Eintrag bei und wählen Sie die Deduplizierungsmethode **Zufällig** aus.

![Beispiel einer Aktivität „Deduplizierung“ in einem Workflow](../assets/workflow-deduplication-example.png)