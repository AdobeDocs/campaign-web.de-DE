---
audience: end-user
title: Erstellen von Transaktionsnachrichten
description: Informationen zum Erstellen einer Transaktionsnachricht in der Campaign Web-Benutzeroberfläche
source-git-commit: e55b9c875b7700c7ee9d38b8386cc2742ad1f908
workflow-type: ht
source-wordcount: '1189'
ht-degree: 100%

---

# Erstellen von Transaktionsnachrichten

In Transaktionsnachrichten wird der Versand einer personalisierten Nachricht durch ein Ereignis ausgelöst.
Um dies zu aktivieren, müssen Sie für jeden Ereignistyp eine Nachrichtenvorlage erstellen. Diese Vorlagen enthalten alle notwendigen Informationen zur Personalisierung der Transaktionsnachricht.

## Erstellen einer Transaktionsnachrichtenvorlage {#transactional-template}

In der Campaign Web-Benutzeroberfläche besteht der erste Schritt in der Konfiguration der Transaktionsnachrichten aus der Erstellung der Vorlage oder der direkten Erstellung der Nachricht. Dies unterscheidet sich von [der Konfiguration von Transaktionsnachrichten in der Client-Konsole](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/real-time/transactional).

Eine Transaktionsnachrichtenvorlage kann verwendet werden, um den vom Profil empfangenen Versandinhalt in der Vorschau anzuzeigen, bevor er die endgültige Zielgruppe erreicht. Beispielsweise kann eine Administratorin bzw. ein Administrator die Vorlagen einrichten und konfigurieren, damit sie für Marketing-Fachleute nutzbar sind.

Gehen Sie wie folgt vor, um eine Transaktionsnachrichtenvorlage zu erstellen:

* Navigieren Sie im Abschnitt **[!UICONTROL Ausgelöste Nachrichten]** zu **[!UICONTROL Transaktionsnachrichten]**. Auf der Registerkarte **[!UICONTROL Vorlagen]** werden alle Versandvorlagen für Transaktionsnachrichten angezeigt. Klicken Sie auf die Schaltfläche **[!UICONTROL Transaktionsnachrichtenvorlage erstellen]**, um mit dem Erstellen Ihrer Vorlage zu beginnen.

  ![](assets/transactional-templates.png){zoomable="yes"}

* Wählen Sie auf der neuen angezeigten Seite den Kanal Ihrer Vorlage aus. Für unser Beispiel wählen wir den Kanal **[!UICONTROL E-Mail]** aus. Sie können auch eine andere Nachrichtenvorlage verwenden und diese in der Vorlagenliste auswählen.

  ![](assets/transactional-template-channel.png){zoomable="yes"}

  Klicken Sie erneut auf die Schaltfläche **[!UICONTROL Transaktionsnachricht erstellen]**, um die Erstellung Ihrer Vorlage für den ausgewählten Kanal zu validieren.

* Jetzt haben Sie Zugriff auf die Konfiguration Ihrer Transaktionsnachrichtenvorlage.

  ![](assets/transactional-template-configuration.png){zoomable="yes"}

### Eigenschaften der Transaktionsnachricht {#transactional-properties}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_properties"
>title="Eigenschaften von Transaktionsnachrichten"
>abstract="Füllen Sie dieses Formular aus, um die Eigenschaften der Transaktionsnachrichten zu konfigurieren."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_email_properties"
>title="Eigenschaften von Transaktionsnachrichten per E-Mail"
>abstract="Füllen Sie dieses Formular aus, um die Eigenschaften von per E-Mail versendeten Transaktionsnachrichten zu konfigurieren"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_sms_properties"
>title="Eigenschaften von Transaktionsnachrichten per SMS"
>abstract="Füllen Sie dieses Formular aus, um die Eigenschaften von per SMS versendeten Transaktionsnachrichten zu konfigurieren"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_push_properties"
>title="Eigenschaften von Transaktionsnachrichten per Push"
>abstract="Füllen Sie dieses Formular aus, um die Eigenschaften von per Push versendeten Transaktionsnachrichten zu konfigurieren"

Der Abschnitt **[!UICONTROL Eigenschaften]** einer Transaktionsnachricht hilft Ihnen bei der Einrichtung:

* Das **[!UICONTROL Label]** ist der Name, der in der Liste der Transaktionsnachrichten angezeigt wird. Verwenden Sie ein eindeutiges Label für Recherche- und zukünftige Verwendungszwecke.
* Der **[!UICONTROL interne Name]** ist ein eindeutiger Name, der Ihre Nachricht von den anderen erstellten Nachrichten unterscheidet.
* Unter **[!UICONTROL Ordner]** geben Sie an, wo die Transaktionsnachricht erstellt wird.
* Im **[!UICONTROL Ausführungsordner]** wird die Nachricht nach der Ausführung gespeichert.
* Der **[!UICONTROL Versandcode]**: Ein Code, der bei Bedarf dazu beiträgt, die Nachricht für das Reporting zu erkennen.
* Die **[!UICONTROL Beschreibung]**
* Die **[!UICONTROL Art]** ist die Art Ihres Versands, wie in der Auflistung *deliveryNature* aufgeführt. [Weitere Informationen zu Auflistungen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/config/configuration/ui-settings#enumerations)

![](assets/template-properties.png){zoomable="yes"}

### Mobile App {#mobile-app}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_mobileapp"
>title="Transaktionsnachrichten per Mobile App"
>abstract="In diesem Abschnitt können Sie die App auswählen, in der Sie Ihre Push-Benachrichtigung senden möchten."

In diesem Abschnitt können Sie die App auswählen, in der Sie Ihre Push-Benachrichtigung senden möchten.

Durch Klicken auf das Forschungssymbol gelangen Sie zu einer in Ihrer Adobe Campaign-Instanz aufgelisteten Mobile App.

![](assets/transactional-mobileapp.png){zoomable="yes"}

### Kontextbeispiel {#context-sample}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_context"
>title="Kontext von Transaktionsnachrichten"
>abstract="Im Kontextbeispiel können Sie ein Testereignis erstellen, um eine Vorschau der mit der Profilpersonalisierung empfangenen Transaktionsnachricht anzuzeigen."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_addcontext"
>title="Kontext von Transaktionsnachrichten"
>abstract="Im Kontextbeispiel können Sie ein Testereignis erstellen, um eine Vorschau der mit der Profilpersonalisierung empfangenen Transaktionsnachricht anzuzeigen. "

Im Kontextbeispiel können Sie ein Testereignis erstellen, um eine Vorschau der mit der Profilpersonalisierung empfangenen Transaktionsnachricht anzuzeigen.

Dieser Schritt ist optional. Sie können die Vorlage ohne das Kontextbeispiel verwenden. Der Nachteil: Sie können die personalisierten Inhalte nicht in einer Vorschau anzeigen.

In unserem Beispiel, bei dem es um das Festlegen des Passworts geht, sendet das Ereignis den Vornamen und Nachnamen der Person sowie einen personalisierten Link, um das Passwort zurückzusetzen. Der Kontext kann wie unten dargestellt konfiguriert werden.

Der Kontextinhalt hängt von der benötigten Personalisierung ab.

![](assets/transactional-context.png){zoomable="yes"}

### Inhalte für Transaktionsnachrichtenvorlagen {#transactional-content}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_content"
>title="Inhalte für Transaktionsnachrichten"
>abstract="Erfahren Sie, wie Sie Inhalte für Transaktionsnachrichten erstellen."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_personalization"
>title="Personalisierung von Transaktionsnachrichten"
>abstract="Erfahren Sie, wie Sie Inhalte von Transaktionsnachrichten personalisieren."

Die Bearbeitung des Inhalts einer Transaktionsnachricht ist wie die Inhaltserstellung für einen Versand. Klicken Sie auf **[!UICONTROL E-Mail-Designer öffnen]** oder **[!UICONTROL E-Mail-Text bearbeiten]** und wählen Sie einen Vorlageninhalt aus oder importieren Sie Ihren HTML-Code.

![](assets/template-content.png){zoomable="yes"}

Um den Inhalt zu personalisieren, klicken Sie auf den gewünschten Abschnitt und wählen Sie das Symbol **[!UICONTROL Personalisierung hinzufügen]** aus.

![](assets/template-perso.png){zoomable="yes"}

Sie können auf das Fenster **[!UICONTROL Personalisierung bearbeiten]** zugreifen.
Um die Variablen aus dem Trigger-Ereignis hinzuzufügen, klicken Sie auf das Symbol **[!UICONTROL Ereigniskontext]**. Sie können in dem für Ihre Vorlage definierten Kontext navigieren ([weitere Informationen zum Kontext](#context-sample)) und auf die Schaltfläche **[!UICONTROL +]** klicken, um die benötigte Variable einzufügen.

In der Abbildung unten sehen Sie, wie zur Personalisierung der Vorname hinzugefügt wird.

![](assets/template-firstname.png){zoomable="yes"}

In unserem Beispiel fügen wir den Vornamen sowie den Nachnamen hinzu und personalisieren den Link für die Schaltfläche **[!UICONTROL Passwort zurücksetzen]**.

![](assets/template-button.png){zoomable="yes"}

### Anzeigen der Vorlage in einer Vorschau

In dieser Phase der Vorlagenerstellung können Sie eine Vorschau des Vorlageninhalts anzeigen und die Personalisierung überprüfen.

Füllen Sie dazu das [Kontextbeispiel](#context-sample) aus und klicken Sie auf die Schaltfläche **[!UICONTROL Inhalte simulieren]**.

![](assets/template-preview.png){zoomable="yes"}

## Erstellen einer Transaktionsnachricht {#transactional-message}

Sie können eine Transaktionsnachricht direkt oder mithilfe einer Transaktionsnachrichtenvorlage erstellen. [Erfahren Sie, wie Sie eine Transaktionsnachrichtenvorlage erstellen](#transactional-template).

Gehen Sie wie folgt vor, um eine Transaktionsnachricht zu erstellen:

* Navigieren Sie im Abschnitt **[!UICONTROL Ausgelöste Nachrichten]** zu **[!UICONTROL Transaktionsnachrichten]**. Auf der Registerkarte **[!UICONTROL Durchsuchen]** werden alle erstellten Transaktionsnachrichten angezeigt. Klicken Sie auf die Schaltfläche **[!UICONTROL Transaktionsnachricht erstellen]**, um Ihre Nachricht zu erstellen.

  ![](assets/transactional-browse.png){zoomable="yes"}

* Legen Sie auf der neu angezeigten Seite den Kanal Ihrer Nachricht fest und wählen Sie die gewünschte Vorlage aus. Für unser Beispiel wählen wir [die hier erstellte Vorlage](#transactional-template).

  ![](assets/transactional-channel.png){zoomable="yes"}

  Klicken Sie erneut auf die Schaltfläche **[!UICONTROL Transaktionsnachricht erstellen]**, um die Erstellung Ihrer Nachricht für den ausgewählten Kanal zu validieren.

* Nun haben Sie Zugriff auf die Konfiguration Ihrer Transaktionsnachricht. Ihre Nachricht übernimmt die Konfiguration der Vorlage. Diese Seite ist nahezu identisch mit der Konfigurationsseite der Transaktionsnachrichtenvorlage, sie enthält aber auch die Konfiguration des Ereignistyps.

  ![](assets/transactional-configuration.png){zoomable="yes"}

  Füllen Sie die Konfiguration Ihrer Nachricht wie für eine Vorlage aus:
   * [die Eigenschaften der Transaktionsnachricht,](#transactional-properties)
   * [das Kontextbeispiel,](#context-sample)
   * [den Nachrichteninhalt](#transactional-content)
und [konfigurieren Sie den Ereignistyp](#event-type), wie unten beschrieben.

* Klicken Sie nach der [Validierung Ihrer Transaktionsnachricht](validate-transactional.md) auf die Schaltfläche **[!UICONTROL Überprüfen und veröffentlichen]**, um Ihre Nachricht zu erstellen und zu veröffentlichen.
Die Trigger können jetzt den Versand Ihrer Transaktionsnachricht per Push durchführen.

### Über den Ereignistyp {#event-type}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_event"
>title="Transaktionsnachrichtenereignis"
>abstract="Die Konfiguration des Ereignistyps verknüpft die Nachricht mit dem Trigger-Ereignis."

Die Konfiguration des Ereignistyps verknüpft die Nachricht mit dem Trigger-Ereignis.

In der Campaign Web-Benutzeroberfläche können Sie einen bereits erstellten Ereignistyp auswählen und Ihren Ereignistyp direkt auf dieser Konfigurationsseite erstellen.

![](assets/transactional-event-type.png){zoomable="yes"}

>[!CAUTION]
>
>Wenn Sie einen Ereignistyp auswählen, der derzeit von einer anderen Transaktionsnachricht verwendet wird, werden die beiden Nachrichten ausgelöst. Als Best Practice **wird dringend empfohlen, EINEN Ereignistyp nur mit EINER Transaktionsnachricht zu verknüpfen**.

## Hinzufügen von Angeboten zu Transaktionsnachrichten {#transactional-offers}

Sie können Angebote in Ihre Transaktionsnachrichten aufnehmen, damit Sie Ihren Endbenutzenden relevante Vorschläge unterbreiten können, selbst wenn die Nachricht durch ein Ereignis ausgelöst wird.

Diese Funktion ist während der Inhaltsbearbeitung Ihrer Transaktionsnachricht verfügbar. Klicken Sie einfach auf die Schaltfläche **[!UICONTROL Angebote einrichten]**, um sie zu konfigurieren.

Der Einrichtungsprozess ist identisch mit dem Konfigurieren von Angeboten für Standardsendungen.  [Erfahren Sie, wie Sie Angebote zu Ihrer Nachricht hinzufügen](../msg/offers.md).

![](assets/transactional-offers.png){zoomable="yes"}
