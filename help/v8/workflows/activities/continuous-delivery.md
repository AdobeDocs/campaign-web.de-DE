---
audience: end-user
title: Verwenden einer Workflow-Aktivität „Versand (fortlaufend)“
description: Erfahren Sie, wie Sie die Workflow-Aktivität „Versand (fortlaufend)“ verwenden
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
TQID: https://experienceleague.adobe.com/uWGhvUmHdS0ixFI4d-uEPgpxSnZoOwNRMbn8aZfqA98
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 242
ht-degree: 100%

---

# Versand (fortlaufend) {#continuous-delivery}

Die Aktivität **Versand (fortlaufend)** ermöglicht das Hinzufügen neuer Empfänger bzw. Empfängerinnen zu einem bestehenden Versand. Bei diesem Versandtyp muss nicht jedes Mal ein neuer Versand erstellt werden, was ihn effizienter für Warnhinweise für geringes Volumen oder Benachrichtigungen macht, die bei Bedarf gesendet werden.

Bei einem fortlaufenden Versand wird eine einzige Versandinstanz erstellt. Alle Versandlogs (broadLog) und Trackinglogs verweisen auf diesen Versand und vereinfachen das Monitoring und das Reporting.

## Konfigurieren der Aktivität „Versand (fortlaufend)“ {#configure}

1. Fügen Sie Ihrer Workflow-Arbeitsfläche eine Aktivität **Versand (fortlaufend)** hinzu.

   ![Screenshot zur Aktivität „Versand (fortlaufend)“](../assets/continuous-delivery.png){zoomable="yes"}

1. Geben Sie der Aktivität ein benutzerdefiniertes **[!UICONTROL Label]** (optional). Standardmäßig wird sie mit „Versand (fortlaufend)“ gekennzeichnet.

1. Klicken Sie neben dem Feld **[!UICONTROL Vorlage]** auf das Suchsymbol, um eine Versandvorlage auszuwählen. Nur Vorlagen (keine Standardsendungen) stehen zur Auswahl. Die Vorlage definiert den Versandkanal, den Inhalt und die Konfiguration.

1. Wählen Sie unter **[!UICONTROL Targeting-Optionen]** aus, wie die Zielpopulation definiert werden soll:

   * **[!UICONTROL Wird durch die Eingangsereignisse angegeben]**: Die Zielgruppe stammt aus der eingehenden Transition (aus Upstream-Aktivitäten wie „Zielgruppe erstellen“ oder „Inkrementelle Abfrage“). Dies ist die gängigste Option.

   * **[!UICONTROL Wird in der Versandvorlage angegeben]**: Das Ziel wird in der Vorlage selbst definiert.

   * **[!UICONTROL Datei wird durch das Eingangsereignis angegeben]**: Das Ziel wird über eine Datei bereitgestellt, die durch den Workflow übergeben wird.

Die Aktivität „Versand (fortlaufend)“ generiert automatisch eine ausgehende Transition, um den Workflow fortzusetzen.

## Verwandte Themen {#related}

* [Über Workflow-Aktivitäten](about-activities.md)
* [Automatischer Versand](automated-delivery.md)
* [E-Mail-, SMS-, Push- und Briefpost-Aktivitäten](channels.md)
* [Versandvorlagen](../../msg/delivery-template.md)
