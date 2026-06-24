---
title: Verwalten eines externen Kontos
description: Informationen zum Konfigurieren externer Konten
exl-id: 99648377-112b-428a-8faf-5268d730f19a
TQID: https://experienceleague.adobe.com/ZkfG6g4YYAkefJI1Pi7xsdulm1zS1BFJdXBTS37x2T8
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 213
ht-degree: 100%

---

# Externe Konten zur Integration von Adobe-Lösungen {#integration-external-account}

Führen Sie je nach ausgewähltem Typ des externen Kontos für die Integration von Adobe-Lösungen die folgenden Schritte aus, um die Verbindungs- und Kontoeinstellungen für eine nahtlose Integration mit Adobe-Services zu konfigurieren.

## Adobe Experience Cloud

Um über eine Adobe ID eine Verbindung zur Adobe Campaign-Konsole herzustellen, müssen Sie das externe Adobe Experience Cloud (MAC)-Konto konfigurieren.

![Screenshot der Konfigurationsfelder für das externe Adobe Experience Cloud MAC-Konto.](assets/external-MAC.png)

Um das externe Konto **[!UICONTROL Adobe Experience Cloud]** zu konfigurieren, füllen Sie folgende Felder aus:

* **[!UICONTROL IMS-Server]**

  URL Ihres IMS-Servers. Stellen Sie sicher, dass sowohl Staging- als auch Produktionsinstanzen auf denselben IMS-Produktionsendpunkt verweisen.

* **[!UICONTROL IMS-Umfang]**

  Der hier definierte Umfang muss eine Teilmenge der vom IMS bereitgestellten Perimeter sein.

* **[!UICONTROL Kennung des IMS-Clients]**

  Die ID Ihres IMS-Client

* **[!UICONTROL IMS-Client-Secret]**

  Anmeldedaten Ihres IMS-Client-Geheimnisses.

* **[!UICONTROL Callback-Server]**

  Zugriffs-URL Ihrer Adobe Campaign-Instanz.

* **[!UICONTROL Kennung der IMS-Organisation]**

  ID Ihrer Organisation. Auf [dieser Seite](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=de){target=_blank} finden Sie Ihre Organisations-ID.

* **[!UICONTROL Zuordnungsmaske]**

  Syntax, die es ermöglicht, Konfigurationsnamen im Enterprise Dashboard mit den Gruppen in Adobe Campaign zu synchronisieren

* **[!UICONTROL Server]**

  URL Ihrer Adobe Experience Cloud-Instanz

* **[!UICONTROL Mandant]**

  Name Ihres Adobe Experience Cloud-Mandanten
