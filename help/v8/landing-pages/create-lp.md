---
title: Erstellen einer Landingpage
description: Erfahren Sie, wie Sie eine Landingpage im Campaign Web konfigurieren und veröffentlichen
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 7d28b76b824d8bac1364e29e83bc07af51c9ac56
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 8%

---

# Landingpages erstellen und veröffentlichen {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Landingpages erstellen und verwalten"
>abstract="Mit Adobe Campaign können Sie Landingpages erstellen, entwerfen und freigeben, um Ihre Benutzer auf Online-Webseiten weiterzuleiten, auf denen Sie anhand integrierter Vorlagen Nutzungsszenarios für die Verwaltung, Akquise, An-/Abmeldung und Blockierungsliste verwalten können."

Mit Adobe Campaign können Sie Landingpages erstellen, entwerfen und freigeben, um Ihre Benutzer auf Online-Webseiten weiterzuleiten, auf denen Sie anhand integrierter Vorlagen Nutzungsszenarios für die Verwaltung, Akquise, An-/Abmeldung und Blockierungsliste verwalten können.

## Auf Landingpages zugreifen {#access-landing-pages}

Um auf die Landingpage-Liste zuzugreifen, wählen Sie **[!UICONTROL Kampagnenverwaltung]** > **[!UICONTROL Landingpages]** über das Menü links.

![](assets/lp-inventory.png)

Die **[!UICONTROL Landingpages]** inventory zeigt alle erstellten Elemente an. Sie können sie mithilfe der **Filter anzeigen** Schaltfläche. Sie können die Ergebnisse über die Dropdown-Liste auf einen bestimmten [Ordner](../get-started/permissions.md#folders) beschränken oder mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzufügen.

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!NOTE]
>
>Landingpages, die über die Clientkonsole erstellt wurden, können nicht im Campaign-Web angezeigt werden. Weitere Informationen finden Sie unter [Dokumentation zur Campaign Console](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Sie können eine Landingpage duplizieren oder löschen. Klicken Sie auf die drei Punkte neben einer Landingpage, um die gewünschte Aktion auszuwählen.

## Erstellen einer Landingpage {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Landingpage-Eigenschaften definieren"
>abstract="Füllen Sie die Eigenschaftenfelder wie den Titel aus und ändern Sie bei Bedarf das Schema. Darüber hinaus können Sie den internen Namen bearbeiten, den Ordner ändern, in dem die Landingpage gespeichert ist, und eine Beschreibung angeben."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Seiteninhalt definieren"
>abstract="Bearbeiten Sie den Inhalt jeder Seite, die Teil dieser Landingpage ist."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Landingpage planen"
>abstract="Sie können ein Start- und ein Enddatum für Ihre Landingpage definieren. Wenn die Seite abgelaufen ist, wird die **Ablauf** angezeigt."


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
   * **[!UICONTROL Abonnement]**: Verwenden Sie diese Vorlage, um Abonnements für einen Dienst anzubieten.
   * **[!UICONTROL Abmeldung]**: Diese Vorlage kann von einer an Abonnenten gesendeten E-Mail-Adresse aus mit der Möglichkeit verknüpft werden, sich von diesem Dienst abzumelden.
   * **[!UICONTROL Blockierungsliste]**: Diese Vorlage sollte verwendet werden, wenn ein Profil nicht mehr von Campaign kontaktiert werden möchte. Erfahren Sie mehr über die Verwaltung von Blockierungslisten

   ![](assets/lp-templates.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Füllen Sie die Eigenschaftenfelder wie den Titel aus. Landingpages werden standardmäßig im **[!UICONTROL Webanwendungen]** Ordner. Sie können sie ändern, indem Sie zur gewünschten Position im **[!UICONTROL Zusätzliche Optionen]**. [Erfahren Sie mehr über die Arbeit mit Ordnern](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. Im **[!UICONTROL Datenvorbereitung]** -Bereich, sind die beiden folgenden Optionen standardmäßig ausgewählt:

   * Die **[!UICONTROL Vorausfüllen mit den im Formular referenzierten Daten]** -Option können Sie automatisch die Daten vorab laden, die den Eingabe- und Zusammenführungsfeldern im Formular entsprechen.

   * Wenn Sie keine Profile aktualisieren möchten, muss die Option **[!UICONTROL Bei nicht angegebener Identifizierung vorausgefüllte Informationen ignorieren]** ausgewählt werden. In diesem Fall wird jedes eingegebene Profil nach Genehmigung des Formulars der Datenbank hinzugefügt. Diese Option wird beispielsweise verwendet, wenn das Formular auf einer Website veröffentlicht wird.

1. Im **[!UICONTROL Seiten]** klicken Sie auf die **[!UICONTROL Inhalt bearbeiten]** für jede Seite, die Sie für diese Landingpage erstellen möchten. Der Inhalt jeder Seite ist bereits vorausgefüllt. Bearbeiten Sie sie nach Bedarf. [Weitere Informationen](lp-content.md)

   ![](assets/lp-pages.png)

1. Die **[!UICONTROL Vorausgefüllten Datensatz aktualisieren]** ist standardmäßig ausgewählt. Wenn Sie die in der Datenbank gespeicherten Profile über die Landingpage aktualisieren möchten, können Sie eine Vorausfüllen-Komponente verwenden. Im Feld Vorausfüllen können Sie angeben, wie der zu aktualisierende Datensatz in der Datenbank gefunden werden soll. Sie können auch aus den Feldern wählen, die im aktuellen Kontext der Landingpage verwendet werden, um das entsprechende Profil in der Datenbank zu finden.

   ![](assets/lp-storage-schedule.png)

1. Sie können ein Start- und ein Enddatum für Ihre Landingpage definieren. Auswählen **[!UICONTROL Aktivieren der Planung]** und legen Sie die Daten fest. Wenn die Seite abgelaufen ist, wird die **[!UICONTROL Ablauf]** angezeigt.

1. Klicks **[!UICONTROL Überprüfen und veröffentlichen]**.

Nachdem Sie alle Seiten konfiguriert und entworfen haben, können Sie [test](#test-landing-page) und [publish](#publish-landing-page) Ihre Landingpage.

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
>Sie müssen über Testprofile verfügen, damit Sie eine Vorschau Ihrer Nachrichten anzeigen und Testsendungen durchführen können. Erfahren Sie, wie [Testprofile erstellen](../audience/test-profiles.md).

1. Klicken Sie in der Landingpage auf die Schaltfläche **[!UICONTROL Inhalt simulieren]** -Schaltfläche, um auf die Auswahl des Testprofils zuzugreifen.

   ![](assets/lp-simulate-content.png)

1. Aus dem **[!UICONTROL Simulieren]** ein oder mehrere Testprofile aus.

   Die Schritte zum Auswählen von Testprofilen sind mit denen beim Testen einer Nachricht identisch. Sie werden im Abschnitt [Vorschau und Test](../preview-test/preview-test.md) Abschnitt.

1. Auswählen **[!UICONTROL Vorschau öffnen]** , um Ihre Landingpage zu testen.

   ![](assets/lp-open-preview.png)

1. Die Vorschau Ihrer Landingpage wird in einem neuen Tab geöffnet. Personalisierte Elemente werden durch die ausgewählten Testprofildaten ersetzt.

   ![](assets/lp-preview.png)

1. Wählen Sie weitere Testprofile aus, um das Rendering für jede Variante Ihrer Landingpage in der Vorschau anzuzeigen.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Landingpage veröffentlichen {#publish-landing-page}

Sobald Ihre Landingpage fertig ist, können Sie sie veröffentlichen, um sie für die Verwendung in einer Nachricht verfügbar zu machen.

Sobald Ihre Landingpage publiziert wurde, wird sie mit der **[!UICONTROL Veröffentlicht]** -Status. Es ist jetzt live und kann verwendet werden.

![](assets/lp-published.png)

Nach der Veröffentlichung können Sie die **[!UICONTROL Landingpage-URL]** , die oben auf der Seite in einem Webbrowser angezeigt wird.

Sie können die Auswirkungen Ihrer Landingpage über Protokolle und spezifische Berichte überwachen.
