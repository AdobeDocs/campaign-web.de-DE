---
audience: end-user
title: Push-Benachrichtigungsversand erstellen
description: Erfahren Sie, wie Sie einen Push-Benachrichtigungsversand mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
source-git-commit: a9c9079a64dd7113aa7da1040aa30cef2c9c0aec
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 29%

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

* Die **[!UICONTROL Datennachricht]e** wird von der Client-App verarbeitet. Diese Nachrichten werden direkt an die Mobile App gesendet, die eine Android-Benachrichtigung auf dem Gerät generiert und anzeigt. Datennachrichten enthalten nur die von Ihnen definierten Anwendungsvariablen.

  Um den Inhalt zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen, klicken Sie auf die Schaltfläche **[!UICONTROL Nachricht]** und verwenden Sie den Ausdruckseditor. Sie können auf diesen Editor zugreifen, um Ihre Nachrichten anzupassen In **[!UICONTROL Anwendungsvariablen]** -Menü, werden Ihre Anwendungsvariablen automatisch hinzugefügt. Mit diesen Variablen können Sie das Verhalten von Benachrichtigungen definieren. Sie können beispielsweise einen bestimmten Anwendungsbildschirm konfigurieren, der angezeigt wird, wenn der Benutzer die Benachrichtigung aktiviert.

  ![](assets/push_content_4.png)

* Die **[!UICONTROL Benachrichtigungsinhalt]**, wird automatisch vom FCM-SDK verarbeitet. FCM zeigt die Nachricht automatisch auf den Geräten Ihrer Benutzer im Namen der Client-App an. Benachrichtigungsinhalte enthalten einen vordefinierten Satz von Parametern und Optionen, können aber mit benutzerspezifischen Anwendungsvariablen weiter personalisiert werden.

  Um Ihre Nachricht zu erstellen, klicken Sie auf die Schaltfläche **[!UICONTROL Titel]** und **[!UICONTROL body]** -Felder. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen.

  Um Ihre Push-Benachrichtigung weiter zu personalisieren, können Sie ein Bild auswählen, das zu Ihrer Push-Benachrichtigung hinzugefügt werden soll, das Symbol der Benachrichtigung, das auf den Geräten Ihrer Profile angezeigt werden soll, und die Farbe auswählen.

  ![](assets/push_content_3.png)

>[!TAB iOS]

Um Ihre Nachricht zu erstellen, klicken Sie auf die Schaltfläche **[!UICONTROL Titel]** und **[!UICONTROL body]** -Felder. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen.

Sie können einen **[!UICONTROL Untertitel]** hinzufügen, den Wert des Parameters „subtitle“ der iOS-Benachrichtigungs-Payload. Weitere Informationen finden Sie in diesem Abschnitt.

Im Modus Stille Push kann eine &quot;stille&quot;Benachrichtigung an eine Mobile App gesendet werden. Dem Benutzer wird die Ankunft der Benachrichtigung nicht mitgeteilt. Sie wird direkt an die Mobile App übertragen.

![](assets/push_content_1.png)

>[!ENDTABS]

## Erweiterte Einstellungen {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Ton]** | Legen Sie den Ton fest, der abgespielt werden soll, wenn das Gerät Ihre Benachrichtigung erhält. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legen Sie die Anzahl der neuen ungelesenen Informationen fest, die direkt auf dem Anwendungssymbol angezeigt werden sollen. Dadurch kann der Benutzer die Anzahl der ausstehenden Benachrichtigungen schnell sehen. |
| **[!UICONTROL Kennung des Kanals]** | Legen Sie die Kanal-ID Ihrer Benachrichtigung fest. Die Mobile App muss einen Kanal mit dieser Kennung erstellen, bevor eine Benachrichtigung mit dieser Kanalkennung empfangen werden kann. |
| **[!UICONTROL Klickaktion]** | Definieren Sie die Aktion, die einem Benutzer zugeordnet ist, der auf Ihre Benachrichtigung klickt. Dies bestimmt das Verhalten bei der Interaktion des Benutzers mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App. |
| **[!UICONTROL Tag]** | Legen Sie eine Kennung fest, die zum Ersetzen vorhandener Benachrichtigungen in der Benachrichtigungsablage verwendet wird. Dadurch wird verhindert, dass mehrere Benachrichtigungen gesammelt werden, und es wird sichergestellt, dass nur die jeweils letzte relevante Benachrichtigung angezeigt wird. |
| **[!UICONTROL Versandpriorität]** | Legen Sie die Prioritätsstufe Ihrer Benachrichtigung fest, bei der es sich um Standard, Minimum, Niedrig oder Hoch handeln kann. Die Prioritätsstufe bestimmt die Wichtigkeit und Dringlichkeit der Benachrichtigung und beeinflusst deren Anzeige sowie die Frage, ob sie bestimmte Systemeinstellungen umgehen kann. Weitere Informationen hierzu finden Sie in der [FCM-Dokumentation](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Sichtbarkeit]** | Legen Sie die Sichtbarkeitsstufe Ihrer Benachrichtigung fest, die öffentlich, privat oder geheim sein kann. Die Sichtbarkeitsstufe bestimmt, wie viel des Benachrichtigungsinhalts auf dem Sperrbildschirm und anderen sensiblen Bereichen angezeigt wird. Weitere Informationen finden Sie im Abschnitt [FCM-Dokumentation](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Sticky]** | Bei Aktivierung bleibt die Benachrichtigung auch dann sichtbar, wenn der Benutzer darauf klickt. <br>Wenn diese Option deaktiviert ist, wird die Benachrichtigung automatisch verworfen, wenn der Benutzer damit interagiert. Durch das Sticky-Verhalten können wichtige Benachrichtigungen über längere Zeiträume auf dem Bildschirm beibehalten werden. |
| **[!UICONTROL Anwendungsvariablen]** | Ermöglicht die Definition des Benachrichtigungsverhaltens. Diese Variablen können vollständig angepasst werden und sind Teil der Payload der Nachricht, die an das Mobilgerät gesendet wird. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parameter | Beschreibung |
|---------|---------|
| **[!UICONTROL Kritischer Alarmmodus]** | Aktivieren Sie diese Option, um Ihrer Benachrichtigung Ton hinzuzufügen, selbst wenn das Handy des Benutzers auf den Fokusmodus eingestellt ist oder der iPhone stummgeschaltet ist. Dadurch wird sichergestellt, dass wichtige Warnhinweise vom Benutzer wahrgenommen werden. |
| **[!UICONTROL Badge entfernen]** | Aktivieren Sie diese Option, um den auf dem Anwendungssymbol angezeigten Badge-Wert zu aktualisieren. Dadurch wird sichergestellt, dass das Badge die Anzahl der neuen ungelesenen Informationen genau widerspiegelt. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legen Sie eine Zahl fest, die direkt auf dem Anwendungssymbol angezeigt wird und die die Anzahl der neuen ungelesenen Informationen angibt. Dies bietet eine schnelle visuelle Referenz für den Benutzer. |
| **[!UICONTROL Anzahl]** | Lautstärke Ihres Tons von 0 bis 100. |
| **[!UICONTROL Veränderlicher Inhalt]** | Aktivieren Sie diese Option, damit die Mobile App mit der Benachrichtigung verknüpfte Medieninhalte herunterladen kann. Weiterführende Informationen dazu finden Sie im [Handbuch für Apple-Entwickler](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Relevanzwert]** | Setzen Sie einen Relevanzwert von 0 bis 100, um die Reihenfolge der Benachrichtigungen in der Benachrichtigungszusammenfassung zu priorisieren. Höhere Werte zeigen wichtigere Benachrichtigungen an. |
| **[!UICONTROL Unterbrechungsgrad]** | <ul> <li>**[!UICONTROL Aktiv]**: Ist dies als Standardeinstellung festgelegt, wird die Benachrichtigung sofort angezeigt, der Bildschirm wird beleuchtet und eventuell wird ein Ton abgespielt. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**[!UICONTROL Passiv]**: Die Benachrichtigung wird zur Benachrichtigungsliste hinzugefügt, ohne dass der Bildschirm beleuchtet oder ein Ton abgespielt wird. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**[!UICONTROL Zeitabhängig]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet, eventuell wird ein Ton abgespielt und der Fokusmodus kann umgangen werden. Für diese Stufe ist keine spezielle Berechtigung von Apple erforderlich.</li> <li>**[!UICONTROL Kritisch]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet und der Stummschaltungs- oder Fokusmodus wird umgangen. Beachten Sie, dass für diese Ebene eine spezielle Berechtigung von Apple erforderlich ist.</ul> |
| **[!UICONTROL Thread-ID]** | Kennung, mit der verknüpfte Benachrichtigungen gruppiert werden. Benachrichtigungen mit derselben Thread-ID sind als eine einzige Konversation oder einen einzigen Thread in der Benachrichtigungsliste organisiert. |
| **[!UICONTROL Kategorie]** | Geben Sie den Namen der Kategorie-ID an, die mit der Benachrichtigung verknüpft ist. Dies ermöglicht die Anzeige von Aktionsschaltflächen, mit denen der Benutzer direkt aus der Benachrichtigung heraus verschiedene Aufgaben ausführen kann, ohne die Anwendung zu öffnen. |
| **[!UICONTROL Zielinhalts-ID]** | Kennung, die angibt, welches Anwendungsfenster beim Öffnen der Benachrichtigung vorgezogen werden soll. |
| **[!UICONTROL Startbild]** | Geben Sie den Namen der Bilddatei für den Launch an, die angezeigt werden soll, wenn der Benutzer die Anwendung über die Benachrichtigung startet. Das ausgewählte Bild wird anstelle des regulären Startbildschirms Ihrer Anwendung angezeigt. |
| **[!UICONTROL Anwendungsvariablen]** | Ermöglicht die Definition des Benachrichtigungsverhaltens. Diese Variablen können vollständig angepasst werden und sind Teil der Payload der Nachricht, die an das Mobilgerät gesendet wird. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



