---
title: Erstellen von Testprofilen in Campaign
description: Erfahren Sie, wie Sie in Adobe Campaign Testprofile erstellen und verwalten.
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 59094528cb3683dba7264e6b63b5166a0a91f8ed
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 14%

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
>Testprofile werden automatisch aus Berichten für die folgenden Versandstatistiken ausgeschlossen: **[!UICONTROL Klicks]**, **[!UICONTROL Öffnungen]**, **[!UICONTROL Abmeldungen]**.

## Testprofile aufrufen und verwalten {#access-test-profiles}

Um auf die Liste der Inhaltsvorlagen zuzugreifen, wählen Sie **[!UICONTROL Kundenverwaltung]** > **[!UICONTROL Profile]** Wählen Sie im linken Menü die Option **[!UICONTROL Testprofile]** Registerkarte.

Sie können nach [Ordner](../get-started/permissions.md#folders) über die Dropdown-Liste oder das Hinzufügen von Regeln mithilfe der [Abfragemodellierung](../query/query-modeler-overview.md).

Um ein Testprofil zu bearbeiten, klicken Sie in der Liste auf das gewünschte Element.

Um ein Testprofil zu löschen, wählen Sie die entsprechende Option aus dem **[!UICONTROL Mehr Aktionen]** Menü.

## Erstellen eines Testprofils {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Zusätzliche Daten zu Testprofilen"
>abstract="Geben Sie die Personalisierungsdaten an, die für die in den Data-Management-Workflows erstellten Sendungen verwendet werden und denen Sie einen bestimmten Wert zuweisen möchten."

Gehen Sie wie folgt vor, um ein Testprofil zu erstellen.

1. Navigieren Sie zu **[!UICONTROL Kundenverwaltung]** > **[!UICONTROL Profile]**.

1. Wählen Sie die **[!UICONTROL Testprofile]** Registerkarte.

   ![](assets/test-profile-list.png)

1. Klicken Sie auf **[!UICONTROL Testprofil erstellen]** Schaltfläche.

1. Füllen Sie die Testprofildetails aus. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >Der Titel der Adresse wird automatisch mit dem von Ihnen definierten Vor- und Nachnamen ausgefüllt.

1. Standardmäßig werden Testprofile im **[!UICONTROL Testadressen]** Ordner. Sie können sie ändern, indem Sie zur gewünschten Position navigieren. [Weitere Informationen](#seed-addresses-folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. Im **[!UICONTROL Kontaktangaben]** geben Sie die E-Mail-Adresse und andere relevante Daten ein. Die E-Mail-Adresse wird in eckigen Klammern hinter der Testprofilbeschriftung angezeigt.

   ![](assets/test-profile-address.png)

1. Wenn Sie die **[!UICONTROL No longer contact (by any channel)]** aktivieren, befindet sich das Profil auf der Blockierungsliste. Ein solcher Empfänger ist in keinem Kanal mehr enthalten (E-Mail, SMS usw.).

1. Im **[!UICONTROL Zusätzliche Daten]** Geben Sie die Personalisierungsdaten für die in den Data Management-Workflows erstellten Sendungen ein, denen Sie einen bestimmten Wert zuweisen möchten. [Weitere Informationen zu Workflows](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Stellen Sie sicher, dass in der Workflow-Aktivität **[!UICONTROL Anreicherung]** zusätzliche Zielgruppendaten mit einem Alias definiert wurden, der mit „@“ beginnt. Andernfalls können Sie sie nicht ordnungsgemäß mit Ihren Testadressen in der Versandaktivität verwenden. [Erfahren Sie mehr über die Aktivität Anreicherung .](../workflows/activities/enrichment.md)

1. Auf den Button **[!UICONTROL Speichern]** klicken.

Das soeben erstellte Testprofil kann jetzt zum Senden eines Tests verwendet werden. [Weitere Informationen](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Verwalten von Testadressenordnern {#seed-addresses-folders}

Testadressen werden in einem dedizierten Knoten der Adobe Campaign-Hierarchie gespeichert: **[!UICONTROL Explorer]** > **[!UICONTROL Ressourcen]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Testadressen]**.

Um Testprofile zu organisieren, können Sie in der Dropdownliste Mehr Aktionen Unterordner erstellen. [Erfahren Sie, wie Sie Ordner erstellen](../get-started/permissions.md#folders)

![](assets/test-profile-sub-folders.png)

Sie können ein Testprofil auch aus einer beliebigen **[!UICONTROL Testadressen]** Ordner oder Unterordner. Füllen Sie alle Details auf die gleiche Weise aus wie Sie es mit der **[!UICONTROL Kundenverwaltung]** > **[!UICONTROL Profile]** Menü. [Weitere Informationen](#create-test-profile)

Um Testprofile zu bearbeiten, klicken Sie auf deren Titel entweder im **[!UICONTROL Testprofile]** oder aus dem Ordner, in dem sie gespeichert ist.

