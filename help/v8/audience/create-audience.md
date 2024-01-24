---
audience: end-user
title: Zielgruppen erstellen
description: Erfahren Sie, wie Sie Zielgruppen in Adobe Campaign Web erstellen.
badge: label="Eingeschränkte Verfügbarkeit"
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 1206da29f9987b55b957b6845e3dbf1e71ef03ed
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 57%

---

# Erstellen von Zielgruppen {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Zielgruppen-Komposition"
>abstract="Erstellen Sie neue Zielgruppen in einer visuellen Workflow-Arbeitsfläche. Sie können nicht nur von Grund auf eine einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppe zu präzisieren. Sie können beispielsweise mehrere Zielgruppen zu einer einzigen zusammenfassen, Ihre Zielgruppe mit externen Attributen anreichern oder eine Zielgruppe basierend auf Regeln Ihrer Wahl in mehrere Zielgruppen unterteilen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=de" text="Siehe Versionshinweise"

<!--TO REMOVE BELOW-->

>[!CONTEXTUALHELP]
>id="acw_homepage_rn1"
>title="Zielgruppen-Komposition"
>abstract="Erstellen Sie neue Zielgruppen in einer visuellen Workflow-Arbeitsfläche. Sie können nicht nur von Grund auf eine einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppe zu präzisieren. Sie können beispielsweise mehrere Zielgruppen zu einer einzigen zusammenfassen, Ihre Zielgruppe mit externen Attributen anreichern oder eine Zielgruppe basierend auf Regeln Ihrer Wahl in mehrere Zielgruppen unterteilen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=de" text="Siehe Versionshinweise"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Zielgruppen"
>abstract="Auf diesem Bildschirm kann die Liste aller Zielgruppen aufgerufen werden, die in Ihren Sendungen ausgewählt werden können. Auf **Erstellen** klicken, um mithilfe verschiedener Workflow-Aktivitäten, wie z. B. **Aufspaltung** oder **Ausschließen**, neue Zielgruppen in einer visuellen Arbeitsfläche zu erstellen."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Zielgruppeneinstellungen"
>abstract="Geben Sie den Namen der Zielgruppe und weitere Optionen ein und klicken Sie auf die Schaltfläche **Zielgruppe erstellen**."

Mit Campaign Web können Sie neue Zielgruppen in einer visuellen Workflow-Arbeitsfläche erstellen. Sie können nicht nur von Grund auf eine einfache Zielgruppe erstellen, sondern auch Workflow-Aktivitäten nutzen, um Ihre Zielgruppe zu präzisieren. Sie können beispielsweise mehrere Zielgruppen zu einer einzigen zusammenfassen, Ihre Zielgruppe mit externen Attributen anreichern oder eine Zielgruppe basierend auf Regeln Ihrer Wahl in mehrere Zielgruppen unterteilen.

Nachdem Sie Ihren Workflow erstellt haben, werden die resultierenden Zielgruppen automatisch in der Campaign-Datenbank zusammen mit den bereits vorhandenen Zielgruppen gespeichert. Diese Zielgruppen können dann in Workflows oder in eigenständigen Sendungen ausgewählt werden.

## Erstellen Ihrer ersten Zielgruppe {#create}

Gehen Sie wie folgt vor, um eine Zielgruppe zu erstellen:

1. Navigieren Sie zum Menü **[!UICONTROL Zielgruppen]** und klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe erstellen]** oben rechts.

1. Ein neuer Workflow wird automatisch erstellt, mit dem Sie Aktivitäten zur Erstellung Ihrer Audience kombinieren können. Die Arbeitsfläche enthält standardmäßig zwei Hauptaktivitäten:

   * Die &quot;Abfrage&quot; **[!UICONTROL Audience erstellen]** -Aktivität ist der Ausgangspunkt Ihres Workflows, über den Sie eine Audience erstellen und diese als Grundlage für Ihren Workflow verwenden können.

   * Die &quot;neue Zielgruppe&quot; **[!UICONTROL Audience-Speicherung]** -Aktivität stellt den letzten Schritt in Ihrem Workflow dar, mit dem Sie die Ergebnisse als neue Zielgruppe speichern können.

   ![](assets/create-audience-blank.png)

   >[!IMPORTANT]
   >
   >Zielgruppen-Workflows werden im **Workflows** neben Ihren anderen Campaign-Workflows. Sie sind speziell für die Erstellung von Zielgruppen konzipiert und können anhand ihrer vertikalen Arbeitsfläche identifiziert werden.

1. Für eine bessere Lesbarkeit empfehlen wir, den Namen des Workflows in den Workflow-Einstellungen zu ändern. **Titel** -Feld. [Erfahren Sie, wie Sie Workflow-Einstellungen konfigurieren](../workflows/workflow-settings.md)

1. Öffnen Sie die **[!UICONTROL Audience erstellen]** und verwenden Sie das Abfragemodell, um die Population zu definieren, die in Ihre Audience aufgenommen werden soll, indem Sie die in der Datenbank enthaltenen Daten filtern. [Erfahren Sie, wie Sie eine Aktivität „Zielgruppe erstellen“ konfigurieren können](../workflows/activities/build-audience.md)

1. Wenn Sie mit dem Workflow zusätzliche Vorgänge für die Zielpopulation durchführen möchten, fügen Sie so viele Aktivitäten wie erforderlich hinzu und verbinden Sie sie miteinander. Weiterführende Informationen zur Konfiguration von Workflow-Aktivitäten finden Sie in der [Dokumentation zu Workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanalaktivitäten stehen nicht zur Verwendung in Zielgruppen-Workflows zur Verfügung.

   ![](assets/audience-creation-canvas.png)

1. Konfigurieren Sie die Aktivität **[!UICONTROL Zielgruppe speichern]**, um anzugeben, wie die zuvor im Workflow berechnete Population gespeichert werden soll. [Erfahren Sie, wie Sie eine Aktivität „Zielgruppe speichern“ konfigurieren können](../workflows/activities/save-audience.md)

1. Wenn Ihr Workflow bereit ist, klicken Sie auf **[!UICONTROL Starten]**, um ihn auszuführen.

Der Workflow wird im **[!UICONTROL Workflows]** Liste, während die resultierenden Zielgruppen in der **[!UICONTROL Zielgruppen]** Liste mit dem in der **Audience-Speicherung** -Aktivität. Erfahren Sie, wie Sie Zielgruppen in überwachen und verwalten [diesem Abschnitt](manage-audience.md)

Jetzt können Sie diese Zielgruppe als Hauptzielgruppe eines Versands verwenden. [Weitere Informationen](add-audience.md)

## Beispiel für einen Zielgruppen-Workflow {#example}

Das folgende Beispiel zeigt einen Zielgruppen-Workflow, der so konfiguriert ist, dass Kundinnen, die in New York leben, ausgewählt werden und je nach ihrem letzten Kauf (Joga- oder Laufkleidung) zwei neue Zielgruppen erstellt werden.

![](assets/audiences-example.png)

1. Die Aktivität **[!UICONTROL Zielgruppe erstellen]** richtet sich an alle in New York lebenden weiblichen Profile.
1. Die Aktivität **[!UICONTROL Anreicherung]** erweitert die Zielgruppe um Informationen aus der Tabelle „Käufe“, um zu ermitteln, welcher Produkttyp von den Kundinnen gekauft wurde.
1. Die Aktivität **[!UICONTROL Aufspaltung]** unterteilt den Workflow in zwei Pfade, die auf dem aktuellen Kauf der Kundinnen basieren.
1. Die Aktivitäten **[!UICONTROL Zielgruppe speichern]** am Ende jedes Pfads erstellen zwei neue Zielgruppen in der Datenbank, einschließlich der in jedem Pfad berechneten Population.

## Bearbeiten einer Zielgruppe {#edit}

Sie können eine aus einem Workflow generierte Audience bei Bedarf ändern, indem Sie den entsprechenden Workflow erneut ausführen. Auf diese Weise können Sie Zielgruppendaten mühelos aktualisieren oder die Zielgruppe verfeinern, indem Sie die Abfrage an Ihre Anforderungen anpassen.

1. Navigieren Sie zum **Zielgruppen** und öffnen Sie die Zielgruppe, die Sie bearbeiten möchten.
1. Im **Übersicht** Registerkarte, die **Letzter Workflow** enthält einen Link zum Workflow, der zur Erstellung der Audience verwendet wird. Klicken Sie darauf, um auf den Workflow zuzugreifen.
1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie auf die **Starten** Schaltfläche, um den Workflow erneut auszuführen. Nach Abschluss des Workflows wird die aus dem Workflow resultierende Audience automatisch mit den neuesten Workflow-Ergebnissen aktualisiert.

Standardmäßig ersetzt die erneute Ausführung eines Zielgruppen-Workflows den gesamten Inhalt der Audience durch neue Daten, wodurch frühere Daten verloren gehen.

Wenn Sie die vorhandenen Zielgruppenergebnisse nicht ersetzen möchten, konfigurieren Sie die **Audience-Speicherung** Aktivitäten an Ihre Anforderungen anzupassen. Sie können beispielsweise die **Zielgruppenbezeichnung** um die neuen Ergebnisse in einer neuen Audience zu speichern oder die neuen Ergebnisse zum vorhandenen Audience-Inhalt hinzuzufügen, ohne vorherige Daten zu löschen. [Erfahren Sie, wie Sie die Aktivität Audience-Speicherung konfigurieren](../workflows/activities/save-audience.md)

![](assets/edit-audience-save.png)
