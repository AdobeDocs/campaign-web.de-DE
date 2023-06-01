---
audience: end-user
title: Push-Benachrichtigungsversand erstellen
description: Erfahren Sie, wie Sie einen Push-Benachrichtigungsversand mit Adobe Campaign Web erstellen
badge: label="Alpha" type="Positive"
source-git-commit: 965c2d72d81233c98beb4e4bc3c76692c7bf3990
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 57%

---

# Push-Versand erstellen {#content-push}

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

Um Ihre Nachricht zu erstellen, klicken Sie auf die Schaltfläche **[!UICONTROL Titel]** und **[!UICONTROL body]** -Felder. Verwenden Sie den Ausdruckseditor, um Inhalte zu definieren, Daten zu personalisieren und dynamischen Inhalt hinzuzufügen.

Sie können einen **[!UICONTROL Untertitel]** hinzufügen, den Wert des Parameters „subtitle“ der iOS-Benachrichtigungs-Payload. Weitere Informationen finden Sie in diesem Abschnitt.

Im Modus Stille Push kann eine &quot;stille&quot;Benachrichtigung an eine Mobile App gesendet werden. Dem Benutzer wird die Ankunft der Benachrichtigung nicht mitgeteilt. Sie wird direkt an die Mobile App übertragen.

>[!ENDTABS]

## Erweiterte Einstellungen {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL Ton]**: Legt den Ton fest, der abgespielt werden soll, wenn das Gerät Ihre Benachrichtigung empfängt.

* **[!UICONTROL Anzahl der Benachrichtigungen]**: Legt die Zahl der neuen ungelesenen Informationen fest, die direkt auf dem Mobile-App-Symbol angezeigt werden.

* **[!UICONTROL Kanal-ID]**: Legen Sie die Kanal-ID Ihrer Benachrichtigung fest. Die Mobile App muss einen Kanal mit dieser Kennung erstellen, bevor eine Benachrichtigung mit dieser Kanalkennung empfangen werden kann.

* **[!UICONTROL Klick-Aktion]**: Legt die Aktion fest, die für das Klicken eines Benutzers auf Ihre Benachrichtigung zugewiesen ist.

* **[!UICONTROL Tag]**: Legt die Kennung fest, die zum Ersetzen bestehender Benachrichtigungen in der Benachrichtigungsablage verwendet werden soll.

* **[!UICONTROL Priorität]**: Legen Sie die Prioritätsstufen Ihrer Benachrichtigung auf &quot;Standard&quot;, &quot;Minimum&quot;, &quot;Niedrig&quot;oder &quot;Hoch&quot;fest. Weitere Informationen hierzu finden Sie in der FCM-Dokumentation.

* **[!UICONTROL Sichtbarkeit]**: Sie können für Ihre Benachrichtigung die Sichtbarkeitsstufen &quot;Öffentlich&quot;, &quot;Privat&quot; oder &quot;Geheim&quot; festlegen. Weitere Informationen hierzu finden Sie in der FCM-Dokumentation.

* **[!UICONTROL Sticky]**: Wenn diese Option deaktiviert ist, wird die Benachrichtigung automatisch verworfen, wenn der Benutzer darauf klickt. Wenn diese Option aktiviert ist, wird die Benachrichtigung auch dann angezeigt, wenn der Benutzer darauf klickt.

>[!TAB iOS]

* **[!UICONTROL Kritischer Warnmodus]**: Aktivieren Sie diese Option, um Ihrer Benachrichtigung Ton hinzuzufügen, selbst wenn das Handy des Benutzers im Fokusmodus eingestellt ist oder wenn der iPhone stummgeschaltet ist.

* **[!UICONTROL Badge entfernen]**: Aktivieren Sie diese Optionen, um den Badge-Wert zu aktualisieren.

* **[!UICONTROL Benachrichtigungsanzahl]**: Legen Sie eine Zahl fest, mit der die Anzahl der neuen ungelesenen Informationen direkt auf dem Anwendungssymbol angezeigt wird.

* **[!UICONTROL Lautstärke]**: Lautstärke Ihres Tons auf einer Skala von 0 bis 100.

* **[!UICONTROL Veränderlicher Inhalt]** (Nur iOS): Sendet das Flag für veränderlichen Inhalt in der Push-Payload und ermöglicht die Änderung des Inhalts der Push-Benachrichtigung durch eine im iOS SDK bereitgestellte Erweiterung der Benachrichtigungsdienstanwendung. Weiterführende Informationen dazu finden Sie im [Handbuch für Apple-Entwickler](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). Aktivieren Sie diese Option, damit die Mobile App Medieninhalte herunterladen kann.

* **[!UICONTROL Relevanzwert]**: Legen Sie einen Relevanzwert auf der Skala von 0 bis 100 fest. Das System verwendet diesen Wert, um die Benachrichtigungen in der Benachrichtigungszusammenfassung zu sortieren.

* **[!UICONTROL Unterbrechungsgrad]**:

   * **[!UICONTROL Aktiv]**: Ist dies als Standardeinstellung festgelegt, wird die Benachrichtigung sofort angezeigt, der Bildschirm wird beleuchtet und eventuell wird ein Ton abgespielt. Benachrichtigungen umgehen nicht den Fokusmodus.

   * **[!UICONTROL Passiv]**: Die Benachrichtigung wird zur Benachrichtigungsliste hinzugefügt, ohne dass der Bildschirm beleuchtet oder ein Ton abgespielt wird. Benachrichtigungen umgehen nicht den Fokusmodus.

   * **[!UICONTROL Zeitabhängig]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet, eventuell wird ein Ton abgespielt und der Fokusmodus kann umgangen werden. Für diese Stufe ist keine spezielle Berechtigung von Apple erforderlich.

   * **[!UICONTROL Kritisch]**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet und der Stummschaltungs- oder Fokusmodus wird umgangen. Beachten Sie, dass für diese Ebene eine spezielle Berechtigung von Apple erforderlich ist.

* **[!UICONTROL Thread-ID]**: Kennung, die verwendet wird, um verknüpfte Benachrichtigungen zu gruppieren.

* **[!UICONTROL Kategorie]**: Name Ihrer Kategorie-ID, über die Aktionsschaltflächen angezeigt werden. Mit diesen Benachrichtigungen können Benutzer rascher unterschiedliche Aufgaben ausführen, ohne die Anwendung öffnen oder darin navigieren zu müssen.

* **[!UICONTROL Zielgruppen-Inhalts-ID]**: Bezeichner, mit dem festgelegt wird, welches Anwendungsfenster beim Öffnen der Benachrichtigung vorgezogen werden soll.

* **[!UICONTROL Startbild]**: Name der anzuzeigenden Startbilddatei. Wenn der Benutzer Ihre Anwendung startet, wird das ausgewählte Bild anstelle des Startbildschirms Ihrer Anwendung angezeigt.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



