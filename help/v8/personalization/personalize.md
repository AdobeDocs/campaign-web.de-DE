---
title: Personalisieren von Inhalten in Campaign
description: Erfahren Sie, wie Sie Inhalte in Adobe Campaign Web personalisieren
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 68%

---


# Personalisieren von Inhalten {#add-personalization}

Personalization von Versandinhalten ist eine wichtige Funktion, mit der Sie Nachrichten an einzelne Empfänger anpassen und so die Kommunikation relevanter und ansprechender gestalten können.

In Adobe Campaign können Sie mithilfe von [Profildaten](#data-personalization), z. B. den Namen, den Speicherort oder frühere Interaktionen des Profils, und bestimmten [Variablen Ihres Versands](#variables-personalization), Elemente wie Text, Bilder und Angebote dynamisch anpassen.

Die Personalisierung des Versands verbessert nicht nur das Benutzererlebnis, sondern verbessert auch die Interaktionsraten, was zu einer höheren Konversion und Kundenzufriedenheit führt.

## Verwenden von Profildaten zur Personalisierung {#data-personalization}

Sie können jeden Versand mit Profildaten personalisieren, indem Sie den Ausdruckseditor verwenden, auf den in Feldern mit dem Symbol **[!UICONTROL Personalisierungsdialogfeld öffnen]** zugegriffen werden kann, z. B. die Betreffzeile, E-Mail-Links und die Komponenten für Text-/Schaltflächeninhalt. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen](gs-personalization.md/#access)

### Personalisierungssyntax {#syntax}

Personalisierungs-Tags folgen einer bestimmten Syntax: `<%= table.field %>`. Um beispielsweise den Nachnamen der Empfängerin bzw. des Empfängers aus der Empfängertabelle einzufügen, verwenden Sie die Syntax `<%= recipient.lastName %>`.

Während der Versandvorbereitung interpretiert Adobe Campaign diese Tags automatisch und ersetzt sie durch die entsprechenden Feldwerte für jede Person. Sie können die tatsächliche Ersetzung anzeigen, indem Sie Ihren Inhalt simulieren.

Beim Hochladen von Kontakten aus einer externen Datei für einen eigenständigen E-Mail-Versand sind alle Felder in der Eingabedatei zur Personalisierung verfügbar. Die Syntax sieht folgendermaßen aus: `<%= dataSource.field %>`.

### Hinzufügen von Personalisierungs-Tags {#add}

Gehen Sie wie folgt vor, um einem Versand Personalisierungs-Tags hinzuzufügen:

1. Öffnen Sie den Ausdruckseditor mithilfe des Symbols **[!UICONTROL Personalisierungsdialog öffnen]**, auf das über Textbearbeitungsfelder (wie die Betreffzeile oder der SMS-Text) zugegriffen werden kann. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. Der Ausdruckseditor wird geöffnet. Die in der Adobe Campaign-Datenbank verfügbaren Personalisierungsfelder sind in verschiedene Menüs auf der linken Seite des Bildschirms unterteilt:

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menü | Beschreibung |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Das Menü **[!UICONTROL Abonnentenanwendung]** enthält Felder, die mit den Abonnentinnen und Abonnenten einer Anwendung in Verbindung stehen, wie z. B. das verwendete Terminal oder das Betriebssystem. *Dieses Menü ist nur für Push-Benachrichtigungen verfügbar* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Im Menü **[!UICONTROL Empfänger]** werden die in der Empfängertabelle definierten Felder aufgelistet, z. B. Namen, Alter oder Adressen der Empfängerinnen und Empfänger. Beim [Hochladen von Kontakten aus einer externen Datei](../audience/file-audience.md) für einen eigenständigen E-Mail-Versand enthält dieses Menü alle in der Eingabedatei verfügbaren Felder. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Das Menü **[!UICONTROL Nachricht]** enthält Felder, die mit den Versandlogs in Verbindung stehen. Dazu gehören alle Nachrichten, die über alle Kanäle an Empfängerinnen und Empfänger oder Geräte gesendet werden, z. B. das Datum des letzten Ereignisses im Zusammenhang mit einer bestimmten Person. |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Das Menü **[!UICONTROL Versand]** listet Felder auf, die sich auf die Parameter beziehen, die für die Durchführung von Sendungen erforderlich sind, wie beispielsweise den Versandkanal oder die Bezeichnung. |

   >[!NOTE]
   >
   >Standardmäßig werden in jedem Menü alle Felder der ausgewählten Tabelle aufgelistet (Empfänger/Nachricht/Versand). Wenn Sie Felder aus mit der ausgewählten Tabelle verknüpften Tabellen einbeziehen möchten, aktivieren Sie die Option **[!UICONTROL Erweiterte Attribute anzeigen]** unterhalb der Liste.

1. Um ein Personalisierungsfeld hinzuzufügen, positionieren Sie den Cursor an der gewünschten Stelle in Ihrem Inhalt und klicken Sie zum Einfügen auf die Schaltfläche `+`.

1. Sobald Ihr Inhalt fertig ist, können Sie ihn speichern und das Rendering der Personalisierung testen, indem Sie Ihren Inhalt simulieren. Das folgende Beispiel zeigt die Personalisierung einer SMS-Nachricht mit dem Vornamen der Empfängerinnen und Empfänger.

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Variablen für die Personalisierung verwenden {#variables-personalization}

Sie können auch Variablen verwenden, um Ihren Versand zu personalisieren.
Erfahren Sie mehr über [Hinzufügen von Variablen zu einem Versand](../advanced-settings/delivery-settings.md#variables-delivery).

Beispielsweise ist die Variable `deliveryType` wie unten definiert.

![](assets/variables-deliveryType.png){zoomable="yes"}

Diese Variable kann im Versandinhalt verwendet werden, indem für unser Beispiel das Symbol **[!UICONTROL Personalization hinzufügen]** und der Ausdruck `<%= variables.deliveryType %>` verwendet werden.

![](assets/variables-perso.png){zoomable="yes"}

Sie können die Verwendung Ihrer Variablen mit der Schaltfläche **[!UICONTROL Inhalt simulieren]** überprüfen.

![](assets/variables-simulate.png){zoomable="yes"}
