---
title: Arbeiten mit vordefinierten Filtern
description: Erfahren Sie, wie Sie in Adobe Campaign Web vordefinierte Filter erstellen und verwalten
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: 97b6de0763dbeb133d7d0346e6af4d056cc731e3
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 78%

---

# Arbeiten mit vordefinierten Filtern {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Verwaltung von vordefinierten Filtern"
>abstract="Die Campaign-Web-Benutzeroberfläche bietet eine benutzerfreundliche Oberfläche, mit der vordefinierte Filter einfach verwaltet und an Ihre spezifischen Anforderungen angepasst werden können. Filter einmal erstellen und für zukünftige Verwendungen speichern."


<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card4"
>title="Verwaltung von vordefinierten Filtern"
>abstract="Campaign Web bietet jetzt eine benutzerfreundliche Oberfläche, mit der man vordefinierte Filter mühelos verwalten und an Ihre spezifischen Anforderungen anpassen kann. Filter einmal erstellen und für zukünftige Verwendungen speichern."

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Vordefinierte Filter"
>abstract="Die Campaign-Webbenutzeroberfläche bietet eine benutzerfreundliche Oberfläche, mit der Sie vordefinierte Filter mühelos verwalten und an Ihre spezifischen Anforderungen anpassen können. Filter einmal erstellen und für zukünftige Verwendungen speichern."

Vordefinierte Filter sind benutzerdefinierte Filter, die für zukünftige Verwendungen erstellt und gespeichert werden. Sie können als Verknüpfungen bei allen Filtervorgängen mit dem Abfrage-Modeller verwendet werden, zum Beispiel beim Filtern einer Liste von Daten oder beim Erstellen der Zielgruppe eines Versands.

Sie können vorhandene integrierte Filter verwenden, um auf einen bestimmten Teil Ihrer Daten zuzugreifen, oder eigene vordefinierte Filter erstellen und speichern.

![](assets/predefined-filters-menu.png){zoomable=&quot;yes&quot;}{zoomable=&quot;yes&quot;}

## Erstellen eines vordefinierten Filters {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Erstellen eines vordefinierten Filters"
>abstract="Geben Sie eine Kennzeichnung für den vordefinierten Filter ein und wählen Sie die Tabelle aus, auf die er angewendet werden soll. Öffnen Sie die zusätzlichen Optionen, um eine Beschreibung hinzuzufügen und diesen Filter als Favoriten festzulegen. Definieren Sie dann mithilfe der Schaltfläche „Regel erstellen“ die Filterbedingungen."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Erstellen der vordefinierten Filterregeln"
>abstract="Um die Filterbedingungen Ihres benutzerspezifischen Filters zu definieren, klicken Sie auf die Schaltfläche „Regel erstellen“."

### Erstellen eines Filters mit dem Abfrage-Modeler {#create-from-rule-builder}

Sie können einen benutzerdefinierten Filter im [Abfrage-Modeler](../query/query-modeler-overview.md) speichern, damit er für zukünftige Verwendungen verfügbar ist. Führen Sie folgende Schritte aus:

1. Öffnen Sie den Abfrage-Modeler und definieren Sie Ihre Filterbedingungen. Im folgenden Beispiel filtern Sie Empfängerinnen und Empfänger, die in Madrid leben und einen Newsletter abonniert haben.
1. Klicken Sie auf die Schaltfläche **Filter auswählen oder speichern** und wählen Sie **Als Filter speichern**.

   ![](assets/predefined-filters-save.png){zoomable=&quot;yes&quot;}

1. Wählen Sie **Neuen Filter erstellen** und geben Sie einen Namen und eine Beschreibung für diesen Filter ein.

   ![](assets/predefined-filters-save-filter.png){zoomable=&quot;yes&quot;}

   Sie können den Filter bei Bedarf als Favorit speichern. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

1. Klicken Sie auf **Bestätigen**, um Ihre Änderungen zu speichern.

Ihr benutzerdefinierter Filter ist jetzt in der Liste der **vordefinierten Filter** verfügbar und für alle Campaign-Benutzenden zugänglich.


### Erstellen eines Filters in der Filterliste {#create-filter-from-list}

Sie können einen Filter im Eintrag **Vordefinierte Filter** im linken Menü erstellen. Gehen Sie dazu wie folgt vor:

1. Navigieren Sie zum Eintrag **Vordefinierte Filter** im linken Menü.
1. Klicken Sie auf die Schaltfläche **Erstellen**.
1. Geben Sie den Namen des Filters ein und wählen Sie im Feld **Dokumenttyp** das Schema aus, auf das er angewendet wird. Das Standardschema lautet `Recipients(nms)`.


1. Definieren Sie die Regel für den Filter. Zum Beispiel Profile, die älter als 30 sind.

   ![](assets/filter-30+.png){zoomable=&quot;yes&quot;}


1. Speichern Sie Ihre Änderungen.

   ![](assets/new-filter.png){zoomable=&quot;yes&quot;}


Der Filter wird zur Liste der vordefinierten Filter hinzugefügt. Sie können den Filter bei Bedarf als Favorit speichern. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).


## Speichern des Filters als Favorit {#fav-filter}

Bei der Erstellung eines vordefinierten Filters können Sie die Option **Als Favorit speichern** aktivieren, wenn Sie diesen vordefinierten Filter in Ihren Favoriten sehen möchten.


Wenn ein Filter als Favorit gespeichert wird, steht er allen Benutzenden im Abschnitt **Favoritenfilter** der Filtererstellungsliste zur Verfügung, wie unten dargestellt:

![](assets/predefined-filters-favorite.png){zoomable=&quot;yes&quot;}{width="30%" align="left"}

## Verwenden eines vordefinierten Filters {#use-predefined-filter}

Vordefinierte Filter sind beim Definieren von Regeleigenschaften verfügbar. Um auf vordefinierte Filter zuzugreifen, wählen Sie die Option **Benutzerdefinierten Filter auswählen** in der Dropdown-Liste des Abfrage-Modelers.

Sie können dann auf die vollständige Liste vordefinierter Filter zugreifen, die für den aktuellen Kontext verfügbar sind, und die im Abschnitt verfügbaren Verknüpfungen verwenden. **Favoritenfilter** des Dropdown-Menüs aus. Weitere Informationen zu Favoriten finden Sie in [diesem Abschnitt](#fav-filter).

Gehen Sie wie folgt vor, um beispielsweise eine Zielgruppe aus einem vordefinierten Filter zu erstellen:

1. Navigieren Sie zum **Zielgruppen** im linken Menü ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen** in der oberen linken Ecke der Zielgruppenliste.
1. Geben Sie den Namen der Zielgruppe ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen**.
1. Wählen Sie die **Abfrage** und klicken Sie im rechten Bereich auf das **Erstellen einer Zielgruppe** Schaltfläche.

   ![](assets/build-audience-from-filter.png){zoomable=&quot;yes&quot;}

1. Aus dem **Filter auswählen oder speichern** -Schaltfläche, wählen Sie die **Benutzerspezifischen Filter auswählen** -Option.

   ![](assets/build-audience-select-custom-filter.png){zoomable=&quot;yes&quot;}

1. Navigieren Sie zum vordefinierten Filter, der zum Erstellen der Zielgruppe verwendet werden soll, wählen Sie ihn aus und bestätigen Sie die Wahl.

   ![](assets/build-audience-filter-list.png){zoomable=&quot;yes&quot;}

1. Überprüfen Sie die Regeleigenschaften für diesen Filter und bestätigen Sie sie.

   Der Filter wird jetzt als Abfrage in der **Abfrage**-Aktivität genutzt.

   ![](assets/build-audience-confirm.png){zoomable=&quot;yes&quot;}

1. Speichern Sie Ihre Änderungen und klicken Sie auf die Schaltfläche **Starten**, um die Zielgruppe zu erstellen und in der Zielgruppenliste verfügbar zu machen.

## Verwalten Ihrer vordefinierten Filter {#manage-predefined-filter}

Alle vordefinierten Filter werden im entsprechenden Eintrag des linken Navigationsmenüs gruppiert.

![](assets/list-of-filters.png){zoomable=&quot;yes&quot;}

Aus dieser Liste können Sie wie oben beschrieben einen neuen Filter erstellen und die unten aufgeführten Aktionen ausführen:

* Bearbeiten Sie einen vorhandenen Filter und ändern Sie ihn anhand von Regeln und Eigenschaften.
* Duplizieren Sie einen vordefinierten Filter.
* Löschen Sie einen vordefinierten Filter.

Sie können beim Erstellen Ihrer Zielgruppen auch einen vordefinierten Filter als Favoriten für einen schnellen Zugriff hinzufügen. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->
