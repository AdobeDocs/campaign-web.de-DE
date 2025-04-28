---
title: Arbeiten mit vordefinierten Filtern
description: Erfahren Sie, wie Sie in Adobe Campaign Web vordefinierte Filter erstellen und verwalten
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 100%

---

# Arbeiten mit vordefinierten Filtern {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Verwaltung von vordefinierten Filtern"
>abstract="Die Campaign Web-Benutzeroberfläche bietet eine benutzerfreundliche Oberfläche, mit der vordefinierte Filter einfach verwaltet und an Ihre individuellen Anforderungen angepasst werden können. Erstellen Sie Filter einmal und speichern Sie sie zur zukünftigen Verwendung."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Vordefinierte Filter"
>abstract="Die Campaign Web-Benutzeroberfläche bietet eine benutzerfreundliche Oberfläche, mit der vordefinierte Filter einfach verwaltet und an Ihre individuellen Anforderungen angepasst werden können. Erstellen Sie Filter einmal und speichern Sie sie zur zukünftigen Verwendung."

Vordefinierte Filter sind benutzerdefinierte Filter, die für zukünftige Verwendungen erstellt und gespeichert werden. Sie fungieren beim Filtern von Vorgängen mit dem Abfrage-Modeler als Verknüpfungen. Sie können beispielsweise beim Filtern einer Datenliste oder beim Erstellen der Zielgruppe eines Versands verwendet werden.

Sie können vorhandene integrierte Filter verwenden, um auf eine bestimmte Teilmenge Ihrer Daten zuzugreifen, oder eigene vordefinierte Filter erstellen und speichern.

![Menüoberfläche „Vordefinierte Filter“](assets/predefined-filters-menu.png){zoomable="yes"}

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

Speichern Sie einen benutzerdefinierten Filter im [Abfrage-Modeler](../query/query-modeler-overview.md), damit er für zukünftige Verwendungen verfügbar ist. Gehen Sie dazu wie folgt vor:

1. Öffnen Sie den Abfrage-Modeler und definieren Sie Ihre Filterbedingungen. Im folgenden Beispiel werden Empfängerinnen und Empfänger gefiltert, die in Madrid leben und einen Newsletter abonniert haben.
1. Klicken Sie auf die Schaltfläche **Filter auswählen oder speichern** und wählen Sie **Als Filter speichern**.

   ![Benutzeroberfläche zum Speichern eines vordefinierten Filters](assets/predefined-filters-save.png){zoomable="yes"}

1. Wählen Sie **Neuen Filter erstellen** und geben Sie einen Namen und eine Beschreibung für diesen Filter ein.

   ![Benutzeroberfläche zum Speichern von Filterdetails](assets/predefined-filters-save-filter.png){zoomable="yes"}

   Sie können den Filter bei Bedarf als Favorit speichern. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

1. Klicken Sie auf **Bestätigen**, um Ihre Änderungen zu speichern.

Ihr benutzerdefinierter Filter ist jetzt in der Liste der **vordefinierten Filter** verfügbar und für alle Campaign-Benutzenden zugänglich.

### Erstellen eines Filters in der Filterliste {#create-filter-from-list}

Erstellen Sie einen Filter im linken Menü über den Eintrag **Vordefinierte Filter**. Gehen Sie dazu wie folgt vor:

1. Navigieren Sie im linken Menü zum Eintrag **Vordefinierte Filter**.
1. Klicken Sie auf die Schaltfläche **Erstellen**.
1. Geben Sie den Namen des Filters ein und wählen Sie im Feld **Dokumenttyp** das Schema aus, auf das er angewendet wird. Das Standardschema lautet `Recipients(nms)`.

1. Definieren Sie die Regel für den Filter. Zum Beispiel Profile, die älter als 30 sind.

   ![Filterregel für Profile, die älter als 30 Tage sind](assets/filter-30+.png){zoomable="yes"}

1. Speichern Sie Ihre Änderungen.

   ![Benutzeroberfläche mit neuem gespeichertem Filter](assets/new-filter.png){zoomable="yes"}

Der Filter wird zur Liste der vordefinierten Filter hinzugefügt. Sie können den Filter bei Bedarf als Favorit speichern. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

## Speichern des Filters als Favorit {#fav-filter}

Aktivieren Sie bei der Erstellung eines vordefinierten Filters die Option **Als Favorit speichern**, damit dieser vordefinierte Filter als Favorit angezeigt wird.

Wenn ein Filter als Favorit gespeichert wird, steht er allen Benutzenden im Abschnitt **Favoritenfilter** der Filtererstellungsliste zur Verfügung, wie unten dargestellt:

![Abschnitt „Bevorzugte Filter“](assets/predefined-filters-favorite.png){zoomable="yes"}{width="30%" align="left"}

## Verwenden eines vordefinierten Filters {#use-predefined-filter}

Vordefinierte Filter sind beim Definieren von Regeleigenschaften verfügbar. Um auf vordefinierte Filter zuzugreifen, wählen Sie im Dropdown des Abfrage-Modelers die Option **Benutzerdefinierten Filter auswählen**.

Greifen Sie auf die vollständige Liste vordefinierter Filter zu, die für den aktuellen Kontext verfügbar sind, und verwenden Sie die Verknüpfungen, die im Abschnitt **Bevorzugte Filter** des Dropdown-Menüs verfügbar sind. Weitere Informationen zu Favoriten finden Sie in [diesem Abschnitt](#fav-filter).

Gehen Sie wie folgt vor, um beispielsweise eine Zielgruppe aus einem vordefinierten Filter zu erstellen:

1. Durchsuchen Sie den Eintrag **Zielgruppen** im linken Menü und klicken Sie auf die Schaltfläche **Zielgruppe erstellen** in der oberen linken Ecke der Zielgruppenliste.
1. Geben Sie den Namen der Zielgruppe ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen**.
1. Wählen Sie die Aktivität **Abfrage** aus und klicken Sie im rechten Fenster auf die Schaltfläche **Zielgruppe erstellen**.

   ![Benutzeroberfläche zum Erstellen von Zielgruppen](assets/build-audience-from-filter.png){zoomable="yes"}

1. Wählen Sie über die Schaltfläche zum **Filter auswählen oder speichern** die Option **Benutzerdefinierten Filter auswählen** aus.

   ![Option „Benutzerdefinierten Filter auswählen“](assets/build-audience-select-custom-filter.png){zoomable="yes"}

1. Navigieren Sie zum vordefinierten Filter, der zum Erstellen der Zielgruppe verwendet werden soll, wählen Sie ihn aus und bestätigen Sie die Wahl.

   ![Benutzeroberfläche mit Liste vordefinierter Filter](assets/build-audience-filter-list.png){zoomable="yes"}

1. Überprüfen Sie die Regeleigenschaften für diesen Filter und bestätigen Sie sie.

   Der Filter wird jetzt als Abfrage in der **Abfrage**-Aktivität genutzt.

   ![Abfrageaktivität mit vordefiniertem Filter](assets/build-audience-confirm.png){zoomable="yes"}

1. Speichern Sie Ihre Änderungen und klicken Sie auf die Schaltfläche **Starten**, um die Zielgruppe zu erstellen und in der Zielgruppenliste verfügbar zu machen.

## Verwalten Ihrer vordefinierten Filter {#manage-predefined-filter}

Alle vordefinierten Filter werden im dedizierten Eintrag des linken Navigationsmenüs gruppiert.

![Liste vordefinierter Filter](assets/list-of-filters.png){zoomable="yes"}

Von dieser Liste ausgehend können Sie einen neuen Filter erstellen wie oben beschrieben und die unten aufgeführten Aktionen durchführen:

* einen vorhandenen Filter bearbeiten und seine Regeln und Eigenschaften ändern
* einen vordefinierten Filter duplizieren
* einen vordefinierten Filter löschen

Sie können beim Erstellen Ihrer Zielgruppen auch einen vordefinierten Filter als Favoriten hinzufügen, um schnell darauf zugreifen zu können. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->