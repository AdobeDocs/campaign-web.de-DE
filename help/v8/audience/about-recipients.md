---
title: Erste Schritte mit Profilen
description: Erfahren Sie, wie Sie Profile in Adobe Campaign Web überwachen und verwalten können.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 35%

---

# Erste Schritte mit Profilen {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profile"
>abstract="Ein Profil ist ein Datensatz, der an den Empfang von Nachrichten gerichtet ist, die von Adobe Campaign gesendet werden. In dieser Liste können die Details der Profile anhand der Berechtigungen angezeigt werden. Verwenden Sie die Filteroptionen, um diese Liste zu durchsuchen. Eine kleine Gruppe von Profilattributen kann bearbeitet und aktualisiert werden."

## Was ist ein Profil? {#what}

Ein **Profil** in der Client-Konsole auch als „Empfänger“ bezeichnet, stellt einen in der Campaign-Datenbank gespeicherten Datensatz dar. Es dient als Schlüsselkomponente zum [ von Zielgruppen ](create-audience.md) Sendungen und zum [ von Personalisierungsdaten ](../personalization/personalize.md) Ihren Inhalten. Adobe Campaign ermöglicht die nahtlose Verwaltung von Profilen, einschließlich der Erstellung neuer Einträge und des Zugriffs auf eine umfassende Ansicht aller Profilattribute und Service-Abonnements über die Campaign Web-Benutzeroberfläche.

Darüber hinaus **[!UICONTROL „Testprofile]** in der Client-Konsole als „Testprofile“ gekennzeichnet und ermöglichen es, zusätzliche Empfänger anzusprechen, die nicht den Zielgruppenkriterien eines bestimmten Versands entsprechen. Diese Profile enthalten fiktive Kontaktinformationen oder Kontaktinformationen, die vom Absender gesteuert werden. Testprofile sind Testversand-Empfänger, die zum Testen von Nachrichten durch Senden von Testsendungen verwendet werden. [Erfahren Sie, wie Sie mit Testprofilen arbeiten](test-profiles.md)

Sowohl Profile als auch Testprofile sind nützlich, um Sendungen zu testen, bevor sie die vorgesehene Zielgruppe erreichen. Dies ermöglicht die Vorschau des Nachrichteninhalts und der Personalisierung, das Senden von Testsendungen für Tests und Validierung, das Bewerten des E-Mail-Renderings auf verschiedenen Plattformen und Geräten sowie das Testen von Landingpages. [Weitere Informationen dazu, wie Sendungen in der Vorschau angezeigt und getestet werden können](../preview-test/preview-test.md)

➡️ [Diese Funktion im Video](#video)

## Zugriff auf die Liste der Profile {#access}

Profile sind in Adobe Campaign Web über **[!UICONTROL Kunden-Management]** > **Profile** in der linken Navigationsleiste verfügbar und bearbeitbar. Sie können auf sie auch in der Ansicht **[!UICONTROL Explorer]** über den Knoten **[!UICONTROL Profile und Zielgruppen]** > **[!UICONTROL Empfänger]** zugreifen. Durchsuchen, erstellen und verwalten Sie von dort aus Ordner oder Unterordner und überprüfen Sie die zugehörigen Berechtigungen. [Erfahren Sie, wie Sie Ordner erstellen](../get-started/permissions.md#folders).

>[!NOTE]
>
>Je nach Ihren Berechtigungen haben Sie möglicherweise keinen Zugriff auf die vollständige Liste der in der Datenbank gespeicherten Profile. [Erfahren Sie mehr über Berechtigungen](../get-started/permissions.md)

Filtern Sie die **[!UICONTROL Profile]** mithilfe des Suchfelds oder der Filter, die über die Schaltfläche **Filter anzeigen** verfügbar sind. Beschränken Sie die Ergebnisse mithilfe [ Dropdown-Liste auf einen bestimmten ](../get-started/permissions.md#folders)Ordner“ oder fügen Sie Regeln mithilfe des [Abfragemodellierers“ ](../query/query-modeler-overview.md).

![In der Profilliste verfügbare Filter](assets/profiles-list-filters.png){zoomable="yes"}

Um auf die Details eines Profils zuzugreifen, klicken Sie in der Liste auf seinen Namen. Es wird eine detaillierte Ansicht des Profils geöffnet, in der die Attribute und Services, die das Profil abonniert hat, erläutert werden. [Erfahren Sie, wie Sie die Profildetails durchsuchen können.](create-profile.md)

Um ein Profil zu löschen, wählen Sie die entsprechende Option im Menü **[!UICONTROL Mehr Aktionen]**.

## Anleitungsvideo {#video}

Informationen dazu, wie Sie mit der Campaign Web-Benutzeroberfläche auf Profile zugreifen und diese verwalten und erkunden können

>[!VIDEO](https://video.tv.adobe.com/v/3448373?quality=12&captions=ger)