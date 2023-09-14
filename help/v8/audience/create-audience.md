---
audience: end-user
title: Audiences erstellen
description: Erfahren Sie, wie Sie Zielgruppen im Adobe Campaign Web erstellen
badge: label="Beta"
source-git-commit: 1b17dcbdaadcbf45b2c26d9099e6d139143d253c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 1%

---


# Audiences erstellen {#create-audiences}

Mit Campaign Web können Sie Workflows erstellen, in denen Sie bestehende Audiences in einer visuellen Arbeitsfläche kombinieren können. Durch die Integration verschiedener Workflow-Aktivitäten wie Aufspaltung oder Ausschließen können Sie neue und erweiterte Zielgruppen erstellen.

Nachdem Sie Ihren Workflow erstellt haben, werden die resultierenden Zielgruppen automatisch im Campaign Web gespeichert und mit den bereits vorhandenen gespeichert. Diese Zielgruppen können dann in Kampagnen oder eigenständigen Sendungen ausgewählt werden.

Gehen Sie wie folgt vor, um eine Audience zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Zielgruppen]** und klicken Sie auf **[!UICONTROL Zielgruppe erstellen]** -Schaltfläche oben rechts.
1. Geben Sie einen Titel für Ihre Zielgruppe an.
1. Erweitern Sie die **[!UICONTROL Zusätzliche Optionen]** Abschnitt zur Konfiguration der erweiterten Zielgruppenparameter.

   Standardmäßig werden Zielgruppen im **[!UICONTROL Profile und Zielgruppen]** / **[!UICONTROL Listen]** Explorer-Menü. Sie können den standardmäßigen Speicherort mithilfe des **[!UICONTROL Ordner]** -Feld.

   ![](assets/audiences-settings.png)

1. Nachdem Sie die Zielgruppeneinstellungen konfiguriert haben, klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe erstellen]** Schaltfläche.

1. Es wird eine Arbeitsfläche mit zwei Standardaktivitäten angezeigt:

   * **[!UICONTROL Audience erstellen]**: Dies ist der Ausgangspunkt Ihres Workflows, mit dem Sie eine Audience erstellen und diese als Grundlage für Ihren Workflow verwenden können.
   * **[!UICONTROL Audience-Speicherung]**: Dies ist der letzte Schritt in Ihrem Workflow, mit dem Sie die Ergebnisse als neue Zielgruppe speichern können.

1. Passen Sie Ihren Workflow an, indem Sie beliebig viele Aktivitäten hinzufügen. Weiterführende Informationen zur Konfiguration von Workflow-Aktivitäten finden Sie im Abschnitt [Dokumentation zu Workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktivitäten stehen nicht zur Verwendung in Zielgruppen-Workflows zur Verfügung.

   ![](assets/audience-creation-canvas.png)

1. Wenn Ihr Workflow fertig ist, klicken Sie auf **[!UICONTROL Starten]** um es auszuführen.

1. Der Workflow wird im **[!UICONTROL Workflows]** Liste, während die resultierenden Zielgruppen in der **[!UICONTROL Zielgruppen]** Liste. [Erfahren Sie, wie Sie Audiences überwachen und verwalten.](access-audiences.md)
