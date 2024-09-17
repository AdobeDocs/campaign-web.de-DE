---
audience: end-user
title: Informationen zu Quarantäne
description: Über die Verwaltung der Quarantäne-Adressen
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: 3e99bf1453ef38ec915dc82828f44c7d7ffb2acd
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 90%

---

# Quarantäneverwaltung {#quarantines}

Adobe Campaign verwaltet Quarantäne-Adressen für E-Mail-, Push- und SMS-Kanäle.

Eine Quarantäne gilt nur für eine **E-Mail-Adresse**, eine **Telefonnummer** oder ein **Geräte-Token**, aber nicht für das Profil selbst.  Wenn beispielsweise ein Profil mit einer in Quarantäne befindlichen E-Mail-Adresse eine neue Adresse angibt, kann es erneut in Versandzielgruppen aufgenommen werden. Wenn zwei Profile dieselbe Telefonnummer haben, sind sie beide betroffen, wenn die Nummer unter Quarantäne gestellt wird.

>[!CAUTION]
>
>Bei der Quarantänefunktion in Adobe Campaign wird die Groß-/Kleinschreibung beachtet.

## Was ist Quarantäne? {#quarantines-what}

Mit der Quarantäne werden **die ungültigen Adressen in Sendungen verwaltet**.

Wenn ein Versand eine hohe Anzahl ungültiger Adressen aufweist, wird er möglicherweise als Spam angesehen. Durch die Verwaltung mittels Quarantäne wird verhindert, dass diese Adressen von Internet-Anbietern auf eine Blockierungsliste gesetzt werden.  Das ist wichtig für Ihren Ruf.

Wenn eine Adresse in Adobe Campaign unter Quarantäne gestellt wird, wird das Profil bei der Versandanalyse automatisch aus der Zielgruppe ausgeschlossen.

Quarantäne hilft Ihnen auch, die Kosten des SMS-Versands zu senken, indem fehlerhafte Telefonnummern aus Sendungen ausgeschlossen werden.

Weitere Informationen zu Quarantänen finden Sie in der Dokumentation zu [Campaign v8 (Konsole)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} .


## Warum eine Adresse unter Quarantäne gestellt wird {#quarantines-why}

Eine Adresse kann aus vielen Gründen unter Quarantäne gestellt werden:

* SMS: Fehlerhafte Telefonnummern
* SMS: Das Profil antwortet auf eine SMS-Nachricht mit einem Schlüsselwort wie „STOP“.
* E-Mail: Ihre Nachricht wird als Spam gemeldet.  Die Nachricht wird automatisch an ein von Adobe verwaltetes, technisches Postfach weitergeleitet. Die E-Mail-Adresse der Person wird dann automatisch unter Quarantäne gestellt und der Status in „Auf Blockierungsliste“ geändert.
* Eine E-Mail-Adresse kann unter Quarantäne gestellt werden, wenn beispielsweise das Postfach voll ist, die E-Mail-Adresse nicht existiert oder der E-Mail-Server nicht verfügbar ist.

Weitere Informationen zu fehlgeschlagenen Sendungen finden Sie in der Dokumentation zu [Campaign v8 (Konsole)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"} .

## Wo finden Sie die Quarantäne-Adressen? {#quarantines-where}

Sie können alle Quarantäne-Adressen Ihrer Instanz unter **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Kampagnenverwaltung]** > **[!UICONTROL Unzustellbarkeitsverwaltung]** > **[!UICONTROL Adressen unzustellbarer Sendungen]** anzeigen. In diesem Abschnitt werden die unter Quarantäne gestellten Elemente für die Kanäle „E-Mail“, „SMS“ und „Push-Benachrichtigungen“ aufgeführt.

![](assets/quarantine_location.png){zoomable="yes"}

Sie können auch den Bericht über die Quarantäne in Ihrer Instanz erhalten:

![](assets/quarantine_reports.png){zoomable="yes"}

Die Versandzusammenfassung gibt für jeden Versand Aufschluss über die Anzahl der Adressen in Quarantäne in der Zielgruppe des Versands:

![](assets/quarantine_delivery.png){zoomable="yes"}

In der Adobe Campaign-Konsole stehen Ihnen weitere Optionen zur Verwaltung der Quarantäne-Adressen zur Verfügung. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
