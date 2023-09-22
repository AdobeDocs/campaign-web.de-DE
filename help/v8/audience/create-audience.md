---
audience: end-user
title: Erstellen und Verwalten von Zielgruppen
description: Erfahren Sie, wie Sie Zielgruppen im Adobe Campaign Web erstellen und verwalten
badge: label="Beta"
source-git-commit: ab445f332b62baa98f9f9e84a80cc336cd88efe0
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---


# Audiences erstellen {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Zielgruppen"
>abstract="Auf diesem Bildschirm können Sie die Liste aller Zielgruppen aufrufen, die in Ihren Sendungen ausgewählt werden können. Klicks **Erstellen** , um mithilfe verschiedener Workflow-Aktivitäten, wie z. B. **Aufspaltung** oder **Ausschließen**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Zielgruppeneinstellungen"
>abstract="Geben Sie den Namen der Audience und weitere Optionen ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen** Schaltfläche."

Mit Campaign Web können Sie neue Zielgruppen in einer Arbeitsfläche für visuelle Workflows erstellen. Sie können nicht nur von Grund auf eine einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppe zu verfeinern. Sie können beispielsweise mehrere Zielgruppen zu einer einzigen zusammenfassen, Ihre Zielgruppe mit externen Attributen anreichern oder eine Zielgruppe basierend auf Regeln Ihrer Wahl in mehrere Zielgruppen unterteilen.

Nachdem Sie Ihren Workflow erstellt haben, werden die resultierenden Zielgruppen automatisch in der Campaign-Datenbank und den bereits vorhandenen gespeichert. Diese Zielgruppen können dann in Kampagnen oder eigenständigen Sendungen ausgewählt werden.

## Erstellen der ersten Zielgruppe {#create}

Gehen Sie wie folgt vor, um eine Audience zu erstellen:

1. Navigieren Sie zum **[!UICONTROL Zielgruppen]** und klicken Sie auf **[!UICONTROL Zielgruppe erstellen]** -Schaltfläche oben rechts.
1. Geben Sie einen Titel für Ihre Zielgruppe an.
1. Erweitern Sie die **[!UICONTROL Zusätzliche Optionen]** Abschnitt zur Konfiguration der erweiterten Zielgruppenparameter.

   Standardmäßig werden Zielgruppen im **[!UICONTROL Profile und Zielgruppen]** / **[!UICONTROL Listen]** Explorer-Menü. Sie können den standardmäßigen Speicherort mithilfe des **[!UICONTROL Ordner]** -Feld.

   ![](assets/audiences-settings.png)

1. Nachdem Sie die Zielgruppeneinstellungen konfiguriert haben, klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe erstellen]** Schaltfläche. Es wird eine Arbeitsfläche mit zwei Standardaktivitäten angezeigt:

   * **[!UICONTROL Audience erstellen]**: Dies ist der Ausgangspunkt Ihres Workflows, mit dem Sie eine Audience erstellen und diese als Grundlage für Ihren Workflow verwenden können.

   * **[!UICONTROL Audience-Speicherung]**: Dies ist der letzte Schritt in Ihrem Workflow, mit dem Sie die Workflow-Ergebnisse als neue Zielgruppe speichern können.

1. Öffnen Sie die **[!UICONTROL Audience erstellen]** und verwenden Sie den Regel-Builder, um die Population zu definieren, die in Ihre Audience aufgenommen werden soll, indem Sie die in der Datenbank enthaltenen Daten filtern. [Erfahren Sie, wie Sie eine Aktivität vom Typ Audience erstellen konfigurieren](../workflows/activities/build-audience.md)

1. Wenn Sie zusätzliche Vorgänge für die Zielpopulation des Workflows durchführen möchten, fügen Sie so viele Aktivitäten wie erforderlich hinzu und verbinden Sie sie. Weiterführende Informationen zur Konfiguration von Workflow-Aktivitäten finden Sie im Abschnitt [Dokumentation zu Workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktivitäten stehen nicht zur Verwendung in Zielgruppen-Workflows zur Verfügung.

   ![](assets/audience-creation-canvas.png)

1. Konfigurieren Sie die **[!UICONTROL Audience-Speicherung]** -Aktivität, um anzugeben, wie die zuvor im Workflow berechnete Population gespeichert werden soll. [Erfahren Sie, wie Sie eine Audience-Speicherung-Aktivität konfigurieren](../workflows/activities/save-audience.md)

1. Wenn Ihr Workflow fertig ist, klicken Sie auf **[!UICONTROL Starten]** um es auszuführen.

Der Workflow wird im **[!UICONTROL Workflows]** Liste, während die resultierenden Zielgruppen in der **[!UICONTROL Zielgruppen]** Liste.

## Beispiel für Zielgruppen-Workflow {#example}

Das folgende Beispiel zeigt einen Zielgruppen-Workflow, der so konfiguriert ist, dass weibliche Kunden, die in New York leben, ausgewählt werden und je nach letztem Kauf (Yoga- oder Running-Gerät) zwei neue Zielgruppen erstellt werden.

![](assets/audiences-example.png)

1. Die **[!UICONTROL Audience erstellen]** Die Aktivität richtet sich an alle in New York lebenden weiblichen Profile.
1. Die **[!UICONTROL Anreicherung]** -Aktivität erweitert die Zielgruppe um Informationen aus der Verkauf -Tabelle, um zu ermitteln, welcher Produkttyp von den Kunden gekauft wurde.
1. Die **[!UICONTROL Aufspaltung]** -Aktivität unterteilt den Workflow in zwei Pfade, die auf dem aktuellen Kauf des Kunden basieren.
1. Die **[!UICONTROL Audience-Speicherung]** Aktivitäten am Ende jedes Pfads erstellen zwei neue Zielgruppen in die Datenbank, einschließlich der in jedem Pfad berechneten Population.

## Zielgruppen überwachen und verwalten {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Zielgruppenfehler"
>abstract="Zielgruppendaten sind nicht verfügbar. Warten Sie bis zum Ende der Workflow-Ausführung."

Die Liste der Zielgruppen, die im Campaign Web verwendet werden können, ist über den Link **[!UICONTROL Zielgruppen]** Menü.

![](assets/audiences-list.png)

Zielgruppen können aus mehreren Quellen stammen. Die **[!UICONTROL Origin]** gibt an, wo eine bestimmte Zielgruppe erstellt wurde:

* **[!UICONTROL Adobe Campaign]**: Diese Zielgruppen werden in der Adobe Campaign V8-Konsole erstellt. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=de){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Diese Zielgruppen werden in Adobe Experience Platform erstellt und mithilfe der Adobe-Quellen- und Zielintegration in Campaign Web integriert. Erfahren Sie, wie Sie diese Integration in [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign WebUI]**: Diese Zielgruppen werden mithilfe von Workflows für Campaign-Webzielgruppen erstellt. [Erfahren Sie, wie Sie Audiences erstellen](create-audience.md)

Um weitere Informationen zu einer Audience zu erhalten, öffnen Sie sie in der Liste. Die Eigenschaften der Audience werden zusammen mit der Anzahl der in der Audience enthaltenen Profile angezeigt. Sie können die Anzahl der Zielgruppen jederzeit mit der Funktion **[!UICONTROL berechnen]** Schaltfläche.

Die **[!UICONTROL Daten]** -Tab ermöglicht die Visualisierung der Profile, die Teil der Audience sind. Sie können diese Ansicht anpassen, indem Sie weitere Spalten hinzufügen oder erweiterte Filter nutzen, um die angezeigten Daten zu verfeinern.

![](assets/audiences-details.png)

Um eine Zielgruppe zu duplizieren oder zu löschen, klicken Sie auf die Schaltfläche **[!UICONTROL Mehr Aktionen]** in der Zielgruppenliste neben dem Zielgruppennamen oder im Bildschirm mit den Zielgruppendetails verfügbar.
