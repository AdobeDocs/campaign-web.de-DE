---
audience: end-user
title: Erste Schritte mit Kampagnen
description: Erfahren Sie, wie Sie mit kanalübergreifenden Kampagnen beginnen
badge: label="Beta"
source-git-commit: 1bbbcd0ad2e83bad2e35c28184d13a63da77c081
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 77%

---


# Zugreifen auf und Verwalten von Kampagnen{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Kampagnenzeitplan"
>abstract="Legen Sie Ihren Kampagnenzeitplan fest oder ändern Sie ihn."

Um eine neue Kampagne zu erstellen oder bestehende Kampagnen zu verwalten, klicken Sie im linken Navigationsbereich auf das Menü **[!UICONTROL Kampagnen]**.

## Kampagnenliste {#access-campaigns}

In der Kampagnenliste stehen zwei Registerkarten zur Verfügung:

* Die Registerkarte **Durchsuchen** enthält alle vorhandenen Kampagnen. Sie können auf eine Kampagne klicken, um ihr Dashboard zu öffnen, oder eine neue Kampagne erstellen, indem Sie auf die Schaltfläche **Kampagne erstellen** klicken. Weitere Informationen finden Sie in [diesem Abschnitt](create-campaigns.md#create-campaigns).

* Auf der Registerkarte **Vorlagen** sind alle verfügbaren Kampagnenvorlagen aufgeführt. Sie können eine vorhandene Vorlage anzeigen oder eine neue erstellen. [Weitere Informationen](#manage-campaign-templates)

![Liste der Kampagnen](assets/campaign-list.png)

Standardmäßig enthält jede Kampagne in der Liste verschiedene Informationen, etwa zum aktuellen Status, zum Erstellungsdatum und zum letzten Änderungszeitpunkt.

Sie können die angezeigten Spalten anpassen, indem Sie auf das Symbol **Spalte für ein benutzerdefiniertes Layout konfigurieren** in der oberen rechten Ecke der Liste klicken. Auf diese Weise können Sie der Liste zusätzliche Informationen hinzufügen. Darüber hinaus stehen eine Suchleiste und Filter zur Verfügung, um die Suche innerhalb der Liste zu erleichtern. [Weitere Informationen](../get-started/user-interface.md#list-screens).

Sie können beispielsweise nach Ihrem Kampagnenkalender filtern. Öffnen Sie das Panel „Filter“ und verwenden Sie den Abschnitt **Anfangsdatum – Enddatum**:

![Kampagnenfilter](assets/campaign-filter-on-dates.png)

## Kampagnen-Dashboard{#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Liste der Sendungen in der Kampagne"
>abstract="Die Registerkarte **Sendungen** listet jeden mit der Kampagne verbundenen Versand auf. Klicken Sie auf den Namen eines Versands, um ihn zu bearbeiten. Verwenden Sie die Schaltfläche Versand erstellen , um einen neuen Versand für diese Kampagne hinzuzufügen."

Klicken Sie in der Kampagnenliste auf der Registerkarte **Durchsuchen** auf eine Kampagne, um deren Details anzuzeigen.

![Kampagnen-Dashboard](assets/campaign-dashboard.png)

Der Status und der Zeitplan der Kampagne werden oben im Bildschirm angezeigt. Über das Symbol **Kampagneneinstellungen konfigurieren** können Sie die Eigenschaften der Kampagne ändern, die bei der Erstellung der Kampagne definiert wurden. Es stehen drei Schaltflächen zur Verfügung, mit denen Sie Protokolle anzeigen, Berichte erstellen, die Kampagne duplizieren oder sie löschen können. Siehe diesen [Abschnitt](create-campaigns.md#create-campaigns)

Zwei Registerkarten sind verfügbar:

* Die Registerkarte **Workflows** enthält alle mit der Kampagne verknüpften Workflows. In dieser Registerkarte können Sie auch einen neuen Workflow innerhalb der Kampagne erstellen. Siehe diesen [Abschnitt](create-campaigns.md#create-campaigns).

* Die Registerkarte **Sendungen** listet jeden mit der Kampagne verbundenen Versand auf. Sie können auch einen neuen Versand innerhalb der Kampagne erstellen. Weitere Informationen finden Sie in [diesem Abschnitt](create-campaigns.md#create-campaigns).

## Duplizieren und Löschen einer Kampagne

Sie können eine Kampagne duplizieren oder löschen:

* Klicken Sie in der Kampagnenliste auf die Schaltfläche mit den Auslassungspunkten und wählen Sie **Duplizieren** oder **Löschen**.
* Klicken Sie in der Kampagne selbst auf die Schaltfläche **Mehr** und wählen Sie dann **Duplizieren** oder **Löschen**.

>[!NOTE]
>
>Auf der Registerkarte **Sendungen** werden alle mit der Kampagne verbundenen Sendungen angezeigt. Sendungen, die in einem Workflow erstellt wurden, können dort jedoch nicht gelöscht werden. Um einen im Rahmen eines Workflows erstellten Versand zu löschen, ist die Löschung der Versandaktivität aus dem Workflow erforderlich. [Weitere Informationen](../msg/gs-messages.md#delivery-delete).

## Verwenden von Kampagnenvorlagen{#manage-campaign-templates}

Kampagnenvorlagen enthalten vorkonfigurierte Einstellungen, die zur Erstellung neuer Workflows wiederverwendet werden können. Für die ersten Schritte steht Ihnen eine Reihe integrierter Vorlagen zur Verfügung. Sie können Ihre Kampagnenvorlagen erstellen und konfigurieren und dann Kampagnen aus diesen Vorlagen erstellen.

Eine Kampagnenvorlage kann die folgenden Informationen speichern:

* der Kampagne **Eigenschaften** und **Zeitplan** settings
* Workflow-Vorlagen
* Versandvorlagen

Gehen Sie wie folgt vor, um eine Kampagnenvorlage zu erstellen:

1. Klicken Sie auf **[!UICONTROL Kampagnen]** Menü, navigieren Sie zum **Vorlagen** und klicken Sie auf die **[!UICONTROL Vorlage erstellen]** Schaltfläche.
1. Wählen Sie die zu verwendende **Vorlage** und geben Sie eine Bezeichnung für die Kampagne ein. Auf diese Weise können Sie Ihre neue Vorlage auf einer bereits erstellten Vorlage basieren.
1. Bei Bedarf können Sie die folgenden **zusätzlichen Optionen** ändern: interner Name, Ordner, Zuweisung, Beschreibung und Art.
1. Definieren Sie den **Zeitplan** für Ihre Kampagne. Erfahren Sie, wie Sie den Kampagnenkalender in [diesem Abschnitt](create-campaigns.md#campaign-schedule)
1. Wählen Sie **Erstellen** aus.
1. Fügen Sie Ihrer Kampagne Workflows und Versandvorlagen hinzu.
