---
audience: end-user
title: Push-Benachrichtigungsversand erstellen
description: Erfahren Sie, wie Sie einen Push-Benachrichtigungsversand mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
source-git-commit: fbedfc5d1886b86932c156574037549270480f44
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 47%

---

# Push-Versand erstellen {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Pushen von Android-Inhalten"
>abstract="Definieren Sie den Push-Inhalt für Android."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Pushen von iOS-Inhalten"
>abstract="Definieren Sie den Push-Inhalt für iOS."

## Nachricht {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Bei Firebase Cloud Messaging stehen Ihnen zwei Nachrichtentypen zur Auswahl:

* Die **Datennachricht**, die von der Client-App verarbeitet werden. Nachrichten werden direkt an die Mobile App gesendet, die die Android-Benachrichtigung erstellt und auf dem Gerät anzeigt. Datennachrichten enthalten nur die von Ihnen definierten Anwendungsvariablen.

   Klicken Sie auf **[!UICONTROL Nachricht]** und verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen.

* Die Benachrichtigungsmeldung, die automatisch vom FCM-SDK verarbeitet wird. FCM zeigt die Nachricht automatisch auf den Geräten Ihrer Benutzer im Namen der Client-App an. Benachrichtigungsinhalte enthalten einen vordefinierten Satz von Parametern und Optionen, können aber mit benutzerspezifischen Anwendungsvariablen weiter personalisiert werden.

   Um Ihre Nachricht zu erstellen, klicken Sie auf die Schaltfläche **[!UICONTROL Titel]** und **[!UICONTROL body]** -Felder. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen.

   Um Ihre Push-Benachrichtigung weiter zu personalisieren, können Sie ein Bild auswählen, das zu Ihrer Push-Benachrichtigung hinzugefügt werden soll, das Symbol der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll, und die Farbe auswählen.

>[!TAB iOS]

![](assets/push_content_1.png)

Um Ihre Nachricht zu erstellen, klicken Sie auf die Schaltfläche **[!UICONTROL Titel]** und **[!UICONTROL body]** -Felder. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen.

Sie können einen **[!UICONTROL Untertitel]** hinzufügen, den Wert des Parameters „subtitle“ der iOS-Benachrichtigungs-Payload. Weitere Informationen finden Sie in diesem Abschnitt.

Im Modus Stille Push kann eine &quot;stille&quot;Benachrichtigung an eine Mobile App gesendet werden. Dem Benutzer wird die Ankunft der Benachrichtigung nicht mitgeteilt. Sie wird direkt an die Mobile App übertragen.

>[!ENDTABS]

## Erweiterte Einstellungen {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Ton]** | Legen Sie den Ton fest, der abgespielt werden soll, wenn das Gerät Ihre Benachrichtigung erhält. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legen Sie die Anzahl der neuen ungelesenen Informationen fest, die direkt auf dem Anwendungssymbol angezeigt werden sollen. |
| **[!UICONTROL Kennung des Kanals]** | Legen Sie die Kanal-ID Ihrer Benachrichtigung fest. Die Mobile App muss einen Kanal mit dieser Kennung erstellen, bevor eine Benachrichtigung mit dieser Kanalkennung empfangen werden kann. |
| **[!UICONTROL Klickaktion]** | Legen Sie die Aktion fest, die einem Benutzer zugeordnet ist, der auf Ihre Benachrichtigung klickt. |
| **[!UICONTROL Tag]** | Legt die Kennung fest, die zum Ersetzen bestehender Benachrichtigungen in der Benachrichtigungsablage verwendet werden soll. |
| **[!UICONTROL Versandpriorität]** | Legen Sie die Prioritätsstufen Ihrer Benachrichtigung auf &quot;Standard&quot;, &quot;Minimum&quot;, &quot;Niedrig&quot;oder &quot;Hoch&quot;fest. Weitere Informationen hierzu finden Sie in der FCM-Dokumentation. |
| **[!UICONTROL Sichtbarkeit]** | Stellen Sie die Sichtbarkeitsstufen Ihrer Benachrichtigung auf öffentlich, privat oder geheim ein. Weitere Informationen hierzu finden Sie in der FCM-Dokumentation. |
| **[!UICONTROL Sticky]** | Wenn diese Option deaktiviert ist, wird die Benachrichtigung automatisch verworfen, wenn der Benutzer darauf klickt. Wenn diese Option aktiviert ist, wird die Benachrichtigung auch dann angezeigt, wenn der Benutzer darauf klickt. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Kritischer Alarmmodus]** | Aktivieren Sie diese Option, um Ihrer Benachrichtigung Ton hinzuzufügen, selbst wenn das Handy des Benutzers im Fokusmodus eingestellt ist oder wenn der iPhone stummgeschaltet ist. |
| **[!UICONTROL Badge entfernen]** | Aktivieren Sie diese Optionen, um den Badge-Wert zu aktualisieren. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legen Sie eine Zahl fest, mit der die Anzahl der neuen ungelesenen Informationen direkt auf dem Anwendungssymbol angezeigt wird. |
| **[!UICONTROL Anzahl]** | Lautstärke Ihres Tons von 0 bis 100. |
| **[!UICONTROL Veränderlicher Inhalt]** | Aktivieren Sie diese Option, damit die Mobile App Medieninhalte herunterladen kann. Weiterführende Informationen dazu finden Sie im [Handbuch für Apple-Entwickler](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Relevanzwert]** | Legen Sie einen Relevanzwert von 0 bis 100 fest. Das System verwendet diesen Wert, um die Benachrichtigungen in der Benachrichtigungszusammenfassung zu sortieren. |
| **[!UICONTROL Unterbrechungsgrad]** | <ul> <li>**[!UICONTROL Aktiv]**: Ist dies als Standardeinstellung festgelegt, wird die Benachrichtigung sofort angezeigt, der Bildschirm wird beleuchtet und eventuell wird ein Ton abgespielt. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**[!UICONTROL Passiv]**: Die Benachrichtigung wird zur Benachrichtigungsliste hinzugefügt, ohne dass der Bildschirm beleuchtet oder ein Ton abgespielt wird. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**[!UICONTROL Zeitabhängig]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet, eventuell wird ein Ton abgespielt und der Fokusmodus kann umgangen werden. Für diese Stufe ist keine spezielle Berechtigung von Apple erforderlich.</li> <li>**[!UICONTROL Kritisch]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet und der Stummschaltungs- oder Fokusmodus wird umgangen. Beachten Sie, dass für diese Ebene eine spezielle Berechtigung von Apple erforderlich ist.</ul> |
| **[!UICONTROL Thread-ID]** | Kennung, mit der verknüpfte Benachrichtigungen gruppiert werden. |
| **[!UICONTROL Kategorie]** | Name der Kategorie-ID, die Aktionsschaltflächen anzeigt. Mit diesen Benachrichtigungen können Benutzer rascher unterschiedliche Aufgaben ausführen, ohne die Anwendung öffnen oder darin navigieren zu müssen. |
| **[!UICONTROL Zielinhalts-ID]** | Kennung, die angibt, welches Anwendungsfenster beim Öffnen der Benachrichtigung vorgezogen werden soll. |
| **[!UICONTROL Startbild]** | Name der anzuzeigenden Startbilddatei. Wenn der Benutzer Ihre Anwendung startet, wird das ausgewählte Bild anstelle des Startbildschirms Ihrer Anwendung angezeigt. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



