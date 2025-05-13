---
audience: end-user
title: Validieren von Transaktionsnachrichten
description: Informationen zum Validieren einer Transaktionsnachricht in der Campaign Web-Benutzeroberfläche
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '293'
ht-degree: 100%

---

# Validieren von Transaktionsnachrichten

Während oder nach der Erstellung der Transaktionsnachricht können Sie den Inhalt mithilfe eines Datenbeispiels validieren.

## Simulieren von Inhalten {#simulate-content}

Führen Sie die folgenden Schritte aus, um den Inhalt Ihrer Nachricht zu simulieren:

* Stellen Sie sicher, dass der Personalisierungspfad in Ihrem Nachrichteninhalt mit Ihrem Kontextbeispiel übereinstimmt. Verwenden Sie im folgenden Beispiel zum Anzeigen des Vornamens des Testprofils den Pfad *rtEvent.ctx.basicDetails.firstName*.

  Sie können den Nachrichteninhalt oder das Kontextbeispiel ändern, um sie anzugleichen.

  ![Screenshot mit der Überprüfung der Personalisierungspfade im Nachrichteninhalt](assets/validate-verification.png){zoomable="yes"}

* Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalte simulieren]**, um Ihre Transaktionsnachricht mit den im Kontextbeispiel eingegebenen Daten in der Vorschau anzuzeigen.

  ![Screenshot mit der Schaltfläche „Inhalte simulieren“ und der Vorschaufunktion](assets/validate-simulate.png){zoomable="yes"}

  Klicken Sie nach Überprüfung des Inhalts auf die Schaltfläche **[!UICONTROL Schließen]**.

* Achten Sie darauf, auf die Schaltfläche **[!UICONTROL Erneut veröffentlichen]** zu klicken, wenn Sie Änderungen an Ihrem Inhalt vorgenommen haben.

## Senden eines Testversands

Verwenden Sie die Funktion „Testversand“, um die Transaktionsnachricht so zu testen und zu erleben, wie sie über Ihren ausgewählten Kanal gesendet wird (z. B. E-Mail, SMS oder Push-Benachrichtigung).

Klicken Sie im [Fenster mit dem Simulationsinhalt](#simulate-content) auf die Schaltfläche **[!UICONTROL Testversand durchführen]**.

![Screenshot der Schaltfläche „Testversand senden“ im Fenster „Simulationsinhalt“](assets/transactional-proof.png){zoomable="yes"}

Geben Sie im sich öffnenden Fenster je nach Kanal die E-Mail-Adresse oder Telefonnummer an, an die Sie den Testversand erhalten möchten. Nachdem Sie die gewünschte Adresse eingegeben haben, klicken Sie auf die Schaltflächen **[!UICONTROL Testversand senden]** und **[!UICONTROL Bestätigen]**. Diese Aktion sendet ein Beispiel Ihrer Transaktionsnachricht, um sicherzustellen, dass alle Personalisierungen, dynamischen Inhalte und Formatierungen für Ihre Endbenutzenden korrekt angezeigt werden.

![Screenshot mit der Funktion „Testversand senden“ und dem Bestätigungsprozess](assets/transactional-sendproof.png){zoomable="yes"}

Dies ist ein wichtiger Schritt zur Identifizierung potenzieller Probleme vor der Veröffentlichung der Transaktionsnachricht.