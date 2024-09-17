---
audience: end-user
title: Erstellen eines Rich-Push-Benachrichtigungsversands
description: Erfahren Sie, wie Sie mit Adobe Campaign Web einen Rich-Push-Benachrichtigungs-Versand für Android erstellen.
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: 86214576e08df6596860826bb6511c1f4138c2ad
workflow-type: tm+mt
source-wordcount: '3372'
ht-degree: 100%

---

# Entwerfen eines Rich-Push-Versands für Android {#rich-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="Schaltfläche „Später erinnern“"
>abstract="Die Schaltfläche **Später erinnern** bietet die Möglichkeit, eine Erinnerung zu planen. Das Feld „Zeitstempel“ erfordert einen Wert, der eine Zeitspanne in Sekunden darstellt."

>[!IMPORTANT]
>
>* Diese Funktion erfordert eine Aktualisierung auf Campaign v8.6.3 <!--or v8.7.2-->. Weitere Informationen finden Sie in den [Versionshinweisen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} zur Campaign v8 Client-Konsole.
>
>* Bevor Sie eine Rich-Push-Benachrichtigung entwerfen, müssen Sie zunächst Ihren V2-Connector konfigurieren. Eine detaillierte Vorgehensweise dazu finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign-classic/using/sending-messages/sending-push-notifications/configure-the-mobile-app/configuring-the-mobile-application-android#configuring-external-account-android){target="_blank"}.


Bei Firebase Cloud Messaging stehen Ihnen zwei Nachrichtentypen zur Auswahl:

* Die **[!UICONTROL Datenmeldung]** wird von der Client-App verarbeitet. Diese Meldungen werden direkt an die App gesendet, die auf dem Gerät eine Android-Benachrichtigung generiert und anzeigt. Datennachrichten enthalten nur die von Ihnen definierten Anwendungsvariablen.

* Die **[!UICONTROL Benachrichtigungsmeldung]** wird automatisch vom FCM SDK verarbeitet. FCM übernimmt für die Client-App automatisch das Anzeigen der Nachricht auf den Geräten Ihrer Benutzenden. Benachrichtigungsmeldungen enthalten einen vordefinierten Satz von Parametern und Optionen, können aber mit benutzerspezifischen Anwendungsvariablen weiter personalisiert werden.

![](assets/rich_push.png){zoomable="yes"}

## Festlegen des Inhalts der Benachrichtigung {#push-message}

Nach der Erstellung Ihres Push-Versands können Sie dessen Inhalt mit einer der folgenden Vorlagen definieren:

* **Standard** ermöglicht es Ihnen, Benachrichtigungen mit einem einfachen Symbol und einem zugehörigen Bild zu senden.

* **Einfach** ermöglicht es Ihnen, Text, Bilder und Schaltflächen in Ihre Benachrichtigungen einzufügen.

* **Karussell** ermöglicht es Ihnen, Benachrichtigungen mit Text und mehreren Bildern zu senden, zwischen denen die Benutzenden hin und her wischen können.

* **Symbolschaltflächen** ermöglichen es Ihnen, Benachrichtigungen mit einem einfachen Symbol und einem zugehörigen Bild zu versenden.

* **Eingabefeld** erfasst Benutzereingaben und Feedback direkt über die Benachrichtigung.

* **Produktkatalog** zeigt eine Vielzahl von Produktbildern an.

* **Produktbewertung** ermöglicht Benutzenden die Rückmeldung von Feedback und Bewertung von Produkten.

* **Timer** fügt einen Live-Countdown-Timer in Ihre Benachrichtigungen ein.

* **Rahmenlos** verwendet die gesamte Hintergrundfläche für ein Bild mit nahtlos überlagertem Text.

Navigieren Sie durch die folgenden Registerkarten, um mehr über die Personalisierung dieser Vorlagen zu erfahren.

>[!BEGINTABS]

>[!TAB Standard]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Standard]** aus.

   ![](assets/rich_push_default.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]** und **[!UICONTROL Nachricht]** ein.

   ![](assets/rich_push_default_2.png)

1. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Definieren Sie die **[!UICONTROL Klick-Aktion]**, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Push-Benachrichtigungen können weiter personalisiert werden. Dazu können Sie eine **[!UICONTROL Bild]**-URL auswählen, die der Push-Benachrichtigung hinzugefügt werden soll, sowie das **[!UICONTROL Symbol]** der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll.

   ![](assets/rich_push_default_3.png)

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Einfach]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Einfach]**.

   ![](assets/rich_push_basic.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der Text der **[!UICONTROL Nachricht]** wird in der ausgeblendeten Ansicht angezeigt, während die **[!UICONTROL Erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![](assets/rich_push_basic_2.png)

1. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. Push-Benachrichtigungen können weiter personalisiert werden. Dazu können Sie eine **[!UICONTROL Bild]**-URL auswählen, die der Push-Benachrichtigung hinzugefügt werden soll, sowie das **[!UICONTROL Symbol]** der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Klicken Sie auf **[!UICONTROL Schaltfläche hinzufügen]** und füllen Sie folgende Felder aus:

   * **[!UICONTROL Titel]**: Text, der auf der Schaltfläche angezeigt wird.
   * **[!UICONTROL Link-URI]**: Geben Sie den URI an, der beim Klicken auf die Schaltfläche ausgeführt werden soll.
   * **[!UICONTROL Link-Typ]**: Wählen Sie als Link-Typ entweder **[!UICONTROL Web-URL]**, **[!UICONTROL Deeplink]** oder **[!UICONTROL Open App]**.

   Sie haben die Möglichkeit, bis zu drei Schaltflächen in Ihre Push-Benachrichtigung einzubauen. Wenn Sie sich für die **[!UICONTROL Schaltfläche „Später erinnern“]** entscheiden, können Sie maximal zwei Schaltflächen einfügen.

   ![](assets/rich_push_basic_4.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL „Später erinnern“ hinzufügen]**, um Ihrer Push-Benachrichtigung die Option „Später erinnern“ hinzuzufügen. Geben Sie einen **[!UICONTROL Titel]** und einen **[!UICONTROL Zeitstempel]** an.

   Das Feld „Zeitstempel“ erfordert einen Wert, der eine Zeitspanne in Sekunden darstellt.

   ![](assets/rich_push_basic_5.png)

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Karussell]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Karussell]**.

   ![](assets/rich_push_carousel.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der Text der **[!UICONTROL Nachricht]** wird in der ausgeblendeten Ansicht angezeigt, während die **[!UICONTROL Erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![](assets/rich_push_carousel_1.png)

1. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL aus, die Sie in das Feld **[!UICONTROL Klick-Aktion]** eingefügt haben:

   * **[!UICONTROL Web URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. Um Ihre Push-Benachrichtigung weiter zu personalisieren, können Sie das **[!UICONTROL Symbol]** der Benachrichtigung auswählen, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Wählen Sie, wie das **[!UICONTROL Karussell]** bedient werden soll:

   * **[!UICONTROL Automatisch]**: Die Bilder werden automatisch in vordefinierten Intervallen als Folien wiedergegeben.
   * **[!UICONTROL Manuell]**: Benutzende können manuell zwischen den Folien streichen, um durch die Bilder zu navigieren.

     Aktivieren Sie die Option **[!UICONTROL Filmstreifen]**, um die Vorschau der vorherigen und der nächsten Bilder neben der Hauptfolie einzuschließen.

1. Klicken Sie auf **[!UICONTROL Bild hinzufügen]** und geben Sie Ihre Bild-URL und Ihren Text ein.

   Stellen Sie sicher, dass Sie mindestens drei und maximal fünf Bilder einfügen.

   ![](assets/rich_push_carousel_3.png)

1. Bearbeiten Sie die Reihenfolge Ihrer Bilder mit den nach oben bzw. nach unten zeigenden Pfeilen.

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Symbolschaltflächen]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Symbolschaltflächen]** aus.

   ![](assets/rich_push_icon_1.png)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_icon_2.png)

1. Um Ihre Push-Benachrichtigung weiter zu personalisieren, können Sie das **[!UICONTROL Symbol]** der Benachrichtigung auswählen, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Geben Sie die URL für das **[!UICONTROL Bild der Schaltfläche „Abbrechen“]** an.

1. Klicken Sie auf **[!UICONTROL Symbol hinzufügen]** und geben Sie die **Bild-URL** und den **[!UICONTROL Link-URI]** ein und wählen Sie Ihren **[!UICONTROL Link-Typ]** aus.

   Stellen Sie sicher, dass Sie mindestens drei und maximal fünf Symbole einfügen.

   ![](assets/rich_push_icon_3.png)

1. Bearbeiten Sie die Reihenfolge Ihrer Bilder mit den nach oben bzw. nach unten zeigenden Pfeilen.

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

   ![](assets/rich_push_icon_4.png)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Eingabefeld]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Art der Benachrichtigung]** die Option **[!UICONTROL Eingabefeld]** aus.

   ![](assets/rich_push_input_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der Text der **[!UICONTROL Nachricht]** wird in der ausgeblendeten Ansicht angezeigt, während die **[!UICONTROL Erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![](assets/rich_push_input_2.png)

1. Verwenden Sie dynamische Personalisierungsfelder, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

1. Push-Benachrichtigungen können weiter personalisiert werden. Dazu können Sie eine **[!UICONTROL Bild]**-URL auswählen, die der Push-Benachrichtigung hinzugefügt werden soll, sowie das **[!UICONTROL Symbol]** der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Tragen Sie die folgenden Optionen für Ihr **Eingabefeld** ein:

   * **[!UICONTROL Namen der Empfängerin bzw. des Empfängers eingeben]**: Geben Sie den Namen oder die Kennung für die Empfängerin bzw. den Empfänger der Eingabe ein.
   * **[!UICONTROL Eingabetext]**: Geben Sie den Text für das **Eingabefeld** ein.
   * **[!UICONTROL Feedback-Text]**: Geben Sie den Text ein, der nach einer Antwort angezeigt werden soll.
   * **[!UICONTROL Feedback-Bild]**: Fügen Sie die URL für das Bild hinzu, das nach einer Antwort angezeigt wird.

   ![](assets/rich_push_input_3.png)

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Produktkatalog]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Art der Benachrichtigung]** die Option **[!UICONTROL Produktkatalog]** aus.

   ![](assets/rich_push_catalog_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]** und **[!UICONTROL Nachricht]** ein.

   ![](assets/rich_push_catalog_2.png)

1. Verwenden Sie dynamische Personalisierungsfelder, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

1. Um Ihre Push-Benachrichtigung weiter zu personalisieren, können Sie das **[!UICONTROL Symbol]** der Benachrichtigung auswählen, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Geben Sie Ihren **Click-to-Action-Text** und Ihr **Bild** ein.

1. Wählen Sie für den **[!UICONTROL Anzeigetyp]** horizontal oder vertikal aus.

1. Tragen Sie die Informationen zu den Elementen im **[!UICONTROL Katalog]** ein.

   Stellen Sie sicher, dass Sie mindestens drei und maximal fünf Elemente einfügen.

   ![](assets/rich_push_catalog_3.png)

1. Bearbeiten Sie die Reihenfolge Ihrer Bilder mit den nach oben bzw. nach unten zeigenden Pfeilen.

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Produktbewertung]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Art der Benachrichtigung]** die Option **[!UICONTROL Produktbewertung]** aus.

   ![](assets/rich_push_rating_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der Text der **[!UICONTROL Nachricht]** wird in der ausgeblendeten Ansicht angezeigt, während die **[!UICONTROL Erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![](assets/rich_push_rating_2.png)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

1. Push-Benachrichtigungen können weiter personalisiert werden. Dazu können Sie eine **[!UICONTROL Bild]**-URL auswählen, die der Push-Benachrichtigung hinzugefügt werden soll, sowie das **[!UICONTROL Symbol]** der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Fügen Sie die URLs für das **[!UICONTROL Bewertungssymbol im nicht ausgewählten Zustand]** und das **[!UICONTROL Bewertungssymbol im ausgewählten Zustand]** ein.

   ![](assets/rich_push_rating_3.png)

1. Klicken Sie auf **[!UICONTROL Bewertung hinzufügen]** und geben Sie die **[!UICONTROL Link-URL]** und den **[!UICONTROL Link-Typ]** ein.

   Stellen Sie sicher, dass Sie mindestens drei und maximal fünf Bewertungen einfügen.

   ![](assets/rich_push_rating_4.png)

1. Bearbeiten Sie die Reihenfolge Ihrer Bilder mit den nach oben bzw. nach unten zeigenden Pfeilen.

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Timer]

1. Wählen Sie in der Dropdown-Liste **[!UICONTROL Benachrichtigungstyp]** die Option **[!UICONTROL Timer]** aus.

   ![](assets/rich_push_timer_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]** und **[!UICONTROL Nachricht]** ein.

   Verwenden Sie dynamische Personalisierungsfelder, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

   ![](assets/rich_push_timer_2.png)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_timer_3.png)

1. Push-Benachrichtigungen können weiter personalisiert werden. Dazu können Sie eine **[!UICONTROL Bild]**-URL auswählen, die der Push-Benachrichtigung hinzugefügt werden soll, sowie das **[!UICONTROL Symbol]** der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll.

1. Stellen Sie die **[!UICONTROL Dauer des Timers]** in Sekunden oder den **[!UICONTROL Zeitstempel für Timer-Ende]** auf einen bestimmten Epoch-Zeitstempel ein.

   ![](assets/rich_push_timer_4.png)

1. Geben Sie den Text und das Bild, die nach Ablauf des Timers angezeigt werden sollen, in die Felder **[!UICONTROL Alternativer Titel]**, **[!UICONTROL Alternative Nachricht]**, **[!UICONTROL Alternative erweiterte Nachricht]** und **[!UICONTROL Alternatives Startbild]** ein.

   ![](assets/rich_push_timer_5.png)

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Rahmenlos]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Art der Benachrichtigung]** die Option **[!UICONTROL Rahmenlos]** aus.

   ![](assets/rich_push_bezel_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der Text der **[!UICONTROL Nachricht]** wird in der ausgeblendeten Ansicht angezeigt, während die **[!UICONTROL Erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![](assets/rich_push_bezel_2.png)

1. Verwenden Sie dynamische Personalisierungsfelder, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die mit einem Benutzerklick auf Ihre Benachrichtigung verbunden ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie den **[!UICONTROL Link-Typ]** der URL, die Sie zum Feld **[!UICONTROL Klick-Aktion]** hinzugefügt haben:

   * **[!UICONTROL Web-URL]**: Web-URLs leiten Benutzende zu Online-Inhalten weiter. Beim Anklicken öffnen sie den Standard-Webbrowser des Geräts und navigieren zu der angegebenen URL.

   * **[!UICONTROL Deeplink]**: Deeplinks sind URLs, die Benutzende zu bestimmten Abschnitten in einer App führen, selbst wenn die App geschlossen ist. Beim Anklicken kann ein Dialogfeld angezeigt werden, in dem Benutzende aus verschiedenen Apps wählen können, die den Link verarbeiten können.

   * **[!UICONTROL Open App]**: Open App-URLs ermöglichen es Ihnen, sich direkt mit Inhalten innerhalb einer Anwendung zu verbinden. Diese Art von URL ermöglicht es Ihrer Anwendung, sich als Standard-Handler für einen bestimmten Link-Typ zu etablieren und so das Dialogfeld zur Disambiguierung zu umgehen.

   Weitere Informationen über die Handhabung von Android-App-Links finden Sie in der [Entwicklerdokumentation zu Android](https://developer.android.com/training/app-links).

1. Push-Benachrichtigungen können weiter personalisiert werden. Dazu können Sie eine **[!UICONTROL Bild]**-URL auswählen, die der Push-Benachrichtigung hinzugefügt werden soll, sowie das **[!UICONTROL Symbol]** der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll.

   ![](assets/rich_push_bezel_3.png)

1. Wählen Sie für Ihre Benachrichtigung die Option **[!UICONTROL Ausgeblendeter Benachrichtigungsstil]** aus, unabhängig davon, ob in der Benachrichtigung in erster Linie ein Bild oder Text angezeigt wird.

1. Konfigurieren Sie die **[!UICONTROL erweiterten Einstellungen]** Ihrer Push-Benachrichtigung. [Weitere Informationen](#push-advanced)

Sobald Sie den Inhalt Ihrer Nachricht definiert haben, können Sie Testabonnentinnen und -abonnenten verwenden, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!ENDTABS]

## Erweiterte Einstellungen für Push-Benachrichtigungen {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Symbolfarbe]** | Legen Sie die Farbe Ihres Symbols mit Ihren Hexadezimal-Farb-Codes fest. |
| **[!UICONTROL Titelfarbe]** | Legen Sie die Farbe Ihres Titels mit Ihren Hexadezimal-Farb-Codes fest. |
| **[!UICONTROL Farbe des Nachrichtentextes]** | Legen Sie die Farbe Ihres Nachrichtentextes mit Ihren Hexadezimal-Farb-Codes fest. |
| **[!UICONTROL Timer-Farbe]** | Legen Sie die Farbe für Ihren Timer mit den Hexadezimal-Farb-Codes fest. |
| **[!UICONTROL Hintergrundfarbe der Benachrichtigungen]** | Legt die Farbe des Benachrichtigungshintergrunds mit den gewünschten Hexadezimal-Farb-Codes fest. |
| **[!UICONTROL Ton]** | Legt den Ton fest, der abgespielt werden soll, wenn das Gerät Ihre Benachrichtigung erhält. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legt die Zahl der neuen ungelesenen Informationen fest, die direkt auf dem Symbol der App angezeigt werden. Dadurch können die Benutzenden schnell die Anzahl der ausstehenden Benachrichtigungen sehen. |
| **[!UICONTROL Kanal-ID]** | Legen Sie die Kanal-ID Ihrer Benachrichtigung fest. Die App muss einen Kanal mit dieser Kanal-ID erstellen, bevor eine Benachrichtigung mit dieser Kanal-ID empfangen werden kann. |
| **[!UICONTROL Tag]** | Legt eine Kennung fest, die zum Ersetzen bestehender Benachrichtigungen in der Benachrichtigungsablage verwendet wird. Dadurch wird verhindert, dass sich mehrere Benachrichtigungen ansammeln, und sichergestellt, dass nur die jeweils letzte relevante Benachrichtigung angezeigt wird. |
| **[!UICONTROL Priorität]** | Legen Sie die Prioritätsstufe Ihrer Benachrichtigung fest. Dies kann „Standard“, „Minimum“, „Niedrig“ oder „Hoch“ sein. Die Prioritätsstufe bestimmt die Wichtigkeit und Dringlichkeit der Benachrichtigung und beeinflusst deren Anzeige sowie die Frage, ob sie bestimmte Systemeinstellungen umgehen kann. Weitere Informationen hierzu finden Sie in der [FCM-Dokumentation](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Sichtbarkeit]** | Legen Sie die Sichtbarkeitsstufe Ihrer Benachrichtigung fest. Dies kann öffentlich, privat oder geheim sein. Die Sichtbarkeitsstufe bestimmt, wie viel des Benachrichtigungsinhalts auf dem Sperrbildschirm und anderen sensiblen Bereichen angezeigt wird. Weitere Informationen finden Sie in der [FCM-Dokumentation](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Sticky-Benachrichtigung]** | Wenn diese Option aktiviert ist, bleibt die Benachrichtigung auch dann sichtbar, wenn darauf geklickt wird. <br>Wenn sie deaktiviert ist, wird die Benachrichtigung automatisch verworfen, sobald damit interagiert wird. Durch das Sticky-Verhalten können wichtige Benachrichtigungen über längere Zeiträume auf dem Bildschirm beibehalten werden. |
| **[!UICONTROL Anwendungsvariablen]** | Damit können Sie das Verhalten von Benachrichtigungen definieren. Diese Variablen sind vollständig anpassbar und Teil der an das Mobilgerät gesendeten Nachrichten-Payload. |
