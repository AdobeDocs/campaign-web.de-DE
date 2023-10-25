---
audience: end-user
title: Erkunden der Benutzeroberfläche
description: Web-Benutzeroberfläche von Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: 233f5b045256bf22df4debef8b2bfe375880fa3e
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 90%

---

# Erkunden der Benutzeroberfläche {#user-interface}

Die neue Web-Oberfläche von Campaign v8 bietet ein modernes und intuitives Benutzererlebnis, das die Gestaltung und den Versand von Marketing-Kampagnen vereinfacht. Diese neue Benutzeroberfläche ist in Adobe Experience Cloud-Apps und -Lösungen integriert.


>[!NOTE]
>
>Die vorliegende Dokumentation wird entsprechend den neuesten Änderungen an der Benutzeroberfläche des Produkts regelmäßig aktualisiert. Manche Screenshots können jedoch geringfügig von Ihrer Benutzeroberfläche abweichen.


## Linkes Navigationsmenü {#user-interface-left-nav}

Mithilfe der Links auf der linken Seite können Sie auf die Campaign v8 Web-Funktionen zugreifen. Mehrere Links zeigen Listen von Objekten an, die sortiert und gefiltert werden können. Sie können auch Spalten so konfigurieren, dass alle benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens). Einige Listenbildschirme sind schreibgeschützt. Welche Elemente im linken Navigationsmenü und in den Listen angezeigt werden, hängt von Ihren Benutzerberechtigungen ab. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](permissions.md).

![](assets/home.png)

### Startseite {#user-interface-home}

Dieser Bildschirm enthält wichtige Links und Ressourcen für den Schnellzugriff auf die wichtigsten Campaign v8 Web-Funktionen.

Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt den Kanal, den Status, die Besitzerin bzw. den Besitzer sowie das Erstellungs- und Änderungsdatum.

Die **wichtigen Leistungsindikatoren** ermöglichen es Ihnen, die Effektivität Ihrer Plattform mithilfe gängiger KPIs zu überprüfen. Weitere Informationen über diese KPIs finden Sie auf [dieser Seite](../reporting/kpis.md).

Greifen Sie über den Abschnitt **Lernen** auf der Startseite auf die wichtigsten Hilfeseiten von Campaign v8 Web zu.

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


### Kunden-Management {#user-interface-customer-management}

Im Abschnitt KUNDEN-MANAGEMENT können Sie Ihre Empfängerinnen und Empfänger, Zielgruppen und Abonnements anzeigen. Diese Listen sind schreibgeschützt.

* **Empfänger**: Greifen Sie auf Ihre Empfängerdatenbank zu. Standardmäßig können Sie die E-Mail-Adresse sowie den Vor- und Nachnamen sehen. Weitere Informationen zu Empfängerinnen und Empfängern finden Sie in [diesem Abschnitt](../audience/about-recipients.md).
* **Zielgruppen**: Dies ist die Liste Ihrer Zielgruppen. Standardmäßig können Sie den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und die Kennzeichnung sehen. Die Liste kann nach Herkunft gefiltert werden. Weitere Informationen zu Zielgruppen und Listen finden Sie in [diesem Abschnitt](../audience/about-recipients.md).
* **Abonnements**: Durchsuchen Sie Ihre Abonnements. Standardmäßig können Sie den Typ, den Modus und die Kennzeichnung sehen. Erfahren Sie mehr über die Verwaltung von Abonnements und Abmeldungen in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=de){target="_blank"}.

### Entscheidungs-Management {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Angebote"
>abstract="Durchsuchen Sie die Listen mit Angeboten und Angebotsvorlagen, die in der Konsole erstellt wurden, mithilfe des Moduls **Interaktion**. Diese Listen sind schreibgeschützt."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=de" text="Hinzufügen von Angeboten zu einem Versand"

Im Abschnitt ENTSCHEIDUNGS-MANAGEMENT können Sie die Angebote und Angebotsvorlagen anzeigen. Diese Listen sind schreibgeschützt.

* **Angebote** – Durchsuchen Sie die Liste der Angebote und Angebotsvorlagen, die in der Konsole erstellt wurden, mithilfe des Moduls **Interaktion**. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status oder Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar.

Erfahren Sie, wie Sie in E-Mails und SMS Angebote erstellen und senden, in [diesem Abschnitt](../content/offers.md).



## Kontextuelle Hilfe {#user-interface-help}

Eine kontextuelle Hilfe ist in der Benutzeroberfläche verfügbar. Wenn verfügbar, klicken Sie auf das `?`-Symbol, um Hilfeinformationen und zugehörige Dokumentations-Links anzuzeigen.

![](assets/context-help.png){width="40%" align="left"}

In der neuen Beta-Version revolutioniert der **Wissensassistent mit generativer KI**, der in der kontextuellen Hilfe eingebettet ist, das Suchen in der Dokumentation und das Beantworten von Fragen zu Problemlösungen, indem er mühelos riesige Dokumentations-Repositorys durchkämmt und sofort die Informationen anzeigt, die Sie benötigen.

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
>title="Empfängererstellung"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Empfängerdetails"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Kontaktinformationen der Empfänger"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Empfängeradresse"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Empfängerkonto"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Benutzerdefinierte Felder für Empfänger"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Übersicht über die Empfängerkarte"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Touchpoints der Empfänger"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Abonnementliste der Empfänger"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Auswahl der Empfänger-Abonnements"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Empfängerangebote auf der Liste"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Vorschau der Angebote für Empfänger"
>abstract="TBC"





>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Vorlage für den Abonnement-Versand"
>abstract="TBC"





>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Landingpages"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Eigenschaften von Landingpages"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Landingpages"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Landingpage-Zeitplan"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Landing Pages primary page"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Landingpage-Abonnement"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Landingpage-Aktionsaufruf"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Landingpage-Simulation"
>abstract="TBC"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Aktivität nicht bearbeitbar"
>abstract="TBC"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragmente"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Fragmente speichern"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Fragmenterstellung"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Fragmenteigenschaften"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Fragmenttyp"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Fragmentliste"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentdetails"
>abstract="TBC"




>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Inhaltsvorlage"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Eigenschaften der Inhaltsvorlage"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Entwurf von Inhaltsvorlagen"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Auswahl der Inhaltsvorlagen"
>abstract="TBC"






>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Datei laden  Aktivität"
>abstract="TBC"






>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Aktivität &quot;Abstimmung&quot;"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Abstimmung der Zielgruppe"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Abstimmregeln"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Zielgruppendimension der Abstimmung"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Abstimmungsauswahlfeld"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Attribut zur Abstimmauswahl"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Bedingung zur Erstellung der Abstimmung"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Komplement abstimmen"
>abstract="TBC"





>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Filter zum Speichern bedingter Inhalte"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Filter zur Auswahl bedingter Inhalte"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Bedingter Inhalt in der Betreffzeile"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Bedingung der Subjektlinie für bedingten Inhalt"
>abstract="TBC"

