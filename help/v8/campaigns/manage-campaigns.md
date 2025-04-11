---
audience: end-user
title: Erste Schritte mit Kampagnen
description: Erfahren Sie, wie Sie mit kanalübergreifenden Kampagnen beginnen
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 68%

---

# Zugreifen auf und Verwalten von Kampagnen {#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Kampagnenzeitplan"
>abstract="Legen Sie Ihren Kampagnenzeitplan fest oder ändern Sie ihn."

Um auf Ihre Kampagnen zuzugreifen und sie zu verwalten, klicken Sie auf das Menü **[!UICONTROL Kampagnen]** in der linken Navigation.

## Kampagnenliste {#access-campaigns}

In der Kampagnenliste stehen zwei Registerkarten zur Verfügung:

* Die Registerkarte **Durchsuchen** enthält alle vorhandenen Kampagnen. Sie können auf eine Kampagne klicken, um ihr Dashboard zu öffnen, oder eine neue Kampagne erstellen, indem Sie auf die Schaltfläche **Kampagne erstellen** klicken. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

* Auf der Registerkarte **Vorlagen** sind alle verfügbaren Kampagnenvorlagen aufgeführt. Sie können eine vorhandene Vorlage anzeigen oder eine neue erstellen. [Weitere Informationen](#manage-campaign-templates)

![Beschreibung: Der Bildschirm der Kampagnenliste mit den Registerkarten Durchsuchen und Vorlagen sowie den Optionen zum Erstellen oder Anzeigen von Kampagnen](assets/campaign-list.png)

Standardmäßig enthält jede Kampagne in der Liste verschiedene Informationen, etwa zum aktuellen Status, zum Start- und Enddatum, zum Erstellungsdatum und zum Zeitpunkt der letzten Änderung.

Sie können die angezeigten Spalten anpassen, indem Sie auf das Symbol **Spalte für ein benutzerdefiniertes Layout konfigurieren** in der oberen rechten Ecke der Liste klicken. Auf diese Weise können Sie Spalten in der Kampagnenliste hinzufügen oder entfernen und Informationen neu anordnen.

Darüber hinaus stehen eine Suchleiste und Filter zur Verfügung, um die Suche innerhalb der Liste zu erleichtern. [Weitere Informationen](../get-started/user-interface.md#list-screens).

Sie können beispielsweise nach Ihrem Kampagnenkalender filtern. Öffnen Sie das Panel „Filter“ und verwenden Sie den Abschnitt **Anfangsdatum – Enddatum**:

![Beschreibung: Das Filterbedienfeld, das Optionen zum Filtern von Kampagnen nach Start- und Enddatum anzeigt](assets/campaign-filter-on-dates.png)

## Kampagnen-Dashboard {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Liste der Sendungen in der Kampagne"
>abstract="Die Registerkarte **Sendungen** listet jeden mit der Kampagne verbundenen Versand auf. Klicken Sie auf den Namen eines Versands, um ihn zu bearbeiten. Verwenden Sie die Schaltfläche „Versand erstellen“, um einen neuen Versand für diese Kampagne hinzuzufügen."

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Workflow-Liste in einer Kampagne"
>abstract="Die Registerkarte **Workflows** enthält alle mit der aktuellen Kampagne verknüpften Workflows."

Klicken Sie in der Kampagnenliste auf der Registerkarte **Durchsuchen** auf den Namen einer Kampagne, um deren Details anzuzeigen.

![Beschreibung: Das Dashboard der Kampagne mit Status, Zeitplan und Registerkarten für Workflows und Sendungen](assets/campaign-dashboard.png)

Der Status und der Zeitplan der Kampagne werden oben im Bildschirm angezeigt. Verwenden Sie die **Einstellungen**, um die Eigenschaften Ihrer Kampagne wie Titel, Ordner und Beschreibung zu aktualisieren. Sie können die Planung Ihrer Kampagne auch über den Einstellungsbildschirm ändern. Weiterführende Informationen zur Kampagnenplanung finden Sie in [diesem Abschnitt](create-campaigns.md#campaign-schedule).

Verwenden Sie auf dem Kampagnen-Dashboard die Schaltflächen **Protokolle** und **Berichte**, um Ihre Kampagne zu überwachen. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

Für jede Kampagne zeigt das Dashboard zwei Hauptregisterkarten: „Workflows“ und „Sendungen“.

* Auf **Registerkarte** Workflows“ werden alle mit der Kampagne verbundenen Workflows aufgelistet. Auf dieser Registerkarte können Sie auch einen neuen Workflow innerhalb der Kampagne erstellen. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

* Die Registerkarte **Sendungen** listet alle in der aktuellen Kampagne erstellten Sendungen auf. Sie können auch einen neuen Versand innerhalb der Kampagne erstellen. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>Auf der Registerkarte **Sendungen** werden alle mit der Kampagne verbundenen Sendungen angezeigt. Sendungen, die in einem Workflow erstellt wurden, können dort jedoch nicht gelöscht werden. Um einen im Rahmen eines Workflows erstellten Versand zu löschen, löschen Sie die Versandaktivität aus dem Workflow. [Weitere Informationen](../msg/gs-messages.md#delivery-delete).

## Löschen einer Kampagne {#campaign-delete}

Sie haben zwei Möglichkeiten, eine Kampagne zu löschen:

* Klicken Sie in der Kampagnenliste auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Löschen**.

  ![Beschreibung: Der Bildschirm der Kampagnenliste mit der Schaltfläche mit den Auslassungspunkten und der Option „Löschen“](assets/delete-a-campaign-from-list.png)

* Klicken Sie in der Kampagne selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Löschen**.

  ![Beschreibung: Der Bildschirm des Kampagnen-Dashboards mit der Schaltfläche Mehr und der Option Löschen ](assets/delete-a-campaign-from-dashboard.png)

## Duplizieren einer Kampagne {#campaign-duplicate}

Sie haben zwei Möglichkeiten, eine Kampagne zu duplizieren:

* Klicken Sie in der Kampagnenliste auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Duplizieren**.

* Klicken Sie in der Kampagne selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Duplizieren**.

Bestätigen Sie in beiden Fällen die Duplizierung, um die neue Kampagne zu erstellen. Der Titel der Kampagne lautet **Kopie von`<label of the initial campaign>`**. Gehen Sie zu den Kampagneneinstellungen, um diesen Titel zu aktualisieren.

## Arbeiten mit Kampagnenvorlagen {#manage-campaign-templates}

Kampagnenvorlagen enthalten vorkonfigurierte Einstellungen, die zur Erstellung neuer Kampagnen wiederverwendet werden können. Für die ersten Schritte steht Ihnen eine Reihe integrierter Vorlagen zur Verfügung. Sie können Ihre Kampagnenvorlagen erstellen und konfigurieren und dann Kampagnen aus diesen Vorlagen erstellen.

Eine Kampagnenvorlage kann die folgenden Informationen speichern:

* Die Kampagne **Einstellungen**
* Die Kampagne **Zeitplan**
* Workflow-Vorlagen
* Versandvorlagen

Gehen Sie wie folgt vor, um eine Kampagnenvorlage zu erstellen:

1. Klicken Sie auf das Menü **[!UICONTROL Kampagnen]**, navigieren Sie zur Registerkarte **Vorlagen** und klicken Sie auf die Schaltfläche **[!UICONTROL Vorlage erstellen]**.
1. Wählen Sie die **Vorlage** aus, die verwendet werden soll. Auf diese Weise können Sie Ihre neue Vorlage auf der Grundlage einer zuvor erstellten Vorlage erstellen.
1. Geben Sie einen Titel für Ihre Vorlage an.
1. Ändern Sie bei Bedarf die folgenden **Zusätzliche Optionen**: interner Name, Ordner, Zuweisung, Beschreibung und Art.
1. Definieren Sie den **Zeitplan** für Ihre Kampagne. Näheres dazu, wie Sie Ihren Kampagnenkalender festlegen, finden [ in diesem Abschnitt ](create-campaigns.md#campaign-schedule).
1. Klicken Sie auf **Erstellen**.
1. Fügen Sie Ihrer Kampagne Workflows und Versandvorlagen hinzu.