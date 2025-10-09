---
audience: end-user
title: Profilanreicherung in Transaktionsnachrichten
description: Informationen zum Erstellen einer Transaktionsnachricht in der Campaign Web-Benutzeroberfläche
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 8%

---


# Transaktionsnachrichten mit Profildaten anreichern{#profile-enrichment}

>[!AVAILABILITY]
>
>Diese Funktion ist nur für eine Reihe von Organisationen verfügbar (eingeschränkte Verfügbarkeit) und wird in einer zukünftigen Version global eingeführt. Ihr Server muss auf Version 8.8.2 oder höher aktualisiert werden.
>
>Diese Funktion ist derzeit nur für E-Mails verfügbar.

Mit dieser Funktion können Sie Transaktionsnachrichten personalisieren, indem Sie Adobe Campaign-Datenbankfelder mit dem Nachrichteninhalt verknüpfen. Sie können Zielgruppen-Mappings, Anreicherungsspalten und einen Abstimmschlüssel auswählen, um eine genaue Echtzeit-Personalisierung unter Einhaltung der Leistungsschwellen sicherzustellen.

* Ereignisbasierte Transaktionsnachrichten verwenden Daten, die im Ereignis selbst enthalten sind.
* Profilbasierte Transaktionsnachrichten verwenden Daten aus der Adobe Campaign-Datenbank.

Gehen Sie wie folgt vor, um die Profilanreicherung einzurichten:

1. Transaktionsnachricht erstellen, [mehr dazu](#create-enrichment)
1. Ereignistyp definieren, [mehr dazu](#event-enrichment)
1. Einrichten der Anreicherungseinstellungen, [mehr dazu](#settings-enrichment)
1. Inhalt definieren, [mehr dazu](#content-enrichment)
1. Validieren und Senden, [mehr dazu](#send-enrichment)

## Erstellen der Transaktionsnachricht{#create-enrichment}

Zunächst müssen Sie eine neue Transaktionsnachricht erstellen.

1. Gehen Sie **[!UICONTROL Abschnitt „Ausgelöste]**&quot; zu **[!UICONTROL Transaktionsnachrichten]** und erstellen Sie eine neue Transaktionsnachricht.

   ![](assets/transactional-browse.png){zoomable="yes"}

1. Wählen Sie eine Vorlage aus und definieren Sie die Eigenschaften. Weiterführende Informationen hierzu finden Sie auf [dieser Seite](create-transactional.md#transactional-message).

## Ereignistyp definieren{#event-enrichment}

Anschließend müssen Sie das Ereignis als profilbasiert definieren, um in der Adobe Campaign-Datenbank enthaltene Zieldaten zu erhalten.

1. Wählen Sie im Abschnitt **Ereignistyp** die Option **Ereignistyp auswählen** und wählen Sie dann aus, ob Sie einen vorhandenen Ereignistyp verwenden oder Ihren eigenen erstellen möchten.

   >[!NOTE]
   >
   >Sie können keinen Ereignistyp auswählen, der bereits in einer anderen Transaktionsnachrichtenvorlage verwendet wird.

   ![](assets/profile-enrich.png){zoomable="yes"}

1. Geben Sie die Informationen zum Ereignistyp ein:

   * Wählen Sie einen vorhandenen Ereignistyp aus der Liste aus.
   * Fügen Sie für eine neue Bezeichnung einen Namen hinzu.

1. Wählen Sie dann **Profil-RT** in der **Ereignistyp** aus.

   ![](assets/profile-enrich1.png){zoomable="yes"}

## Einrichten der Anreicherungseinstellungen{#settings-enrichment}

Fügen wir nun dem Ereignis Felder hinzu, mit denen Sie die Transaktionsnachricht personalisieren können.

1. Klicken **Abschnitt &quot;**&quot; auf **Anreicherungseinstellungen**.

   ![](assets/profile-enrich2.png){zoomable="yes"}

   >[!NOTE]
   >
   >Diese Schaltfläche ist nur verfügbar, wenn Sie ein profilbasiertes Ereignis definieren.

1. Klicken Sie **Abschnitt „Zusätzliche**&quot; auf **Attribut hinzufügen** und wählen Sie die erforderlichen Felder aus.

   ![](assets/profile-enrich3.png){zoomable="yes"}

1. Definieren, welches Attribut als Abstimmschlüssel verwendet wird.

1. Wählen Sie aus, was passieren soll, wenn der Schlüssel nicht in der Payload verfügbar ist.

   * Nachricht wird ohne Personalisierung gesendet
   * Nachricht wird nicht gesendet

## Definieren des Inhalts{#content-enrichment}

Anschließend müssen Sie den Inhalt der Transaktionsnachricht definieren.

1. Klicken Sie im **Inhalt** auf die Schaltfläche **Inhalt bearbeiten** und definieren Sie den Nachrichteninhalt. Mehr dazu erfahren Sie auf [dieser Seite](create-transactional.md#transactional-content).

   ![](assets/template-content.png){zoomable="yes"}

1. Wenn Sie beispielsweise eine Personalisierung in der Betreffzeile verwenden, verwenden Sie das Menü **Profilanreicherung**, um die zuvor definierten profilbasierten Felder hinzuzufügen.

   ![](assets/profile-enrich4.png){zoomable="yes"}


## Validieren und senden{#send-enrichment}

Abschließend müssen Sie den Versand validieren und versenden.

1. Validieren Sie den Versand, indem Sie den Inhalt simulieren und Testsendungen durchführen. Mehr dazu erfahren Sie auf [dieser Seite](validate-transactional.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Überprüfen und veröffentlichen]** um die Nachricht zu erstellen und zu veröffentlichen. Die Trigger können jetzt den Versand Ihrer Transaktionsnachricht starten.


<!--
When creating the event configuration, select the Profile event targeting dimension (see Creating an event).

Add fields to the event, in order to be able to personalize the transactional message (see Defining the event attributes). You must add at least one field to create an enrichment. You do not need to create other fields such as First name and Last name as you will be able to use personalization fields from the Adobe Campaign database.

Create an enrichment in order to link the event to the Profile resource (see Enriching the event) and select this enrichment as the Targeting enrichment.


IMPORTANT
This step is mandatory for profile-based events.
Preview and publish the event (see Previewing and publishing the event).

When previewing the event, the REST API does not contain an attribute specifying the email address, mobile phone, or push notification specific attributes, as it will be retrieved from the Profile resource.

Once the event has been published, a transactional message linked to the new event is automatically created. In order for the event to trigger sending a transactional message, you must modify and publish the message that was just created…

Integrate the event into your website (see Integrate the event triggering).
-->

