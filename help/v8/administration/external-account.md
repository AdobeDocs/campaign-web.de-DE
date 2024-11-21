---
title: Externes Konto
description: Informationen zum Konfigurieren externer Konten
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 100%

---

# Konfigurieren externer Konten {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Externe Konten"
>abstract="Sie können jetzt eine Verbindung mit weiteren Plattformen herstellen oder die Verbindungen an Ihren Workflow anpassen und einfach neue externe Konten erstellen, um Ihre spezifischen Anforderungen zu erfüllen und nahtlose Datenübertragungen zu gewährleisten."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"


>[!AVAILABILITY]
>
> Beachten Sie, dass externe Konten derzeit nur für Bounce-E-Mails (POP3) und die Ausführungsinstanz verfügbar sind. In Zukunft werden zusätzliche Kontotypen hinzugefügt.
> Nicht unterstützte externe Konten, die in der Adobe Campaign-Konsole erstellt wurden, sind in der Web-Benutzeroberfläche sichtbar, können jedoch nicht bearbeitet oder aufgerufen werden.

Adobe Campaign verfügt über eine Reihe vordefinierter externer Konten, sodass eine einfache Integration mit verschiedenen Systeme möglich ist.  Wenn Sie eine Verbindung zu zusätzlichen Plattformen herstellen oder die Verbindungen an Ihren Workflow anpassen müssen, können Sie jetzt einfach neue externe Konten über die Web-Benutzeroberfläche erstellen, um Ihre spezifischen Anforderungen zu erfüllen und eine nahtlose Datenübertragung zu gewährleisten.

## Erstellen eines externen Kontos {#create-ext-account}

Gehen Sie wie folgt vor, um ein neues externes Konto zu erstellen.  Detaillierte Einstellungen hängen vom Typ des externen Kontos ab.

1. Wählen Sie im Menü im linken Fensterbereich unter **[!UICONTROL Administration]** die Option **[!UICONTROL Externe Konten]** aus.

1. Klicken Sie auf **[!UICONTROL Externes Konto erstellen]**.

   ![](assets/external_account_create_1.png)

1. Geben Sie Ihr **[!UICONTROL Label]** ein und wählen Sie den **[!UICONTROL Typ]** Ihres externen Kontos aus.

   ![](assets/external_account_create_2.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Über die Dropdown-Liste **[!UICONTROL Erweiterte Optionen]** können Sie bei Bedarf den **[!UICONTROL internen Namen]** oder den **[!UICONTROL Ordnerpfad]** ändern.

   ![](assets/external_account_create_3.png)

1. Aktivieren Sie die Option **[!UICONTROL Automatisch exportieren]**, wenn die von diesem externen Konto verwalteten Daten automatisch exportiert werden sollen.

1. Konfigurieren Sie den Zugriff auf das Konto, indem Sie die Anmeldedaten entsprechend dem gewählten externen Kontotyp angeben.

1. Klicken Sie auf **[!UICONTROL Verbindung testen]**, um zu prüfen, ob Ihre Konfiguration korrekt ist.

1. Sie können Ihr externes Konto über das Menü **[!UICONTROL Details...]** duplizieren oder löschen.

   ![](assets/external_account_create_4.png)

1. Klicken Sie nach Abschluss der Konfiguration auf **[!UICONTROL Speichern]**.

## Campaign-spezifische externe Konten {#campaign-specific}

### Bounce Messages (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 wird derzeit nicht unterstützt.

Das externe Konto „Bounce-E-Mails“ gibt das externe POP3-Konto an, das für die Verbindung mit dem E-Mail-Service verwendet werden soll.  Alle Server, die für den POP3-Zugriff konfiguriert sind, können Antwortsendungen empfangen.

![](assets/external_account_bounce.png)

Um das externe Konto **[!UICONTROL Bounce Messages (POP3)]** zu konfigurieren, benötigen Sie folgende Informationen:

* **[!UICONTROL Server]**

  URL des POP3-Servers

* **[!UICONTROL Port]**

  Nummer des POP3-Verbindungs-Ports (der Standard-Port ist 110)

* **[!UICONTROL Konto]**

  Name der Benutzerin bzw. des Benutzers

* **[!UICONTROL Passwort]**

  Passwort des Benutzerkontos

* **[!UICONTROL Verschlüsselung]**

  Typ der gewählten Verschlüsselung zwischen:

   * Standardmäßig (POP3 wenn Port 110, POP3S wenn Port 995)
   * POP3 schaltet auf SSL nach Übermittlung von STARTTLS
   * POP3 nicht gesichert (standardmäßig Port 110)
   * POP3 gesichert über SSL (standardmäßig Port 995)

* **[!UICONTROL Funktion]**

  Eingehende E-Mail, wenn das externe Konto für den Empfang eingehender E-Mails konfiguriert ist, oder SOAP-Router für die Verarbeitung SOAP-Anfragen.

### Ausführungsinstanz{#instance-exec}

Im Falle einer segmentierten Architektur müssen Sie die mit der Kontrollinstanz verknüpften Ausführungsinstanzen identifizieren und Verbindungen zwischen ihnen herstellen. Transaktionsnachrichtenvorlagen werden in der Ausführungsinstanz bereitgestellt.

![](assets/external_account_exec.png)

So konfigurieren Sie das externe Konto **[!UICONTROL Ausführungsinstanz]**:

* **[!UICONTROL URL]**

  URL des Servers, auf dem die Ausführungsinstanz installiert ist.

* **[!UICONTROL Konto]**

  Name des Kontos, muss mit dem Message Center Agent übereinstimmen, der im Benutzerordner definiert ist

* **[!UICONTROL Passwort]**

  Passwort des Kontos, wie es im Benutzerordner definiert ist

* **[!UICONTROL Methode]**

  Wählen Sie zwischen Web-Dienst oder Federated Data Access (FDA).
Wählen Sie im Falle der FDA-Methode Ihr FDA-Konto aus. Die Verbindung von Campaign mit externen Systemen ist erfahrenen Benutzenden vorbehalten und nur über die Client-Konsole verfügbar. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Erstellen eines Archivierungs-Workflows]**

  Für jede im Message Center registrierte Ausführungsinstanz müssen Sie, unabhängig davon, ob eine oder mehrere Instanzen vorhanden sind, einen separaten Archivierungs-Workflow für jedes externe Konto erstellen, das mit der Ausführungsinstanz verknüpft ist.
