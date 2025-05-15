---
title: Erste Schritte mit Profilen
description: Erfahren Sie, wie Sie Profile in Adobe Campaign Web überwachen und verwalten können.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 100%

---

# Erste Schritte mit Profilen {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profile"
>abstract="Ein Profil ist ein Eintrag, der gezielt Nachrichten von Adobe Campaign erhält. In dieser Liste können die Details der Profile anhand der Berechtigungen angezeigt werden. Verwenden Sie die Filteroptionen, um diese Liste zu durchsuchen. Eine kleine Gruppe von Profilattributen kann bearbeitet und aktualisiert werden."

## Was ist ein Profil? {#what}

Ein **Profil**, in der Client-Konsole auch als Empfängerin oder Empfänger bezeichnet, ist ein in der Campaign-Datenbank gespeicherter Eintrag. Es dient als Schlüsselkomponente zum [Erstellen von Zielgruppen](create-audience.md) für Sendungen und zum [Hinzufügen von Personalisierungsdaten](../personalization/personalize.md) zu Ihren Inhalten. Adobe Campaign ermöglicht die nahtlose Verwaltung von Profilen, einschließlich der Erstellung neuer Einträge und des Zugriffs auf eine umfassende Übersicht aller Profilattribute und Dienstabonnements, und zwar über die Campaign Web-Benutzeroberfläche.

Außerdem können mit **[!UICONTROL Testprofilen]**, die in der Client-Konsole ebenfalls als „Testprofile“ bezeichnet werden, zusätzliche Empfängerinnen und Empfänger angesprochen werden, die nicht den Zielgruppenbestimmungskriterien eines bestimmten Versands entsprechen. Diese Profile enthalten fiktive Kontaktinformationen oder Kontaktinformationen, die von der Absenderin oder dem Absender kontrolliert werden. Testprofile sind Empfängerinnen und Empfänger eines Testversands, mit denen Nachrichten durch Testsendungen getestet werden können. [Erfahren Sie, wie Sie mit Testprofilen arbeiten](test-profiles.md)

Profile und Testprofile sind nützlich, um Sendungen zu testen, bevor sie die gewünschte Zielgruppe erreichen. Dadurch können Sie eine Vorschau des Nachrichteninhalts und der Personalisierung anzeigen, Testsendungen zum Testen und Validieren durchführen, das E-Mail-Rendering auf verschiedenen Plattformen und Geräten auswerten und Landingpages testen. [Weitere Informationen dazu, wie Sendungen in der Vorschau angezeigt und getestet werden können](../preview-test/preview-test.md)

➡️ [Entdecken Sie diese Funktion im Video](#video)

## Zugriff auf die Liste der Profile {#access}

Profile sind in Adobe Campaign Web über **[!UICONTROL Kunden-Management]** > **Profile** in der linken Navigationsleiste verfügbar und bearbeitbar. Der Zugriff auf sie kann auch mithilfe der **[!UICONTROL Explorer-Ansicht]** über den Knoten **[!UICONTROL Profile und Zielgruppen]** > **[!UICONTROL Empfangende]** erfolgen. Dort können Sie Ordner oder Unterordner durchsuchen, erstellen und verwalten sowie die zugehörigen Berechtigungen überprüfen. [Erfahren Sie, wie Sie Ordner erstellen](../get-started/permissions.md#folders).

>[!NOTE]
>
>Je nach Ihren Berechtigungen haben Sie möglicherweise keinen Zugriff auf die vollständige Liste der in der Datenbank gespeicherten Profile. [Erfahren Sie mehr über Berechtigungen](../get-started/permissions.md).

Filtern Sie die Liste **[!UICONTROL Profile]** mit dem Suchfeld oder mit den über die Schaltfläche **Filter anzeigen** verfügbaren Filtern. Beschränken Sie die Ergebnisse über die Dropdown-Liste auf einen bestimmten [Ordner](../get-started/permissions.md#folders) oder fügen Sie mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzu.

![In der Liste „Profile“ verfügbare Filter](assets/profiles-list-filters.png){zoomable="yes"}

Um auf die Details eines Profils zuzugreifen, klicken Sie in der Liste auf dessen Namen. Eine detaillierte Ansicht des Profils wird geöffnet, in der Sie die zugehörigen Attribute und die abonnierten Dienste einsehen können. [Erfahren Sie, wie Sie die Profildetails durchsuchen können.](create-profile.md)

Um ein Profil zu löschen, wählen Sie die entsprechende Option im Menü **[!UICONTROL Mehr Aktionen]**.

## Anleitungsvideo {#video}

Informationen dazu, wie Sie mit der Campaign Web-Benutzeroberfläche auf Profile zugreifen und diese verwalten und erkunden können

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)