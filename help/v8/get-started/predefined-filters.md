---
title: Arbeiten mit vordefinierten Filtern
description: Erfahren Sie, wie Sie in Adobe Campaign Web vordefinierte Filter erstellen und verwalten
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 60%

---

# Arbeiten mit vordefinierten Filtern {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Verwaltung von vordefinierten Filtern"
>abstract="Die Web-Benutzeroberfläche von Campaign bietet eine benutzerfreundliche Oberfläche zur mühelosen Verwaltung und Anpassung vordefinierter Filter an Ihre spezifischen Anforderungen. Erstellen Sie Filter einmal und speichern Sie sie zur zukünftigen Verwendung."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Vordefinierte Filter"
>abstract="Die Web-Benutzeroberfläche von Campaign bietet eine benutzerfreundliche Oberfläche zur mühelosen Verwaltung und Anpassung vordefinierter Filter an Ihre spezifischen Anforderungen. Erstellen Sie Filter einmal und speichern Sie sie zur zukünftigen Verwendung."

Vordefinierte Filter sind benutzerdefinierte Filter, die für die zukünftige Verwendung erstellt und gespeichert werden. Sie dienen beim Filtern von Vorgängen mit dem Abfrage-Modellierer als Tastaturbefehle. Sie können beispielsweise beim Filtern einer Datenliste oder beim Erstellen der Audience eines Versands verwendet werden.

Sie können vorhandene integrierte Filter verwenden, um auf eine bestimmte Untergruppe Ihrer Daten zuzugreifen oder Ihre eigenen vordefinierten Filter erstellen und speichern.

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

Speichern Sie einen benutzerdefinierten Filter aus dem [Abfrage-Modellierer](../query/query-modeler-overview.md), um ihn für die zukünftige Verwendung verfügbar zu machen. Führen Sie folgende Schritte aus:

1. Öffnen Sie den Abfrage-Modeler und definieren Sie Ihre Filterbedingungen. Im folgenden Beispiel werden Empfänger gefiltert, die in Madrid leben und einen Newsletter abonniert haben.
1. Klicken Sie auf die Schaltfläche **Filter auswählen oder speichern** und wählen Sie **Als Filter speichern**.

   ![Vordefinierte Filterschnittstelle speichern](assets/predefined-filters-save.png){zoomable="yes"}

1. Wählen Sie **Neuen Filter erstellen** und geben Sie einen Namen und eine Beschreibung für diesen Filter ein.

   ![Oberfläche für Filterdetails speichern](assets/predefined-filters-save-filter.png){zoomable="yes"}

   Sie können den Filter bei Bedarf als Favorit speichern. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

1. Klicken Sie auf **Bestätigen**, um Ihre Änderungen zu speichern.

Ihr benutzerdefinierter Filter ist jetzt in der Liste der **vordefinierten Filter** verfügbar und für alle Campaign-Benutzenden zugänglich.

### Erstellen eines Filters in der Filterliste {#create-filter-from-list}

Erstellen Sie einen Filter aus dem **Vordefinierte Filter** Eintrag im linken Menü. Gehen Sie dazu wie folgt vor:

1. Navigieren Sie im linken **zum Eintrag** Vordefinierte Filter“.
1. Klicken Sie auf die Schaltfläche **Erstellen**.
1. Geben Sie den Namen des Filters ein und wählen Sie im Feld **Dokumenttyp** das Schema aus, auf das er angewendet wird. Das Standardschema lautet `Recipients(nms)`.

1. Definieren Sie die Regel für den Filter. Zum Beispiel Profile, die älter als 30 sind.

   ![Filterregel für Profile, die älter als 30 ](assets/filter-30+.png){zoomable="yes"}

1. Speichern Sie Ihre Änderungen.

   ![Neue gespeicherte Filterschnittstelle](assets/new-filter.png){zoomable="yes"}

Der Filter wird zur Liste der vordefinierten Filter hinzugefügt. Sie können den Filter bei Bedarf als Favorit speichern. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

## Speichern des Filters als Favorit {#fav-filter}

Aktivieren Sie beim Erstellen eines vordefinierten Filters die Option **Als Favorit speichern**, um diesen vordefinierten Filter in Ihren Favoriten anzuzeigen.

Wenn ein Filter als Favorit gespeichert wird, steht er allen Benutzenden im Abschnitt **Favoritenfilter** der Filtererstellungsliste zur Verfügung, wie unten dargestellt:

![Abschnitt „Favoritenfilter“](assets/predefined-filters-favorite.png){zoomable="yes"}{width="30%" align="left"}

## Verwenden eines vordefinierten Filters {#use-predefined-filter}

Vordefinierte Filter sind beim Definieren von Regeleigenschaften verfügbar. Um auf vordefinierte Filter zuzugreifen, wählen **die Option Benutzerdefinierter Filter** aus der Dropdown-Liste des Abfrage-Modellierers aus.

Greifen Sie auf die vollständige Liste der für den aktuellen Kontext verfügbaren vordefinierten Filter zu und verwenden Sie Tastaturbefehle **Abschnitt &quot;**&quot; der Dropdown-Liste. Weitere Informationen zu Favoriten finden Sie in [diesem Abschnitt](#fav-filter).

Gehen Sie wie folgt vor, um beispielsweise eine Zielgruppe aus einem vordefinierten Filter zu erstellen:

1. Durchsuchen Sie den Eintrag **Zielgruppen** im linken Menü und klicken Sie auf die Schaltfläche **Zielgruppe erstellen** in der oberen linken Ecke der Zielgruppenliste.
1. Geben Sie den Namen der Zielgruppe ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen**.
1. Wählen Sie die Aktivität **Abfrage** aus und klicken Sie im rechten Fenster auf die Schaltfläche **Zielgruppe erstellen**.

   ![Zielgruppen-Benutzeroberfläche erstellen](assets/build-audience-from-filter.png){zoomable="yes"}

1. Wählen Sie über die Schaltfläche zum **Auswählen oder Speichern von Filtern** die Option **Benutzerdefinierten Filter auswählen** aus.

   ![Benutzerdefinierte Filteroption auswählen](assets/build-audience-select-custom-filter.png){zoomable="yes"}

1. Navigieren Sie zum vordefinierten Filter, der zum Erstellen der Zielgruppe verwendet werden soll, wählen Sie ihn aus und bestätigen Sie die Wahl.

   ![Oberfläche der vordefinierten Filterliste](assets/build-audience-filter-list.png){zoomable="yes"}

1. Überprüfen Sie die Regeleigenschaften für diesen Filter und bestätigen Sie sie.

   Der Filter wird jetzt als Abfrage in der **Abfrage**-Aktivität genutzt.

   ![Abfrageaktivität mit vordefiniertem Filter](assets/build-audience-confirm.png){zoomable="yes"}

1. Speichern Sie Ihre Änderungen und klicken Sie auf die Schaltfläche **Starten**, um die Zielgruppe zu erstellen und in der Zielgruppenliste verfügbar zu machen.

## Verwalten Ihrer vordefinierten Filter {#manage-predefined-filter}

Alle vordefinierten Filter werden im dedizierten Eintrag des linken Navigationsmenüs gruppiert.

![Liste der vordefinierten Filter](assets/list-of-filters.png){zoomable="yes"}

Aus dieser Liste können Sie einen neuen Filter erstellen, wie oben beschrieben, und die unten aufgeführten Aktionen durchführen:

* Bearbeiten Sie einen vorhandenen Filter und ändern Sie dessen Regeln und Eigenschaften.
* einen vordefinierten Filter duplizieren
* einen vordefinierten Filter löschen

Sie können beim Erstellen Ihrer Zielgruppen auch einen vordefinierten Filter als Favoriten für den Schnellzugriff hinzufügen. Weiterführende Informationen finden Sie in [diesem Abschnitt](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->