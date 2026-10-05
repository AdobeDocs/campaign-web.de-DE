---
title: Branding
description: Entdecken Sie alle verfügbaren Tools zum Verwalten Ihrer Markenidentitäten
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: f6438303-5ae8-47c6-8c34-8e586f4b6fe7
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 100%
---
# Erste Schritte mit Branding {#branding-gs}

>[!AVAILABILITY]
>
>Diese Funktion ist nur auf Anfrage und nur für neue Implementierungen verfügbar. Wenden Sie sich für Zugriff an den Adobe-Support.

Jedes Unternehmen verfügt über Markenrichtlinien, die sowohl visuelle Elemente als auch technische Details definieren. Adobe Campaign unterstützt Sie bei der zentralen Verwaltung dieser Richtlinien, sodass Sie Ihrer Kundschaft immer und überall ein konsistentes Markenbild präsentieren können – von den Logos in E-Mails bis hin zu den in Ihren Kampagnen verwendeten URLs und Domains.

Technische Admins können mehrere Marken direkt über die Web-Benutzeroberfläche erstellen und verwalten. Auf diese Weise können Sie alle Elemente definieren, aus denen Ihre Markenidentität besteht, einschließlich Logos und sogar E-Mail-Tracking-Einstellungen. Nach der Erstellung können diese Marken einfach mit Ihren Sendungen verknüpft werden. [Erfahren Sie, wie Sie eine Marke erstellen und konfigurieren können](branding-configure.md).

Sie können in Campaign neue Entitäten Ihrer Organisation hinzufügen oder einen neuen E-Mail-Typ erstellen, den Sie unter einer anderen Subdomain senden müssen. Gehen Sie dazu wie folgt vor:

1. **Neue Subdomain konfigurieren**: Damit eine neue Subdomain von Adobe verwendet werden kann, müssen Sie sie zunächst konfigurieren. Sie können dies über das [Control Panel](https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=de) in Campaign durchführen oder sich an Ihren technischen Ansprechpartner bei Adobe wenden. Weitere Informationen zur Konfiguration von Subdomains finden Sie [auf dieser Seite](https://experienceleague.adobe.com/de/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-domain-name-setup).

   >[!NOTE]
   >
   >Das Control Panel steht allen Administratoren zur Verfügung. Die Schritte, um einem Benutzer Administratorzugriff zu gewähren, finden Sie auf [dieser Seite](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=de#discover-control-panel).

1. **Versandvorlage erstellen** – Sobald die neue Marke verfügbar ist, sollten Sie als Best Practice mindestens eine neue leere Versandvorlage erstellen, die auf diese neue Marke verweist. [Weitere Informationen](branding-assign.md).

1. **Zustellbarkeitsrichtlinien prüfen** – Bevor Sie mit der Verwendung der neuen Domain beginnen, sollte die Strategie mit dem Adobe-Zustellbarkeits-Team besprochen werden. Das Team unterstützt bei der Definition von Best Practices, beispielsweise bei der Entscheidung, ob eine neue Affinität erstellt werden soll, um die IPs zwischen den Domains aufzuteilen, und/oder ob ein Einführungsplan definiert werden soll.

## Kompatibilitätshinweis {#compatibility-note}

Das neue zentralisierte Branding-Modell ist nicht mit der [alten Branding-Konfiguration](https://experienceleague.adobe.com/docs/campaign-classic/using/transactional-messaging/configure-transactional-messaging/additional-configurations.html?lang=de#configuring-multibranding){target="_blank"} kompatibel, die zuvor in der Client-Konsole verwendet wurde.

Beim bisherigen Ansatz implementierten Kundinnen und Kunden das Branding, indem sie das Formular „extAccount“ erweiterten und die Registerkarte **Branding** verwendeten.

![Screenshot der Erstellung der Marke.](assets/branding-legacy.png)

Wenn Ihre bestehende Umgebung diese alte Konfiguration verwendet, kann sie nicht direkt zum neuen Modell für zentralisiertes Branding migriert werden. Um das neue System zu übernehmen, müssen die Branding-Einstellungen vollständig neu implementiert werden.