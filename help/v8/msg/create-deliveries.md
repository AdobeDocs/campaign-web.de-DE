---
product: campaign
title: Arbeiten mit Sendungen
description: Erfahren Sie, wie Sie Ihren ersten Versand in Campaign Web erstellen
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 803a20ac-e75f-45c6-af89-054b84eb3405
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '930'
ht-degree: 100%

---

# Erstellen eines Versands {#create-delivery}

Sie können eigenständige Sendungen über das linke Menü **[!UICONTROL Sendungen]** oder im Kontext eines Workflows erstellen, egal ob er in einer Kampagne enthalten ist oder nicht.

Auf den folgenden Registerkarten erfahren Sie, wie Sie einen Versand erstellen:

>[!BEGINTABS]

>[!TAB Erstellen eines eigenständigen Versands]

Gehen Sie wie folgt vor, um einen eigenständigen Versand zu erstellen:

1. Navigieren Sie zum Menü **[!UICONTROL Sendungen]** im linken Navigationsmenü und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

   ![Screenshot mit der Schaltfläche „Versand erstellen“ im Menü „Sendungen“](assets/create-a-delivery.png){zoomable="yes"}

1. Wählen Sie einen Kanal für den Versand aus. 
1. Definieren Sie die Versandzielgruppe sowohl für die Hauptzielgruppe als auch für die Kontrollgruppe. [Weitere Informationen zu Zielgruppen](../audience/about-recipients.md).

   ![Screenshot mit der Benutzeroberfläche zur Zielgruppenauswahl](assets/select-audience.png){zoomable="yes"}{width="70%" align="left"}

1. Definieren Sie den Nachrichteninhalt. Weitere Informationen zu Versandkanälen und zum Definieren von Versandinhalten finden Sie in den folgenden Abschnitten:

   * [E-Mail-Kanal](../email/create-email.md)
   * [Push-Benachrichtigungs-Kanal](../push/gs-push.md)
   * [SMS-Kanal](../sms/create-sms.md)

1. (Optional) Definieren Sie den [Zeitplan](#gs-schedule) für den Versand. Wenn kein Zeitplan definiert ist, werden Nachrichten sofort nach dem Klicken auf die Schaltfläche **[!UICONTROL Senden]** gesendet.
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Überprüfen und senden]**, um Ihre Einstellungen zu überprüfen.
1. Verwenden Sie die Schaltfläche **[!UICONTROL Inhalte simulieren]**, um Ihren Versand und die Personalisierungseinstellungen zu testen. Weitere Informationen zur Simulation von Nachrichten finden Sie in [diesem Abschnitt](../preview-test/preview-test.md).
1. Klicken Sie auf die Schaltfläche **[!UICONTROL Vorbereiten]**, um die Zielgruppen-Population zu berechnen und die Nachrichten zu erstellen. Der Vorbereitungsschritt kann einige Minuten dauern. Nach Abschluss der Vorbereitung sind die Nachrichten versandbereit. Navigieren Sie im Falle eines Fehlers zu den **Logs**, um Benachrichtigungen und Warnungen einzusehen.
1. Überprüfen Sie die Ergebnisse und klicken Sie auf die Schaltfläche **[!UICONTROL Senden]**, um mit dem Senden von Nachrichten zu beginnen.
1. Sobald Nachrichten gesendet wurden, gehen Sie zum Abschnitt **Berichte**, um auf Schlüsselmetriken zuzugreifen. Weitere Informationen zu Versandberichten finden Sie in [diesem Abschnitt](../reporting/delivery-reports.md).

>[!TAB Erstellen eines Versands in einem Workflow]

Gehen Sie wie folgt vor, um einen Versand in einem Workflow zu erstellen:

1. Erstellen Sie einen neuen Workflow oder öffnen Sie einen vorhandenen. [Erfahren Sie mehr über Workflows](../workflows/gs-workflow-creation.md#gs-workflow-steps)
1. Fügen Sie eine Aktivität [**[!UICONTROL Zielgruppe erstellen]**](../workflows/activities/build-audience.md) hinzu und konfigurieren Sie sie. 
1. Klicken Sie auf das `+`-Symbol und wählen Sie eine Versandaktivität aus: **[!UICONTROL E-Mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Push-Benachrichtigung (Android)]** oder **[!UICONTROL Push-Benachrichtigung (iOS)]**. In [diesem Abschnitt](../workflows/activities/channels.md) erfahren Sie mehr über die Versandkanalaktivitäten in einem Workflow und darüber, wie Sie Versandinhalte definieren.

   ![Screenshot mit dem Hinzufügen einer Versandaktivität zu einem Workflow](assets/add-delivery-in-wf.png){zoomable="yes"}

1. Starten Sie den Workflow und überprüfen Sie die Protokolle.

Sie können Sendungen auch in einer Kampagne hinzufügen, ohne einen Workflow zu erstellen. Navigieren Sie dazu zur Registerkarte **[!UICONTROL Sendungen]** Ihrer Kampagne und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

![Screenshot mit der Erstellung eines Versands innerhalb einer Kampagne](assets/new-campaign-delivery.png){zoomable="yes"}

Die Konfigurationsschritte ähneln den Schritten für eigenständige Sendungen.

Weitere Informationen zur Konfiguration einer Kampagne und zur Verwaltung von Sendungen einer Kampagne finden Sie in [diesem Abschnitt](../campaigns/gs-campaigns.md).

>[!ENDTABS]

## Hinzufügen von Personalisierung {#personalization}

Nachrichten, die von Adobe Campaign versendet werden, können auf verschiedene Weise personalisiert werden. [Weitere Informationen zu Personalisierungsfunktionen](../personalization/gs-personalization.md)

Verwenden Sie Campaign, um dynamische Inhalte zu erstellen und personalisierte Nachrichten zu versenden. Personalisierungsfunktionen können kombiniert werden, um Ihre Nachrichten zu verbessern und ein individuelles Benutzererlebnis zu schaffen.

Sie können den Nachrichteninhalt wie folgt personalisieren:

* Einfügen von dynamischen **Personalisierungsfeldern**

  Personalisierungsfelder werden für die oberste Ebene der Nachrichtenpersonalisierung verwendet. Sie können jedes in der Datenbank verfügbare Feld aus dem Personalisierungseditor auswählen. Für einen Versand können Sie jedes Feld auswählen, das sich auf die Empfängerin oder den Empfänger, die Nachricht oder den Versand bezieht. Diese Personalisierungsattribute können in die Betreffzeile oder in den Text Ihrer Nachrichten eingefügt werden. [Weitere Informationen](../personalization/personalize.md)

* Einfügen von vordefinierten **Ausdrucksfragmenten**

  Campaign verfügt über eine Reihe von Ausdrucksfragmenten mit bestimmten Renderings, die Sie in Ihre Sendungen einfügen können. Sie können zum Beispiel ein Logo, eine Grußbotschaft oder einen Link zur Mirrorseite der Nachricht hinzufügen. Ausdrucksfragmente sind über einen eigenen Eintrag im Personalisierungseditor verfügbar. Sie können auch eigene Ausdrucksfragmente erstellen, die Ihren Anforderungen entsprechen. [Erfahren Sie, wie Sie Ausdrucksfragmente verwenden](../content/use-expression-fragments.md)

* Erstellen **bedingter Inhalte**

  Konfigurieren Sie bedingte Inhalte, um beispielsweise eine dynamische Personalisierung basierend auf dem Empfängerprofil hinzuzufügen. Textblöcke und/oder Bilder werden eingefügt, wenn eine bestimmte Bedingung erfüllt ist. [Weitere Informationen](../personalization/conditions.md)

* Hinzufügen **personalisierter Angebote**

  Fügen Sie je nach Empfängerstandort, aktuellem Wetter oder letzter Bestellung personalisierte Angebote in Ihren Nachrichteninhalt ein. [Weitere Informationen](../msg/offers.md)

## Anzeigen einer Vorschau und Testen Ihrer Sendungen

Nachdem der Nachrichteninhalt definiert wurde, können Sie eine Vorschau davon anzeigen, um das Rendering Ihrer Nachrichten zu steuern, und die Personalisierungseinstellungen mit Testprofilen überprüfen. [Weitere Informationen](../preview-test/preview-test.md)

## Planen des Versandzeitpunkts {#gs-schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Festlegen eines Kontaktdatums und einer Kontaktzeit"
>abstract="Das Datum und die genaue Uhrzeit für den Versand festlegen. Durch die Auswahl des für Ihre Marketing-Nachricht am besten geeigneten Zeitpunkts können Sie die Öffnungsraten maximieren."

Sie können für das Senden Ihrer Nachrichten das Datum und die genaue Uhrzeit festlegen. Durch die Auswahl des für Ihre Marketing-Nachricht am besten geeigneten Zeitpunkts können Sie die Öffnungsraten maximieren.

Um einen Versand zeitlich zu planen, öffnen Sie den Versand und navigieren Sie zum Abschnitt **[!UICONTROL Zeitplan]**. Verwenden Sie den Umschalter **[!UICONTROL Zeitplanung aktivieren]**, um dies zu aktivieren, und legen Sie das gewünschte Datum und die gewünschte Uhrzeit für den Versand fest. Nach dem Versand beginnt der eigentliche Versand am von Ihnen definierten Kontaktdatum.

![Screenshot der Planungsbenutzeroberfläche für einen Versand](assets/schedule.png){zoomable="yes"}

Standardmäßig ist die Option **[!UICONTROL Bestätigung vor dem Senden aktivieren]** aktiviert. Für diese Option müssen Sie das Senden bestätigen, bevor der Versand zum geplanten Zeitpunkt gesendet wird. Wenn Sie den Versand automatisch zum geplanten Zeitpunkt durchführen lassen möchten, können Sie diese Option deaktivieren.

Erfahren Sie Schritte für die Durchführung eines zeitlich geplanten Versands in [diesem Abschnitt](../monitor/prepare-send.md#schedule-the-send).

## Überwachung und Trackinglogs {#gs-tracking-logs}

Die Überwachung Ihrer Sendungen nach deren Versand ist ein wichtiger Schritt, um sicherzustellen, dass Ihre Marketing-Kampagnen effizient sind und Ihre Kundschaft erreichen.

Sie können nach dem Versand überwachen sowie nachvollziehen, wie Zustellungsfehler und Quarantänen gehandhabt werden.

Weitere Informationen zu den Überwachungs- und Tracking-Funktionen finden Sie in [diesem Abschnitt](../reporting/gs-reports.md).