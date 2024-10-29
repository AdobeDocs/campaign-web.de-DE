---
audience: end-user
title: Transaktionsnachrichten validieren
description: Erfahren Sie, wie Sie eine Transaktionsnachricht in der Campaign-Webbenutzeroberfläche validieren
source-git-commit: e0d87d22d9712837f085f94f9d9ba63e96f36b36
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# Transaktionsnachrichten validieren

Während oder nach der Erstellung Ihrer Transaktionsnachricht können Sie den Inhalt mithilfe eines Datenbeispiels validieren.

## Inhalte simulieren {#simulate-content}

Führen Sie die folgenden Schritte aus, um den Inhalt Ihrer Nachricht zu simulieren:

* Stellen Sie sicher, dass der Personalisierungspfad in Ihrem Nachrichteninhalt mit Ihrem Kontextbeispiel übereinstimmt. Im folgenden Beispiel verwenden wir zum Anzeigen des Vornamens des Testprofils den Pfad *rtEvent.ctx.basicDetails.firstName*

  Sie können den Nachrichteninhalt oder das Kontextbeispiel ändern, um sie auszurichten.

  ![](assets/validate-verification.png){zoomable="yes"}

* Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt simulieren]** , um Ihre Transaktionsnachricht mit den im Kontextbeispiel eingegebenen Daten in der Vorschau anzuzeigen.

  ![](assets/validate-simulate.png){zoomable="yes"}

  Klicken Sie nach Überprüfung des Inhalts auf die Schaltfläche **[!UICONTROL Schließen]** .

* Vergessen Sie nicht, auf die Schaltfläche **[!UICONTROL Neu veröffentlichen]** zu klicken, wenn Sie Änderungen an Ihrem Inhalt vorgenommen haben.

## Testversand senden

Wenn Sie die Transaktionsnachricht so testen und erleben möchten, wie sie über Ihren ausgewählten Kanal gesendet wird (z. B. E-Mail, SMS oder Push-Benachrichtigung), können Sie die Testversandfunktion verwenden.

Klicken Sie im Fenster [Simulationsinhalt](#simulate-content) auf die Schaltfläche **[!UICONTROL Testversand durchführen]** .

![](assets/transactional-proof.png){zoomable="yes"}

Geben Sie im sich öffnenden Fenster die E-Mail-Adresse (oder Telefonnummer, je nach Kanal) an, an die Sie den Testversand erhalten möchten. Nachdem Sie die gewünschte Adresse eingegeben haben, klicken Sie auf **[!UICONTROL Testversand durchführen]** und auf die Schaltflächen **[!UICONTROL Bestätigen]** . Mit dieser Aktion können Sie eine Stichprobe Ihrer Transaktionsnachricht senden, um sicherzustellen, dass alle Personalisierungen, dynamischen Inhalte und Formatierungen korrekt wie für Ihre Endbenutzer angezeigt werden.

![](assets/transactional-sendproof.png){zoomable="yes"}

Dies ist ein wichtiger Schritt, um potenzielle Probleme vor der Veröffentlichung Ihrer Transaktionsnachricht zu identifizieren.
