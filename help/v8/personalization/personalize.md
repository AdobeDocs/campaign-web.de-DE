---
title: Personalisieren von Inhalten in Campaign
description: Erfahren Sie, wie Sie Inhalte in der Web-Benutzeroberfläche von Adobe Campaign personalisieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: bf5ff77b695a5a8584bad7784597bf1521bcb23e
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 6%

---


# Personalisieren von Inhalten {#add-personalization}

Sie können jeden Versand mithilfe des Ausdruckseditors personalisieren, auf den in Feldern mit der **[!UICONTROL Personalisierungsdialogfeld öffnen]** -Symbol, z. B. die Betreffzeile, E-Mail-Links und Text-/Schaltflächeninhaltskomponenten. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen können.](gs-personalization.md/#access)

## Personalisierungssyntax {#syntax}

Personalisierungs-Tags folgen einer bestimmten Syntax: `<%= table.field %>`. Um beispielsweise den Nachnamen des Empfängers aus der Empfängertabelle einzufügen, verwenden Sie die `<%= recipient.lastName %>` Syntax.

Während der Versandvorbereitung interpretiert Adobe Campaign diese Tags automatisch und ersetzt sie durch die entsprechenden Feldwerte für jeden Empfänger. Sie können die tatsächliche Ersetzung anzeigen, indem Sie Ihren Inhalt simulieren.

Beim Hochladen von Kontakten aus einer externen Datei für einen eigenständigen E-Mail-Versand stehen alle Felder in der Eingabedatei zur Personalisierung zur Verfügung. Die Syntax sieht folgendermaßen aus: `<%= dataSource.field %>`.

## Personalisierungs-Tags hinzufügen {#add}

Gehen Sie wie folgt vor, um einem Versand Personalisierungs-Tags hinzuzufügen:

1. Öffnen Sie den Ausdruckseditor mithilfe der **[!UICONTROL Personalisierungsdialogfeld öffnen]** -Symbol, auf das über Textbearbeitungsfelder wie die Betreffzeile oder den SMS-Textkörper zugegriffen werden kann. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen können.](gs-personalization.md/#access)

   ![](assets/perso-access.png){width="800" align="center"}

1. Der Ausdruckseditor wird geöffnet. Die in der Adobe Campaign-Datenbank verfügbaren Personalisierungsfelder sind in verschiedene Menüs auf der linken Bildschirmseite unterteilt:

   ![](assets/perso-insert-field.png){width="800" align="center"}

   | Menü | Beschreibung |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png) | Die **[!UICONTROL Abonnentenanwendung]** enthält Felder, die mit den Abonnenten einer Anwendung in Verbindung stehen, wie z. B. das verwendete Terminal oder das Betriebssystem. *Dieses Menü ist nur für Push-Benachrichtigungen verfügbar* |
   | ![](assets/do-not-localize/perso-recipients-menu.png) | Die **[!UICONTROL Empfänger]** im Menü werden die in der Empfängertabelle definierten Felder aufgelistet, z. B. die Namen, das Alter oder die Adressen der Empfänger. Wann [Hochladen von Kontakten aus einer externen Datei](../audience/file-audience.md) für einen eigenständigen E-Mail-Versand enthält dieses Menü alle in der Eingabedatei verfügbaren Felder. |
   | ![](assets/do-not-localize/perso-message-menu.png) | Die **[!UICONTROL Nachricht]** enthält Felder, die mit den Versandlogs in Verbindung stehen, einschließlich aller Nachrichten, die über alle Kanäle an Empfänger oder Geräte gesendet werden, z. B. das Datum des letzten Ereignisses mit einem bestimmten Empfänger |
   | ![](assets/do-not-localize/perso-delivery-menu.png) | Die **[!UICONTROL Versand]** im Menü werden die Felder aufgelistet, die sich auf die für die Durchführung der Sendungen erforderlichen Parameter beziehen, wie z. B. den Versandkanal oder den Titel. |

   >[!NOTE]
   >
   >Standardmäßig werden in jedem Menü alle Felder der ausgewählten Tabelle aufgelistet (Empfänger, / Nachricht / Versand). Wenn Sie Felder aus mit der ausgewählten Tabelle verknüpften Tabellen einbeziehen möchten, aktivieren Sie die **[!UICONTROL Erweiterte Attribute anzeigen]** Option unterhalb der Liste.

1. Um ein Personalisierungsfeld hinzuzufügen, positionieren Sie den Cursor an der gewünschten Stelle in Ihrem Inhalt und klicken Sie auf die Schaltfläche `+` -Schaltfläche, um sie einzufügen.

1. Sobald Ihr Inhalt fertig ist, können Sie ihn speichern und das Rendering der Personalisierung testen, indem Sie Ihren Inhalt simulieren. Das folgende Beispiel zeigt die Personalisierung einer SMS-Nachricht mit dem Vornamen der Empfänger.

   ![](assets/perso-preview1.png){width="800" align="center"}

   ![](assets/perso-preview2.png){width="800" align="center"}
