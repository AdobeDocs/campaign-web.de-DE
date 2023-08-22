---
audience: end-user
title: Erkunden der Benutzeroberfläche
description: Web-Benutzeroberfläche von Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha"
source-git-commit: 25cae1698334403e18f6dbede90b3c50b270d30b
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 73%

---

# Erkunden der Benutzeroberfläche {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Erkunden der Benutzeroberfläche"
>abstract="Die neue Web-Benutzeroberfläche von Campaign v8 bietet ein integriertes, intuitives und konsistentes Anwendererlebnis."

Die neue Web-Oberfläche von Campaign v8 bietet ein modernes und intuitives Benutzererlebnis, das die Gestaltung und den Versand von Marketing-Kampagnen vereinfacht. Diese neue Benutzeroberfläche ist in Adobe Experience Platform integriert.


>[!NOTE]
>
>Die vorliegende Dokumentation wird entsprechend den neuesten Änderungen an der Benutzeroberfläche des Produkts regelmäßig aktualisiert. Manche Screenshots können jedoch geringfügig von Ihrer Benutzeroberfläche abweichen.


## Linkes Navigationsmenü {#user-interface-left-nav}

Mithilfe der Links auf der linken Seite können Sie auf die Campaign v8 Web-Funktionen zugreifen. Mehrere Links zeigen Listen von Objekten an, die sortiert und gefiltert werden können. Sie können auch Spalten so konfigurieren, dass alle benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens). Alle Listenbildschirme mit Ausnahme der E-Mail-Sendungsliste sind schreibgeschützt. Das Klicken auf ein Listenelement zur Bearbeitung/Anzeige ist in Alpha nicht verfügbar. In künftigen Versionen werden alle Listen bearbeitbar sein. Welche Elemente im linken Navigationsmenü angezeigt werden, hängt von Ihren Benutzerberechtigungen ab.

![](assets/home.png)

### Startseite {#user-interface-home}

Dieser Bildschirm enthält wichtige Links und Ressourcen für den Schnellzugriff auf die wichtigsten Campaign v8 Web-Funktionen.

Die Liste **Zuletzt ausgewertet** enthält Verknüpfungen zu den kürzlich erstellten und geänderten Sendungen. Diese Liste zeigt den Kanal, den Status, die Besitzerin bzw. den Besitzer sowie das Erstellungs- und Änderungsdatum.

Greifen Sie über den Abschnitt **Lernen** auf der Startseite auf die wichtigsten Hilfeseiten von Campaign v8 Web zu.


#### KPI {#user-interface-key-indicators}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Spam-KPI"

Navigieren Sie zur Startseite, um die wichtigsten Leistungsindikatoren für Ihre Plattform zu überprüfen. Diese Indikatoren zeigen die Anzahl und den Prozentsatz der zugestellten, geöffneten, angeklickten, abgemeldeten und fehlerhaften Nachrichten sowie deren Fehlerraten an.

Die Metriken werden standardmäßig für die Sendungen der letzten sieben Tage berechnet. Sie können den Zeitraum in der Dropdown-Liste oben rechts auf der Karte ändern. Nachrichten, die an Testprofile gesendet werden, sind ausgeschlossen.

Sie können den anzuzeigenden Kanal auswählen. Standardmäßig beziehen sich diese Indikatoren auf Metriken für den E-Mail-Kanal.

![](assets/kpi.png)

#### Nachrichtenzustellung {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Zugestellt"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller erfolgreich verarbeiteten Nachrichten und den Prozentsatz der erfolgreich zugestellten Nachrichten in Bezug auf die Gesamtzahl der gesendeten Nachrichten an."


Die **Zugestellt** zeigt die folgenden KPIs für jeden Kanal an:

* Prozentualer Anteil der erfolgreich zugestellten Nachrichten in Bezug auf die Gesamtzahl der zu sendenden Nachrichten.

* Summe aller erfolgreich verarbeiteten Nachrichten.

In Adobe Campaign lautet die Regel zum Markieren einer Nachricht als &quot;Zugestellt&quot;:

Zählung aller Nachrichten mit Feld &quot;Testadresse&quot; gleich &quot;Nein&quot; und Status &quot;Vom Dienstleister berücksichtigt&quot;(für SMS) oder &quot;Gesendet&quot;(für E-Mails) oder &quot;Auf Mobiltelefon erhalten&quot;(für Push-Benachrichtigungen).


#### Öffnungen gesamt {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Öffnungen"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller geöffneten Nachrichten und den Prozentsatz der geöffneten Nachrichten im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Die **Öffnungen** zeigt die folgenden KPIs für jeden Kanal an:

* Prozentualer Anteil der geöffneten Nachrichten in Bezug auf die Gesamtzahl der erfolgreich zugestellten Nachrichten.

* Summe aller geöffneten Nachrichten pro Kanal.

Adobe Campaign erkennt das Öffnen einer Nachricht, wenn der Empfänger die Bilder in der E-Mail herunterlädt. HTML und Multipart/Alternative E-Mails enthalten ein 0-Pixel-Bild, mit dem Sie geöffnete Nachrichten erkennen können. Da Nachrichten im Textformat keine Bilder enthalten, ist es nicht möglich festzustellen, ob sie geöffnet wurden oder nicht. Die auf der Basis von Öffnungen berechneten Werte sind immer nur Schätzungen. Dies hängt mit der mit der Bildanzeige verbundenen Fehlerspanne zusammen.

#### Klickraten {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Klicks"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller in Nachrichten angeklickten URLs und den Prozentsatz der Klicks in Bezug auf die Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Die **Klicks** zeigt die folgenden KPIs für jeden Kanal an:

* Prozentualer Anteil der Klicks in Bezug auf die Gesamtzahl erfolgreich zugestellter Nachrichten.

* Anzahl unterschiedlicher Personen, die mindestens einmal im betreffenden Versand geklickt haben. Abmelde-Links und Links zur Mirrorseite werden ausgeschlossen.

Diese Metriken basieren auf der Konsolidierten Trackingtabelle (`nms:trackingStats`). Diese Aggregattabelle wird aus Leistungsgründen bei der Anzeige von Berichten anstelle der Tabelle Trackinglogs der Empfänger (`nms:trackingLogRcp`) und wird nicht in Echtzeit berechnet. Die Tabelle wird einige Minuten nach dem Abrufen der Trackinglogs generiert.


#### Abmelderaten {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Abmeldungen"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller Abmeldungen von einem Dienst und den Prozentsatz der Abmeldungen im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Die **Abmeldungen** zeigt die folgenden KPIs für jeden Kanal an:

* Prozentualer Anteil der Abmeldungen in Bezug auf die Gesamtzahl der erfolgreich zugestellten Nachrichten.

* Summe aller Klicks auf einen Abmelde-Link, d. h. mit URL-Kategorie &quot;Abmeldung&quot;.


#### Fehlerquoten {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Fehler"
>abstract="Gesamtzahl an Fehlern in Sendungen und der automatischen Bounce-Verarbeitung. Die zugeordnete Rate wird in Bezug auf die Anzahl zu versendender Nachrichten berechnet."

* Prozentualer Anteil der fehlerhaften Nachrichten in Bezug auf die Gesamtzahl der zu sendenden Nachrichten.

* Gesamtzahl an Fehlern in Sendungen und der automatischen Bounce-Verarbeitung.


### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="Das Menü **Explorer** zeigt alle Campaign-Komponenten und -Objekte mit derselben Ordnerhierarchie wie in der Client-Konsole an. Durchsuchen Sie alle Ihre Komponenten, Ordner und Schemata in Campaign v8 und erstellen Sie Sendungen, Workflows und Kampagnen. Alle anderen Listen sind schreibgeschützt."

Das Menü **Explorer** zeigt alle Campaign-Ressourcen und -Objekte mit derselben Ordnerhierarchie an wie in der Client-Konsole. Durchsuchen Sie alle Ihre Komponenten, Ordner und Schemata in Campaign v8 und erstellen Sie Sendungen, Workflows und Kampagnen. Alle anderen Listen sind schreibgeschützt.

Welche Elemente im Explorer angezeigt werden, hängt von Ihren Benutzerberechtigungen ab.

Wie bei jedem Listenbildschirm können Sie die Spalten so konfigurieren, dass alle von Ihnen benötigten Informationen angezeigt werden. Weitere Informationen finden Sie in [diesem Abschnitt](#list-screens).

Weitere Informationen zum Campaign-Explorer, zur Ordnerhierarchie und zu den Ressourcen finden Sie in dieser [Dokumentation zu Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=de#ac-explorer-ui){target="_blank"}.

### Kampagnen-Management {#user-interface-campaign-management}

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Kampagnen"
>abstract="Dies ist die Liste Ihrer Kampagnen. Sie können nützliche Informationen wie das Anfangsdatum/Enddatum/Datum der letzten Änderung sowie ihren Status anzeigen. Sie können die Liste nach Status oder Anfangsdatum/Enddatum filtern. Klicken Sie auf die Schaltfläche „Kampagne erstellen“, um eine neue Kampagne hinzuzufügen. Wählen Sie eine Kampagne aus, um Inhalt, Sendungen und Details anzuzeigen. Navigieren Sie zur Registerkarte „Vorlagen“, um Vorlagen anzuzeigen oder zu erstellen."



Im Abschnitt KAMPAGNEN-MANAGEMENT haben Sie Zugriff auf Marketing-Kampagnen, Sendungen und Workflows.

* **Kampagnen** – Dies ist die Liste Ihrer Kampagnen und Kampagnenvorlagen. Standardmäßig können Sie für jede Kampagne die Datumsangaben für Start, Ende, Erstellung und letzte Änderung, den aktuellen Status und den Namen der Campaign-Benutzerin bzw. des -Benutzers anzeigen, die bzw. der die Kampagne erstellt hat. Sie können die Liste nach Status, Start-/Enddatum oder Ordner filtern oder einen erweiterten Filter erstellen, um eigene Filterkriterien zu definieren. Weiterführende Informationen zu Marketing-Kampagnen finden Sie in [diesem Abschnitt](../campaigns/gs-campaigns.md).

* **Sendungen**: Durchsuchen Sie Ihre Sendungenliste. Standardmäßig können Sie ihren Status, das Datum der letzten Änderung sowie wichtige KPIs sehen. Sie können die Liste nach Status, Kontaktdatum oder Kanal filtern. Klicken Sie auf einen E-Mail-Versand, um sein Dashboard zu öffnen und sich einen Überblick über die Versanddetails zu verschaffen. Sendungen über andere Kanäle sind schreibgeschützt. Weitere Informationen zu Sendungen finden Sie in [diesem Abschnitt](../msg/gs-messages.md).

  Verwenden Sie die Schaltfläche **Mehr Aktionen**, um einen Versand zu löschen oder zu duplizieren.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** – Auf diesem Bildschirm können Sie auf die vollständige Liste der Workflows und Workflow-Vorlagen zugreifen. Sie können den Status und das letzte bzw. nächste Ausführungsdatum überprüfen und einen neuen Workflow oder eine neue Workflow-Vorlage erstellen. Sie können die Liste nach denselben Kriterien filtern wie für andere Objekte. Darüber hinaus können Sie Workflows filtern, die zu einer Kampagne gehören oder nicht. Weiterführende Informationen zu Workflows finden Sie [in diesem Abschnitt](../workflows/gs-workflows.md).


### Kunden-Management {#user-interface-customer-management}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Empfänger"
>abstract="Greifen Sie auf Ihre Empfängerdatenbank zu. Sie können nützliche Informationen wie die E-Mail-Adresse, den Vornamen und den Nachnamen der Empfänger anzeigen. Diese Liste ist schreibgeschützt."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Zielgruppen"
>abstract="Dies ist die Liste Ihrer Audiences. Sie können den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und das Label anzeigen. Sie können die Liste nach Herkunft filtern. Diese Liste ist schreibgeschützt."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Abonnementlisten"
>abstract="Durchsuchen Sie Ihre Abonnementlisten. Sie können ihren Typ, Modus und ihre Beschriftung anzeigen. Diese Liste ist schreibgeschützt."


Im Bereich KUNDENVERWALTUNG können Sie Ihre Empfängerinnen und Empfänger, Zielgruppen und Abonnements anzeigen. Diese Listen sind schreibgeschützt.

* **Empfänger**: Greifen Sie auf Ihre Empfängerdatenbank zu. Standardmäßig können Sie die E-Mail-Adresse sowie den Vor- und Nachnamen sehen. Weitere Informationen zu Empfängerinnen und Empfängern finden Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/gs-audiences.html?lang=de){target="_blank"}.
* **Zielgruppen**: Dies ist die Liste Ihrer Zielgruppen. Standardmäßig können Sie den Typ, die Herkunft, das Erstellungsdatum/Datum der letzten Änderung und die Kennzeichnung sehen. Sie können die Liste nach Herkunft filtern. Weitere Informationen zu Zielgruppen und Listen finden Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=de){target="_blank"}.
* **Abonnements**: Durchsuchen Sie Ihre Abonnements. Standardmäßig können Sie den Typ, den Modus und die Kennzeichnung sehen. Erfahren Sie mehr über die Verwaltung von Abonnements und Abmeldungen in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=de){target="_blank"}.

### Entscheidungs-Management

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Angebote"
>abstract="Durchsuchen Sie Ihre Liste von Interaktionsangeboten. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status oder Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar. Diese Listen sind schreibgeschützt."

* **Angebote**: Durchsuchen Sie Ihre Liste von Interaktionsangeboten. Standardmäßig können Sie den Status, das Start-/Enddatum und die Umgebung sehen. Sie können die Liste nach Status oder Start-/Enddatum filtern. Angebotsvorlagen sind ebenfalls verfügbar. Diese Listen sind schreibgeschützt.

Erfahren Sie in der [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=de){target="_blank"}, wie Sie Angebote verwalten und erstellen können.

## Obere Leiste

Verwenden Sie die obere Leiste der Benutzeroberfläche, um folgende Aktionen durchzuführen:

* Ihr Feedback als Alpha-Testerin oder -Tester teilen
* zwischen Organisationen und Instanzen wechseln
* zwischen Adobe Experience Cloud-Anwendungen wechseln
* auf Hilfeseiten zugreifen, den Support kontaktieren und Feedback geben. Sie können Hilfe-Artikel und Videos mithilfe des Suchfelds suchen.

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Kontextuelle Hilfe {#contextual-help}

Eine kontextuelle Hilfe ist in der Benutzeroberfläche verfügbar. Wenn verfügbar, klicken Sie auf das `?`-Symbol, um Hilfeinformationen und zugehörige Dokumentations-Links anzuzeigen.

![](assets/context-help.png){width="40%" align="left"}

<!--An on-boarding guide is also available to help you get started with Campaign v8 Web. Click the icon in the bottom right corner, choose one of the available step-by-step scenarios, and simply follow the instructions.

![](assets/onboarding.png){width="70%" align="left"}-->

## Unterstützte Browser {#browsers}

Campaign v8 Web ist so konzipiert, dass es mit den neuesten Versionen von Google Chrome, Safari und Microsoft Edge optimal funktioniert. Bei der Verwendung bestimmter Funktionen in älteren Versionen oder anderen Browsern können Probleme auftreten.

## Sprachvoreinstellungen {#language-pref}

Campaign v8 Web ist derzeit in den folgenden Sprachen verfügbar:

<table>
<tr>
<td>
<p>Englisch (US) – EN-US</p>
<p>Französisch – FR</p>
<p>Deutsch – DE</p>
<p>Italienisch – IT</p>
</td>
<td>
<p>Spanisch – ES</p>
<p>Portugiesisch (Brasilianisch) – PTBR</p>
<p>Japanisch – JP</p>
</td>
<td>
<p>Koreanisch – KR</p>
<p>Vereinfachtes Chinesisch – CHS</p>
<p>Traditionelles Chinesisch – CHT</p>
</td>
</tr>
</table>

Die Standardsprache der Benutzeroberfläche wird von der in Ihrem Benutzerprofil angegebenen bevorzugten Sprache bestimmt.

So ändern Sie Ihre Sprache:

1. Klicken Sie auf das Profilsymbol oben rechts und wählen Sie dann **Voreinstellungen**.
1. Klicken Sie dann auf den Sprach-Link, der unter Ihrer E-Mail-Adresse angezeigt wird.
1. Wählen Sie Ihre bevorzugte Sprache aus und klicken Sie auf **Speichern**. Sie können eine zweite Sprache auswählen, falls die von Ihnen verwendete Komponente nicht in Ihrer gewählten Sprache lokalisiert ist.


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
>id="acw_targetdata_personalization_enrichmentdata"
>title="Anreicherungsdaten"
>abstract="Noch nicht definiert"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Versandberichte"
>abstract="Prüfen Sie die Versandindikatoren für die Kampagnenberichte."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Tracking-Berichte"
>abstract="Prüfen Sie die Tracking-Indikatoren für die Kampagnenberichte."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Berichte – Übersicht"
>abstract="Schlüsselmetriken für den Versand."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Berichte für Zielgruppenstatistiken"
>abstract="In diesem Abschnitt werden spezifische Metriken entsprechend den Zielgruppen angezeigt."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Aggregierte Berichte für Sendungen"
>abstract="Wählen Sie mindestens zwei Sendungen aus, um einen aggregierten Datenbericht anzuzeigen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Deduplizierungsfelder"
>abstract="Noch nicht definiert"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Deduplizierungseinstellungen"
>abstract="Noch nicht definiert"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Deduplizierungskomplement"
>abstract="Noch nicht definiert"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Dimensionskomplement"
>abstract="Noch nicht definiert"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Berechtigung erforderlich"
>abstract="Ihre Admins müssen Ihnen die Berechtigung erteilen, bevor Sie ein Segment erstellen können."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Berechtigung erforderlich"
>abstract="Ihre Admins müssen Ihnen die Berechtigung erteilen, bevor Sie ein Segment erstellen können."


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Diese Kampagne ist schreibgeschützt"
>abstract="Keine Berechtigung, diese Kampagne zu bearbeiten. Bei Bedarf Admin kontaktieren, um Zugriff zu erhalten."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Dieser Versand ist schreibgeschützt"
>abstract="Keine Berechtigung, diesen Versand zu bearbeiten. Bei Bedarf Admin kontaktieren, um Zugriff zu erhalten."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Dieser Service ist schreibgeschützt"
>abstract="Keine Berechtigung, diesen Service zu bearbeiten. Bei Bedarf Admin kontaktieren, um Zugriff zu erhalten."

<!-- Workflows-->

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Liste der Workflows"
>abstract="Liste der für Ihre Kampagne verfügbaren Workflows. Verwenden Sie die Schaltfläche „Workflow erstellen“, um einen Workflow zu Ihrer Kampagne hinzuzufügen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Ausgehende Transition zur Speicherung der Zielgruppe"
>abstract="tbc"

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="Speichern einer Zielgruppe"
>abstract="Verwenden Sie diese Aktivität, um die Workflow-Zielgruppe zu speichern."


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Dieser Workflow ist schreibgeschützt"
>abstract="Keine Berechtigung, diesen Workflow zu bearbeiten. Bei Bedarf Admin kontaktieren, um Zugriff zu erhalten."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Dieser Workflow ist schreibgeschützt"
>abstract="Dieser Workflow kann aufgrund einer nicht unterstützten oder nicht kompatiblen Arbeitsfläche nicht bearbeitet werden."

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Gültigkeitszeitraum"
>abstract="Diese Option legt die Dauer fest, für die das Tracking für die URLs aktiviert wird."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Versandlaufzeit"
>abstract="Im Feld „Versandlaufzeit“ können Sie die Zeitspanne angeben, in der erneute Zustellversuche unternommen werden sollen. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis nach Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Gültigkeit von Ressourcen"
>abstract="Das Feld „Gültigkeitsdauer“ wird für hochgeladene Ressourcen verwendet, wie etwa die Mirrorseite oder Bilder. Diese Ressourcen sind für eine begrenzte Zeit gültig: Nach Erreichen des Grenzwerts sind keine Ressourcen mehr verfügbar."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Validierungsmodus"
>abstract="Jeder Schritt eines Versands kann einer Validierung unterzogen werden, um eine vollständige Überwachung und Kontrolle der verschiedenen Prozesse zu gewährleisten."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Maximale Anzahl der weiteren Zustellversuche"
>abstract="Wenn ein Nachrichtenversand aufgrund eines temporären Fehlers fehlschlägt, werden weitere Zustellversuche bis zum Ende der Versandlaufzeit durchgeführt."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Wichtigkeit des Empfängers bzw. der Empfängerin"
>abstract="Mit der Wichtigkeit des Empfängers bzw. der Empfängerin wird festgelegt, welche Empfangenden im Falle einer Kapazitätsüberlastung der Typologieregeln beibehalten werden."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Versandgewichtung"
>abstract="Die Versandgewichtung ermöglicht es Ihnen, im Rahmen der Druckverwaltung diejenigen Sendungen festzulegen, die vorrangig durchgeführt werden sollen. Die Nachrichten mit der höchsten Gewichtung haben Vorrang."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologie"
>abstract="Mit einer Typologie können Sie die Durchführung von Sendungen steuern, filtern und überwachen."

>[!CONTEXTUALHELP]
>id="acw_reporting_email_exportation"
>title="Export"
>abstract="Sie können nur die ausgewählte Seite exportieren."

