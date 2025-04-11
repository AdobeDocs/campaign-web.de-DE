---
audience: end-user
title: Validieren von Transaktionsnachrichten
description: Informationen zum Validieren einer Transaktionsnachricht in der Campaign Web-Benutzeroberfläche
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 25%

---

# Validieren von Transaktionsnachrichten

Während oder nach der Erstellung der Transaktionsnachricht können Sie den Inhalt mithilfe eines Datenbeispiels validieren.

## Simulieren von Inhalten {#simulate-content}

Führen Sie die folgenden Schritte aus, um den Inhalt Ihrer Nachricht zu simulieren:

* Stellen Sie sicher, dass der Personalisierungspfad in Ihrem Nachrichteninhalt mit Ihrem Kontextbeispiel übereinstimmt. Im folgenden Beispiel verwenden Sie zum Anzeigen des Vornamens des Testprofils den Pfad *rtEvent.ctx.basicDetails.firstName*.

  Sie können den Nachrichteninhalt oder das Kontextbeispiel ändern, damit sie aufeinander abgestimmt sind.

  ![Screenshot zur Überprüfung der Personalisierungspfade im Nachrichteninhalt](assets/validate-verification.png){zoomable="yes"}

* Klicken Sie auf die **[!UICONTROL Inhalt simulieren]**, um eine Vorschau Ihrer Transaktionsnachricht mit den im Kontextbeispiel eingegebenen Daten anzuzeigen.

  ![Screenshot mit der Schaltfläche „Inhalt simulieren“ und der Vorschaufunktion](assets/validate-simulate.png){zoomable="yes"}

  Klicken Sie nach der Überprüfung Ihres Inhalts auf die Schaltfläche **[!UICONTROL Schließen]**.

* Klicken Sie auf die Schaltfläche **[!UICONTROL Neu veröffentlichen]**, wenn Sie Änderungen am Inhalt vorgenommen haben.

## Senden eines Testversands

Verwenden Sie die Testfunktion, um die Transaktionsnachricht so zu testen und anzusehen, wie sie über Ihren ausgewählten Kanal gesendet wird, z. B. per E-Mail, SMS oder Push-Benachrichtigung.

Klicken Sie im [Fenster mit dem Simulationsinhalt](#simulate-content) auf die Schaltfläche **[!UICONTROL Testversand durchführen]**.

![Screenshot der Schaltfläche „Testversand durchführen“ im Fenster „Simulationsinhalt“](assets/transactional-proof.png){zoomable="yes"}

Geben Sie in dem neu erscheinenden Fenster die E-Mail-Adresse oder Telefonnummer ein, je nach Kanal, über den Sie den Testversand erhalten möchten. Nachdem Sie die gewünschte Adresse eingegeben haben, klicken Sie auf die Schaltflächen **[!UICONTROL Testversand durchführen]** und **[!UICONTROL Bestätigen]**. Diese Aktion sendet ein Beispiel für Ihre Transaktionsnachricht, um sicherzustellen, dass alle Personalisierungen, dynamischen Inhalte und Formatierungen korrekt angezeigt werden, wie es für Ihre Endbenutzenden der Fall wäre.

![Screenshot mit der Funktion „Testversand durchführen“ und dem Bestätigungsprozess](assets/transactional-sendproof.png){zoomable="yes"}

Dieser Schritt ist wichtig, um potenzielle Probleme zu identifizieren, bevor Sie Ihre Transaktionsnachricht veröffentlichen.