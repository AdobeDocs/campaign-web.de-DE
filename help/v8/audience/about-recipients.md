---
title: Erste Schritte mit Profilen
description: Erfahren Sie, wie Sie Profile in Adobe Campaign Web überwachen und verwalten können.
source-git-commit: 55441646867b7dee454a7f37c0a1b696e61926de
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 54%

---

# Erste Schritte mit Profilen {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="360-Grad-Ansicht Ihrer Profile"
>abstract="Erstellen Sie neue Profile und überwachen Sie sie mithilfe leistungsstarker Berichte und Tools. Greifen Sie auf die Attribute, Interaktionen und Protokolle Ihrer Profile zu. Verwenden Sie die Filteroptionen, um die Profilliste zu durchsuchen und ihr Profil zu bearbeiten und zu aktualisieren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=de" text="Siehe Versionshinweise"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360-Grad-Ansicht Ihrer Profile"
>abstract="Erstellen Sie neue Profile und überwachen Sie sie mithilfe leistungsstarker Berichte und Tools. Greifen Sie auf die Attribute, Interaktionen und Protokolle Ihrer Profile zu. Verwenden Sie die Filteroptionen, um die Profilliste zu durchsuchen und ihr Profil zu bearbeiten und zu aktualisieren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=de" text="Siehe Versionshinweise"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profile"
>abstract="Ein Profil ist ein Datensatz, der für den Empfang von Nachrichten bestimmt ist, die von Adobe Campaign gesendet werden. In dieser Liste können die Details der Profile anhand der Berechtigungen angezeigt werden. Verwenden Sie die Filteroptionen, um diese Liste zu durchsuchen. Eine kleine Gruppe von Profilattributen kann bearbeitet und aktualisiert werden."

## Was ist ein Profil? {#what}

A **profile**, in der Client-Konsole auch als &quot;Empfänger&quot;bezeichnet, stellt einen Datensatz dar, der in der Campaign-Datenbank gespeichert ist und als Schlüsselkomponente für [Erstellen von Zielgruppen](create-audience.md) für Sendungen und [Personalisierung hinzufügen](../personalization/personalize.md) Daten an Ihren Inhalt. Adobe Campaign ermöglicht die nahtlose Verwaltung von Profilen, von der Erstellung neuer Einträge bis hin zur umfassenden Übersicht aller Abonnements für Profile und Dienste über die Campaign-Webbenutzeroberfläche.

Darüber hinaus **[!UICONTROL Testprofile]**, in der Clientkonsole als &quot;Testprofile&quot;bezeichnet, ermöglichen es Ihnen, zusätzliche Empfänger anzusprechen, die nicht den Targeting-Kriterien eines bestimmten Versands entsprechen. Diese Profile enthalten fiktive Kontaktinformationen oder Kontaktinformationen, die vom Absender kontrolliert werden. Sie können der Audience einer Nachricht hinzugefügt werden, um beispielsweise Missbrauch bei der Nutzung Ihrer Empfängerdatenbank zu erkennen oder sicherzustellen, dass die E-Mails in den Posteingang eingehen. [Erfahren Sie, wie Sie mit Testprofilen arbeiten](test-profiles.md)

Sie können sowohl Profile als auch Testprofile verwenden, um Ihre Sendungen zu testen, bevor sie die gewünschte Zielgruppe erreichen. Auf diese Weise können Sie eine Vorschau des Nachrichteninhalts und der Personalisierung anzeigen, Testsendungen zum Testen und Validieren durchführen, das E-Mail-Rendering auf verschiedenen Plattformen und Geräten evaluieren und Ihre Landingpages testen. [Erfahren Sie, wie Sie Sendungen in der Vorschau anzeigen und testen können.](../preview-test/preview-test.md)

## Zugriff auf die Liste der Profile {#access}

Die Profile können im Adobe Campaign Web über die **[!UICONTROL Kundenverwaltung]** > **Profile** in der linken Navigationsleiste. Sie können auch im **[!UICONTROL Explorer]** Ansicht aus der **[!UICONTROL Profile und Zielgruppen]** > **[!UICONTROL Empfänger]** Knoten. Dort können Sie Ordner oder Unterordner durchsuchen, erstellen und verwalten sowie die zugehörigen Berechtigungen überprüfen. [Erfahren Sie, wie Sie Ordner erstellen](../get-started/permissions.md#folders)

>[!NOTE]
>
>Je nach Ihren Berechtigungen haben Sie möglicherweise keinen Zugriff auf die vollständige Liste der in der Datenbank gespeicherten Profile. [Erfahren Sie mehr über Berechtigungen](../get-started/permissions.md).

Sie können die Liste der **[!UICONTROL Profile]** mit dem Suchfeld oder den unter **Filter anzeigen** verfügbaren Filtern durchsuchen. Sie können die Ergebnisse über die Dropdown-Liste auf einen bestimmten [Ordner](../get-started/permissions.md#folders) beschränken oder mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzufügen.

![](assets/profiles-list-filters.png){zoomable=&quot;yes&quot;}

Um auf die Details eines Profils zuzugreifen, klicken Sie in der Liste auf dessen Namen. Eine detaillierte Ansicht des Profils wird geöffnet, in der Sie seine Attribute und die Dienste, die es abonniert hat, einsehen können. [Erfahren Sie, wie Sie die Profildetails durchsuchen können.](create-profile.md)

Um ein Profil zu löschen, wählen Sie die entsprechende Option im Menü **[!UICONTROL Mehr Aktionen]**.
