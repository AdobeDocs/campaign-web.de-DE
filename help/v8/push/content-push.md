---
audience: end-user
title: Erstellen eines Push-Benachrichtigungs-Versands
description: Erfahren Sie, wie Sie einen Push-Benachrichtigungs-Versand mit Adobe Campaign Web erstellen
exl-id: 031bc38a-2435-4468-8ee6-3bcf1132da55
source-git-commit: 53f4662e9497c8614036f9f89c1ea2b1233756f0
workflow-type: tm+mt
source-wordcount: '1632'
ht-degree: 96%

---


# Entwerfen eines Push-Versands {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Pushen von Android-Inhalten"
>abstract="Den Inhalt der Push-Benachrichtigung für Android-Geräte definieren. Um mit der Erstellung Ihrer Nachricht zu beginnen, klicken Sie auf die Schaltfläche **Inhalt bearbeiten**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Pushen von iOS-Inhalten"
>abstract="Den Inhalt der Push-Benachrichtigung für iOS-Geräte definieren. Um mit der Erstellung Ihrer Nachricht zu beginnen, klicken Sie auf die Schaltfläche **Inhalt bearbeiten**."

## Festlegen des Inhalts der Benachrichtigung {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="Push-Nachricht für iOS"
>abstract="Den Inhalt der Push-Benachrichtigung für iOS-Geräte definieren. Um eine Nachricht zu verfassen, auf die Felder **Titel** und **Nachricht** klicken. Den Ausdruckseditor verwenden, um Daten zu personalisieren und dynamische Inhalte hinzuzufügen. Weitere benutzerdefinierte Konfigurationen befinden sich im Abschnitt **Erweiterte Einstellungen**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_msg"
>title="Android-Push-Nachricht"
>abstract="Den Inhalt der Push-Benachrichtigung für Android-Geräte definieren. Um eine Nachricht zu verfassen, auf die Felder **Titel** und **Nachricht** klicken. Den Ausdruckseditor verwenden, um Daten zu personalisieren und dynamische Inhalte hinzuzufügen. Dazu kann etwa ein Bild ausgewählt werden, das der Push-Benachrichtigung hinzugefügt werden soll, sowie das Symbol der Benachrichtigung, das auf den Geräten der Profile angezeigt werden soll, und dessen Farbe. Weitere benutzerdefinierte Konfigurationen befinden sich im Abschnitt **Erweiterte Einstellungen**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="Stille Benachrichtigung für iOS"
>abstract="Im Modus „Stilles Pushen“ kann eine „stille“ Benachrichtigung an eine App gesendet werden. Dem Benutzer wird das Eintreffen der Benachrichtigung nicht mitgeteilt. Sie wird direkt an die Mobile App übertragen."

Sobald Ihr Push-Versand erstellt wurde, können Sie seinen Inhalt festlegen. Parameter und Einstellungen hängen vom mobilen Betriebssystem ab: Android oder iOS. Auf den folgenden Registerkarten erfahren Sie, wie Sie eine Nachricht für jedes Betriebssystem erstellen.

>[!BEGINTABS]

>[!TAB Android]

Bei Firebase Cloud Messaging stehen Ihnen zwei Nachrichtentypen zur Auswahl:

* Die **[!UICONTROL Datenmeldung]** wird von der Client-App verarbeitet. Diese Meldungen werden direkt an die App gesendet, die auf dem Gerät eine Android-Benachrichtigung generiert und anzeigt. Datennachrichten enthalten nur die von Ihnen definierten Anwendungsvariablen.

  Um den Inhalt zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen, klicken Sie auf das Feld **[!UICONTROL Nachricht]** und verwenden Sie den Ausdruckseditor. Greifen Sie auf diesen Editor zu, um Ihre Nachrichten anzupassen.
Ihre Anwendungsvariablen werden automatisch im Menü **[!UICONTROL Anwendungsvariablen]** hinzugefügt. Mit diesen Variablen können Sie das Verhalten von Benachrichtigungen definieren. Konfigurieren Sie beispielsweise einen bestimmten Anwendungsbildschirm, der angezeigt wird, wenn die Benutzerin oder der Benutzer die Benachrichtigung aktiviert.

  ![Beschreibung: Beispiel für das Definieren von Inhalten für eine Datennachricht in Android-Benachrichtigungen](assets/push_content_4.png){zoomable="yes"}

* Die **[!UICONTROL Benachrichtigungsmeldung]** wird automatisch vom FCM SDK verarbeitet. FCM übernimmt für die Client-App automatisch das Anzeigen der Nachricht auf den Geräten Ihrer Benutzenden. Benachrichtigungsmeldungen enthalten einen vordefinierten Satz von Parametern und Optionen, können aber mit benutzerspezifischen Anwendungsvariablen weiter personalisiert werden.

  Um eine Nachricht zu verfassen, auf die Felder **[!UICONTROL Titel]** und **[!UICONTROL Nachricht]** klicken. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen.

  Push-Benachrichtigungen können weiter personalisiert werden. Wählen Sie hierzu ein Bild aus, das der Push-Benachrichtigung hinzugefügt werden soll, sowie das Symbol der Benachrichtigung, das auf den Geräten der Profile angezeigt werden soll, und dessen Farbe. 

  ![Beschreibung: Beispiel für das Definieren von Inhalten für eine Benachrichtigung in Android-Benachrichtigungen](assets/push_content_3.png){zoomable="yes"}

>[!TAB iOS]

Um eine Nachricht zu verfassen, auf die Felder **[!UICONTROL Titel]** und **[!UICONTROL Nachricht]** klicken. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamische Inhalte hinzuzufügen.

Sie können einen **[!UICONTROL Untertitel]** hinzufügen, den Wert des Parameters „subtitle“ der iOS-Benachrichtigungs-Payload. Weitere Informationen dazu finden Sie in diesem Abschnitt.

Im Modus „Stilles Pushen“ kann eine „stille“ Benachrichtigung an eine Mobile App gesendet werden. Dem Benutzer wird das Eintreffen der Benachrichtigung nicht mitgeteilt. Sie wird direkt an die Mobile App übertragen.

![Beschreibung: Beispiel für das Definieren von Inhalten für iOS-Benachrichtigungen](assets/push_content_1.png){zoomable="yes"}

>[!ENDTABS]

## Erweiterte Einstellungen für Push-Benachrichtigungen {#push-advanced}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings"
>title="Erweiterte Einstellungen für Push-Benachrichtigungen"
>abstract="Definieren der erweiterten Einstellungen für eine Push-Benachrichtigung, z. B. Priorität, die zugehörige Anzahl an Benachrichtigungen, Anwendungsvariablen und mehr."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_critical"
>title="Kritischer Alarmmodus"
>abstract="Aktivieren Sie diese Option, um Ihrer Benachrichtigung einen Ton hinzuzufügen, selbst wenn das Handy der Person auf den Fokusmodus festgelegt oder das Gerät stummgeschaltet ist. Dadurch wird sichergestellt, dass Benutzende jederzeit über wichtige Warnhinweise informiert werden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_count"
>title="Anzahl der Benachrichtigungen"
>abstract="Verwenden Sie diese Option, damit die Zahl der neuen, ungelesenen Informationen direkt auf dem Symbol der App angezeigt wird. Dadurch können die Benutzenden schnell die Anzahl der ausstehenden Benachrichtigungen sehen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="Veränderlicher Inhalt"
>abstract="Aktivieren Sie diese Option, damit die App mit der Benachrichtigung verknüpfte Medieninhalte herunterladen kann."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_score"
>title="Relevanzwert"
>abstract="Legen Sie einen Relevanzwert von 0 bis 100 fest, um die Reihenfolge der Benachrichtigungen in der Zusammenfassung der Benachrichtigungen zu priorisieren. Höhere Werte weisen auf wichtigere Benachrichtigungen hin."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_app_variables"
>title="Anwendungsvariablen"
>abstract="Verwenden Sie diese Anwendungsvariablen, um das Verhalten von Benachrichtigungen zu definieren. Diese Variablen sind vollständig anpassbar und Teil der an das Mobilgerät gesendeten Nachrichten-Payload."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_category"
>title="Kategorie-ID"
>abstract="Geben Sie den Namen der Kategorie-ID an, die mit der Benachrichtigung verknüpft ist. Dies ermöglicht die Anzeige von Aktionsschaltflächen, mit denen Sie direkt über die Benachrichtigung verschiedene Aufgaben ausführen können, ohne die Anwendung zu öffnen."

Die erweiterten Optionen hängen vom mobilen Betriebssystem ab: Android oder iOS. Auf den folgenden Registerkarten erfahren Sie, wie Sie für jedes Betriebssystem Optionen für Ihre Nachricht definieren.

>[!BEGINTABS]

>[!TAB Android]

![Beschreibung: Beispiel für erweiterte Einstellungen für Android-Benachrichtigungen](assets/push_content_5.png){zoomable="yes"}

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Ton]** | Legt den Ton fest, der abgespielt werden soll, wenn das Gerät Ihre Benachrichtigung erhält. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legt die Zahl der neuen ungelesenen Informationen fest, die direkt auf dem Symbol der App angezeigt werden. Dadurch können die Benutzenden schnell die Anzahl der ausstehenden Benachrichtigungen sehen. |
| **[!UICONTROL Kanal-ID]** | Legen Sie die Kanal-ID Ihrer Benachrichtigung fest. Die App muss einen Kanal mit dieser Kanal-ID erstellen, bevor eine Benachrichtigung mit dieser Kanal-ID empfangen werden kann. |
| **[!UICONTROL Klick-Aktion]** | Legt die Aktion fest, die für das Klicken der Benutzenden auf Ihre Benachrichtigung zugewiesen ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App. |
| **[!UICONTROL Tag]** | Legt eine Kennung fest, die zum Ersetzen bestehender Benachrichtigungen in der Benachrichtigungsablage verwendet wird. Dadurch wird verhindert, dass sich mehrere Benachrichtigungen ansammeln, und sichergestellt, dass nur die jeweils letzte relevante Benachrichtigung angezeigt wird. |
| **[!UICONTROL Priorität]** | Legen Sie die Prioritätsstufe Ihrer Benachrichtigung fest. Dies kann „Standard“, „Minimum“, „Niedrig“ oder „Hoch“ sein. Die Prioritätsstufe bestimmt die Wichtigkeit und Dringlichkeit der Benachrichtigung und beeinflusst deren Anzeige sowie die Frage, ob sie bestimmte Systemeinstellungen umgehen kann. Weitere Informationen hierzu finden Sie in der [FCM-Dokumentation](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Sichtbarkeit]** | Legen Sie die Sichtbarkeitsstufe Ihrer Benachrichtigung fest. Dies kann öffentlich, privat oder geheim sein. Die Sichtbarkeitsstufe bestimmt, wie viel des Benachrichtigungsinhalts auf dem Sperrbildschirm und anderen sensiblen Bereichen angezeigt wird. Weitere Informationen finden Sie in der [FCM-Dokumentation](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Sticky]** | Wenn diese Option aktiviert ist, bleibt die Benachrichtigung auch dann sichtbar, wenn darauf geklickt wird. <br>Wenn sie deaktiviert ist, wird die Benachrichtigung automatisch verworfen, sobald damit interagiert wird. Durch das Sticky-Verhalten können wichtige Benachrichtigungen über längere Zeiträume auf dem Bildschirm beibehalten werden. |
| **[!UICONTROL Anwendungsvariablen]** | Damit können Sie das Verhalten von Benachrichtigungen definieren. Diese Variablen sind vollständig anpassbar und Teil der an das Mobilgerät gesendeten Nachrichten-Payload. |

>[!TAB iOS]

![Beschreibung: Beispiel für erweiterte Einstellungen für iOS-Benachrichtigungen](assets/push_content_2.png){zoomable="yes"}

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Kritischer Alarmmodus]** | Aktivieren Sie diese Option, um Ihrer Benachrichtigung einen Ton hinzuzufügen, selbst wenn das Handy der Person auf den Fokusmodus festgelegt oder das Gerät stummgeschaltet ist. Dadurch wird sichergestellt, dass wichtige Warnhinweise auf Benutzerseite wahrgenommen werden. Wenn diese Option aktiviert ist, können Sie das Volumen der Benachrichtigung über die Leiste für die Lautstärke anpassen. Eine Zahl zwischen 0 und 100 über der Leiste spiegelt Ihre Einstellungen wider. |
| **[!UICONTROL Badge entfernen]** | Aktivieren Sie diese Option, um den auf dem Anwendungssymbol angezeigten Badge-Wert zu aktualisieren. Dadurch wird sichergestellt, dass das Badge die Anzahl der neuen ungelesenen Informationen genau wiedergibt. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Damit wird eine Zahl festgelegt, die direkt auf dem App-Symbol angezeigt wird und die Anzahl der neuen, ungelesenen Informationen angibt. Dies bietet eine schnelle visuelle Referenz für die Benutzenden. |
| **[!UICONTROL Lautstärke]** | Lautstärke Ihres Tons auf einer Skala von 0 bis 100. |
| **[!UICONTROL Veränderlicher Inhalt]** | Aktivieren Sie diese Option, damit die App mit der Benachrichtigung verknüpfte Medieninhalte herunterladen kann. Weiterführende Informationen dazu finden Sie im [Apple-Entwickler-Handbuch](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Inhalt verfügbar]** | Aktivieren Sie diese Option, damit Ihre Benachrichtigung Hintergrundaktualisierungen für Trigger auf iOS-Geräten anzeigen kann, auch wenn die App nicht aktiv geöffnet ist. Dadurch wird sichergestellt, dass Inhalte wie Nachrichten oder Datenaktualisierungen verarbeitet und im Posteingang der Mobile App gespeichert werden können, ohne dass die Benutzerinteraktion erforderlich ist. Wenn diese Option aktiviert ist, wird das `content-available: 1`-Flag gemäß den Standards des Apple Push Notification Service (APNS) zur `aps`-Payload hinzugefügt. |
| **[!UICONTROL Relevanzwert]** | Legen Sie einen Relevanzwert von 0 bis 100 fest, um die Reihenfolge der Benachrichtigungen in der Zusammenfassung der Benachrichtigungen zu priorisieren. Höhere Werte weisen auf wichtigere Benachrichtigungen hin. |
| **[!UICONTROL Unterbrechungsgrad]** | <ul> <li>**[!UICONTROL Aktiv]**: Ist dies als Standardeinstellung festgelegt, wird die Benachrichtigung sofort angezeigt, der Bildschirm wird beleuchtet und eventuell wird ein Ton abgespielt. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**[!UICONTROL Passiv]**: Die Benachrichtigung wird zur Benachrichtigungsliste hinzugefügt, ohne dass der Bildschirm beleuchtet oder ein Ton abgespielt wird. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**[!UICONTROL Zeitabhängig]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet, eventuell wird ein Ton abgespielt und der Fokusmodus kann umgangen werden. Für diese Stufe ist keine spezielle Berechtigung von Apple erforderlich.</li> <li>**[!UICONTROL Kritisch]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet und der Stummschaltungs- oder Fokusmodus wird umgangen. Beachten Sie, dass für diese Stufe eine spezielle Berechtigung von Apple erforderlich ist.</ul> |
| **[!UICONTROL Thread-ID]** | Kennung, die verwendet wird, um verknüpfte Benachrichtigungen zu gruppieren. Benachrichtigungen mit derselben Thread-ID werden in der Benachrichtigungsliste als eine einzige Konversation oder ein einziger Thread organisiert. |
| **[!UICONTROL Kategorie]** | Geben Sie den Namen der Kategorie-ID an, die mit der Benachrichtigung verknüpft ist. Dies ermöglicht die Anzeige von Aktionsschaltflächen, mit denen Sie direkt über die Benachrichtigung verschiedene Aufgaben ausführen können, ohne die Anwendung zu öffnen. |
| **[!UICONTROL Zielgruppen-Inhalts-ID]** | Kennung, die angibt, welches Anwendungsfenster beim Öffnen der Benachrichtigung in den Vordergrund gebracht werden soll. |
| **[!UICONTROL Startbild]** | Geben Sie den Namen der Bilddatei für den Start an, die angezeigt werden soll, wenn die Anwendung über die Benachrichtigung gestartet wird. Das ausgewählte Bild wird anstelle des regulären Startbildschirms Ihrer Anwendung angezeigt. |
| **[!UICONTROL Anwendungsvariablen]** | Damit können Sie das Verhalten von Benachrichtigungen definieren. Diese Variablen sind vollständig anpassbar und Teil der an das Mobilgerät gesendeten Nachrichten-Payload. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->
