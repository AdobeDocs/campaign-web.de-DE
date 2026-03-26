---
audience: end-user
title: Verwenden der Workflow-Aktivität „Fortlaufender Versand“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Fortlaufender Versand“ verwenden
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 17%

---

# Versand (fortlaufend) {#continuous-delivery}

Die Aktivität **Fortlaufender Versand** ermöglicht es Ihnen, einem bestehenden Versand neue Empfänger hinzuzufügen. Bei diesem Versandtyp muss nicht jedes Mal ein neuer Versand erstellt werden, was ihn effizienter für Warnhinweise für geringes Volumen oder Benachrichtigungen macht, die bei Bedarf gesendet werden.

Bei einem fortlaufenden Versand wird eine einzige Versandinstanz erstellt. Alle Versandlogs (broadLog) und Trackinglogs verweisen auf diesen Versand und vereinfachen die Überwachung und das Reporting.

## Konfigurieren der Aktivität Versand (fortlaufend) {#configure}

1. Fügen Sie Ihrer Workflow **Arbeitsfläche eine Aktivität** Fortlaufender Versand“ hinzu.

   ![Screenshot zur Aktivität „Fortlaufender Versand“](../assets/continuous-delivery.png){zoomable="yes"}

1. Geben Sie einen benutzerdefinierten **[!UICONTROL Titel]** für die Aktivität ein (optional). Standardmäßig wird sie mit „Fortlaufender Versand“ gekennzeichnet.

1. Klicken Sie neben dem Feld **[!UICONTROL Vorlage]** auf das Suchsymbol, um eine Versandvorlage auszuwählen. Es stehen nur Vorlagen (keine Standardsendungen) zur Auswahl. Die Vorlage definiert den Versandkanal, den Inhalt und die Konfiguration.

1. Wählen Sie unter **[!UICONTROL Zielgruppenoptionen]** aus, wie die Zielpopulation definiert werden soll:

   * **[!UICONTROL Durch eingehende Ereignisse angegeben]**: Die Zielgruppe stammt aus der eingehenden Transition (aus Upstream-Aktivitäten wie Zielgruppe aufbauen oder inkrementelle Abfrage). Dies ist die häufigste Option.

   * **[!UICONTROL Wird in der Versandvorlage angegeben]**: Die Zielgruppe wird in der Vorlage selbst definiert.

   * **[!UICONTROL Datei, die im Eingangsereignis angegeben ist]**: Das Ziel wird über eine Datei bereitgestellt, die durch den Workflow übergeben wird.

Die Aktivität Fortlaufender Versand generiert automatisch eine ausgehende Transition, um Ihren Workflow fortzusetzen.

## Verwandte Themen {#related}

* [Über Workflow-Aktivitäten](about-activities.md)
* [Automatischer Versand](automated-delivery.md)
* [E-Mail-, SMS-, Push- und Briefpost-Aktivitäten](channels.md)
* [Versandvorlagen](../../msg/delivery-template.md)
