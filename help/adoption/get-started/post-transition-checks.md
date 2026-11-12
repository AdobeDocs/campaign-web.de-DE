---
title: Prüfungen und Fehlerbehebung nach der Umstellung auf Campaign v8
description: Erfahren Sie, was zu überprüfen ist und wie Sie häufige Probleme nach der Umstellung von Campaign Standard auf Campaign v8 beheben können
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 3%
---
# Prüfungen und Fehlerbehebung nach der Umstellung {#post-transition-checks}

Nach dem Übergang von Campaign Standard zu Campaign v8 verhalten sich einige Sendungen, Workflows und Landingpages möglicherweise anders als erwartet. In der folgenden Tabelle sind die von Benutzern nach der Umstellung gemeldeten Symptome mit der Ursache und den zu ergreifenden Maßnahmen aufgeführt. Eine vollständige Liste der Unterschiede finden Sie unter [Unterschiede zwischen Campaign Standard und Campaign v8](acs-v8-differences.md).

| Symptom | Ursache und Vorgehensweise | Weitere Informationen |
|---|---|---|
| Links in einem Versand sind direkte URLs, und es werden keine Klickdaten erfasst. | Das Tracking ist für den Versand oder die Versandvorlage, auf der es basiert, deaktiviert. Überprüfen Sie, ob **Tracking aktivieren** aktiviert ist, insbesondere in den Vorlagen Ihrer wiederkehrenden Sendungen. | [Tracking-Einstellungen](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Empfänger, die sich über die „mailto“-Abmeldemethode abgemeldet haben, befinden sich nicht in Quarantäne. | Dies ist zu erwarten. Diese Empfänger werden nicht unter Quarantäne gestellt. Sie werden vom Dienst, der mit dem Versand verknüpft ist, abgemeldet oder der Blockierungsliste hinzugefügt, wenn der Versand keinen Dienst hat. Um diese Abmeldungen zu verfolgen, überprüfen Sie die Abonnements des Service oder den Abschnitt **Nicht mehr kontaktieren** des Profils. | [Quarantänen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Eine Landingpage speichert keinen Wert, der von einem Skript berechnet oder in einem ausgeblendeten Feld gespeichert wird. | In der Web-Benutzeroberfläche von Campaign erstellte Landingpages unterstützen keine ausgeblendeten Eingabefelder oder benutzerdefinierten JavaScript. Erstellen Sie das Formular stattdessen als Web-Anwendung in der Client-Konsole. | [Landingpages &#x200B;](../../v8/landing-pages/get-started-lp.md) |
| **Dateiübertragung** findet die von einer Briefpost-Aktivität generierte Datei nicht. | Die ausgehende Transition einer Briefpost-Aktivität enthält die ausgewählte Population und nicht die Extraktionsdatei. Fügen Sie **Aktivität** Datenextraktion“ und dann die Aktivität **Dateiübertragung“**. | [Briefpost](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Mehrere Schübe eines Versands werden zusammen gesendet. | Die Schübe werden ab dem Kontaktdatum des Versands geplant. Wenn der Versand nach der geplanten Zeit einiger Wellen beginnt, werden diese Wellen zusammen gesendet, anstatt mit Abständen angeordnet zu werden. | [Senden mit Schüben](../../v8/advanced-settings/send-using-waves.md) |
| Eine Dateimaske mit Zeichen nach dem Sternchen findet keine Datei im Azure Blob-Speicher. | Der Azure Blob-Speicher filtert Dateien nach Namenspräfix. Es wird nur ein nachfolgendes Sternchen unterstützt. | [Externes Konto übertragen](../../v8/administration/transfer-external-account.md) |
| Eine Mirrorseite eines Versands, der vor der Transition gesendet wurde, wird nicht geöffnet. | Mirrorseiten von Sendungen, die von Campaign Standard vor der Umstellung gesendet wurden, sind nicht verfügbar und es gibt keine Problemumgehung. Mirrorseiten der von Campaign v8 gesendeten Sendungen funktionieren wie gewohnt. | [Mirrorseiten](../../v8/email/mirror-page.md) |
| Ein Landingpage- oder Inhaltsbaustein, der benutzerdefinierte JavaScript verwendet, verhält sich anders. | Benutzerdefinierte JavaScript wird während der Migration transformiert, sie jedoch validieren und anpassen, insbesondere wenn sie `queryDef`, Campaign JavaScript-APIs, Sitzungsschreibvorgänge, die Handhabung von Organisationseinheiten oder die Erstellung benutzerdefinierter URLs verwendet. | [Landingpages &#x200B;](../../v8/landing-pages/get-started-lp.md) |
