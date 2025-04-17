---
product: campaign
title: Audit-Protokoll
description: Erfahren Sie, wie Sie Ihre Instanz mit dem Audit-Protokoll von Campaign überwachen.
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 33%

---

# Audit-Protokoll {#audit-trail}

In der Web-Benutzeroberfläche von Adobe Campaign bietet die Funktion **[!UICONTROL Audit-Protokoll]** Benutzern vollständige Einblicke in alle Änderungen, die an wichtigen Entitäten in Ihrer Instanz vorgenommen wurden. Dies betrifft in der Regel diejenigen Änderungen, die den reibungslosen Betrieb der Instanz erheblich beeinträchtigen.

>[!IMPORTANT]
>
>* Die Web-Benutzeroberfläche von Adobe Campaign überwacht keine Änderungen, die in Benutzerrechten, Vorlagen, Personalisierung oder Kampagnen vorgenommen wurden.
>* Nur Administratoren der Instanz können das Audit-Protokoll verwalten.

Die **[!UICONTROL Audit-Protokoll]**-Funktion zeichnet kontinuierlich und in Echtzeit ein detailliertes Protokoll der Aktionen und Ereignisse auf, die innerhalb der Adobe Campaign-Instanz stattfinden. Sie bietet eine praktische Methode für den Zugriff auf einen chronologischen Datensatz mit Daten und adressiert Abfragen wie den Status von Workflows, die neuesten Personen, die sie ändern möchten, oder die Aktivitäten, die von Benutzern innerhalb der Instanz ausgeführt werden.

+++ Weitere Informationen zu verfügbaren Entitäten des Audit-Protokolls

* **Audit-Protokoll für Source-**: Ermöglicht Ihnen, Aktivitäten und aktuelle Änderungen an Ihren Schemata in der Client-Konsole von Campaign v8 zu überwachen.

  Detaillierte Informationen zu Schemata finden Sie in der [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* Das **Workflow-Audit-Protokoll** ermöglicht es Ihnen, Aktivitäten und aktuelle Änderungen an Workflows zu verfolgen, einschließlich der aktuellen Status wie:

   * Starten
   * Aussetzen
   * Stoppen
   * Neu starten
   * Bereinigung, die der Aktion „Verlauf bereinigen“ entspricht
   * Simulieren, was der Aktion „Im Simulationsmodus starten“ entspricht
   * Wakeup entspricht der Aktion „Ausstehende Aufgaben jetzt ausführen“.
   * Unbedingter Stopp

  Weiterführende Informationen zu Workflows finden Sie auf [dieser Seite](../workflows/gs-workflows.md).

* **Audit-Protokoll für Optionen** ermöglicht es Ihnen, Aktivitäten und aktuelle Änderungen an Ihren Optionen in Campaign v8 zu überwachen.

  Weiterführende Informationen zu Optionen finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* Das **Audit-Protokoll für den Versand** ermöglicht Ihnen die Überprüfung der Aktivitäten und der letzten Änderungen an Ihren Sendungen.

  Weiterführende Informationen zu Sendungen finden Sie auf [dieser Seite](../msg/gs-deliveries.md).

* Mit **Externes Konto** können Sie Änderungen an externen Konten in Campaign v8 überprüfen, die von technischen Prozessen wie technischen Workflows oder Kampagnen-Workflows verwendet werden.

  Weiterführende Informationen zu externen Konten finden Sie auf dieser [Seite](../administration/external-account.md).

* **Versand-Mapping** ermöglicht Ihnen das Überwachen von Aktivitäten und aktuellen Änderungen an Ihrem Versand-Mapping in Campaign v8.

  Weiterführende Informationen zu „Versand-Mapping“ finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Web-Anwendung** ermöglicht es Ihnen, Änderungen an Web-Formularen in Campaign v8 zu überprüfen, die zum Erstellen von Seiten mit Eingabe- und Auswahlfeldern verwendet werden und Daten aus der Datenbank enthalten können.

  Weitere Informationen zu Web-Anwendungen finden Sie auf dieser [Seite](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/content/webapps).

* **Angebot** ermöglicht es Ihnen, die Aktivitäten und letzten Änderungen an Ihren Angeboten zu überprüfen.

  Weiterführende Informationen zu Angeboten finden Sie auf [dieser Seite](../msg/offers.md).

* **Operator** ermöglicht es Ihnen, Aktivitäten und aktuelle Änderungen an Ihren Operatoren in Campaign v8 zu überwachen.

  Weiterführende Informationen zu Benutzerinnen und Benutzern finden Sie auf [dieser Seite](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Zugriff auf das Audit-Protokoll {#accessing-audit-trail}

So greifen auf das **[!UICONTROL Audit-Protokoll]** Ihrer Instanz zu:

1. Wählen Sie im Menü **[!UICONTROL Administration]** die Option **[!UICONTROL Audit-Protokoll]** aus.

   ![Screenshot mit dem Menü Administration mit ausgewählter Option „Audit-Protokoll“](assets/audit-trail-1.png)

1. Das Fenster **[!UICONTROL Audit-Protokoll]** wird mit der Liste Ihrer Entitäten geöffnet. Die Web-Benutzeroberfläche von Adobe Campaign prüft die Aktionen zum Erstellen, Bearbeiten und Löschen von Workflows, Optionen, Sendungen und Schemata.

   Wählen Sie eine der Entitäten aus, um mehr über die letzten Änderungen zu erfahren.

1. Das Fenster **[!UICONTROL Audit-]**&quot; enthält detaillierte Informationen zur ausgewählten Entität, z. B.:

   * **[!UICONTROL type]**: Workflow, Optionen, Sendungen oder Schemata.
   * **[!UICONTROL Entität]**: Interner Name Ihrer Aktivitäten.
   * **[!UICONTROL Geändert von]**: Benutzername der Person, die diese Entität zuletzt geändert hat.
   * **[!UICONTROL Action]**: Letzte Aktion, die an dieser Entität ausgeführt wurde, entweder erstellt, geändert oder gelöscht.
   * **[!UICONTROL Änderungsdatum]**: Datum der letzten Aktion, die an dieser Entität durchgeführt wurde.

   Der Code-Block enthält weitere Informationen darüber, was in Ihrer Entität genau geändert wurde.

   ![Screenshot mit dem Fenster „Audit-Entität“ mit detaillierten Informationen zu Änderungen](assets/audit-trail-2.png)