---
title: Erstellen einer Landingpage
description: Erfahren Sie, wie Sie eine Landingpage im Campaign Web konfigurieren und veröffentlichen
feature: Landing Pages
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: e661517d68c2fe21f4209dbec2d98648740a3a86
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 7%

---

# Landingpages erstellen und veröffentlichen {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Landingpages erstellen und verwalten"
>abstract="Mit Adobe Campaign können Sie Landingpages erstellen, entwerfen und freigeben, um Ihre Benutzer auf Online-Webseiten weiterzuleiten, auf denen Sie anhand integrierter Vorlagen Nutzungsszenarios für Akquise, Abonnement/Abmeldung und Blockierungsliste verwalten können."

Über die Campaign-Webbenutzeroberfläche können Sie Landingpages erstellen, entwerfen und veröffentlichen. Nach der Veröffentlichung können Sie einen Link zu Ihrem Formular in einen Versand einfügen. Nachdem die Empfänger auf diesen Link geklickt haben, werden sie zur entsprechenden Landingpage weitergeleitet.

[!DNL Adobe Campaign] enthält vier Vorlagen zur Verwaltung der folgenden Anwendungsfälle: **Akquise**, **Abonnement**, **Abmeldung**, und **Blockierungsliste**.

## Auf Landingpages zugreifen {#access-landing-pages}

Um auf die Landingpage-Liste zuzugreifen, wählen Sie **[!UICONTROL Kampagnenverwaltung]** > **[!UICONTROL Landingpages]** über das Menü links.

![](assets/lp-inventory.png)

Die **[!UICONTROL Landingpages]** inventory zeigt alle erstellten Elemente an. Sie können sie mithilfe der **Filter anzeigen** Schaltfläche. Sie können die Ergebnisse über die Dropdown-Liste auf einen bestimmten [Ordner](../get-started/permissions.md#folders) beschränken oder mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzufügen.

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Landingpages, die über die Clientkonsole (Webformulare) in der Campaign-Webbenutzeroberfläche erstellt wurden, können nicht angezeigt oder bearbeitet werden. Weitere Informationen finden Sie unter [Dokumentation zur Campaign Console](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Sie können eine Landingpage duplizieren oder löschen. Klicken Sie auf das Auslassungszeichen neben einer Landingpage, um die gewünschte Aktion auszuwählen.

## Erstellen einer Landingpage {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Landingpage-Eigenschaften definieren"
>abstract="Füllen Sie die Eigenschaftenfelder wie den Titel aus und ändern Sie bei Bedarf das Schema. Darüber hinaus können Sie den internen Namen bearbeiten, den Ordner ändern, in dem die Landingpage gespeichert ist, und eine Beschreibung angeben."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Inhalt der einzelnen Seiten definieren"
>abstract="Passen Sie den Inhalt jeder Seite an, die Teil dieser Landingpage ist, z. B. das Formular selbst, die Bestätigungsseite, die beim Senden des Formulars angezeigt wird, oder die Seite, auf die Benutzer im Falle eines Fehlers weitergeleitet werden."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Landingpage planen"
>abstract="Sie können ein Start- und ein Enddatum für Ihre Landingpage definieren. Wenn die Seite das Ende des Gültigkeitszeitraums erreicht, ist das Formular nicht mehr verfügbar. Die **Ablauf** -Seite angezeigt."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Primärseiteneinstellungen definieren"
>abstract="Die primäre Seite wird den Benutzern sofort angezeigt, nachdem sie auf den Link zu Ihrer Landingpage geklickt haben, z. B. über eine E-Mail oder eine Website."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Abonnement-Landingpage festlegen"
>abstract="Über eine Anmeldeseite können Ihre Kunden einen Dienst abonnieren."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. Aus dem **[!UICONTROL Landingpages]** inventory, click **[!UICONTROL Landingpage erstellen]**.

   ![](assets/lp-create-button.png)

1. Wählen Sie eine Vorlage:
   * **[!UICONTROL Akquise]**: Dies ist die Standardvorlage für Landingpages, mit der Sie Profildaten erfassen und aktualisieren können.
   * **[!UICONTROL Abonnement]**: Verwenden Sie diese Vorlage, damit Benutzer sich für eine bestimmte [service](manage-services.md).
   * **[!UICONTROL Abmeldung]**: Diese Vorlage kann in einem Versand verwendet werden, der an Abonnenten eines Dienstes gesendet wird, damit sie sich von dieser Abmeldung abmelden können. [service](manage-services.md).
   * **[!UICONTROL Blockierungsliste]**: Diese Vorlage sollte verwendet werden, wenn ein Profil nicht mehr von Campaign kontaktiert werden möchte. Erfahren Sie mehr über die Verwaltung von Blockierungslisten

   ![](assets/lp-templates.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Füllen Sie die **[!UICONTROL Eigenschaften]** -Felder, z. B. die Beschriftung.

   Landingpages werden standardmäßig im **[!UICONTROL Webanwendungen]** Ordner. Sie können sie ändern, indem Sie zur gewünschten Position im **[!UICONTROL Zusätzliche Optionen]**. [Erfahren Sie mehr über die Arbeit mit Ordnern](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. Im **[!UICONTROL Datenvorbereitung]** -Bereich, sind die beiden folgenden Optionen standardmäßig ausgewählt:

   * Die **[!UICONTROL Vorausfüllen mit den im Formular referenzierten Daten]** -Option können Sie automatisch die Daten vorab laden, die den Eingabe- und Zusammenführungsfeldern im Formular entsprechen.

   * Wenn Sie keine Profile aktualisieren möchten, muss die Option **[!UICONTROL Bei nicht angegebener Identifizierung vorausgefüllte Informationen ignorieren]** ausgewählt werden. In diesem Fall wird jedes eingegebene Profil nach Genehmigung des Formulars der Datenbank hinzugefügt. Diese Option wird beispielsweise verwendet, wenn das Formular auf einer Website veröffentlicht wird.

1. Im **[!UICONTROL Seiten]** klicken Sie auf die **[!UICONTROL Inhalt bearbeiten]** für jede Seite, die Sie für diese Landingpage erstellen möchten. Der Inhalt jeder Seite ist bereits vorausgefüllt. Bearbeiten Sie sie nach Bedarf. [Weitere Informationen](lp-content.md)

   ![](assets/lp-pages.png)

1. Die **[!UICONTROL Vorausgefüllten Datensatz aktualisieren]** ist standardmäßig aktiviert. Dadurch können die in der Datenbank gespeicherten Profile über die Landingpage aktualisiert werden. Im Feld Vorausfüllen können Sie angeben, wie der zu aktualisierende Datensatz in der Datenbank gefunden werden soll.

   Sie können auch aus den Feldern wählen, die im aktuellen Kontext der Landingpage verwendet werden, um das entsprechende Profil in der Datenbank zu finden. Heben Sie dazu die Auswahl der **[!UICONTROL Vorausgefüllten Datensatz aktualisieren]** und aktivieren Sie die gewünschten Felder unter **[!UICONTROL Abstimmoptionen]**.

   ![](assets/lp-storage.png)

1. Sie können ein Start- und ein Enddatum für Ihre Landingpage definieren. Auswählen **[!UICONTROL Aktivieren der Planung]** und legen Sie die Daten fest.

   ![](assets/lp-schedule.png)

   * Die Landingpage wird automatisch am angegebenen Startdatum/zur festgelegten Startzeit veröffentlicht.

     >[!NOTE]
     >
     >Wenn kein Startdatum definiert ist, wird die Landingpage sofort nach der Veröffentlichung live geschaltet.

   * Wenn die Seite das Enddatum erreicht, wird die Veröffentlichung der Landingpage automatisch aufgehoben und das Formular ist nicht mehr verfügbar. Die **[!UICONTROL Ablauf]** -Seite angezeigt.

     >[!NOTE]
     >
     >Aus Sicherheitsgründen und aus Gründen der Plattformleistung empfiehlt Adobe, ein Enddatum festzulegen.

1. Klicks **[!UICONTROL Überprüfen und veröffentlichen]**.

Nachdem Sie alle Einstellungen und [entworfen](lp-content.md) alle Seiten, können Sie [test](#test-landing-page) und [publish](#publish-landing-page) Ihre Landingpage.

## Landingpage testen {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Landingpage simulieren"
>abstract="Sie können eine Vorschau Ihrer Landingpage in der Campaign-Web-Benutzeroberfläche anzeigen oder sie in einem neuen Webbrowser-Tab öffnen."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Vorschau erstellen und Landingpage testen"
>abstract="Nachdem Sie die Einstellungen und den Inhalt Ihrer Landingpage definiert haben, können Sie sie mit Testprofilen in der Vorschau anzeigen."

Nachdem Sie die Einstellungen und den Inhalt Ihrer Landingpage definiert haben, können Sie sie mit Testprofilen in der Vorschau anzeigen. Wenn Sie [personalisierter Inhalt](../personalization/gs-personalization.md)können Sie mithilfe von Testprofildaten überprüfen, wie dieser Inhalt auf der Landingpage dargestellt wird.

>[!CAUTION]
>
>Sie müssen über Testprofile verfügen, damit Sie eine Vorschau Ihrer Nachrichten anzeigen und Testsendungen durchführen können. [Erfahren Sie mehr über Testprofile](../audience/test-profiles.md)

1. Nachdem Sie auf **[!UICONTROL Überprüfen und veröffentlichen]**, wählen Sie die **[!UICONTROL Inhalt simulieren]** -Schaltfläche im Landingpage-Dashboard, um auf die Testprofilauswahl zuzugreifen.

   ![](assets/lp-simulate-content.png)

1. Aus dem **[!UICONTROL Simulieren]** ein oder mehrere Testprofile aus.

   Die Schritte zum Auswählen von Testprofilen sind mit denen beim Testen einer Nachricht identisch. Sie werden im Abschnitt [Vorschau und Test](../preview-test/preview-test.md) Abschnitt.

1. Auswählen **[!UICONTROL Vorschau öffnen]** , um Ihre Landingpage zu testen.

   ![](assets/lp-open-preview.png)

1. Die Vorschau Ihrer Landingpage wird in einem neuen Tab geöffnet. Personalisierte Elemente werden durch die ausgewählten Testprofildaten ersetzt.

   Wenn Sie die Option **[!UICONTROL Vorausfüllen mit den im Formular referenzierten Daten]** in den Landingpage-Einstellungen automatisch die entsprechenden Testprofildaten in die Formularfelder eingefügt.<!--TBC-->

   ![](assets/lp-preview.png)

1. Wählen Sie weitere Testprofile aus, um das Rendering für jede Variante Ihrer Landingpage in der Vorschau anzuzeigen.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Landingpage veröffentlichen {#publish-landing-page}

Sobald Ihre Landingpage fertig ist, veröffentlichen Sie sie, um sie mithilfe der entsprechenden Schaltfläche für einen Versand verfügbar zu machen.

Nach der Veröffentlichung:

* Die Landingpage wird der Landingpage-Liste mit dem **[!UICONTROL Veröffentlicht]** -Status. Es ist jetzt live und kann in Ihren Inhalten referenziert werden.

* Sie können die **[!UICONTROL Landingpage-URL]** , die oben auf der Seite in einem Webbrowser angezeigt wird.

![](assets/lp-published.png)

Sie können die Auswirkungen Ihrer Landingpage über Protokolle überwachen<!--and specific reports-->. Klicken Sie auf **[!UICONTROL Protokolle]** Schaltfläche.
