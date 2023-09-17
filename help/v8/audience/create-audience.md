---
audience: end-user
title: Audiences erstellen
description: Erfahren Sie, wie Sie Zielgruppen im Adobe Campaign Web erstellen
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# Audiences erstellen {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Zielgruppen"
>abstract="Auf diesem Bildschirm können Sie Zielgruppen erstellen und in einer visuellen Arbeitsfläche kombinieren. Hinzufügen verschiedener Workflow-Aktivitäten, z. B. **Aufspaltung** oder **Ausschließen** , um neue und erweiterte Zielgruppen zu erstellen."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Zielgruppeneinstellungen"
>abstract="Geben Sie den Namen der Audience und weitere Optionen ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen** Schaltfläche."

Mit Campaign Web können Sie neue Zielgruppen in einer Arbeitsfläche für visuelle Workflows erstellen. Sie können nicht nur von Grund auf eine einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppen zu verfeinern. Sie können beispielsweise mehrere Zielgruppen in eine einzelne Zielgruppe einteilen, Zielgruppen mit externen Attributen anreichern oder eine bestimmte Zielgruppe in mehrere Zielgruppen unterteilen.

Nachdem Sie Ihren Workflow erstellt haben, werden die resultierenden Zielgruppen automatisch in der Campaign-Datenbank und den bereits vorhandenen gespeichert. Diese Zielgruppen können dann in Kampagnen oder eigenständigen Sendungen ausgewählt werden.

Die wichtigsten Schritte zum Erstellen einer Audience sind:

1. Erstellen Sie einen Zielgruppen-Workflow.
1. Konfigurieren Sie die Aktivität Audience erstellen , um die Datenbank entsprechend Ihren Anforderungen abzufragen.
1. Fügen Sie Workflow-Aktivitäten hinzu, um Ihre Audience zu verfeinern (optional).
1. Konfigurieren Sie die Aktivität Audience-Speicherung .
1. Führen Sie den Workflow aus, um die resultierenden Audiences in der Datenbank zu speichern.


## Erstellen der ersten Zielgruppe {#create}

Gehen Sie wie folgt vor, um eine Audience zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Zielgruppen]** und klicken Sie auf **[!UICONTROL Zielgruppe erstellen]** -Schaltfläche oben rechts.
1. Geben Sie einen Titel für Ihre Zielgruppe an.
1. Erweitern Sie die **[!UICONTROL Zusätzliche Optionen]** Abschnitt zur Konfiguration der erweiterten Zielgruppenparameter.

   Standardmäßig werden Zielgruppen im **[!UICONTROL Profile und Zielgruppen]** / **[!UICONTROL Listen]** Explorer-Menü. Sie können den standardmäßigen Speicherort mithilfe des **[!UICONTROL Ordner]** -Feld.

   ![](assets/audiences-settings.png)

1. Nachdem Sie die Zielgruppeneinstellungen konfiguriert haben, klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe erstellen]** Schaltfläche.

1. Es wird eine Arbeitsfläche mit zwei Standardaktivitäten angezeigt:

   * **[!UICONTROL Audience erstellen]**: Dies ist der Ausgangspunkt Ihres Workflows, mit dem Sie eine Audience erstellen und diese als Grundlage für Ihren Workflow verwenden können. [Erfahren Sie, wie Sie eine Aktivität vom Typ Audience erstellen konfigurieren](../workflows/activities/build-audience.md)

   * **[!UICONTROL Audience-Speicherung]**: Dies ist der letzte Schritt in Ihrem Workflow, mit dem Sie die Ergebnisse als neue Zielgruppe speichern können. [Erfahren Sie, wie Sie eine Audience-Speicherung-Aktivität konfigurieren](../workflows/activities/save-audience.md)

1. Wenn Sie nach dem **[!UICONTROL Audience erstellen]** Aktivität können Sie so viele Aktivitäten wie nötig in Ihren Workflow einfügen. Weiterführende Informationen zur Konfiguration von Workflow-Aktivitäten finden Sie im Abschnitt [Dokumentation zu Workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktivitäten stehen nicht zur Verwendung in Zielgruppen-Workflows zur Verfügung.

   ![](assets/audience-creation-canvas.png)

1. Wenn Ihr Workflow fertig ist, klicken Sie auf **[!UICONTROL Starten]** um es auszuführen.

1. Der Workflow wird im **[!UICONTROL Workflows]** Liste, während die resultierenden Zielgruppen in der **[!UICONTROL Zielgruppen]** Liste. [Erfahren Sie, wie Sie Audiences überwachen und verwalten.](access-audiences.md)

## Beispiel für Zielgruppen-Workflow {#example}

Das folgende Beispiel zeigt einen Zielgruppen-Workflow, der so konfiguriert ist, dass weibliche Kunden, die in New York leben, angesprochen werden und zwei neue Zielgruppen erstellt werden, je nach Schwerpunkt auf Yoga oder Running-Ausrüstung. Die beiden Zielgruppen werden um zusätzliche Informationen zu den Käufen der Kunden erweitert.

SCREENSHOT HINZUFÜGEN

1. Die Aktivität Audience erstellen dient der Bestimmung aller in New York lebenden weiblichen Profile.
1. Die Aktivität Anreicherung reichert die Zielgruppe mit Attributen aus der Verkauf -Tabelle an.
1. Die Aktivität Aufspaltung unterteilt den Workflow in zwei Pfade, die auf den Zielgruppen der Kunden basieren.
1. Die Aktivitäten Audience-Speicherung am Ende jedes Pfades zum Speichern der einzelnen Audience in der Datenbank.
