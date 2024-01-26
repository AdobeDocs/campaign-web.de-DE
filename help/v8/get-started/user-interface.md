---
audience: end-user
title: Erkunden der Benutzeroberfläche
description: Adobe Campaign Web-Benutzeroberfläche
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: f614919e0ad253aa4625f774e7fe102426e25807
workflow-type: tm+mt
source-wordcount: '1697'
ht-degree: 76%

---

# Erkunden der Benutzeroberfläche {#user-interface}

Die neue Adobe Campaign-Webschnittstelle bietet ein modernes und intuitives Benutzererlebnis, um die Erstellung und Bereitstellung von Marketingkampagnen zu vereinfachen. Diese neue Benutzeroberfläche ist in Adobe Experience Cloud-Apps und -Lösungen integriert.

Erfahren Sie, wie Sie eine Verbindung zu Adobe Campaign herstellen, und lernen Sie die Grundlagen der Experience Cloud-Navigation kennen. [in diesem Artikel](connect-to-campaign.md).


>[!NOTE]
>
>Die vorliegende Dokumentation wird entsprechend den neuesten Änderungen an der Benutzeroberfläche des Produkts regelmäßig aktualisiert. Manche Screenshots können jedoch geringfügig von Ihrer Benutzeroberfläche abweichen.

## Kampagnen-Startseite {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Zuletzt ausgewertet"
>abstract="Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt den Kanal, den Status, die Besitzerin bzw. den Besitzer sowie das Erstellungs- und Änderungsdatum."

Auf der Kampagnen-Startseite können Sie schnell und einfach die wichtigsten Ressourcen, Indikatoren und Komponenten durchsuchen.

Der obere Abschnitt der Startseite enthält Details zu den neuesten Updates und neuen Funktionen, die im Produkt verfügbar sind, mit einem Link zu Versionshinweisen und einer detaillierten Dokumentation. Verwenden Sie den linken Pfeil, um die Funktionskarten zu scrollen.

![](assets/home.png)

Die **wichtigen Performance-Indikatoren** ermöglichen es Ihnen, die Effektivität Ihrer Plattform mithilfe gängiger KPIs zu überprüfen. Weitere Informationen über diese KPIs finden Sie auf [dieser Seite](../reporting/kpis.md).

Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt den Kanal, den Status, die Besitzerin bzw. den Besitzer sowie das Erstellungs- und Änderungsdatum. Klicken Sie auf den Link **Mehr anzeigen**, um weitere Sendungen zu laden.

Darüber hinaus können Sie über die **Lernen** -Abschnitt der Seite.

## Linkes Navigationsmenü {#user-interface-left-nav}

Durchsuchen Sie die Links auf der linken Seite, um auf Adobe Campaign Web-Funktionen zuzugreifen. Mehrere Links zeigen Listen von Objekten an, die sortiert und gefiltert werden können. Sie können auch Spalten so konfigurieren, dass alle benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens). Einige Listenbildschirme sind schreibgeschützt. Welche Elemente im linken Navigationsmenü und in den Listen angezeigt werden, hängt von Ihren Benutzerberechtigungen ab. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](permissions.md).


### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="Das Menü **Explorer** zeigt alle Campaign-Komponenten und -Objekte mit derselben Ordnerhierarchie wie in der Client-Konsole an. Durchsuchen Sie alle Komponenten, Ordner und Schemata in Campaign v8, überprüfen Sie die zugehörigen Berechtigungen und erstellen Sie Ordner und Unterordner über dieses Menü."

Das Menü **Explorer** zeigt alle Campaign-Ressourcen und -Objekte mit derselben Ordnerhierarchie an wie in der Client-Konsole. Durchsuchen Sie alle Ihre Komponenten, Ordner und Schemata in Campaign v8 und erstellen Sie Sendungen, Workflows und Kampagnen.

Welche Elemente im **Explorer** angezeigt werden, hängt von Ihren Benutzerberechtigungen ab. Wenn Sie über entsprechende Berechtigungen verfügen, können Sie auch Ordner und Unterordner hinzufügen. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](permissions.md).

Sie können Spalten konfigurieren, um die Anzeige anzupassen und so alle benötigten Informationen anzuzeigen. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens). Sie können auch Ordner und Unterordner hinzufügen, wie in [diesem Abschnitt](permissions.md#folders) ausführlich beschrieben wird.

Weitere Informationen zum Campaign-Explorer, zur Ordnerhierarchie und zu den Ressourcen finden Sie in dieser [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=de#ac-explorer-ui){target="_blank"}.

### Kampagnen-Management {#user-interface-campaign-management}

Im Abschnitt KAMPAGNEN-MANAGEMENT haben Sie Zugriff auf Marketing-Kampagnen, Sendungen und Workflows.

* **Kampagnen** – Dies ist die Liste Ihrer Kampagnen und Kampagnenvorlagen. Standardmäßig können Sie für jede Kampagne die Datumsangaben für Start, Ende, Erstellung und letzte Änderung, den aktuellen Status und den Namen der Campaign-Benutzerin bzw. des -Benutzers anzeigen, die bzw. der die Kampagne erstellt hat. Sie können die Liste nach Status, Start-/Enddatum oder Ordner filtern oder einen erweiterten Filter erstellen, um eigene Filterkriterien zu definieren. Weiterführende Informationen zu Marketing-Kampagnen finden Sie in [diesem Abschnitt](../campaigns/gs-campaigns.md).

* **Sendungen**: Durchsuchen Sie Ihre Sendungenliste. Standardmäßig können Sie ihren Status, das Datum der letzten Änderung sowie wichtige KPIs sehen. Sie können die Liste nach Status, Kontaktdatum oder Kanal filtern. Klicken Sie auf einen E-Mail-Versand, um sein Dashboard zu öffnen und sich einen Überblick über die Versanddetails zu verschaffen. Sendungen über andere Kanäle sind schreibgeschützt. Weitere Informationen zu Sendungen finden Sie in [diesem Abschnitt](../msg/gs-messages.md).

  Verwenden Sie die Schaltfläche **Mehr Aktionen**, um einen Versand zu löschen oder zu duplizieren.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** – Auf diesem Bildschirm können Sie auf die vollständige Liste der Workflows und Workflow-Vorlagen zugreifen. Sie können den Status und das letzte bzw. nächste Ausführungsdatum überprüfen und einen neuen Workflow oder eine neue Workflow-Vorlage erstellen. Sie können die Liste nach denselben Kriterien filtern wie für andere Objekte. Darüber hinaus können Sie Workflows filtern, die zu einer Kampagne gehören oder nicht. Weiterführende Informationen zu Workflows finden Sie [in diesem Abschnitt](../workflows/gs-workflows.md).


### Content-Management {#user-interface-content-management}

Im Abschnitt CONTENT MANAGEMENT können Sie Ihre Inhaltsvorlagen und Fragmente anzeigen.

* **Inhaltsvorlagen** - Für einen beschleunigten und verbesserten Design-Prozess können Sie eigenständige Vorlagen erstellen, um benutzerdefinierte Inhalte einfach in allen [!DNL Adobe Campaign]. Diese Funktion ist nur für E-Mails verfügbar und ermöglicht inhaltsorientierten Benutzern die Arbeit an eigenständigen Vorlagen, sodass Marketing-Benutzer diese in ihren E-Mail-Kampagnen wiederverwenden und anpassen können. Weiterführende Informationen finden Sie in [diesem Abschnitt](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Kunden-Management {#user-interface-customer-management}

Im Bereich KUNDENVERWALTUNG können Sie Ihre Profile, Audiences und Abonnements anzeigen. Diese Listen sind schreibgeschützt.

* **Profile** - Erstellen und verwalten Sie Profile und greifen Sie auf Ihre Empfängerdatenbank zu. Standardmäßig können Sie die E-Mail-Adresse sowie den Vor- und Nachnamen sehen. Weitere Informationen zu Profilen finden Sie in [diesem Abschnitt](../audience/about-recipients.md).
* **Zielgruppen**: Dies ist die Liste Ihrer Zielgruppen. Standardmäßig können Sie den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und die Kennzeichnung sehen. Die Liste kann nach Herkunft gefiltert werden. Weitere Informationen zu Zielgruppen und Listen finden Sie in [diesem Abschnitt](../audience/about-recipients.md).
* **Abonnementdienste** - Durchsuchen Sie Ihre Abonnementlisten. Standardmäßig können Sie den Typ, den Modus und die Kennzeichnung sehen. Erfahren Sie mehr über die Verwaltung von Abonnements und Abmeldungen in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=de){target="_blank"}.
* **Vordefinierte Filter** - Vordefinierte Filter sind benutzerdefinierte Filter, die erstellt und gespeichert werden und für die zukünftige Verwendung verfügbar sind. Sie können bei allen Filtervorgängen mit dem Abfragemodell als Verknüpfungen verwendet werden, z. B. beim Filtern einer Datenliste oder beim Erstellen der Zielgruppe eines Versands. Weiterführende Informationen finden Sie in [diesem Abschnitt](predefined-filters.md).


### Entscheidungs-Management {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Angebote"
>abstract="Durchsuchen Sie die Listen mit Angeboten und Angebotsvorlagen, die in der Konsole erstellt wurden, mithilfe des Moduls **Interaktion**. Diese Listen sind schreibgeschützt."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=de" text="Hinzufügen von Angeboten zu einem Versand"

Im Abschnitt ENTSCHEIDUNGS-MANAGEMENT können Sie die Angebote und Angebotsvorlagen anzeigen. Diese Listen sind schreibgeschützt.

* **Angebote** – Durchsuchen Sie die Liste der Angebote und Angebotsvorlagen, die in der Konsole erstellt wurden, mithilfe des Moduls **Interaktion**. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status oder Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar.

Erfahren Sie, wie Sie in E-Mails und SMS Angebote erstellen und senden, in [diesem Abschnitt](../msg/offers.md).

### Reporting {#left-nav-reporting}

* **Berichte** - die **Bericht** -Eintrag bietet eine konsolidierte Zusammenfassung der Traffic- und Interaktionsmetriken für jeden Kanal in Ihrer Campaign-Umgebung. Diese Berichte bestehen aus verschiedenen Widgets, von denen jede einen bestimmten Blickwinkel auf Ihre Kampagnen- oder Versandleistung bietet. Weiterführende Informationen finden Sie in [diesem Abschnitt](../reporting/global-reports.md).


## Kontextuelle Hilfe {#user-interface-help}

Eine kontextuelle Hilfe ist in der Benutzeroberfläche verfügbar. Wenn verfügbar, klicken Sie auf das `?`-Symbol, um Hilfeinformationen und zugehörige Dokumentations-Links anzuzeigen.

![](assets/do-not-localize/context-help.png){width="40%" align="left"}

Aktuell als Beta-Version in der neuen Campaign-Web-Benutzeroberfläche veröffentlicht: **KI-gestützter Knowledge Assistant** eingebettet in die kontextuelle Hilfe revolutioniert die Dokumentationssuche und Beantwortung von Fragen durch mühelose Durchblättern von umfangreichen Dokumentations-Repositorys und zeigt sofort die benötigten Informationen an.

Dank der Funktionen der generativen KI von Campaign verwandelt dieser Assistent Ihr Erlebnis völlig und macht das Abrufen von Informationen und die Problembehebung zu einem Kinderspiel. Unser Wissensassistent mit generativer KI ist Ihr ultimativer Begleiter bei Fragen zu komplexen Aufgaben oder zur Navigation in umfangreichen Dokumenten und bietet Ihnen bei jeder Interaktion höchste Effizienz und Genauigkeit.

Weiterführende Informationen finden Sie in [diesem Abschnitt](using-ai.md).



## Weitere Informationen {#learn-more}

Erfahren Sie [auf dieser Seite](list-filters.md), wie Sie in Ihrer Campaign-Umgebung verfügbare Listen lesen, durchsuchen und filtern können.



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Berechtigung erforderlich"
>abstract="Ihre Admins müssen Ihnen die Berechtigung erteilen, bevor Sie ein Segment erstellen können."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Berechtigung erforderlich"
>abstract="Ihre Admins müssen Ihnen die Berechtigung erteilen, bevor Sie ein Segment erstellen können."


<!-- Waves-->


>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Waagen-Definition"
>abstract="Definieren Sie Schübe, um Sendungen in mehrere Teilsendungen zu unterteilen, anstatt große Mengen von Nachrichten gleichzeitig zu senden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Größe der Welle"
>abstract="Die Größe des Schubs ist erforderlich. Geben Sie entweder einen numerischen Wert (Anzahl Nachrichten) oder einen Prozentsatz (0-100 %) in das Feld &quot;Größe&quot;ein."



<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Senden von globalen Berichten"
>abstract="Auf diesem Bildschirm werden Tracking-Berichtsmetriken angezeigt"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Tracking globaler Berichte"
>abstract="Auf diesem Bildschirm werden Tracking-Berichtsmetriken angezeigt"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Workflow-Liste in einer Kampagne"
>abstract="Workflow-Liste in einer Kampagne"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Empfänger – Erstellung"
>abstract="Empfänger – Erstellung"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Empfängerkarte – Übersicht"
>abstract="Empfängerkarte – Übersicht"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Empfänger – Touchpoints"
>abstract="Empfänger – Touchpoints"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Empfänger – Abonnementauswahl"
>abstract="Empfänger – Abonnementauswahl"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Empfängerangebote – Liste geeigneter Angebote"
>abstract="Empfängerangebote – Liste geeigneter Angebote"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Empfängerangebote – Vorschau"
>abstract="Empfängerangebote – Vorschau"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Empfänger – Schreibgeschütztes Profil"
>abstract="Empfänger – Schreibgeschütztes Profil"


>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Landingpages"
>abstract="Landingpages"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Landingpages – Eigenschaften"
>abstract="Landingpages – Eigenschaften"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Landingpages – Seiten"
>abstract="Landingpages – Seiten"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Landingpages – Zeitplan"
>abstract="Landingpages – Zeitplan"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Landingpages – Primärseite"
>abstract="Landingpages – Primärseite"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Landingpages – Abonnement"
>abstract="Landingpages – Abonnement"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Landingpages – Aktionsaufruf"
>abstract="Landingpages – Aktionsaufruf"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Landingpages – Simulieren"
>abstract="Landingpages – Simulieren"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Aktivität nicht bearbeitbar"
>abstract="Aktivität nicht bearbeitbar"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragmente"
>abstract="Fragmente"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Fragmente – Speichern"
>abstract="Fragmente – Speichern"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Fragmente – Erstellung"
>abstract="Fragmente – Erstellung"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragmente – Eigenschaften"
>abstract="Fragmente – Eigenschaften"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Fragmente – Typ"
>abstract="Fragmente – Typ"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Fragmente – Liste"
>abstract="Fragmente – Liste"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmente – Details"
>abstract="Fragmente – Details"






>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Bedingter Inhalt – Filter speichern"
>abstract="Bedingter Inhalt – Filter speichern"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Bedingter Inhalt – Filter auswählen"
>abstract="Bedingter Inhalt – Filter auswählen"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Bedingter Inhalt in Betreffzeile"
>abstract="Bedingter Inhalt in Betreffzeile"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Bedingter Inhalt – Betreffzeilenbedingung"
>abstract="Bedingter Inhalt – Betreffzeilenbedingung"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Testprofile simulieren"
>abstract="Testprofile simulieren"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Testprofile simulieren – Auswahl"
>abstract="Testprofile simulieren – Auswahl"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Testprofile simulieren – Versand"
>abstract="Testprofile simulieren – Versand"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="E-Mail-Protokoll simulieren"
>abstract="E-Mail-Protokoll simulieren"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Inhalt für Briefpost"
>abstract="Inhalt für Briefpost"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Dateieigenschaften für Briefpost"
>abstract="Dateieigenschaften für Briefpost"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Inhaltseigenschaften für Briefpost"
>abstract="Inhaltseigenschaften für Briefpost"


<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Anzeigen von erweiterten Attributen"
>abstract="In der Attributliste werden standardmäßig nur die häufigsten Attribute angezeigt. Aktivieren Sie den Umschalter **Erweiterte Attribute anzeigen**, um alle verfügbaren Attribute für die aktuelle Liste in der linken Palette des Regel-Builders anzuzeigen, z. B. Knoten, Gruppierungen, 1:1-Links und 1:n-Links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Erweiterte Felder des Regel-Builders"
>abstract="In der Attributliste werden standardmäßig nur die häufigsten Attribute angezeigt. Aktivieren Sie den Umschalter **Erweiterte Attribute anzeigen**, um alle verfügbaren Attribute für die aktuelle Liste in der linken Palette des Regel-Builders anzuzeigen, z. B. Knoten, Gruppierungen, 1:1-Links und 1:n-Links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Erweiterte Attribute des Regel-Builders"
>abstract="In der Attributliste werden standardmäßig nur die häufigsten Attribute angezeigt. Aktivieren Sie den Umschalter **Erweiterte Attribute anzeigen**, um alle verfügbaren Attribute für die aktuelle Liste in der linken Palette des Regel-Builders anzuzeigen, z. B. Knoten, Gruppierungen, 1:1-Links und 1:n-Links."



>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="Diese Vorlage ist nur bereit"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Alle Teilmengen in derselben Tabelle erzeugen"
>abstract="TBC"
