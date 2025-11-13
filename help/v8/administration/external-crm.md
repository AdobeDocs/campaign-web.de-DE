---
title: Verwalten eines externen Kontos
description: Informationen zum Konfigurieren externer CRM-Konten
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: ht
source-wordcount: '857'
ht-degree: 100%

---

# Externes CRM-Konto {#external-crm}

Verwenden Sie ein externes Konto vom Typ „CRM“, um Adobe Campaign mit einer Drittanbieterdatenbank zu verbinden.

Die Konfigurationseinstellungen für dieses externe Konto sind von der konkreten Datenbank-Engine abhängig, mit der Sie eine Verbindung herstellen. Detaillierte Anweisungen zur Einrichtung der einzelnen unterstützten Datenbanken finden Sie in den folgenden Abschnitten.

## Microsoft Dynamics CRM

Über das externe Konto „Microsoft Dynamics CRM“ können Sie Ihre Campaign-Instanz mit Ihrer externen Microsoft Dynamics CRM-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Microsoft Dynamics CRM“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Microsoft Dynamics CRM“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Microsoft Dynamics CRM]** zu konfigurieren, füllen Sie folgende Felder aus:

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Microsoft Dynamics CRM“.](assets/crm-microsoft-1.png)

   +++ Für „CRM-OAuth-Typ“: Passwort-Anmeldedaten

   * **[!UICONTROL Server]**: Geben Sie die URL Ihres Microsoft CRM-Servers ein.

     Um die URL Ihres Microsoft CRM-Servers zu finden, melden Sie sich bei Ihrem Microsoft Dynamics CRM-Konto an, wählen Sie „Dynamics 365“ aus und öffnen Sie dann Ihre Anwendung. Die Server-URL wird in der Adressleiste Ihres Browsers angezeigt, z. B.:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Konto]**: Geben Sie das Konto an, das für die Anmeldung bei Microsoft CRM verwendet wird.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem angegebenen Konto verknüpfte Passwort ein.

   * **[!UICONTROL Clientkennung]**: Geben Sie die Client-ID ein, die im Verwaltungsportal von Microsoft Azure zu finden ist.

   * **[!UICONTROL CRM-Version]**: Hier wählen Sie die CRM-Version „Dynamics CRM 365“ aus.

   +++

   </br>

   +++ Für „CRM-OAuth-Typ“: Zertifikat

   * **[!UICONTROL Server]**: Geben Sie die URL Ihres Microsoft CRM-Servers ein.

     Um die URL Ihres Microsoft CRM-Servers zu finden, melden Sie sich bei Ihrem Microsoft Dynamics CRM-Konto an, wählen Sie „Dynamics 365“ aus und öffnen Sie dann Ihre Anwendung. Die Server-URL wird in der Adressleiste Ihres Browsers angezeigt, z. B.:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Privater Schlüssel (Base64-kodiert)]**: Geben Sie den im Base64-Format kodierten privaten Schlüssel an.

     Dazu können Sie einen Base64-Encoder oder die Befehlszeile `base64 -w0 private.key` für Linux verwenden.

   * **[!UICONTROL Benutzerdefinierte Schlüsselkennung]**: Geben Sie die benutzerdefinierte Schlüsselkennung ein, die für Ihr Zertifikat verwendet wird.

   * **[!UICONTROL Schlüsselkennung]**: Geben Sie die Schlüssel-ID ein, die mit Ihrem Zertifikat verknüpft ist.

   * **[!UICONTROL Clientkennung]**: Geben Sie die Client-ID ein, die in der Microsoft Azure-Verwaltung zu finden ist.

   * **[!UICONTROL CRM-Version]**: Hier wählen Sie die CRM-Version „Dynamics CRM 365“ aus.

   +++

1. Rufen Sie nach dem Einrichten der Verbindung den **[!UICONTROL Konfigurationsassistenten für Microsoft CRM]** auf, um Ihre Microsoft CRM-Tabellenliste zu generieren.

   Klicken Sie auf **[!UICONTROL Weiter]**, um die erforderlichen Tabellen auszuwählen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Microsoft Dynamics CRM“.](assets/crm-microsoft-2.png)

1. Wählen Sie die abzurufenden Microsoft CRM-Tabellen aus oder fügen Sie eine Remote-Tabelle hinzu, indem Sie das **[!UICONTROL Tabellen-Label]** und den **[!UICONTROL internen Tabellennamen]** angeben und dann den Umschalter **[!UICONTROL Ausgewählt]** aktivieren.

   Klicken Sie auf **[!UICONTROL Weiter]**.

1. Klicken Sie auf **[!UICONTROL Start]**, um mit der Erstellung des Microsoft CRM-Schemas basierend auf den ausgewählten Tabellen zu beginnen.

1. Befolgen Sie die Anweisungen am Bildschirm, um Seiten aus dem Marketing-Verlauf und der Abonnementverwaltung von Adobe Campaign direkt in Microsoft Dynamics CRM einzufügen.

1. Klicken Sie auf **[!UICONTROL Marketing-Verlaufs-URLs anzeigen]**, um die URLs für die Integration von Seiten aus dem Marketing-Verlauf anzuzeigen, oder auf **[!UICONTROL URLs für Lead-Abonnements anzeigen]**, um die URLs für die Integration von Seiten aus der Abonnementverwaltung anzuzeigen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Microsoft Dynamics CRM“.](assets/crm-microsoft-3.png)

1. Klicken Sie nach Abschluss der Konfiguration Ihres externen Kontos „Microsoft CRM“ auf **[!UICONTROL Speichern]**.

1. Nachdem Sie Ihr externes Konto erstellt haben, können Sie auf **[!UICONTROL Auflistungssynchronisation…]** klicken, um automatisch Auflistungen von Microsoft CRM mit der Adobe Campaign Web-Benutzeroberfläche zu synchronisieren.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Microsoft CRM“.](assets/crm-microsoft-4.png)

1. Wählen Sie die Adobe Campaign-Auflistung aus, die der Microsoft CRM-Auflistung entspricht.

   Um Adobe Campaign-Werte durch Microsoft CRM-Werte zu ersetzen, aktivieren Sie die Option **[!UICONTROL Ersetzen]**.

## Salesforce {#salesforce}

Um dieses externe Konto „Salesforce“ für die gemeinsame Verwendung mit Adobe Campaign zu konfigurieren, müssen Sie die folgenden Informationen eingeben:

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Salesforce.com“ als **[!UICONTROL Anbietertyp]** aus.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Salesforce“.](assets/crm-salesforce-1.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Salesforce]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL CRM-OAuth-Typ]**: **[!UICONTROL Passwort-Anmeldedaten]** oder **[!UICONTROL Anmeldedaten]**

   * **[!UICONTROL Konto]**: Das für die Anmeldung bei Salesforce CRM verwendete Konto.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem angegebenen Konto verknüpfte Passwort ein.

   * **[!UICONTROL Security-Token]**: Geben Sie das mit dem Konto verknüpfte Salesforce-Security-Token ein.

   * **[!UICONTROL API-Version]**: Wählen Sie „Version 49“ aus.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Salesforce“.](assets/crm-salesforce-2.png)

1. Öffnen Sie den **[!UICONTROL Konfigurationsassistenten für Salesforce CRM]**, um Ihre Salesforce CRM-Tabellenliste zu generieren, und klicken Sie dann auf **[!UICONTROL Weiter]**.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Salesforce CRM“.](assets/crm-salesforce-3.png)

1. Wählen Sie die abzurufenden Salesforce CRM-Tabellen aus oder fügen Sie eine Remote-Tabelle hinzu, indem Sie das **[!UICONTROL Tabellen-Label]** und den **[!UICONTROL internen Tabellennamen]** angeben und dann den Umschalter **[!UICONTROL Ausgewählt]** aktivieren.

   Klicken Sie auf **[!UICONTROL Weiter]**.

1. Klicken Sie auf **[!UICONTROL Start]**, um mit der Erstellung des Salesforce CRM-Schemas basierend auf den ausgewählten Tabellen zu beginnen.

1. Klicken Sie auf **[!UICONTROL Assistent zum Erstellen von Links in Salesforce…]**, um die Weblinks in Salesforce zu generieren.

   Klicken Sie dann auf **[!UICONTROL Weiter]**, um die Weblinks für **Leads** und **Kontakte** aus Salesforce abzurufen.

1. Wählen Sie die Links aus, die in die Liste der Salesforce-Weblinks exportiert werden sollen.

1. Befolgen Sie die Anweisungen am Bildschirm, um Seiten aus dem **Marketing-Verlauf** und der **Abonnementverwaltung** der Adobe Campaign Web-Benutzeroberfläche direkt in Salesforce CRM einzufügen.

1. Klicken Sie nach Abschluss der Konfiguration Ihres externen Kontos „Salesforce CRM“ auf **[!UICONTROL Speichern]**.

1. Nachdem Sie Ihr externes Konto erstellt haben, können Sie auf **[!UICONTROL Auflistungssynchronisation…]** klicken, um automatisch Auflistungen von Salesforce CRM mit der Adobe Campaign Web-Benutzeroberfläche zu synchronisieren.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Salesforce CRM“.](assets/crm-salesforce-4.png)

1. Wählen Sie die Adobe Campaign-Auflistung aus, die der Salesforce-Auflistung entspricht.

   Um Adobe Campaign-Werte durch Salesforce-Werte zu ersetzen, aktivieren Sie die Option **[!UICONTROL Ersetzen]**.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Salesforce CRM“.](assets/crm-salesforce-5.png)

