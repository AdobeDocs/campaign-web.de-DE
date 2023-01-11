---
audience: end-user
title: Erkunden der Benutzeroberfläche
description: Web-Benutzeroberfläche von Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 86%

---

# Erkunden der Benutzeroberfläche {#user-interface}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Schnittstelle"
>abstract="Die neue Campaign v8-Webschnittstelle bietet ein integriertes, intuitives und konsistentes Benutzererlebnis."

Die neue Campaign v8-Webschnittstelle bietet ein modernes und intuitives Benutzererlebnis, um die Erstellung und Bereitstellung von Marketingkampagnen zu vereinfachen. Diese neue Benutzeroberfläche ist in Adobe Experience Platform integriert.

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>Die vorliegende Dokumentation wird entsprechend den neuesten Änderungen an der Benutzeroberfläche des Produkts regelmäßig aktualisiert. Manche Screenshots können jedoch geringfügig von Ihrer Benutzeroberfläche abweichen.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Linkes Navigationsmenü

Klicken Sie auf die Links auf der linken Seite, um auf die Web-Funktionen von Campaign v8 zuzugreifen. Mehrere Links zeigen Listen von Objekten an, die sortiert und gefiltert werden können. Sie können auch Spalten so konfigurieren, dass alle benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens). Alle Listenbildschirme mit Ausnahme der E-Mail-Versandliste sind schreibgeschützt. Das Klicken auf ein Listenelement zur Bearbeitung/Anzeige ist in Alpha nicht verfügbar. Alle Listen können in Beta- und GA-Versionen bearbeitet werden. Die im linken Navigationsmenü angezeigten Elemente hängen von Ihren Benutzerberechtigungen ab.

![](assets/home.png)

### Startseite

Dieser Bildschirm enthält wichtige Links und Ressourcen für einen schnellen Zugriff auf die wichtigsten Webfunktionen von Campaign v8. Die **Letzte** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt ihr jeweiliges Erstellungs- und Änderungsdatum sowie den Status

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Greifen Sie über den unteren Bereich der Startseite auf die Hilfeseiten für den Web-Schlüssel von Campaign v8 zu.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="Das **Explorer**-Menü zeigt die gleiche Ordnerhierarchie wie in der Client-Konsole an. Durchsuchen Sie alle Komponenten, Ordner und Schemata von Campaign v8. Alle Listenbildschirme mit Ausnahme der E-Mail-Versandliste sind schreibgeschützt."

Das **Explorer**-Menü zeigt die gleiche Ordnerhierarchie wie in der Client-Konsole an. Durchsuchen Sie alle Komponenten, Ordner und Schemata von Campaign v8. Alle Listenbildschirme mit Ausnahme der E-Mail-Versandliste sind schreibgeschützt.

Welche Elemente im Explorer angezeigt werden, hängt von Ihren Benutzerberechtigungen ab.

Wie bei jedem Listenbildschirm können Sie die Spalten so konfigurieren, dass alle von Ihnen benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens).

Weitere Informationen zu Campaign-Explorer finden Sie in dieser [Dokumentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/campaign-workspace/adobe-campaign-explorer.html?lang=de).
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Kampagnen-Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Kampagnen"
>abstract="Dies ist die Liste Ihrer Kampagnen. Sie können nützliche Informationen wie das Anfangsdatum/Enddatum/Datum der letzten Änderung sowie ihren Status anzeigen. Sie können die Liste nach Status oder Anfangsdatum/Enddatum filtern. Darüber hinaus stehen Kampagnenvorlagen zur Verfügung. Diese Listen sind schreibgeschützt."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Sendungen"
>abstract="Durchsuchen Sie Ihre Sendungenliste. Sie können ihren Status, das Datum der letzten Änderung sowie wichtige KPIs anzeigen. Sie können die Liste nach Status, Kontaktdatum oder Kanal filtern. Klicken Sie auf einen E-Mail-Versand, um das zugehörige Dashboard zu öffnen. Andere Elemente sind schreibgeschützt. Darüber hinaus stehen Versandvorlagen zur Verfügung."

* **Kampagnen**: Dies ist die Liste Ihrer Kampagnen. Standardmäßig können Sie nützliche Informationen wie das Anfangsdatum/Enddatum/Datum der letzten Änderung sowie ihren Status sehen. Sie können die Liste nach Status oder Anfangsdatum/Enddatum filtern. Darüber hinaus stehen Kampagnenvorlagen zur Verfügung. Diese Listen sind schreibgeschützt.

* **Sendungen**: Durchsuchen Sie Ihre Sendungenliste. Standardmäßig können Sie ihren Status, das Datum der letzten Änderung sowie wichtige KPIs sehen. Sie können die Liste nach Status, Kontaktdatum oder Kanal filtern. Klicken Sie auf einen E-Mail-Versand, um sein Dashboard zu öffnen und sich einen Überblick über die Versanddetails zu verschaffen. Sendungen über andere Kanäle sind schreibgeschützt. Versandvorlagen sind auch im schreibgeschützten Modus verfügbar. Sie können sie über die Client-Konsole bearbeiten. Weitere Informationen finden Sie in dieser [Dokumentation](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-delivery-templates/about-templates.html?lang=de).

### Kunden-Management

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Empfänger"
>abstract="Greifen Sie auf Ihre Empfängerdatenbank zu. Sie können nützliche Informationen wie die E-Mail-Adresse, den Vornamen und den Nachnamen der Empfänger anzeigen. Diese Liste ist schreibgeschützt."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="Dies ist die Liste Ihrer Audiences. Sie können den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und das Label anzeigen. Sie können die Liste nach Herkunft filtern. Diese Liste ist schreibgeschützt."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Abonnementlisten"
>abstract="Durchsuchen Sie Ihre Abonnementlisten. Sie können ihren Typ, Modus und ihre Beschriftung anzeigen. Diese Liste ist schreibgeschützt."

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Zielgruppenbestimmungs-Workflows"
>abstract="Greifen Sie auf Ihre Liste der Kampagnen-Workflows zu. Sie können den Status, das letzte/nächste Verarbeitungsdatum und die Umgebung anzeigen. Sie können die Liste nach Status, Datum der letzten Verarbeitung und Workflow-Typ filtern. Auch Workflow-Vorlagen sind verfügbar. Diese Listen sind schreibgeschützt."

* **Empfänger**: Greifen Sie auf Ihre Empfängerdatenbank zu. Standardmäßig können Sie die E-Mail-Adresse sowie den Vor- und Nachnamen sehen. Diese Liste ist schreibgeschützt.
* **Audiences**: Dies ist die Liste Ihrer Zielgruppen. Standardmäßig können Sie den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und die Kennzeichnung sehen. Sie können die Liste nach Herkunft filtern. Diese Liste ist schreibgeschützt.
* **Abonnementlisten**: Durchsuchen Sie Ihre Abonnementlisten. Standardmäßig können Sie den Typ, den Modus und die Kennzeichnung sehen. Diese Liste ist schreibgeschützt.
* **Zielgruppenbestimmungs-Workflows**: Greifen Sie auf Ihre Liste der Kampagnen-Workflows zu. Standardmäßig können Sie den Status, das letzte/nächste Verarbeitungsdatum und die Umgebung sehen. Sie können die Liste nach Status, Datum der letzten Verarbeitung und Workflow-Typ filtern. Auch Workflow-Vorlagen sind verfügbar. Diese Listen sind schreibgeschützt.

### Entscheidungs-Management

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Angebote"
>abstract="Durchsuchen Sie Ihre Liste von Interaktionsangeboten. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status und Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar. Diese Listen sind schreibgeschützt."

* **Angebote**: Durchsuchen Sie Ihre Liste von Interaktionsangeboten. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status und Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar. Diese Listen sind schreibgeschützt.

## Obere Symbolleiste

In der oberen Leiste der Benutzeroberfläche haben Sie folgende Möglichkeiten:

* Freigeben Ihres Feedbacks als Alpha-Tester
* Zwischen Organisationen und Instanzen wechseln
* zwischen Adobe Experience Cloud-Anwendungen wechseln
* auf Hilfeseiten zugreifen, den Support kontaktieren und Feedback geben. Sie können Hilfe-Artikel und Videos mithilfe des Suchfelds suchen.

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Kontextuelle Hilfe und Onboarding-Handbuch

Eine kontextuelle Hilfe ist in der Benutzeroberfläche verfügbar. Wenn verfügbar, klicken Sie auf das Symbol **?**, um Hilfeinformationen und zugehörige Dokumentations-Links anzuzeigen.

![](assets/context-help.png){width="70%" align="left"}

Darüber hinaus finden Sie eine Onboarding-Anleitung, die Ihnen bei den ersten Schritten mit Campaign v8 Web hilft. Klicken Sie auf das Symbol unten rechts, wählen Sie eines der verfügbaren schrittweisen Szenarien aus und befolgen Sie einfach die Anweisungen.

![](assets/onboarding.png){width="70%" align="left"}

## Konfigurieren von Listenbildschirmen {#list-screens}

Verschiedene Links aus dem linken Navigationsmenü, z. B. **Sendungen** oder **Kampagnen**, zeigen Listen von Objekten an. Alle Listenbildschirme sind mit Ausnahme der E-Mail-Versandliste schreibgeschützt.

Um Elemente schneller zu finden, können Sie die Suchleiste verwenden oder die Liste nach Kontextkriterien filtern.

![](assets/filter.png){width="70%" align="left"}

Listen werden in Spalten angezeigt. Sie können auch zusätzliche Informationen anzeigen, indem Sie die Spaltenkonfiguration ändern. Klicken Sie dazu auf das Symbol oben rechts in der Liste. Sie können Spalten hinzufügen oder entfernen und die Reihenfolge ändern, in der sie angezeigt werden.

![](assets/columns.png){width="70%" align="left"}

Sie können Elemente in der Liste sortieren, indem Sie auf eine beliebige Spaltenüberschrift klicken. Ein Aufwärts- oder Abwärtspfeil zeigt an, dass die Liste in dieser Spalte sortiert ist. Bei numerischen Spalten oder Datumsspalten bedeutet der Aufwärtspfeil, dass die Liste in aufsteigender Reihenfolge sortiert ist, während ein Abwärtspfeil eine absteigende Reihenfolge kennzeichnet. Bei Zeichenfolge- oder alphanumerischen Spalten werden die Werte in alphabetischer Reihenfolge aufgeführt.

<!--
## Supported browsers {#browsers}

Adobe [!DNL Journey Optimizer] interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->