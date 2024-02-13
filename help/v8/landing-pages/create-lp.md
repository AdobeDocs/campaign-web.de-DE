---
title: Erstellen einer Landingpage
description: Hier erfahren Sie, wie Sie in Campaign Web eine Landingpage konfigurieren und veröffentlichen können.
feature: Landing Pages
source-git-commit: 26c41105a4c04b72e0aedf05a4b3268b0e475d40
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 42%

---

# Erstellen und Veröffentlichen von Landingpages {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Erstellen und Verwalten von Landingpages"
>abstract="Mit Adobe Campaign können Sie Landingpages erstellen, entwerfen und freigeben, um Ihre Benutzer auf Online-Webseiten weiterzuleiten, auf denen Sie anhand integrierter Vorlagen Nutzungsszenarios für Akquise, Abonnement/Abmeldung und Blockierungsliste verwalten können."

Über die Campaign-Webbenutzeroberfläche können Sie Landingpages erstellen, entwerfen und veröffentlichen. Nach der Veröffentlichung können Sie einen Link zu Ihrem Formular in einen Versand einfügen. Nachdem die Empfänger auf diesen Link geklickt haben, werden sie zur entsprechenden Landingpage weitergeleitet.

[!DNL Adobe Campaign] enthält vier Vorlagen zur Verwaltung der folgenden Anwendungsfälle: **Akquise**, **Abonnement**, **Abmeldung**, und **Blockierungsliste**.

## Zugreifen auf Landingpages {#access-landing-pages}

Um auf die Liste der Landingpages zuzugreifen, wählen Sie **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Landingpages]** über das Menü links aus.

![](assets/lp-inventory.png){zoomable=&quot;yes&quot;}

Das Inventar der **[!UICONTROL Landingpages]** zeigt alle erstellten Elemente an. Sie können sie mithilfe der Schaltfläche **Filter anzeigen** filtern. Sie können die Ergebnisse über die Dropdown-Liste auf einen bestimmten [Ordner](../get-started/permissions.md#folders) beschränken oder mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) Regeln hinzufügen.

![](assets/lp-inventory-filter.png){zoomable=&quot;yes&quot;}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Landingpages, die über die Clientkonsole (Webformulare) in der Campaign-Webbenutzeroberfläche erstellt wurden, können nicht angezeigt oder bearbeitet werden. Weitere Informationen finden Sie in der [Dokumentation zur Campaign-Konsole](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=de){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Sie können eine Landingpage duplizieren oder löschen. Klicken Sie auf das Auslassungszeichen neben einer Landingpage, um die gewünschte Aktion auszuwählen.

## Erstellen einer Landingpage {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definieren der Eigenschaften der Landingpage"
>abstract="Füllen Sie die Eigenschaftenfelder wie den Titel aus und ändern Sie bei Bedarf das Schema. Darüber hinaus können Sie den internen Namen bearbeiten, den Ordner ändern, in dem die Landingpage gespeichert ist, und eine Beschreibung angeben."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Inhalt der einzelnen Seiten definieren"
>abstract="Passen Sie den Inhalt jeder Seite an, die Teil dieser Landingpage ist, z. B. das Formular selbst, die Bestätigungsseite, die beim Senden des Formulars angezeigt wird, oder die Seite, auf die Benutzer im Falle eines Fehlers weitergeleitet werden."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Zeitliches Planen der Landingpage"
>abstract="Sie können ein Start- und ein Enddatum für Ihre Landingpage definieren. Wenn die Seite das Ende des Gültigkeitszeitraums erreicht, ist das Formular nicht mehr verfügbar. Die **Ablauf** -Seite angezeigt."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definieren der primären Seiteneinstellungen"
>abstract="Die primäre Seite wird den Benutzenden sofort angezeigt, nachdem sie auf den Link zu Ihrer Landingpage geklickt haben, z. B. über eine E-Mail oder eine Website."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Festlegen der Anmelde-Landingpage"
>abstract="Über eine Anmeldeseite können Ihre Kundinnen und Kunden einen Dienst abonnieren."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

Gehen Sie wie folgt vor, um eine Landingpage zu erstellen:

1. Klicken Sie im Inventar der **[!UICONTROL Landingpages]** auf **[!UICONTROL Landingpage erstellen]**.

   ![](assets/lp-create-button.png){zoomable=&quot;yes&quot;}

1. Wählen Sie eine Vorlage aus:
   * **[!UICONTROL Akquise]**: Dies ist die Standardvorlage für Landingpages, mit der Sie Profildaten erfassen und aktualisieren können.
   * **[!UICONTROL Abonnement]**: Verwenden Sie diese Vorlage, damit Benutzer sich für eine bestimmte [service](../audience/manage-services.md).
   * **[!UICONTROL Abmeldung]**: Diese Vorlage kann in einem Versand verwendet werden, der an Abonnenten eines Dienstes gesendet wird, damit sie sich von dieser Abmeldung abmelden können. [service](../audience/manage-services.md).
   * **[!UICONTROL Blockierungsliste]**: Diese Vorlage sollte verwendet werden, wenn ein Profil in einem Versand auf einen Abmelde-Link klickt und nicht mehr kontaktiert werden möchte.

   ![](assets/lp-templates.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Erfahren Sie, wie Sie die verschiedenen Anwendungsfälle für jede Vorlage implementieren können in [diese Seite](lp-use-cases.md).

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Füllen Sie die **[!UICONTROL Eigenschaften]** -Felder, z. B. die Beschriftung.

   Standardmäßig werden Landingpages im Ordner **[!UICONTROL Web-Anwendungen]** gespeichert. Sie können dies ändern, indem Sie unter **[!UICONTROL Zusätzliche Optionen]** zum gewünschten Speicherort wechseln. [Erfahren Sie mehr über die Arbeit mit Ordnern](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png){zoomable=&quot;yes&quot;}

1. Im Abschnitt **[!UICONTROL Datenvorbereitung]** sind die beiden folgenden Optionen standardmäßig ausgewählt:

   * Wenn die Variable **[!UICONTROL Vorausfüllen mit den im Formular referenzierten Daten]** aktiviert ist, werden die Profilinformationen automatisch im Formular vorausgefüllt, wenn der Besucher der Landingpage mit einem Profil aus der Datenbank übereinstimmt. Der Benutzer muss nur die fehlenden Felder ausfüllen und bei Bedarf die vorhandenen Werte aktualisieren. Auf diese Weise können Daten für vorhandene Profile zusammengeführt werden, anstatt Duplikate zu erstellen.

   * Wenn Sie keine Profile aktualisieren möchten, muss die Option **[!UICONTROL Bei nicht angegebener Identifizierung vorausgefüllte Informationen ignorieren]** ausgewählt werden. In diesem Fall wird jedes eingegebene Profil nach Genehmigung des Formulars der Datenbank hinzugefügt. Diese Option wird beispielsweise verwendet, wenn das Formular auf einer Website veröffentlicht wird.

1. Eine Landingpage kann über nachfolgende Seiten verfügen. Um Seiten hinzuzufügen, durchsuchen Sie die **[!UICONTROL Seiten]** und klicken Sie auf das **[!UICONTROL Inhalt bearbeiten]** für jede Seite, die Sie für diese Landingpage erstellen möchten. Der Inhalt jeder Seite ist bereits vorausgefüllt. Bearbeiten Sie ihn nach Bedarf. [Weitere Informationen](lp-content.md)

   ![](assets/lp-pages.png){zoomable=&quot;yes&quot;}

1. Die **[!UICONTROL Vorausgefüllten Datensatz aktualisieren]** ist standardmäßig aktiviert. Dadurch können die in der Datenbank gespeicherten Profile über die Landingpage aktualisiert werden. Im Feld Vorausfüllen können Sie angeben, wie der zu aktualisierende Datensatz in der Datenbank gefunden werden soll.

   Sie können auch aus den Feldern wählen, die im aktuellen Kontext der Landingpage verwendet werden, um das entsprechende Profil in der Datenbank zu finden. Heben Sie dazu die Auswahl der **[!UICONTROL Vorausgefüllten Datensatz aktualisieren]** und aktivieren Sie die gewünschten Felder unter **[!UICONTROL Abstimmoptionen]**.

   ![](assets/lp-storage.png){zoomable=&quot;yes&quot;}

1. Sie können ein Start- und ein Enddatum für Ihre Landingpage definieren. Auswählen **[!UICONTROL Aktivieren der Planung]** und legen Sie die Daten fest.

   ![](assets/lp-schedule.png){zoomable=&quot;yes&quot;}

   * Die Landingpage wird automatisch am angegebenen Startdatum/zur festgelegten Startzeit veröffentlicht.

     >[!NOTE]
     >
     >Wenn kein Startdatum definiert ist, wird die Landingpage sofort nach der Veröffentlichung live geschaltet.

   * Wenn die Seite das Enddatum erreicht, <!--the landing page is automatically unpublished and -->das Formular nicht mehr verfügbar ist. Die **[!UICONTROL Ablauf]** -Seite angezeigt.

     >[!NOTE]
     >
     >Aus Sicherheitsgründen und aus Gründen der Plattformleistung empfiehlt Adobe, ein Enddatum festzulegen.

1. Klicken Sie auf **[!UICONTROL Überprüfen und veröffentlichen]**.

Nachdem Sie alle Einstellungen und [entworfen](lp-content.md) alle Seiten, können Sie [test](#test-landing-page) und [publish](#publish-landing-page) Ihre Landingpage wie unten beschrieben.

## Testen der Landingpage {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulation der Landingpage"
>abstract="Sie können eine Vorschau Ihrer Landingpage in der Campaign Web-Benutzeroberfläche anzeigen oder sie in einer neuen Registerkarte des Webbrowsers öffnen."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Erstellen einer Vorschau und Testen der Landingpage"
>abstract="Nachdem Sie die Einstellungen und den Inhalt Ihrer Landingpage definiert haben, können Sie sie mit Testprofilen in der Vorschau anzeigen."

Nachdem Sie die Einstellungen und den Inhalt Ihrer Landingpage definiert haben, können Sie sie mit Testprofilen in der Vorschau anzeigen. Bei Verwendung von [personalisierten Inhalten](../personalization/gs-personalization.md) können Sie prüfen, wie diese Inhalte auf der Landingpage angezeigt werden, und dabei Daten von Testprofilen nutzen.

>[!CAUTION]
>
>Um Ihre Nachrichten in der Vorschau darzustellen und einen Testversand durchzuführen, benötigen Sie verfügbare Testprofile. [Erfahren Sie mehr über Testprofile](../audience/test-profiles.md)

Gehen Sie wie folgt vor, um Ihre Landingpage zu testen:

1. Nachdem Sie auf **[!UICONTROL Überprüfen und veröffentlichen]**, wählen Sie die **[!UICONTROL Inhalt simulieren]** -Schaltfläche im Landingpage-Dashboard, um auf die Testprofilauswahl zuzugreifen.

   ![](assets/lp-simulate-content.png){zoomable=&quot;yes&quot;}

1. Wählen Sie auf dem Bildschirm **[!UICONTROL Simulieren]** ein oder mehrere Testprofile aus.

   Die Schritte zum Auswählen von Testprofilen sind mit denen beim Testen einer Nachricht identisch. Sie werden im Abschnitt [Vorschau und Testen](../preview-test/preview-test.md) beschrieben.

1. Wählen Sie **[!UICONTROL Vorschau öffnen]** aus, um Ihre Landingpage zu testen.

   ![](assets/lp-open-preview.png){zoomable=&quot;yes&quot;}

1. Die Vorschau Ihrer Landingpage wird in einer neuen Registerkarte geöffnet. Personalisierte Elemente werden durch die ausgewählten Testprofildaten ersetzt.

   Wenn Sie die Option **[!UICONTROL Vorausfüllen mit den im Formular referenzierten Daten]** in den Landingpage-Einstellungen automatisch die entsprechenden Testprofildaten in die Formularfelder eingefügt.<!--TBC-->

   ![](assets/lp-preview.png){zoomable=&quot;yes&quot;}

1. Wählen Sie weitere Testprofile aus, um das Rendering für jede Variante Ihrer Landingpage in der Vorschau anzuzeigen.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Veröffentlichen der Landingpage {#publish-landing-page}

Sobald Ihre Landingpage fertig und validiert ist, veröffentlichen Sie sie mit der entsprechenden Schaltfläche, um sie für einen Versand verfügbar zu machen.

Nach der Veröffentlichung:

* Die Landingpage wird der Landingpage-Liste mit dem **[!UICONTROL Veröffentlicht]** -Status. Es ist jetzt live und kann in Ihren Inhalten referenziert werden.

* Sie können die **[!UICONTROL Landingpage-URL]** die oben auf der Seite in einem Webbrowser angezeigt wird, um eine Vorschau Ihrer Landingpage anzuzeigen.

>[!CAUTION]
>
>Um Ihre Landingpage vollständig zu testen oder zu nutzen, können Sie diesen Link nicht direkt in einen Webbrowser oder in Ihre Sendungen kopieren und einfügen. Verwenden Sie stattdessen die [Inhalt simulieren](#test-landing-page) , um sie zu testen, und führen Sie die Schritte unter [diesem Abschnitt](lp-use-cases.md) , um Ihre Landingpage richtig zu nutzen.

![](assets/lp-published.png){zoomable=&quot;yes&quot;}

Sie können die Auswirkungen Ihrer Landingpage über Protokolle überwachen<!--and specific reports-->. Klicken Sie auf **[!UICONTROL Protokolle]** Schaltfläche.
