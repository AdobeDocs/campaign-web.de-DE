---
title: Erstellen von Testprofilen in Campaign
description: Erfahren Sie, wie Sie in Adobe Campaign Testprofile erstellen und verwalten.
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 74%

---

# Erstellen und Verwalten von Testprofilen {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Erstellen von Testprofilen"
>abstract="Testprofile sind zusätzliche Empfänger, mit denen Sie die Personalisierung und das Rendering vor dem Nachrichtenversand in der Vorschau ansehen und testen können. Sie können bei der Vorschau eines Nachrichteninhalts ein Testprofil auswählen und Testsendungen an die Testprofile durchführen, um den Nachrichteninhalt und die Einstellungen zu steuern und zu validieren."

Testprofile werden verwendet, um Testsendungen durchzuführen und den Inhalt und die Einstellungen Ihrer Nachricht zu validieren. Bei diesen Profilen handelt es sich um zusätzliche Empfänger, mit denen Sie die Personalisierung und das Rendering vor dem Nachrichtenversand in der Vorschau ansehen und testen können. Sie können bei der Vorschau eines Nachrichteninhalts ein Testprofil auswählen und Testsendungen an die Testprofile durchführen, um den Nachrichteninhalt und die Einstellungen zu steuern und zu validieren.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

Die Schritte zum Senden von Testsendungen an Testprofile werden im Abschnitt [diesem Abschnitt](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>* Testprofile werden in der Client-Konsole als Testadressen erstellt.
>
>* Testprofile werden automatisch aus Berichten für die folgenden Versandstatistiken ausgeschlossen: **[!UICONTROL Klicks]**, **[!UICONTROL Öffnungen]**, **[!UICONTROL Abmeldungen]**.

## Zugreifen auf und Verwalten von Testprofilen {#access-test-profiles}

Um auf die Testprofilliste zuzugreifen, wählen Sie **[!UICONTROL Kunden-Management]** > **[!UICONTROL Profile]** im linken Menü und öffnen Sie die Registerkarte **[!UICONTROL Testprofile]**.

![](assets/test-profile-list.png){zoomable=&quot;yes&quot;}

* Über die Dropdown-Liste können Sie nach einem bestimmten [Ordner](../get-started/permissions.md#folders) filtern oder mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzufügen.

  ![](assets/test-profile-list-filters.png){zoomable=&quot;yes&quot;}

* Sie können jedes Testprofil nach Bedarf duplizieren und aktualisieren. Die Schritte zum Bearbeiten eines Testprofils sind dieselben wie beim [Erstellen eines Testprofils](#create-test-profile).

* Um ein Testprofil zu löschen, wählen Sie die entsprechende Option aus dem Menü **[!UICONTROL Mehr Aktionen]**.

  ![](assets/test-profile-list-delete.png){zoomable=&quot;yes&quot;}

* Klicken Sie auf das gewünschte Element in der Liste, um ein Testprofil zu bearbeiten. Die Schritte zum Bearbeiten eines Testprofils sind dieselben wie beim [Erstellen eines Testprofils](#create-test-profile).

Sie können auch in der **[!UICONTROL Explorer]**-Ansicht unter dem Knoten **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Testadressen]** auf Testprofile zugreifen.

Dort können Sie Ordner oder Unterordner durchsuchen, erstellen und verwalten sowie die zugehörigen Berechtigungen überprüfen. [Erfahren Sie, wie Sie Ordner erstellen](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png){zoomable=&quot;yes&quot;}

In der **[!UICONTROL Explorer]**-Ansicht können Sie Testprofile auch filtern, löschen, bearbeiten und [erstellen](#create-test-profile).

## Erstellen eines Testprofils {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Zusätzliche Daten zu Testprofilen"
>abstract="Die Personalisierungsdaten angben, die für die in den Data-Management-Workflows erstellten Sendungen verwendet werden und denen ein bestimmter Wert zugeweisen werden soll."

Gehen Sie wie folgt vor, um ein Testprofil zu erstellen:

1. Navigieren Sie zu **[!UICONTROL Kunden-Management]** > **[!UICONTROL Profile]** und öffnen Sie die Registerkarte **[!UICONTROL Testprofile]**.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Testprofil erstellen]**.

   ![](assets/test-profile-create.png){zoomable=&quot;yes&quot;}

1. Geben Sie die Details des Testprofils nach Bedarf ein. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Das Feld **[!UICONTROL Titel]** wird automatisch mit dem von Ihnen festgelegten Vor- und Nachnamen ausgefüllt.

1. Standardmäßig werden Testprofile im Ordner **[!UICONTROL Testadressen]** gespeichert. Sie können ihn ändern, indem Sie zum gewünschten Speicherort navigieren. [Erfahren Sie mehr über die Arbeit mit Ordnern](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. Geben Sie im Abschnitt **[!UICONTROL Kontaktdaten]** die E-Mail-Adresse und andere relevante Daten ein. Die E-Mail-Adresse wird in eckigen Klammern hinter der Testprofilbezeichnung angezeigt.

   ![](assets/test-profile-address.png){zoomable=&quot;yes&quot;}

1. Wenn Sie die Option **[!UICONTROL Nicht mehr kontaktieren (alle Kanäle)]** aktivieren, befindet sich das Testprofil auf der Blockierungsliste. Solch eine Person wird auf keinem Kanal (E-Mail, SMS, usw.) mehr ausgewählt.

1. Geben Sie in der Registerkarte **[!UICONTROL Zusätzliche Daten]** die Personalisierungsdaten ein, mit denen die Sendungen in den Daten-Management-Workflows erstellt wurden und denen Sie einen bestimmten Wert zuweisen möchten. [Erfahren Sie mehr über Workflows](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png){zoomable=&quot;yes&quot;}

   Stellen Sie sicher, dass in der Workflow-Aktivität **[!UICONTROL Anreicherung]** zusätzliche Zielgruppendaten mit einem Alias definiert wurden, der mit „@“ beginnt. Andernfalls können Sie sie in der Versandaktivität nicht ordnungsgemäß mit Ihren Testadressen verwenden. [Erfahren Sie mehr über die Anreicherungs-Aktivität](../workflows/activities/enrichment.md)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Speichern]**.

Das soeben erstellte Testprofil kann jetzt zur Durchführung einer Testsendung verwendet werden. [Weitere Informationen](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->
