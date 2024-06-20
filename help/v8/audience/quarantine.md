---
audience: end-user
title: Über Quarantäne
description: Funktionsweise der Quarantäne-Adressen
source-git-commit: 9abf58c35fcf396e3003f9ecba728cd77df844a1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 20%

---

# Quarantäne

Adobe Campaign verwaltet Quarantäne-Adressen (E-Mail, SMS, Push-Benachrichtigungen).

Quarantäne gilt nur für eine **Email-Adresse**, a **Telefonnummer** oder **Geräte-Token**, aber nicht zum Profil selbst. Wenn beispielsweise ein Profil mit einer in Quarantäne befindlichen E-Mail-Adresse eine neue Adresse angibt, kann es erneut in Versandzielgruppen aufgenommen werden. Wenn zwei Profile dieselbe Telefonnummer haben, sind beide betroffen, wenn die Nummer unter Quarantäne gestellt wird.


>[!CAUTION]
>
>Bei der Quarantäne in Adobe Campaign wird zwischen Groß- und Kleinschreibung unterschieden.

## Was ist Quarantäne?

Die Quarantäne ist der richtige Weg **die ungültigen Adressen in Sendungen verwalten**.

Wenn ein Versand eine hohe Anzahl ungültiger Adressen aufweist, kann er als Spam betrachtet werden. Durch die Quarantäneverwaltung werden Sie nicht von Internetanbietern auf die Blockierungsliste gesetzt. Das ist wichtig für Ihren Ruf.

Wenn eine Adresse in Adobe Campaign unter Quarantäne gestellt wird, wird das Profil bei der Versandanalyse automatisch aus der Zielgruppe ausgeschlossen.

Durch die Quarantäne können Sie die Kosten für den SMS-Versand senken, indem fehlerhafte Telefonnummern aus Sendungen ausgeschlossen werden.

## Warum eine Adresse unter Quarantäne gestellt wird

Eine Adresse kann aus vielen Gründen unter Quarantäne gestellt werden:

- Für SMS: fehlerhafte Telefonnummern
- Bei SMS: Wenn das Profil auf eine SMS-Nachricht mit einem Schlüsselwort wie &quot;STOP&quot; antwortet
- E-Mail: Wenn Ihre Nachricht als Spam gemeldet wird. Die Nachricht wird automatisch an ein von Adobe verwaltetes technisches Postfach weitergeleitet. Die E-Mail-Adresse des Benutzers wird dann automatisch unter Quarantäne gestellt und der Status Auf die Blockierungsliste gesetzt.
- Eine E-Mail-Adresse kann unter Quarantäne gestellt werden, wenn beispielsweise das Postfach voll ist, die E-Mail-Adresse nicht existiert oder der E-Mail-Server nicht verfügbar ist.

[Weitere Informationen zu fehlgeschlagenen Sendungen](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/monitoring-deliveries/understanding-delivery-failures)

## Wo finde ich die Quarantäne-Adressen?

Sie können alle Quarantäne-Adressen Ihrer Instanz in **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Verwaltung von Fehlern]** > **[!UICONTROL Fehler und Adressen]**. In diesem Abschnitt werden unter Quarantäne gestellte Elemente für die Kanäle E-Mail, SMS und Push-Benachrichtigungen aufgeführt.

![](assets/quarantine_location.png){zoomable="yes"}

Sie können auch den Bericht über die Quarantäne in Ihrer Instanz erhalten:

![](assets/quarantine_reports.png){zoomable="yes"}

Sie können für jeden Versand auch den Bericht Versandzusammenfassung überprüfen: Er zeigt die Anzahl der Adressen in Quarantäne in der Versandzielgruppe an:

![](assets/quarantine_delivery.png){zoomable="yes"}

In der Adobe Campaign Console können Sie die Quarantäne-Adressen mehr verwalten. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
