---
title: Personalisieren von Inhalten in Campaign
description: Erfahren Sie, wie Sie Inhalte in Adobe Campaign Web personalisieren
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '658'
ht-degree: 100%

---

# Personalisieren von Inhalten {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="Aktuelles Datum hinzufügen"
>abstract="Dieses Menü enthält Funktionen zur Datumsformatierung, die Sie zur Personalisierung Ihrer Inhalte verwenden können."

Die Personalisierung von Versandinhalten ist eine Schlüsselfunktion, mit der Sie Nachrichten an einzelne Empfängerinnen und Empfänger anpassen und so die Kommunikation relevanter und ansprechender gestalten können.

Passen Sie in Adobe Campaign mithilfe von [Profildaten](#data-personalization), z. B. Name, Standort oder frühere Interaktionen des Profils, und bestimmten [Variablen Ihres Versands](#variables-personalization) Elemente wie Text, Bilder und Angebote in Ihren Mitteilungen dynamisch an.

Die Personalisierung des Versands verbessert das Anwendererlebnis und die Interaktionsraten, was zu höherer Konversion und Kundenzufriedenheit führt.

## Verwenden von Profildaten zur Personalisierung {#data-personalization}

Personalisieren Sie jeden Versand mit Profildaten, indem Sie den Ausdruckseditor verwenden. Auf den Ausdruckseditor können Sie in allen Feldern mit dem Symbol **[!UICONTROL Personalisierungsdialog öffnen]** zugreifen, z. B. Betreffzeile, E-Mail-Links und Text-/Schaltflächen-Inhaltskomponenten. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen](gs-personalization.md/#access).

### Personalisierungssyntax {#syntax}

Personalisierungs-Tags folgen einer bestimmten Syntax: `<%= table.field %>`. Um beispielsweise den Nachnamen der Empfängerin bzw. des Empfängers aus der Empfängertabelle einzufügen, verwenden Sie die Syntax `<%= recipient.lastName %>`.

Während der Versandvorbereitung interpretiert Adobe Campaign diese Tags und ersetzt sie durch die entsprechenden Feldwerte für jede Person. Zeigen Sie die tatsächliche Ersetzung an, indem Sie Ihren Inhalt simulieren.

Beim Hochladen von Kontakten aus einer externen Datei für einen eigenständigen E-Mail-Versand sind alle Felder in der Eingabedatei zur Personalisierung verfügbar. Die Syntax sieht folgendermaßen aus: `<%= dataSource.field %>`.

### Hinzufügen von Personalisierungs-Tags {#add}

Gehen Sie wie folgt vor, um einem Versand Personalisierungs-Tags hinzuzufügen:

1. Öffnen Sie den Ausdruckseditor mithilfe des Symbols **[!UICONTROL Personalisierungsdialog öffnen]**, auf das über Textbearbeitungsfelder (wie Betreffzeile oder SMS-Text) zugegriffen werden kann. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen](gs-personalization.md/#access).

   ![Screenshot, der zeigt, wie auf das Personalisierungsdialogfeld zugegriffen wird](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. Der Ausdruckseditor wird geöffnet. Die in der Adobe Campaign-Datenbank verfügbaren Personalisierungsfelder sind in verschiedene Menüs auf der linken Seite des Bildschirms unterteilt:

   ![Screenshot mit dem Menü für Personalisierungsfelder](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menü | Beschreibung |
   |------|-------------|
   | ![Menüsymbol für abonnierte Anwendungen](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Das Menü **[!UICONTROL Abonnentenanwendung]** enthält Felder, die mit den Abonnentinnen und Abonnenten einer Anwendung in Verbindung stehen, wie z. B. das verwendete Terminal oder das Betriebssystem. *Dieses Menü ist nur für Push-Benachrichtigungen verfügbar.* |
   | ![Menüsymbol „Empfangende“](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Im Menü **[!UICONTROL Empfänger]** werden die in der Empfängertabelle definierten Felder aufgelistet, z. B. Namen, Alter oder Adressen der Empfängerinnen und Empfänger. Beim [Hochladen von Kontakten aus einer externen Datei](../audience/file-audience.md) für einen eigenständigen E-Mail-Versand enthält dieses Menü alle in der Eingabedatei verfügbaren Felder. |
   | ![Menüsymbol „Nachricht“](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Das Menü **[!UICONTROL Nachricht]** enthält Felder, die mit den Versandlogs in Verbindung stehen. Dazu gehören alle Nachrichten, die über alle Kanäle an Empfängerinnen und Empfänger oder Geräte gesendet werden, z. B. das Datum des letzten Ereignisses im Zusammenhang mit einer bestimmten Person. |
   | ![Menüsymbol „Versand“](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Das Menü **[!UICONTROL Versand]** enthält Felder, die sich auf die Parameter beziehen, die für die Durchführung von Sendungen erforderlich sind, wie z. B. Versandkanal oder Label. |

   >[!NOTE]
   >
   >Standardmäßig werden in jedem Menü alle Felder der ausgewählten Tabelle aufgelistet (Empfänger/Nachricht/Versand). Wenn Sie Felder aus mit der ausgewählten Tabelle verknüpften Tabellen einbeziehen möchten, aktivieren Sie die Option **[!UICONTROL Erweiterte Attribute anzeigen]** unterhalb der Liste.

1. Um ein Personalisierungsfeld hinzuzufügen, positionieren Sie den Cursor an der gewünschten Stelle in Ihrem Inhalt und klicken Sie zum Einfügen auf die Schaltfläche `+`.

1. Sobald Ihr Inhalt fertig ist, speichern Sie ihn und testen Sie das Rendering der Personalisierung, indem Sie Ihren Inhalt simulieren. Das folgende Beispiel zeigt die Personalisierung einer SMS-Nachricht mit dem Vornamen der Empfängerinnen und Empfänger.

   ![Screenshot der Vorschau der SMS-Personalisierung mit dem Vornamen der Empfängerin bzw. des Empfängers](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![Screenshot der Vorschau der SMS-Personalisierung mit dem Vornamen der Empfängerin bzw. des Empfängers](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Verwenden von Variablen für die Personalisierung {#variables-personalization}

Zudem werden Variablen verwendet, um Ihren Versand zu personalisieren. Erfahren Sie mehr über das [Hinzufügen von Variablen zu einem Versand](../advanced-settings/delivery-settings.md#variables-delivery).

Beispielsweise ist die Variable `deliveryType` wie folgt definiert:

![Screenshot zur Definition der Variablen „deliveryType“](assets/variables-deliveryType.png){zoomable="yes"}

Diese Variable wird im Versandinhalt verwendet, indem für dieses Beispiel das Symbol **[!UICONTROL Personalisierung hinzufügen]** und der Ausdruck `<%= variables.deliveryType %>` verwendet werden.

![Screenshot zur Verwendung der Variablen „deliveryType“ bei der Personalisierung](assets/variables-perso.png){zoomable="yes"}

Überprüfen Sie die Verwendung Ihrer Variablen mit der Schaltfläche **[!UICONTROL Inhalte simulieren]**.

![Screenshot der Simulation von Inhalten mit der Variablen „deliveryType“](assets/variables-simulate.png){zoomable="yes"}