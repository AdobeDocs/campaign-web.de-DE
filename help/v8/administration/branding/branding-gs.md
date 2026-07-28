---
title: Branding
description: Entdecken Sie alle verfügbaren Tools zum Verwalten Ihrer Markenidentitäten
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: f6438303-5ae8-47c6-8c34-8e586f4b6fe7
source-git-commit: 5c9d3db95905f77dddffaf824156c87b9d79013c
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 73%

---

# Erste Schritte mit Branding {#branding-gs}

>[!AVAILABILITY]
>
>Diese Funktion ist nur auf Anfrage und nur für neue Implementierungen verfügbar. Wenden Sie sich für Zugriff an den Adobe-Support.

Jedes Unternehmen verfügt über Markenrichtlinien, die sowohl visuelle Elemente als auch technische Details definieren. Adobe Campaign unterstützt Sie bei der zentralen Verwaltung dieser Richtlinien, sodass Sie Ihrer Kundschaft immer und überall ein konsistentes Markenbild präsentieren können – von den Logos in E-Mails bis hin zu den in Ihren Kampagnen verwendeten URLs und Domains.

Technische Administratoren können mehrere Marken direkt über die Web-Benutzeroberfläche erstellen und verwalten. Auf diese Weise können Sie alle Elemente definieren, aus denen Ihre Markenidentität besteht, einschließlich Logos und sogar E-Mail-Tracking-Einstellungen. Nach der Erstellung können diese Marken einfach mit Ihren Sendungen verknüpft werden. [Erfahren Sie, wie Sie eine Marke erstellen und konfigurieren](branding-configure.md).

Sie können in Campaign neue Entitäten Ihrer Organisation hinzufügen oder einen neuen E-Mail-Typ erstellen, den Sie unter einer anderen Subdomain senden müssen. Gehen Sie dazu wie folgt vor:

1. **Neue Subdomain konfigurieren**: Damit eine neue Subdomain von Adobe verwendet werden kann, müssen Sie sie zunächst konfigurieren. Sie können dies über das [Control Panel](https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=de) in Campaign durchführen oder sich an Ihren technischen Ansprechpartner bei Adobe wenden. Weitere Informationen zur Konfiguration von Subdomains finden Sie [auf dieser Seite](https://experienceleague.adobe.com/de/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-domain-name-setup).

   >[!NOTE]
   >
   >Das Control Panel steht allen Administratoren zur Verfügung. Die Schritte, um einem Benutzer Administratorzugriff zu gewähren, finden Sie auf [dieser Seite](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=de#discover-control-panel).

1. **Erstellen einer Versandvorlage** - Sobald die neue Marke verfügbar ist, empfiehlt es sich, mindestens eine neue leere Versandvorlage zu erstellen, die auf diese neue Marke verweist. [Weitere Informationen](branding-assign.md).

1. **Zustellbarkeitsrichtlinien überprüfen** - Bevor Sie mit der Verwendung der neuen Domain beginnen, sollte die Strategie mit dem Adobe Zustellbarkeits-Team besprochen werden. Sie helfen bei der Definition der Best Practices, wenn beispielsweise eine neue Affinität zur Aufspaltung der IPs zwischen Domains erstellt werden soll und/oder wenn ein Hochlaufplan definiert werden soll.

## Kompatibilitätshinweis {#compatibility-note}

Das neue zentralisierte Branding-Modell ist nicht mit der [alten Branding-Konfiguration](https://experienceleague.adobe.com/docs/campaign-classic/using/transactional-messaging/configure-transactional-messaging/additional-configurations.html#configuring-multibranding){target="_blank"} kompatibel, die zuvor in der Client-Konsole verwendet wurde.

Beim bisherigen Ansatz implementierten Kundinnen und Kunden das Branding, indem sie das Formular „extAccount“ erweiterten und die Registerkarte **Branding** verwendeten.

![Screenshot zur Erstellung der Marke.](assets/branding-legacy.png)

Wenn Ihre bestehende Umgebung diese alte Konfiguration verwendet, kann sie nicht direkt zum neuen Modell für zentralisiertes Branding migriert werden. Um das neue System zu übernehmen, müssen die Branding-Einstellungen vollständig neu implementiert werden.