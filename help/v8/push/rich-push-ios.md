---
audience: end-user
title: Erstellen eines Versands von Rich-Push-Benachrichtigungen für iOS
description: Erfahren Sie, wie Sie einen Versand von Rich-Push-Benachrichtigungen für iOS mit Adobe Campaign Web erstellen.
exl-id: e6058d60-9f34-412b-aac2-6e319a3ab898
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 48%

---

# Erstellen eines Rich-Push-Versands für iOS {#rich-push}

>[!IMPORTANT]
>
>Bevor Sie eine Rich-Push-Benachrichtigung entwerfen, müssen Sie Ihren V2-Connector konfigurieren. Eine detaillierte Vorgehensweise dazu finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign-classic/using/sending-messages/sending-push-notifications/configure-the-mobile-app/configuring-the-mobile-application).

## Festlegen des Inhalts der Benachrichtigung {#push-message}

Nachdem Ihr Push-Versand erstellt wurde, definieren Sie seinen Inhalt mithilfe einer der folgenden Vorlagen:

* **Standard** ermöglicht es Ihnen, Benachrichtigungen mit einem einfachen Symbol und einem zugehörigen Bild zu senden.
* **Einfach** ermöglicht es Ihnen, Text, Bilder und Schaltflächen in Ihre Benachrichtigungen einzufügen.
* **Karussell** ermöglicht es Ihnen, Benachrichtigungen mit Text und mehreren Bildern zu senden, zwischen denen die Benutzenden hin und her wischen können.
* **Timer** fügt einen Live-Countdown-Timer in Ihre Benachrichtigungen ein.

Weitere Informationen zum Personalisieren dieser Vorlagen finden Sie auf den folgenden Registerkarten.

>[!BEGINTABS]

>[!TAB Standard]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Standard]** aus.

   ![Standardbildschirm zur Vorlagenauswahl](assets/rich_push_ios_default_1.png)

1. Geben Sie in das Feld **[!UICONTROL Titel]** die Bezeichnung ein, die in der Liste der im Benachrichtigungscenter verfügbaren Benachrichtigungen erscheinen soll.

   Dieses Feld definiert den Wert des **title** der iOS-Benachrichtigungs-Payload.

1. Sie können optional einen **[!UICONTROL Untertitel]** hinzufügen, der dem Parameter **subtitle** der iOS-Benachrichtigungs-Payload entspricht.

1. Geben Sie den Inhalt der Nachricht in das Feld **[!UICONTROL Nachricht]** ein.

1. Mit dem Ausdruckseditor können Sie Inhalte definieren, Daten personalisieren und dynamische Inhalte hinzufügen. [Weitere Informationen](../personalization/personalize.md)

   ![Bildschirm des Ausdruckseditors](assets/rich_push_ios_default_2.png)

1. Um Ihre Push-Benachrichtigung weiter zu personalisieren, wählen Sie eine URL **[!UICONTROL Startbild]**, die Sie Ihrer Push-Benachrichtigung hinzufügen können.

1. Navigieren Sie in der Dropdown-Liste **[!UICONTROL Erweiterte Einstellungen]** zur Registerkarte **[!UICONTROL Ton und Badge]**, um zusätzliche Einstellungen wie Ton- und Badge-Optionen für Ihre Benachrichtigungen anzupassen. [Weitere Informationen](#sound-badge)

   ![Bildschirm für Ton- und Badge-Einstellungen](assets/rich_push_ios_default_3.png)

1. Weitere Anpassungsmöglichkeiten finden Sie unter **[!UICONTROL zusätzlichen Optionen]** für Ihre Push-Benachrichtigungen. [Weitere Informationen](#push-advanced)

   ![Bildschirm mit zusätzlichen Optionen](assets/rich_push_ios_default_4.png)

1. Ihre **[!UICONTROL Anwendungsvariablen]** werden automatisch von der Registerkarte **[!UICONTROL Anwendungsvariablen]** hinzugefügt. Damit können Sie das Benachrichtigungsverhalten definieren, z. B. die Konfiguration eines bestimmten Anwendungsbildschirms, der angezeigt werden soll, wenn Benutzende die Benachrichtigung aktivieren.

Nachdem Sie den Nachrichteninhalt definiert haben, verwenden Sie Testabonnentinnen und Testabonnenten, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Einfach]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Einfach]**.

   ![Grundlegender Bildschirm zur Vorlagenauswahl](assets/rich_push_ios_basic_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Erweiterter Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der **[!UICONTROL Nachricht]**-Text wird in der reduzierten Ansicht angezeigt, während die **[!UICONTROL erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![Bildschirm für die Nachrichtenkomposition](assets/rich_push_ios_basic_2.png)

1. Mit dem Ausdruckseditor können Sie Inhalte definieren, Daten personalisieren und dynamische Inhalte hinzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Sie können optional einen **[!UICONTROL Untertitel]** hinzufügen, der dem Parameter **subtitle** der iOS-Benachrichtigungs-Payload entspricht.

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die einem Benutzerklick auf Ihre Benachrichtigung zugeordnet ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Um Ihre Push-Benachrichtigung weiter zu personalisieren, wählen Sie eine URL **[!UICONTROL Startbild]**, die Sie Ihrer Push-Benachrichtigung hinzufügen können.

1. Navigieren Sie in der Dropdown-Liste **[!UICONTROL Erweiterte Einstellungen]** zur Registerkarte **[!UICONTROL Ton und Badge]**, um zusätzliche Einstellungen wie Ton- und Badge-Optionen für Ihre Benachrichtigungen anzupassen. [Weitere Informationen](#sound-badge)

   ![Bildschirm für Ton- und Badge-Einstellungen](assets/rich_push_ios_basic_3.png)

1. Geben Sie im Menü **[!UICONTROL Farboptionen]** hexadezimale Farbcodes für die Felder **[!UICONTROL Hintergrundfarbe der Benachrichtigung]**, **[!UICONTROL Hintergrundfarbe der Benachrichtigung]** und **[!UICONTROL Textfarbe der Nachricht]** ein.

   ![Bildschirm mit Farboptionen](assets/rich_push_ios_basic_4.png)

1. Weitere Anpassungsmöglichkeiten finden Sie unter **[!UICONTROL zusätzlichen Optionen]** für Ihre Push-Benachrichtigungen. [Weitere Informationen](#push-advanced)

1. Ihre **[!UICONTROL Anwendungsvariablen]** werden automatisch von der Registerkarte **[!UICONTROL Anwendungsvariablen]** hinzugefügt. Damit können Sie das Benachrichtigungsverhalten definieren, z. B. die Konfiguration eines bestimmten Anwendungsbildschirms, der angezeigt werden soll, wenn Benutzende die Benachrichtigung aktivieren.

Nachdem Sie den Nachrichteninhalt definiert haben, verwenden Sie Testabonnentinnen und Testabonnenten, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Karussell]

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Vorlage]** die Option **[!UICONTROL Karussell]**.

   ![Bildschirm zur Karussellvorlagenauswahl](assets/rich_push_ios_carousel_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Erweiterter Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der **[!UICONTROL Nachricht]**-Text wird in der reduzierten Ansicht angezeigt, während die **[!UICONTROL erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![Bildschirm für die Nachrichtenkomposition](assets/rich_push_ios_carousel_2.png)

1. Mit dem Ausdruckseditor können Sie Inhalte definieren, Daten personalisieren und dynamische Inhalte hinzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Sie können optional einen **[!UICONTROL Untertitel]** hinzufügen, der dem Parameter **subtitle** der iOS-Benachrichtigungs-Payload entspricht.

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die einem Benutzerklick auf Ihre Benachrichtigung zugeordnet ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Wählen Sie, wie das **[!UICONTROL Karussell]** bedient werden soll:

   * **[!UICONTROL Automatisch]**: Die Bilder werden automatisch in vordefinierten Intervallen als Folien wiedergegeben.
   * **[!UICONTROL Manuell]**: Benutzende können manuell zwischen den Folien streichen, um durch die Bilder zu navigieren.

1. Klicken Sie **[!UICONTROL Bild hinzufügen]** und geben Sie Ihre **[!UICONTROL Bild]** URL, **[!UICONTROL Text]** und **[!UICONTROL Action-URI]** ein.

   Stellen Sie sicher, dass Sie mindestens drei und maximal fünf Bilder einfügen.

   ![Bildschirm zum Hinzufügen von Karussellbildern](assets/rich_push_ios_carousel_3.png)

1. Bearbeiten Sie die Reihenfolge Ihrer Bilder mit den nach oben bzw. nach unten zeigenden Pfeilen.

1. Navigieren Sie in der Dropdown-Liste **[!UICONTROL Erweiterte Einstellungen]** zur Registerkarte **[!UICONTROL Ton und Badge]**, um zusätzliche Einstellungen wie Ton- und Badge-Optionen für Ihre Benachrichtigungen anzupassen. [Weitere Informationen](#sound-badge)

1. Geben Sie im Menü **[!UICONTROL Farboptionen]** hexadezimale Farbcodes für die Felder **[!UICONTROL Hintergrundfarbe der Benachrichtigung]**, **[!UICONTROL Hintergrundfarbe der Benachrichtigung]** und **[!UICONTROL Textfarbe der Nachricht]** ein.

   ![Bildschirm mit Farboptionen](assets/rich_push_ios_carousel_4.png)

1. Weitere Anpassungsmöglichkeiten finden Sie unter **[!UICONTROL zusätzlichen Optionen]** für Ihre Push-Benachrichtigungen. [Weitere Informationen](#push-advanced)

1. Ihre **[!UICONTROL Anwendungsvariablen]** werden automatisch von der Registerkarte **[!UICONTROL Anwendungsvariablen]** hinzugefügt. Damit können Sie das Benachrichtigungsverhalten definieren, z. B. die Konfiguration eines bestimmten Anwendungsbildschirms, der angezeigt werden soll, wenn Benutzende die Benachrichtigung aktivieren.

Nachdem Sie den Nachrichteninhalt definiert haben, verwenden Sie Testabonnentinnen und Testabonnenten, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!TAB Timer]

1. Wählen Sie in der Dropdown-Liste **[!UICONTROL Benachrichtigungstyp]** die Option **[!UICONTROL Timer]** aus.

   ![Auswahlbildschirm der Timervorlage](assets/rich_push_ios_timer_1.png)

1. Um Ihre Nachricht zu erstellen, geben Sie Ihren Text in die Felder **[!UICONTROL Titel]**, **[!UICONTROL Erweiterter Titel]**, **[!UICONTROL Nachricht]** und **[!UICONTROL Erweiterte Nachricht]** ein.

   Der **[!UICONTROL Nachricht]**-Text wird in der reduzierten Ansicht angezeigt, während die **[!UICONTROL erweiterte Nachricht]** angezeigt wird, wenn die Benachrichtigung erweitert wird.

   ![Bildschirm für die Nachrichtenkomposition](assets/rich_push_ios_timer_2.png)

1. Mit dem Ausdruckseditor können Sie Inhalte definieren, Daten personalisieren und dynamische Inhalte hinzufügen. [Weitere Informationen](../personalization/personalize.md)

1. Sie können optional einen **[!UICONTROL Untertitel]** hinzufügen, der dem Parameter **subtitle** der iOS-Benachrichtigungs-Payload entspricht.

1. Fügen Sie die URL hinzu, die die **[!UICONTROL Klick-Aktion]** definiert, die einem Benutzerklick auf Ihre Benachrichtigung zugeordnet ist. Dies bestimmt das Verhalten bei der Interaktion der Benutzenden mit der Benachrichtigung, z. B. beim Öffnen eines bestimmten Bildschirms oder beim Ausführen einer bestimmten Aktion in der App.

1. Um Ihre Push-Benachrichtigung weiter zu personalisieren, wählen Sie eine URL **[!UICONTROL Startbild]**, die Sie Ihrer Push-Benachrichtigung hinzufügen können.

1. Stellen Sie die **[!UICONTROL Dauer des Timers]** in Sekunden oder den **[!UICONTROL Zeitstempel für Timer-Ende]** auf einen bestimmten Epoch-Zeitstempel ein.

   ![Einstellungsbildschirm für die Timerdauer](assets/rich_push_ios_timer_3.png)

1. Geben Sie den Text und das Bild, die angezeigt werden, nachdem der Timer abgelaufen ist, in die Felder **[!UICONTROL Alternativer Titel]**, **[!UICONTROL Alternative Nachricht]** und **[!UICONTROL Alternatives Startbild]** ein.

   ![Bildschirm für alternative Nachrichteneinstellungen](assets/rich_push_ios_timer_4.png)

1. Navigieren Sie in der Dropdown-Liste **[!UICONTROL Erweiterte Einstellungen]** zur Registerkarte **[!UICONTROL Ton und Badge]**, um zusätzliche Einstellungen wie Ton- und Badge-Optionen für Ihre Benachrichtigungen anzupassen. [Weitere Informationen](#sound-badge)

1. Geben Sie im Menü **[!UICONTROL Farboptionen]** hexadezimale Farbcodes für die Felder **[!UICONTROL Hintergrundfarbe der Benachrichtigung]**, **[!UICONTROL Hintergrundfarbe der Benachrichtigung]** und **[!UICONTROL Textfarbe der Nachricht]** ein.

1. Weitere Anpassungsmöglichkeiten finden Sie unter **[!UICONTROL zusätzlichen Optionen]** für Ihre Push-Benachrichtigungen. [Weitere Informationen](#push-advanced)

1. Ihre **[!UICONTROL Anwendungsvariablen]** werden automatisch von der Registerkarte **[!UICONTROL Anwendungsvariablen]** hinzugefügt. Damit können Sie das Benachrichtigungsverhalten definieren, z. B. die Konfiguration eines bestimmten Anwendungsbildschirms, der angezeigt werden soll, wenn Benutzende die Benachrichtigung aktivieren.

Nachdem Sie den Nachrichteninhalt definiert haben, verwenden Sie Testabonnentinnen und Testabonnenten, um die Nachricht in der Vorschau anzuzeigen und zu testen.

>[!ENDTABS]

## Erweiterte Einstellungen für Push-Benachrichtigungen {#push-advanced}

### Optionen für Ton und Badge {#sound-badge}

| Parameter | Beschreibung |
|-----------|-------------|
| **[!UICONTROL Kritischer Alarmmodus]** | Aktivieren Sie diese Option, um Ihrer Benachrichtigung einen Ton hinzuzufügen, selbst wenn das Handy des Benutzers im Fokusmodus eingestellt oder stummgeschaltet ist. |
| **[!UICONTROL Badge entfernen]** | Aktivieren Sie diese Option, um den Badge-Wert zu aktualisieren. |
| **[!UICONTROL Ton]** | Legt den Ton fest, der abgespielt werden soll, wenn das Gerät Ihre Benachrichtigung erhält. |
| **[!UICONTROL Anzahl der Benachrichtigungen]** | Legen Sie eine Zahl fest, die direkt auf dem Anwendungssymbol angezeigt werden soll und die Anzahl der neuen ungelesenen Benachrichtigungen angibt. |
| **[!UICONTROL Lautstärke]** | Stellen Sie die Lautstärke Ihres Tons auf 0 bis 100 ein. Töne müssen in der App vorhanden sein und bei der Erstellung des Dienstes definiert werden. |

### Farboptionen {#color}

| Parameter | Beschreibung |
|-----------|-------------|
| **[!UICONTROL Hintergrundfarbe der Benachrichtigungen]** | Legen Sie die Farbe Ihres Benachrichtigungshintergrunds mit hexadezimalen Farbcodes fest. |
| **[!UICONTROL Titelfarbe]** | Legen Sie die Farbe Ihres Titels mithilfe von Hex-Farbcodes fest. |
| **[!UICONTROL Farbe des Nachrichtentextes]** | Legen Sie die Farbe Ihres Textes mithilfe von Hex-Farbcodes fest. |

### Erweiterte Optionen {#notification-options}

| Parameter | Beschreibung |
|-----------|-------------|
| **[!UICONTROL Veränderlicher Inhalt]** | Aktivieren Sie diese Option, damit die Mobile App Medieninhalte herunterladen kann. |
| **[!UICONTROL Relevanzwert]** | Legen Sie einen Relevanzwert auf der Skala von 0 bis 100 fest. Das System verwendet diese Einstellung, um Benachrichtigungen in der Zusammenfassung der Benachrichtigungen zu sortieren. |
| **[!UICONTROL Unterbrechungsgrad]** | <ul><li>**Aktiv**: Ist dies als Standardeinstellung festgelegt, wird die Benachrichtigung sofort angezeigt, der Bildschirm wird beleuchtet und eventuell wird ein Ton abgespielt. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**Passiv**: Die Benachrichtigung wird zur Benachrichtigungsliste hinzugefügt, ohne dass der Bildschirm beleuchtet oder ein Ton abgespielt wird. Benachrichtigungen umgehen nicht den Fokusmodus.</li><li>**Zeitabhängig**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet, eventuell wird ein Ton abgespielt und der Fokusmodus wird umgangen. Für diese Ebene ist keine spezielle Berechtigung von Apple erforderlich.</li><li>**Kritisch**: Die Benachrichtigung wird sofort angezeigt, der Bildschirm wird beleuchtet und der Stummschaltungs- oder Fokusmodus wird umgangen. Beachten Sie, dass für diese Ebene eine spezielle Berechtigung von Apple erforderlich ist.</li></ul> |
| **[!UICONTROL Thread-ID]** | Legen Sie die Kennung fest, die zur Gruppierung zusammengehöriger Meldungen verwendet wird. |
| **[!UICONTROL Kategorie]** | Legen Sie den Namen Ihrer Kategorie-ID fest, über die Aktionsschaltflächen angezeigt werden. Diese Benachrichtigungen ermöglichen es Benutzerinnen und Benutzern, verschiedene Aufgaben als Reaktion auf eine Benachrichtigung schneller auszuführen, ohne die App öffnen oder darin navigieren zu müssen. |
| **[!UICONTROL ID des Zielinhalts]** | Legt eine Kennung fest, die angibt, welches Anwendungsfenster beim Öffnen der Benachrichtigung in den Vordergrund gebracht werden soll. |