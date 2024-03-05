---
audience: end-user
title: Erste Schritte mit Kampagnen
description: Erfahren Sie, wie Sie mit kanalübergreifenden Kampagnen beginnen
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: ht
source-wordcount: '719'
ht-degree: 100%

---

# Zugreifen auf und Verwalten von Kampagnen{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Kampagnenzeitplan"
>abstract="Legen Sie Ihren Kampagnenzeitplan fest oder ändern Sie ihn."

Um auf Ihre Kampagnen zuzugreifen und sie zu verwalten, klicken Sie auf das Menü **[!UICONTROL Kampagnen]** in der linken Navigation.

## Kampagnenliste {#access-campaigns}

In der Kampagnenliste stehen zwei Registerkarten zur Verfügung:

* Die Registerkarte **Durchsuchen** enthält alle vorhandenen Kampagnen. Sie können auf eine Kampagne klicken, um ihr Dashboard zu öffnen, oder eine neue Kampagne erstellen, indem Sie auf die Schaltfläche **Kampagne erstellen** klicken. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

* Auf der Registerkarte **Vorlagen** sind alle verfügbaren Kampagnenvorlagen aufgeführt. Sie können eine vorhandene Vorlage anzeigen oder eine neue erstellen. [Weitere Informationen](#manage-campaign-templates)

![Kampagnenliste](assets/campaign-list.png)

Standardmäßig enthält jede Kampagne in der Liste verschiedene Informationen, etwa zum aktuellen Status, zum Start- und Enddatum, zum Erstellungsdatum und zum Zeitpunkt der letzten Änderung.

Sie können die angezeigten Spalten anpassen, indem Sie auf das Symbol **Spalte für ein benutzerdefiniertes Layout konfigurieren** in der oberen rechten Ecke der Liste klicken. So können Sie Spalten hinzufügen oder entfernen und Informationen in der Kampagnenliste neu anordnen.

Darüber hinaus stehen eine Suchleiste und Filter zur Verfügung, um die Suche innerhalb der Liste zu erleichtern. [Weitere Informationen](../get-started/user-interface.md#list-screens).

Sie können beispielsweise nach Ihrem Kampagnenkalender filtern. Öffnen Sie das Panel „Filter“ und verwenden Sie den Abschnitt **Anfangsdatum – Enddatum**:

![Kampagnenfilter](assets/campaign-filter-on-dates.png)

## Kampagnen-Dashboard {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Liste der Sendungen in der Kampagne"
>abstract="Die Registerkarte **Sendungen** listet jeden mit der Kampagne verbundenen Versand auf. Klicken Sie auf den Namen eines Versands, um ihn zu bearbeiten. Verwenden Sie die Schaltfläche „Versand erstellen“, um einen neuen Versand für diese Kampagne hinzuzufügen."

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Workflow-Liste in einer Kampagne"
>abstract="Workflow-Liste in einer Kampagne"

Klicken Sie in der Kampagnenliste auf der Registerkarte **Durchsuchen** auf den Namen einer Kampagne, um deren Details anzuzeigen.

![Kampagnen-Dashboard](assets/campaign-dashboard.png)

Der Status und der Zeitplan der Kampagne werden oben im Bildschirm angezeigt. Sie können die Schaltfläche **Einstellungen** verwenden, um die Eigenschaften Ihrer Kampagne zu aktualisieren, z. B. den Titel, den Ordner und die Beschreibung. Sie können die Planung Ihrer Kampagne auch über den Einstellungsbildschirm ändern. Weiterführende Informationen zur Kampagnenplanung finden Sie in [diesem Abschnitt](create-campaigns.md#campaign-schedule).

Verwenden Sie auf dem Kampagnen-Dashboard die Schaltflächen **Protokolle** und **Berichte**, um Ihre Kampagne zu überwachen. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

Für jede Kampagne zeigt das Dashboard zwei Hauptregisterkarten: „Workflows“ und „Sendungen“.

* Die Registerkarte **Workflows** listet alle mit der Kampagne verknüpften Workflows auf. Auf dieser Registerkarte können Sie auch einen neuen Workflow innerhalb der Kampagne erstellen. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

* Die Registerkarte **Sendungen** listet alle in der aktuellen Kampagne erstellten Sendungen auf. Sie können auch einen neuen Versand innerhalb der Kampagne erstellen. Weitere Informationen finden Sie in diesem [Abschnitt](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>Auf der Registerkarte **Sendungen** werden alle mit der Kampagne verbundenen Sendungen angezeigt. Sendungen, die in einem Workflow erstellt wurden, können dort jedoch nicht gelöscht werden. Um einen im Rahmen eines Workflows erstellten Versand zu löschen, ist die Löschung der Versandaktivität aus dem Workflow erforderlich. [Weitere Informationen](../msg/gs-messages.md#delivery-delete).


## Löschen einer Kampagne {#campaign-delete}

Sie haben zwei Möglichkeiten, eine Kampagne zu löschen:

* Klicken Sie in der Kampagnenliste auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Löschen** aus.

  ![Löschen einer Kampagne aus der Kampagnenliste](assets/delete-a-campaign-from-list.png)

* Klicken Sie in der Kampagne selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Löschen** aus.

  ![Löschen einer Kampagne aus dem Kampagnen-Dashboard](assets/delete-a-campaign-from-dashboard.png)


## Duplizieren einer Kampagne {#campaign-duplicate}

Sie haben zwei Möglichkeiten, eine Kampagne zu duplizieren:

* Klicken Sie in der Kampagnenliste auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Duplizieren** aus.

* Klicken Sie in der Kampagne selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Duplizieren** aus.

Bestätigen Sie in beiden Fällen die Duplizierung, um die neue Kampagne zu erstellen. Der Titel der Kampagne lautet **Kopie von`<label of the initial campaign`**. Gehen Sie zu den Kampagneneinstellungen, um diesen Titel zu aktualisieren.


## Arbeiten mit Kampagnenvorlagen{#manage-campaign-templates}

Kampagnenvorlagen enthalten vorkonfigurierte Einstellungen, die zum Erstellen neuer Kampagnen wiederverwendet werden können. Für die ersten Schritte steht Ihnen eine Reihe integrierter Vorlagen zur Verfügung. Sie können Ihre Kampagnenvorlagen erstellen und konfigurieren und dann Kampagnen aus diesen Vorlagen erstellen.

Eine Kampagnenvorlage kann die folgenden Informationen speichern:

* die **Kampagneneinstellungen**
* die **Kampagnenplanung**
* Workflow-Vorlagen
* Versandvorlagen

Gehen Sie wie folgt vor, um eine Kampagnenvorlage zu erstellen:

1. Klicken Sie auf das Menü **[!UICONTROL Kampagnen]**, navigieren Sie zur Registerkarte **Vorlagen** und klicken Sie auf die Schaltfläche **[!UICONTROL Vorlage erstellen]**.
1. Wählen Sie die **Vorlage** aus, die verwendet werden soll. Auf diese Weise können Sie Ihre neue Vorlage auf der Grundlage einer zuvor erstellten Vorlage erstellen.
1. Geben Sie einen Titel für Ihre Vorlage an.
1. Bei Bedarf können Sie die folgenden **zusätzlichen Optionen** ändern: interner Name, Ordner, Zuweisung, Beschreibung und Art.
1. Definieren Sie den **Zeitplan** für Ihre Kampagne. Erfahren Sie in [diesem Abschnitt](create-campaigns.md#campaign-schedule), wie Sie Ihren Kampagnenzeitplan festlegen.
1. Klicken Sie auf **Erstellen**.
1. Fügen Sie Ihrer Kampagne Workflows und Versandvorlagen hinzu.
