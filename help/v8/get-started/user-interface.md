---
audience: end-user
title: Erkunden der Benutzeroberfläche
description: Adobe Campaign Web-Benutzeroberfläche
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: ht
source-wordcount: '1548'
ht-degree: 100%

---

# Erkunden der Benutzeroberfläche {#user-interface}

Die neue Adobe Campaign Web-Benutzeroberfläche bietet ein modernes und intuitives Anwendererlebnis, das die Gestaltung und den Versand von Marketing-Kampagnen vereinfacht. Diese Benutzeroberfläche kann mit Adobe Experience Cloud-Anwendungen und -Lösungen integriert werden.

[In diesem Artikel](connect-to-campaign.md) erfahren Sie, wie Sie eine Verbindung zu Adobe Campaign herstellen, und Sie lernen die Grundlagen der Navigation in Experience Cloud kennen.

>[!NOTE]
>
>Die vorliegende Dokumentation wird entsprechend den neuesten Änderungen an der Benutzeroberfläche des Produkts regelmäßig aktualisiert. Manche Screenshots können jedoch geringfügig von Ihrer Benutzeroberfläche abweichen.

## Campaign-Startseite {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Zuletzt ausgewertet"
>abstract="Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt den Kanal, den Status, die Besitzerin bzw. den Besitzer sowie das Erstellungs- und Änderungsdatum."

Auf der Campaign-Startseite können Sie schnell und einfach durch die wichtigsten Ressourcen, Indikatoren und Komponenten navigieren.

Im oberen Abschnitt der Startseite finden Sie Informationen zu den neuesten Updates und Funktionen des Produkts sowie einen Link zu Versionshinweisen und der ausführlichen Dokumentation. Verwenden Sie den Pfeil nach links, um durch die Funktionskarten zu blättern.

![Screenshot der Startseite mit Funktionskarten und Navigationsoptionen](assets/home.png){zoomable="yes"}

Mit dem Abschnitt **KPIs** können Sie die Effektivität Ihrer Plattform anhand gängiger KPIs überprüfen. Weitere Informationen über diese KPIs finden Sie auf [dieser Seite](../reporting/kpis.md).

Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt den Kanal, den Status, die Besitzerin bzw. den Besitzer sowie das Erstellungs- und Änderungsdatum. Klicken Sie auf den Link **Mehr anzeigen**, um weitere Sendungen zu laden.

Außerdem können Sie über den Abschnitt **Lernen** der Seite auf die wichtigsten Hilfeseiten zu Adobe Campaign Web zugreifen.

### Link „Info“ {#user-interface-about}

>[!CONTEXTUALHELP]
>id="acw_about"
>title="Seite „Info“"
>abstract="Auf der Seite „Info“ finden Sie Details zu Ihrer Adobe Campaign-Instanz."

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="Informationen zu Instanzen"
>abstract="Der Abschnitt „Instanz“ enthält wichtige Informationen zu Ihrem Konsolen-Client, einschließlich der Version und der zugehörigen Build-Nummer."

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="Informationen zum Web"
>abstract="Im Abschnitt „Web“ wird die Version der Campaign Web-Benutzeroberfläche mit dem Datum der letzten Aktualisierung angezeigt, sofern verfügbar."

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="Informationen zu installierten Paketen"
>abstract="Im Abschnitt „Installierte Pakete“ werden alle Module, Funktionen und Integrationen aufgelistet, die in Ihrer Instanz vorhanden sind."

Unten auf der Seite liefert der Link **[!UICONTROL Info]** Details zu Ihrer Adobe Campaign-Instanz. Diese Details sind schreibgeschützt.

![Screenshot mit dem Link „Info“ unten auf der Seite](assets/about-link.png){zoomable="yes"}

Der Abschnitt **Instanz** enthält wichtige Informationen zu Ihrem Konsolen-Client, einschließlich der **Version** und der zugehörigen **Build**-Nummer.

* Die **Version** bezieht sich auf die offizielle Version, die Sie verwenden.
* Der **Build** bezieht sich auf eine bestimmte Iteration dieser Version.

Sowohl die Versions- als auch die Build-Nummer sind für die Fehlerbehebung von entscheidender Bedeutung. Denn anhand dieser Informationen lässt sich bestimmen, welche Funktionen und Fehlerbehebungen in Ihrer Umgebung vorhanden sind.

Im Abschnitt **Web** wird die Version der Campaign Web-Benutzeroberfläche mit dem Datum des letzten Updates angezeigt, sofern verfügbar. So können Änderungen oder Verbesserungen an der Campaign Web-Benutzeroberfläche verfolgt werden.

Im Abschnitt **Installierte Pakete** werden alle Module, Funktionen und Integrationen aufgelistet, die in Ihrer Instanz vorhanden sind. Diese Pakete erweitern die Funktionalität von Adobe Campaign und ermöglichen es, spezielle Aufgaben durchzuführen, wie die Integration mit anderen Adobe-Lösungen oder die Aktivierung bestimmter Workflows. Angesichts der großen Anzahl von Paketen können Sie in diesem Abschnitt eine Suche durchführen und so schnell überprüfen, ob ein bestimmtes Modul in Ihrer Instanz installiert ist.

![Screenshot mit dem Abschnitt „Installierte Pakete“ samt Suchfunktion](assets/about.png){zoomable="yes"}

## Linkes Navigationsmenü {#user-interface-left-nav}

Mithilfe der Links auf der linken Seite können Sie auf die Adobe Campaign Web-Funktionen zugreifen. Mehrere Links zeigen Listen von Objekten an, die sortiert und gefiltert werden können. Sie können auch Spalten so konfigurieren, dass alle benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in diesem [Abschnitt](#list-screens). Einige Listenbildschirme sind schreibgeschützt. Welche Elemente im linken Navigationsmenü und in den Listen angezeigt werden, hängt von Ihren Benutzerberechtigungen ab. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](permissions.md).

### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="Das Menü **Explorer** zeigt alle Campaign-Komponenten und -Objekte mit derselben Ordnerhierarchie wie in der Client-Konsole an. Durchsuchen Sie alle Komponenten, Ordner und Schemata in Campaign v8, überprüfen Sie die zugehörigen Berechtigungen und erstellen Sie Ordner und Unterordner über dieses Menü."

Das Menü **Explorer** zeigt alle Campaign-Ressourcen und -Objekte mit derselben Ordnerhierarchie an wie in der Client-Konsole. Durchsuchen Sie alle Ihre Komponenten, Ordner und Schemata in Campaign v8 und erstellen Sie Sendungen, Workflows und Kampagnen. 

Welche Elemente im **Explorer** angezeigt werden, hängt von Ihren Benutzerberechtigungen ab. Wenn Sie über entsprechende Berechtigungen verfügen, können Sie auch Ordner und Unterordner hinzufügen. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](permissions.md).

Sie können Spalten konfigurieren, um die Anzeige anzupassen und so alle benötigten Informationen anzuzeigen. Weitere Informationen finden Sie in diesem [Abschnitt](#list-screens). Sie können auch Ordner und Unterordner hinzufügen, wie in [diesem Abschnitt](permissions.md#folders) ausführlich beschrieben wird.

Weitere Informationen zum Campaign-Explorer, zur Ordnerhierarchie und zu den Ressourcen finden Sie in dieser [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=de#ac-explorer-ui){target="_blank"}.

### Kampagnen-Management {#user-interface-campaign-management}

Im Abschnitt **Kampagnen-Management** haben Sie Zugriff auf Marketing-Kampagnen, Sendungen und Workflows.

* **Kampagnen**: Dies ist die Liste Ihrer Kampagnen und Kampagnenvorlagen. Standardmäßig können Sie für jede Kampagne die Datumsangaben für Start, Ende, Erstellung und letzte Änderung, den aktuellen Status und den Namen der Person anzeigen, die die Kampagne erstellt hat. Sie können die Liste nach Status, Start-/Enddatum oder Ordner filtern oder einen erweiterten Filter erstellen, um eigene Filterkriterien zu definieren. Weiterführende Informationen zu Marketing-Kampagnen finden Sie in [diesem Abschnitt](../campaigns/gs-campaigns.md).

* **Sendungen**: Durchsuchen Sie Ihre Sendungsliste. Standardmäßig können Sie den Status, das Datum der letzten Änderung sowie wichtige KPIs sehen. Sie können die Liste nach Status, Kontaktdatum oder Kanal filtern. Klicken Sie auf einen E-Mail-Versand, um sein Dashboard zu öffnen und sich einen Überblick über die Versanddetails zu verschaffen. Sendungen über andere Kanäle sind schreibgeschützt. Weitere Informationen zu Sendungen finden Sie in [diesem Abschnitt](../msg/gs-messages.md).

  Verwenden Sie die Schaltfläche **Mehr Aktionen**, um einen Versand zu löschen oder zu duplizieren.

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"} [Screenshot mit der Schaltfläche „Mehr Aktionen“ mit Optionen zum Löschen oder Duplizieren eines Versands]

* **Workflows** – Auf diesem Bildschirm können Sie auf die vollständige Liste der Workflows und Workflow-Vorlagen zugreifen. Sie können den Status und das letzte bzw. nächste Ausführungsdatum überprüfen und einen neuen Workflow oder eine neue Workflow-Vorlage erstellen. Sie können die Liste nach denselben Kriterien filtern wie für andere Objekte. Darüber hinaus können Sie Workflows filtern, die zu einer Kampagne gehören oder nicht. Weiterführende Informationen zu Workflows finden Sie [in diesem Abschnitt](../workflows/gs-workflows.md).

### Content-Management {#user-interface-content-management}

Im Abschnitt **Content-Management** können Sie Ihre Inhaltsvorlagen und -fragmente einsehen.

* **Inhaltsvorlagen**: Sie können eigenständige Vorlagen erstellen, um den Design-Prozess zu beschleunigen und zu verbessern und benutzerdefinierte Inhalte problemlos in allen Bereichen von [!DNL Adobe Campaign] wiederzuverwenden. Diese nur für E-Mails verfügbare Funktion ermöglicht es inhaltsorientierten Benutzenden, an eigenständigen Vorlagen zu arbeiten, sodass Anwenderinnen und Anwender von Marketing diese in ihren E-Mail-Kampagnen wiederverwenden und anpassen können. Weiterführende Informationen finden Sie in [diesem Abschnitt](../email/create-email-templates.md).

* **Fragmente**: Ein Fragment ist eine wiederverwendbare Komponente, die kampagnenübergreifend in einer oder mehreren Sendungen referenziert werden kann. Wenn Sie ein Fragment ändern, wird jeder Inhalt, der dieses Fragment verwendet, aktualisiert. [Erfahren Sie, wie Sie mit Fragmenten arbeiten](../content/fragments.md).

Diese Funktionalität ermöglicht es, mehrere benutzerdefinierte Inhaltsbausteine vorab zu erstellen, die anschließend von Benutzenden aus dem Marketing verwendet werden können, um E-Mail-Inhalte in einem verbesserten Design-Prozess schnell zusammenzustellen.

### Kunden-Management {#user-interface-customer-management}

Im Abschnitt **Kunden-Management** können Sie Ihre Profile, Zielgruppen und Abonnements einsehen. Diese Listen sind schreibgeschützt.

* **Profile**: Erstellen und verwalten Sie Profile, und greifen Sie auf Ihre Empfängerdatenbank zu. Standardmäßig können Sie die E-Mail-Adresse sowie den Vor- und Nachnamen sehen. Weitere Informationen zu Profile finden Sie in [diesem Abschnitt](../audience/about-recipients.md).
* **Zielgruppen**: Dies ist die Liste Ihrer Zielgruppen. Standardmäßig können Sie den Typ, die Herkunft, das Erstellungsdatum, das Datum der letzten Änderung und die Label sehen. Die Liste kann nach Herkunft gefiltert werden. Weitere Informationen zu Zielgruppen und Listen finden Sie in [diesem Abschnitt](../audience/about-recipients.md).
* **Abonnements**: Durchsuchen Sie Ihre Abonnementlisten. Standardmäßig können Sie den Typ, den Modus und die Label sehen. Weitere Informationen zur Verwaltung von Abonnements und Abmeldungen finden Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=de){target="_blank"}.
* **Vordefinierte Filter**: Vordefinierte Filter sind benutzerdefinierte Filter, die erstellt und gespeichert werden, um für eine spätere Verwendung zur Verfügung zu stehen. Sie können als Verknüpfungen bei allen Filtervorgängen mit dem Abfrage-Modeler verwendet werden, z. B. beim Filtern einer Liste von Daten oder beim Erstellen der Zielgruppe eines Versands. Weiterführende Informationen finden Sie in [diesem Abschnitt](predefined-filters.md).

### Entscheidungs-Management {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Angebote"
>abstract="Durchsuchen Sie die Listen mit Angeboten und Angebotsvorlagen, die in der Konsole erstellt wurden, mithilfe des Moduls **Interaktion**. Diese Listen sind schreibgeschützt."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=de" text="Hinzufügen von Angeboten zu einem Versand"

Im Abschnitt **Entscheidungs-Management** können Sie die Angebote und Angebotsvorlagen anzeigen. Diese Listen sind schreibgeschützt.

* **Angebote**: Durchsuchen Sie die Liste der Angebote und Angebotsvorlagen, die in der Konsole erstellt wurden, mithilfe des Moduls **Interaktion**. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status oder Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar.

Erfahren Sie, wie Sie in E-Mails und SMS Angebote erstellen und senden, in [diesem Abschnitt](../msg/offers.md).

### Reporting {#left-nav-reporting}

* **Berichte**: Der Eintrag **Bericht** bietet eine konsolidierte Zusammenfassung von Traffic- und Interaktionsmetriken für jeden Kanal innerhalb Ihrer Campaign-Umgebungen. Diese Berichte bestehen aus verschiedenen Widgets, von denen jedes eine andere Perspektive auf Ihre Kampagnen- oder Versandleistung bietet. Weiterführende Informationen finden Sie in [diesem Abschnitt](../reporting/global-reports.md).

### Administration {#left-nav-admin}

* **Audit-Protokoll**: Der Eintrag **Audit-Protokoll** bietet Benutzenden vollständige Einsicht in alle Änderungen, die an wichtigen Entitäten in der Instanz vorgenommen wurden. Dies sind typischerweise Änderungen, die den reibungslosen Betrieb der Instanz wesentlich beeinflussen. [Weitere Informationen](../reporting/audit-trail.md).

* **Externe Konten**: Erstellen Sie mithilfe der Web-Benutzeroberfläche neue externe Konten, um Ihre spezifischen Anforderungen zu erfüllen und eine nahtlose Datenübertragung sicherzustellen. [Weitere Informationen](../administration/external-account.md).

* **Schemata**: Benutzerdefinierte Felder sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zu nativen Schemata hinzugefügt werden. [Weitere Informationen](../administration/custom-fields.md).

* **Versandwarnung**: Bei Versandwarnungen handelt es sich um ein System zum Warnungs-Management, über das Benutzergruppen automatisch E-Mail-Benachrichtigungen mit Informationen zu ihren Versandausführungen erhalten.  [Weitere Informationen](../msg/delivery-alerting.md).

## Weitere Informationen {#learn-more}

Erfahren Sie [auf dieser Seite](list-filters.md), wie Sie in Ihrer Campaign-Umgebung verfügbare Listen lesen, durchsuchen und filtern können.