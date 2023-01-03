---
audience: end-user
title: Entdecken Sie die Benutzeroberfläche
description: Web-Benutzeroberfläche von Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 15ee9ea467f9243834374cfe1a3e411f929c2a77
workflow-type: ht
source-wordcount: '717'
ht-degree: 100%

---

# Entdecken Sie die Benutzeroberfläche {#user-interface}

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Schnittstelle"
>abstract="TBC"

Die neue Web-Benutzeroberfläche von Campaign v8 bietet ein integriertes, intuitives und konsistentes Benutzererlebnis.

Die wichtigsten Konzepte beim Durchsuchen der Benutzeroberfläche sind mit denen von Adobe Experience Platform identisch. Weitere Informationen finden Sie in der [Dokumentation zu Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html?lang=de#adobe-experience-platform-ui-guide).

>[!NOTE]
>
>Die vorliegende Dokumentation wird entsprechend den neuesten Änderungen an der Benutzeroberfläche des Produkts regelmäßig aktualisiert. Manche Screenshots können jedoch geringfügig von Ihrer Benutzeroberfläche abweichen.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Linkes Navigationsmenü

Mithilfe der Links auf der linken Seite können Sie auf die Web-Funktionen von Campaign v8 zuzugreifen.

![](assets/home.png)

### Startseite

Die Web-Startseite von Campaign v8 enthält wichtige Links und Ressourcen, mit denen Sie starten können. Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten Sendungen. Diese Liste zeigt ihr jeweiliges Erstellungs- und Änderungsdatum sowie den Status

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Rufen Sie wichtige Hilfeseiten zu Campaign v8 Web über den unteren Abschnitt der Startseite auf.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="TBC"

Das **Explorer**-Menü zeigt die gleiche Ordnerhierarchie wie in der Client-Konsole an. Durchsuchen Sie alle Komponenten, Ordner und Schemata von Campaign v8. Alle Listenbildschirme mit Ausnahme der E-Mail-Versandliste sind schreibgeschützt.

Welche Elemente im Explorer angezeigt werden, hängt von Ihren Benutzerberechtigungen ab.

Wie bei jedem Listenbildschirm können Sie die Spalten so konfigurieren, dass alle benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens).
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Kampagnen-Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Kampagnen"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Sendungen"
>abstract="TBC"

* **Kampagnen**: Dies ist die Liste Ihrer Kampagnen. Sie können nützliche Informationen wie das Anfangsdatum/Enddatum/Datum der letzten Änderung sowie ihren Status anzeigen. Sie können die Liste nach Status oder Anfangsdatum/Enddatum filtern. Darüber hinaus stehen Kampagnenvorlagen zur Verfügung. Diese Listen sind schreibgeschützt.

* **Sendungen**: Durchsuchen Sie Ihre Versandliste. Sie können ihren Status, das Datum der letzten Änderung sowie wichtige KPIs anzeigen. Sie können die Liste nach Status, Kontaktdatum oder Kanal filtern. Klicken Sie auf einen E-Mail-Versand, um das zugehörige Dashboard zu öffnen. Andere Elemente sind schreibgeschützt. Darüber hinaus stehen Versandvorlagen zur Verfügung.

### Kunden-Management

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Empfänger"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Abonnementlisten"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Zielgruppenbestimmungs-Workflows"
>abstract="TBC"

* **Empfänger**: Greifen Sie auf Ihre Empfängerdatenbank zu. Sie können nützliche Informationen wie die E-Mail-Adresse, den Vornamen und den Nachnamen der Empfänger anzeigen. Diese Liste ist schreibgeschützt.
* **Audiences**: Dies ist die Liste Ihrer Zielgruppen. Sie können den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und das Label anzeigen. Sie können die Liste nach Herkunft filtern. Diese Liste ist schreibgeschützt.
* **Abonnementlisten**: Durchsuchen Sie Ihre Abonnementlisten. Sie können ihren Typ, Modus und ihre Beschriftung anzeigen. Diese Liste ist schreibgeschützt.
* **Zielgruppenbestimmungs-Workflows**: Greifen Sie auf Ihre Liste der Kampagnen-Workflows zu. Sie können den Status, das letzte/nächste Verarbeitungsdatum und die Umgebung anzeigen. Sie können die Liste nach Status, Datum der letzten Verarbeitung und Workflow-Typ filtern. Auch Workflow-Vorlagen sind verfügbar. Diese Listen sind schreibgeschützt.

### Entscheidungs-Management

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Angebote"
>abstract="TBC"

* **Angebote**: Durchsuchen Sie Ihre Liste von Interaktions-Angeboten. Sie können ihren Status, ihr Start-/Enddatum und die Umgebung anzeigen. Sie können die Liste nach Status und Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar. Diese Listen sind schreibgeschützt.

## Unified Shell

Campaign v8 Web ist in Unified Shell integriert. In der oberen Leiste auf der rechten Seite sind mehrere Schaltflächen verfügbar.

![](assets/unified-shell.png){width="70%" align="left"}

Mit diesen Schaltflächen können Sie:

* Ihr Feedback als Alpha-Kunde teilen
* zwischen IMS-Organisationen wechseln
* zwischen Adobe Experience Cloud-Anwendungen wechseln
* auf Hilfeseiten zugreifen, den Support kontaktieren und Feedback geben. Sie können Hilfe-Artikel und Videos mithilfe des Suchfelds suchen.

<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Kontextuelle Hilfe und Onboarding-Handbuch

Eine kontextuelle Hilfe ist in der Benutzeroberfläche verfügbar. Wenn verfügbar, klicken Sie auf das Symbol **?**, um Hilfeinformationen und zugehörige Dokumentations-Links anzuzeigen.

![](assets/context-help.png){width="70%" align="left"}

Darüber hinaus finden Sie ein Onboarding-Handbuch, das Ihnen bei den ersten Schritten mit dem Campaign v8 Web hilft. Klicken Sie auf das Symbol unten rechts, wählen Sie eines der verfügbaren schrittweisen Szenarien aus und befolgen Sie einfach die Anweisungen.

![](assets/onboarding.png){width="70%" align="left"}

## Konfigurieren von Listenbildschirmen {#list-screens}

Alle Listenbildschirme mit Ausnahme der E-Mail-Versandliste sind schreibgeschützt.

Um Elemente schneller zu finden, können Sie die Suchleiste verwenden oder die Liste nach Kontextkriterien filtern.

![](assets/filter.png){width="70%" align="left"}

Listen werden in Spalten angezeigt. Jede Spalte kann in auf- oder absteigender Reihenfolge einzeln sortiert werden. Sie können auch zusätzliche Informationen anzeigen, indem Sie die Spaltenkonfiguration ändern. Klicken Sie dazu auf das Symbol oben rechts in der Liste. Sie können Spalten hinzufügen oder entfernen und die Reihenfolge ändern, in der sie angezeigt werden.

![](assets/columns.png){width="70%" align="left"}

<!--
## Supported browsers {#browsers}

Adobe [!DNL Journey Optimizer] interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->