---
title: Verwalten eines externen Kontos
description: Informationen zum Konfigurieren externer Konten
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 97%

---

# Campaign-spezifische externe Konten {#external-account}

Gehen Sie wie folgt vor, um die Kontoeinstellungen je nach ausgewähltem externem Kontotyp zu konfigurieren.

## Bounce Messages (POP3) {#bounce}

Das externe Konto „Bounce-E-Mails“ gibt das externe POP3-Konto an, das für die Verbindung mit dem E-Mail-Service verwendet werden soll.  Alle Server, die für den POP3-Zugriff konfiguriert sind, können Antwort-Mails empfangen.

![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Bounce Messages (POP3)“](assets/external_account_bounce.png)

Um das externe Konto **[!UICONTROL Bounce Messages (POP3)]** zu konfigurieren, füllen Sie folgende Felder aus:

* **[!UICONTROL Server]** – URL des POP3-Servers.

* **[!UICONTROL Port]** – Nummer des POP3-Verbindungs-Ports (der Standard-Port ist 110).

* **[!UICONTROL Konto]** – Name der Benutzerin bzw. des Benutzers.

* **[!UICONTROL Passwort]** – Passwort des Benutzerkontos.

* **[!UICONTROL Verschlüsselung]** – Typ der Verschlüsselung, z. B.:
   * Standardmäßig (POP3 wenn Port 110, POP3S wenn Port 995)
   * POP3 schaltet auf SSL nach Übermittlung von STARTTLS
   * POP3 nicht gesichert (standardmäßig Port 110)
   * POP3 gesichert über SSL (standardmäßig Port 995)

* **[!UICONTROL Funktion]** – Wählen Sie **[!UICONTROL Eingehende E-Mail]** aus, um das Konto für den Empfang eingehender E-Mails zu konfigurieren, oder **[!UICONTROL SOAP-Router]**, um SOAP-Anfragen zu verarbeiten.

>[!IMPORTANT]
>
>Bevor Sie Ihr externes POP3-Konto mit Microsoft OAuth 2.0 konfigurieren, müssen Sie die Anwendung zunächst im Azure-Portal registrieren. Weitere Informationen hierzu finden Sie auf [dieser Seite](https://learn.microsoft.com/de-de/entra/identity-platform/quickstart-register-app){target=_blank}.

Um ein externes POP3-Programm mit Microsoft OAuth 2.0 zu konfigurieren, aktivieren Sie die Option „Microsoft OAuth 2.0“ und füllen Sie die folgenden Felder aus:

* **[!UICONTROL Azure-Mandant]**

  Die Azure-ID (oder Verzeichnis- bzw. Mandanten-ID) finden Sie in der Dropdown-Liste „Grundlagen“ der Anwendungsübersicht im Azure-Portal.

* **[!UICONTROL Azure-Client-ID]**

  Die Client-ID (oder Anwendungs- bzw. Client-ID) finden Sie in der Dropdown-Liste „Grundlagen“ der Anwendungsübersicht im Azure-Portal.

* **[!UICONTROL Azure-Client-Geheimnis]**

  Die Client-Geheimnis-ID finden Sie in der Spalte „Client-Geheimnisse“ im Menü „Zertifikate und Geheimnisse“ Ihrer Anwendung im Azure-Portal.

* **[!UICONTROL Azure-Umleitungs-URL]**

  Die Umleitungs-URL finden Sie im Menü „Authentifizierung“ Ihrer Anwendung im Azure-Portal. Sie sollte mit der folgenden Syntax enden: nl/jsp/oauth.jsp, z. B. `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

Zum Einrichten und Verwenden der Schaltfläche „Verbindung testen“ in der Client-Konsole ist ein Internet-Zugang erforderlich. Nach der Einrichtung kann der inMail-Prozess ohne Internet mit Microsoft-Servern kommunizieren.

Nachdem Sie Ihre unterschiedlichen Anmeldedaten eingegeben haben, können Sie auf „Verbindung einrichten“ klicken, um die Konfiguration Ihres externen Kontos abzuschließen.

## Routing {#routing}

Gehen Sie wie folgt vor, um ein spezielles externes Konto für externe Sendungen zu konfigurieren.

1. Erstellen Sie ein externes Konto. [Weitere Informationen](create-external-account.md)

1. Wählen Sie als Typ **[!UICONTROL Routing]** aus.

   ![Screenshot mit der Auswahl des externen Routing-Kontotyps.](assets/external-account-routing.png){zoomable="yes"}

1. Wählen Sie den gewünschten Kanal aus und klicken Sie auf **[!UICONTROL Erstellen]**.

1. Im Abschnitt **[!UICONTROL Details]** des externen Kontos ist standardmäßig **[!UICONTROL Extern]** als **[!UICONTROL Versandmodus]** ausgewählt.

   ![Screenshot mit der Konfiguration des Versandmodus für externe Routing-Konten.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Derzeit ist **[!UICONTROL Extern]** der einzige verfügbare Modus.

1. Um den Prozess nach der Ausführung des Versands zu verwalten, externalisieren Sie diesen in einen Nachbearbeitungs-Workflow. Erstellen Sie einen Workflow mit der Aktivität [Externes Signal](../workflows/activities/external-signal.md) und wählen Sie ihn aus dem Feld **[!UICONTROL Anschlussvorgang]** aus.

   ![Screenshot der Konfiguration des Felds „Anschlussvorgang“ für externe Routing-Konten.](assets/external-account-post-processing.png){zoomable="yes"}

1. Im Feld **[!UICONTROL Aktivität]** können Sie den Namen der Aktivität für den Anschluss-Workflow bearbeiten, der in den Protokollen angezeigt wird. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Ausführungsinstanz {#instance-exec}

Im Falle einer segmentierten Architektur müssen Sie die mit der Kontrollinstanz verknüpften Ausführungsinstanzen identifizieren und Verbindungen zwischen ihnen herstellen. Transaktionsnachrichtenvorlagen werden in der Ausführungsinstanz bereitgestellt.

![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Ausführungsinstanz“](assets/external_account_exec.png)

So konfigurieren Sie das externe Konto **[!UICONTROL Ausführungsinstanz]**:

* **[!UICONTROL URL]**: URL des Servers, auf dem die Ausführungsinstanz installiert ist.

* **[!UICONTROL Konto]**: Name des Kontos, der mit dem Message Center Agent übereinstimmt, der im Benutzerordner definiert ist

* **[!UICONTROL Passwort]**: Passwort des Kontos, wie es im Benutzerordner definiert ist

* **[!UICONTROL Methode]**: Wählen Sie zwischen „Web-Dienst“ oder „Federated Data Access (FDA)“.

  Wählen Sie für FDA Ihr FDA-Konto aus. Die Verbindung von Campaign mit externen Systemen ist erfahrenen Benutzenden vorbehalten und nur über die Client-Konsole verfügbar. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Archivierungs-Workflow erstellen]**: Erstellen Sie für jede im Message Center registrierte Ausführungsinstanz, unabhängig davon, ob eine oder mehrere Instanzen vorhanden sind, einen separaten Archivierungs-Workflow für jedes externe Konto, das mit der Ausführungsinstanz verknüpft ist.
