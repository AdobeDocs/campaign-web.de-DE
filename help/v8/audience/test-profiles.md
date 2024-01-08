---
title: Erstellen von Testprofilen in Campaign
description: Erfahren Sie, wie Sie in Adobe Campaign Testprofile erstellen und verwalten.
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 1f8a6c9765350f1c39a009afd7c1852967835d73
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 13%

---

# Erstellen und Verwalten von Testprofilen {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Erstellen von Testprofilen"
>abstract="Testprofile werden als Testadressen erstellt. Es handelt sich um zusätzliche Empfänger in der Datenbank, die für die Zielgruppenbestimmung fiktiver Profile verwendet werden, die nicht den definierten Zielkriterien entsprechen."

Testprofile werden als Testadressen erstellt. Es handelt sich um zusätzliche Empfänger in der Datenbank, die für die Zielgruppenbestimmung fiktiver Profile verwendet werden, die nicht den definierten Zielkriterien entsprechen. Sie ermöglichen es, Personalisierung und Rendering in der Vorschau anzuzeigen und zu testen, bevor Sie Ihren Versand durchführen, indem Sie Testsendungen durchführen.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

Die Schritte zum Senden von Testnachrichten an Testadressen werden im Abschnitt [diesem Abschnitt](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>Testprofile werden automatisch aus Berichten für die folgenden Versandstatistiken ausgeschlossen: **[!UICONTROL Klicks]**, **[!UICONTROL Öffnungen]**, **[!UICONTROL Abmeldungen]**. [Weitere Informationen zu Berichten]

## Testprofile aufrufen und verwalten {#access-test-profiles}

Um auf die Testprofilliste zuzugreifen, wählen Sie **[!UICONTROL Kundenverwaltung]** > **[!UICONTROL Profile]** Klicken Sie im linken Menü auf die Schaltfläche **[!UICONTROL Testprofile]** Registerkarte.

![](assets/test-profile-list.png)

* Sie können nach [Ordner](../get-started/permissions.md#folders) über die Dropdown-Liste oder das Hinzufügen von Regeln mithilfe der [Abfragemodellierung](../query/query-modeler-overview.md).

  ![](assets/test-profile-list-filters.png)

* Sie können jedes Testprofil duplizieren und nach Bedarf aktualisieren. Die Schritte zum Bearbeiten eines Testprofils sind dieselben wie beim [Testprofil erstellen](#create-test-profile).

* Um ein Testprofil zu löschen, wählen Sie die entsprechende Option aus dem **[!UICONTROL Mehr Aktionen]** Menü.

  ![](assets/test-profile-list-delete.png)

* Um ein Testprofil zu bearbeiten, klicken Sie in der Liste auf das gewünschte Element. Die Schritte zum Bearbeiten eines Testprofils sind dieselben wie beim [Testprofil erstellen](#create-test-profile).

Testprofile können auch über die **[!UICONTROL Explorer]** Ansicht aus der **[!UICONTROL Ressourcen]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Testadressen]** Knoten.

Dort können Sie Ordner oder Unterordner durchsuchen, erstellen und verwalten sowie die zugehörigen Berechtigungen überprüfen. [Erfahren Sie, wie Sie Ordner erstellen](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png)

Aus dem **[!UICONTROL Explorer]** Sie können auch filtern, löschen, bearbeiten und [erstellen](#create-test-profile) Testprofile.

## Erstellen eines Testprofils {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Zusätzliche Daten zu Testprofilen"
>abstract="Geben Sie die Personalisierungsdaten an, die für die in den Data-Management-Workflows erstellten Sendungen verwendet werden und denen Sie einen bestimmten Wert zuweisen möchten."

Gehen Sie wie folgt vor, um ein Testprofil zu erstellen.

1. Navigieren Sie zu **[!UICONTROL Kundenverwaltung]** > **[!UICONTROL Profile]** und wählen Sie die **[!UICONTROL Testprofile]** Registerkarte.

1. Klicken Sie auf **[!UICONTROL Testprofil erstellen]** Schaltfläche.

   ![](assets/test-profile-create.png)

1. Füllen Sie die Details des Testprofils nach Bedarf aus. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >Die **[!UICONTROL Titel]** automatisch den von Ihnen definierten Vor- und Nachnamen eingeben.

1. Standardmäßig werden Testprofile im **[!UICONTROL Testadressen]** Ordner. Sie können sie ändern, indem Sie zur gewünschten Position navigieren. [Informationen zum Arbeiten mit Ordnern](../get-started/permissions.md#folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. Im **[!UICONTROL Kontaktangaben]** geben Sie die E-Mail-Adresse und andere relevante Daten ein. Die E-Mail-Adresse wird in eckigen Klammern hinter der Testprofilbeschriftung angezeigt.

   ![](assets/test-profile-address.png)

1. Wenn Sie die **[!UICONTROL No longer contact (by any channel)]** aktivieren, befindet sich das Testprofil auf der Blockierungsliste. Ein solcher Empfänger ist in keinem Kanal mehr enthalten (E-Mail, SMS usw.).

1. Im **[!UICONTROL Zusätzliche Daten]** Geben Sie die Personalisierungsdaten für die in den Data Management-Workflows erstellten Sendungen ein, denen Sie einen bestimmten Wert zuweisen möchten. [Weitere Informationen zu Workflows](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Stellen Sie sicher, dass in der Workflow-Aktivität **[!UICONTROL Anreicherung]** zusätzliche Zielgruppendaten mit einem Alias definiert wurden, der mit „@“ beginnt. Andernfalls können Sie sie nicht ordnungsgemäß mit Ihren Testadressen in der Versandaktivität verwenden. [Erfahren Sie mehr über die Aktivität Anreicherung .](../workflows/activities/enrichment.md)

1. Auf den Button **[!UICONTROL Speichern]** klicken.

Das soeben erstellte Testprofil kann jetzt zum Senden eines Tests verwendet werden. [Weitere Informationen](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->



