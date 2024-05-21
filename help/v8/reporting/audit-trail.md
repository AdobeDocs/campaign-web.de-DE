---
product: campaign
title: Audit-Protokoll
description: Erfahren Sie, wie Sie Ihre Instanz mit dem Audit-Protokoll von Campaign überwachen.
feature: Audit Trail, Monitoring, Workflows
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 40%

---

# Audit-Protokoll{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Audit-Protokoll"
>abstract="Die neue Funktion &quot;Audit-Protokoll&quot;enthält eine detaillierte und chronologische Übersicht aller Aktionen und Ereignisse, die in Echtzeit an Ihrer Adobe Campaign-Instanz durchgeführt wurden."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"


In der Adobe Campaign-Webbenutzeroberfläche wird die **[!UICONTROL Audit-Protokoll]** -Funktion bietet Benutzern vollständige Einsicht in alle Änderungen, die an wichtigen Entitäten in Ihrer Instanz vorgenommen wurden, normalerweise jene, die einen reibungslosen Betrieb der Instanz erheblich beeinträchtigen.

>[!IMPORTANT]
>
>* Die Adobe Campaign-Webbenutzeroberfläche prüft keine Änderungen, die an Benutzerrechten, Vorlagen, Personalisierungen oder Kampagnen vorgenommen wurden.
>* Das Audit-Protokoll kann nur von Admins der Instanz verwaltet werden.

**[!UICONTROL Audit-Protokoll]** -Funktion zeichnet ständig ein detailliertes Protokoll der Aktionen und Ereignisse auf, die in der Adobe Campaign-Instanz in Echtzeit stattfinden. Es bietet eine praktische Methode, um auf einen chronologischen Datensatz mit Abfragen zuzugreifen, wie z. B. den Status von Workflows, die neuesten zu ändernden Personen oder die Aktivitäten, die von Benutzern innerhalb der Instanz ausgeführt werden.

+++ Weitere Informationen über die verfügbaren Entitäten im Audit-Protokoll

* **Audit-Protokoll für Quellschemata** ermöglicht es Ihnen, Aktivitäten und aktuelle Änderungen an Ihren Schemas in der Campaign V8-Clientkonsole zu überwachen.

  Detaillierte Informationen zu Schemata finden Sie unter [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Workflow-Audit-Protokoll** ermöglicht es Ihnen, Aktivitäten und aktuelle Änderungen an Workflows zu verfolgen, einschließlich des aktuellen Status wie:

   * Starten
   * Aussetzen
   * Stoppen
   * Neu starten
   * Bereinigen, was der Aktion „Verlauf bereinigen“ entspricht
   * Simulieren, was der Aktion „Starten“ im Simulationsmodus entspricht
   * Wecken, was der Aktion „Vorgezogene Ausführung der ausstehenden Aufgaben“ entspricht
   * Unbedingter Stopp

  Weiterführende Informationen zu Workflows finden Sie auf [dieser Seite](../workflows/gs-workflows.md).

* **Option-Audit-Protokoll** ermöglicht es Ihnen, Aktivitäten und aktuelle Änderungen an Ihren Optionen in Campaign V8 zu überwachen.

  Weiterführende Informationen zu Optionen finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* Das **Audit-Protokoll für den Versand** ermöglicht Ihnen die Überprüfung der Aktivitäten und der letzten Änderungen an Ihren Sendungen.

  Weiterführende Informationen zu Sendungen finden Sie auf [dieser Seite](../msg/gs-deliveries.md).

* **Externes Konto** können Sie Änderungen an externen Konten in Campaign V8 überprüfen, die von technischen Prozessen wie technischen Workflows oder Kampagnen-Workflows verwendet werden.

  Weiterführende Informationen zu „Externes Konto“ finden Sie auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Versandzuordnung** ermöglicht es Ihnen, Aktivitäten und kürzlich an Ihrer Versandzuordnung in Campaign V8 vorgenommene Änderungen zu überwachen.

  Weiterführende Informationen zu „Versand-Mapping“ finden Sie auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Web-Anwendung** ermöglicht Ihnen das Überprüfen von Änderungen an Web-Formularen in Campaign V8, die zum Erstellen von Seiten mit Eingabe- und Auswahlfeldern verwendet werden und die Daten aus der Datenbank enthalten können.

  Weiterführende Informationen zu „Web-Anwendung“ finden Sie auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Angebot** ermöglicht es Ihnen, die Aktivitäten und letzten Änderungen an Ihren Angeboten zu überprüfen.

  Weiterführende Informationen zu Angeboten finden Sie in diesem Abschnitt [page](../msg/offers.md).

* **Operator** ermöglicht Ihnen, Aktivitäten und Änderungen zu überwachen, die in Campaign V8 an Ihren Benutzern vorgenommen wurden.

  Weiterführende Informationen zu Benutzerinnen und Benutzern finden Sie auf [dieser Seite](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Zugriff auf das Audit-Protokoll {#accessing-audit-trail}

So greifen auf das **[!UICONTROL Audit-Protokoll]** Ihrer Instanz zu:

1. Unter dem **[!UICONTROL Administration]** Menü auswählen **[!UICONTROL Audit-Protokoll]** .

   ![](assets/audit-trail-1.png)

1. Das Fenster **[!UICONTROL Audit-Protokoll]** wird mit der Liste Ihrer Entitäten geöffnet. Die Adobe Campaign-Webbenutzeroberfläche überprüft die Aktionen zum Erstellen, Bearbeiten und Löschen von Workflows, Optionen, Sendungen und Schemata.

   Wählen Sie eine der Entitäten aus, um mehr über die letzten Änderungen zu erfahren.

1. Im Fenster **[!UICONTROL Audit-Entität]** erhalten Sie detailliertere Informationen zu der ausgewählten Entität, z. B.:

   * **[!UICONTROL Typ]** : Workflow, Optionen, Sendungen oder Schemata.
   * **[!UICONTROL Entität]** : Interner Name Ihrer Aktivitäten.
   * **[!UICONTROL Geändert von]** : Benutzername der letzten Person, die diese Entität zuletzt geändert hat.
   * **[!UICONTROL Aktion]** : Letzte Aktion, die für diese Entität ausgeführt wurde, entweder &quot;Erstellt&quot;, &quot;Geändert&quot;oder &quot;Gelöscht&quot;.
   * **[!UICONTROL Änderungsdatum]** : Datum der letzten Aktion, die für diese Entität durchgeführt wurde.

   Der Codeblock liefert weitere Informationen darüber, was genau in Ihrer Entität geändert wurde.

   ![](assets/audit-trail-2.png)

