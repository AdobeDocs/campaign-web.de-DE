---
audience: end-user
title: Audiences erstellen
description: Erfahren Sie, wie Sie Zielgruppen im Adobe Campaign Web erstellen
badge: label="Beta"
source-git-commit: 44a280446f9e7f801607dd40326b56fd79ec34e9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---


# Audiences erstellen {#create-audiences}

Mit Campaign Web können Sie Workflows erstellen, mit denen Sie bestehende Audiences in einer visuellen Arbeitsfläche kombinieren und verschiedene Aktivitäten (Aufspaltung, Ausschluss..) nutzen können, um neue Zielgruppen zu erstellen.

Danach werden die resultierenden Zielgruppen zusammen mit vorhandenen Zielgruppen im Campaign Web gespeichert und können in eigenständigen Sendungen oder Kampagnen genutzt werden, um Zielgruppen anzusprechen.

## Erstellen der ersten Zielgruppe {#create}

Gehen Sie wie folgt vor, um eine Audience zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Zielgruppen]** Menü und klicken Sie **[!UICONTROL Zielgruppe erstellen]** in der oberen rechten Ecke.
1. Geben Sie einen Titel für die Zielgruppe an.
1. Erweitern Sie den Abschnitt Zusätzliche Optionen , um erweiterte Parameter für die Audience zu konfigurieren.

   >[!NOTE]
   >
   >Standardmäßig werden Zielgruppen im Explorer-Menü Profile und Zielgruppen/Listen erstellt. Sie können den standardmäßigen Speicherort im **[!UICONTROL Ordner]** -Feld.

1. Klicken Sie nach der Konfiguration der Zielgruppeneinstellungen auf **[!UICONTROL Zielgruppe erstellen]** Schaltfläche.

1. Es wird eine Arbeitsfläche mit zwei Standardaktivitäten angezeigt:

   * **[!UICONTROL Audience erstellen]**: der Ausgangspunkt Ihres Workflows. Mithilfe dieser Aktivität können Sie eine oder mehrere Zielgruppen als Grundlage für Ihren Workflow auswählen.
   * **[!UICONTROL Audience-Speicherung]**: der letzte Schritt Ihres Workflows. Mit dieser Aktivität können Sie das Ergebnis Ihres Workflows in einer neuen Audience speichern.

1. Konfigurieren Sie Ihren Workflow, indem Sie beliebig viele Aktivitäten hinzufügen. Weiterführende Informationen zur Konfiguration der verschiedenen Aktivitäten finden Sie im Abschnitt [Dokumentation zu Workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktivitäten stehen nicht zur Verwendung in Zielgruppen-Workflows zur Verfügung.

   ![](assets/audience-creation-canvas.png)

1. Wenn Ihr Workflow fertig ist, klicken Sie auf **[!UICONTROL Starten]** um es auszuführen.

1. Der Workflow wird im **[!UICONTROL Workflows]** und die resultierenden Zielgruppen in der **[!UICONTROL Zielgruppen]** Liste. [Erfahren Sie, wie Sie auf Zielgruppen zugreifen können](access-audiences.md)
