---
audience: end-user
title: Erste Schritte mit der Angebotsverwaltung
description: Erfahren Sie, wie Sie Angebote in Adobe Campaign Web verwalten.
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: ht
source-wordcount: 763
ht-degree: 100%

---

# Erste Schritte mit der Angebotsverwaltung {#gs-offer-management}

Mit dieser Funktion können Sie Ihren Sendungen personalisierte Angebote hinzufügen und für jedes Profil in einem bestimmten Kontext das relevanteste Angebot präsentieren. Angebote können eine einfache Kommunikationsnachricht oder Werbeaktionen für ein oder mehrere Produkte sein. Basierend auf den Eignungsregeln und Prioritätsgewichtungen wählt das Angebotsmodul den besten Vorschlag aus.

In der Web-Benutzeroberfläche von Campaign können Sie Angebote durchgängig verwalten. Sie können Angebotsumgebungen erstellen und konfigurieren,Platzierungen gestalten, Ihren Angebotskatalog erstellen, Eignungsregeln festlegen, Angebotsinhalte bearbeiten und Angebote veröffentlichen.

Angebote werden den Empfangenden dann durch Sendungen auf der Grundlage von **Eignungsregeln** und **Prioritätsgewichtungen** unterbreitet, sodass für jedes Profil in einem bestimmten Kontext das beste Angebot ausgewählt wird.

>[!NOTE]
>
>Die Web-Benutzeroberfläche von Campaign konzentriert sich auf die häufigste Verwendung der Angebotsverwaltung. Erweiterte Konfigurationen sind weiterhin in der Campaign-Client-Konsole verfügbar. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=de){target="_blank"}.

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## Schlüsselkonzepte {#concepts}

Bevor Sie mit der Arbeit an Angeboten beginnen, machen Sie sich mit den wichtigsten beteiligten Objekten vertraut.

* **Angebotsumgebung** – Container, der einen Angebotskatalog und die zugehörigen Platzierungen enthält. Es gibt zwei Typen: die **Design**-Umgebung, in der Sie Angebote erstellen und konfigurieren, und die schreibgeschützte **[!UICONTROL Live]**-Umgebung, die die validierten und bereitgestellten Objekte enthält, die für den Versand verfügbar sind. [Weitere Informationen](offer-environment.md)

* **Platzierung** – Definiert, wo und wie ein Angebot bereitgestellt wird (E-Mail, Briefpost, SMS, Web-Empfang usw.). In der Platzierung sind die Inhaltsfelder aufgelistet, die im Angebot verwendet werden können, die Rendering-Funktion, mit der die Angebotsdarstellung erstellt wird, und die Speichereinstellungen, die den Vorschlagsstatus steuern. [Weitere Informationen](offer-space.md)

* **Angebotskatalog und Kategorien** – Angebote sind in einem hierarchischen Katalog mit **Kategorien** und Unterkategorien angeordnet. Jede Kategorie kann Eignungsregeln, Gültigkeitsdaten und **Anwendungsthemen** enthalten. In der Design-Umgebung steht eine Standardkategorie zur Verfügung, in der alle Angebote gesammelt werden.

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **Angebot** – Ein individuelles Angebot mit eigenem Eignungszeitraum, Zielgruppenfilter, Gewichtung und Inhalt. Angebote werden validiert und bereitgestellt, bevor sie den Empfangenden vorgelegt werden können. [Weitere Informationen](create-offer.md)

* **Angebotsvorschlag** – Das Ergebnis der Präsentation eines Angebots an einen Kontakt in einer bestimmten Platzierung (z. B. ein Banner auf einer Website, eine E-Mail oder eine SMS). Die Anzahl der Vorschläge pro Versand wird konfiguriert, wenn Sie [Angebote in einem Versand einrichten](../msg/offers.md).

* **Schlichtung** – Das Prinzip, nach dem das Angebotsmodul geeignete Angebote nach Priorität sortiert, um zu entscheiden, welche unterbreitet werden sollen. Die Schlichtung nutzt die Kriterien, die für die Kategorien, die Angebote und die Kontextangebote definiert sind.

## Ablauf der Angebotsverwaltung {#workflow}

Der typische durchgängige Ablauf in der Web-Benutzeroberfläche von Campaign ist wie folgt:

1. **Überprüfen der Einstellungen der Angebotsumgebung** – Überprüfen Sie die Einstellungen für Design/Live-Zuordnung, Eignung und Gewichtungsverwaltung. [Weitere Informationen](offer-environment.md)

1. **Erstellen einer Platzierung** – Definieren Sie die Inhaltsfelder, die Rendering-Funktion und die erweiterten Parameter, die Ihrem Kanal entsprechen. [Weitere Informationen](offer-space.md)

1. **Erstellen von Angeboten im Katalog** – Legen Sie den Eignungszeitraum, den Zielfilter, die Gewichtung und den Inhalt für jedes Angebot fest. [Weitere Informationen](create-offer.md)

1. **Validieren und Bereitstellen** – Senden Sie das Angebot zur Validierung, validieren Sie seinen Inhalt und seine Eignung und lassen Sie es dann vom Bereitstellungsprozess in der Live-Umgebung veröffentlichen. [Weitere Informationen](create-offer.md#approve-deploy)

1. **Hinzufügen des Angebots zu einem Versand** – Referenzieren Sie die Platzierung und die Vorschläge in Ihrem E-Mail-, SMS-, Push- oder Briefpost-Versand. [Weitere Informationen](../msg/offers.md)

## Aufrufen von Angeboten in der Web-Benutzeroberfläche {#access}

Angebote sind über das Menü **[!UICONTROL Angebote]** auf der linken Seite verfügbar. Von dort aus können Sie den Katalog durchsuchen, ein Angebot zur Bearbeitung öffnen und dessen Validierungs- und Bereitstellungsstatus überwachen.

![Screenshot des Menüs „Angebot“.](assets/offers-gs.png){zoomable="yes"}

Der Zugriff auf Angebotsumgebungen und Platzierungen erfolgt über den **[!UICONTROL Explorer]**, indem Sie zum entsprechenden Ordner navigieren.


## Ergänzungen nur für die Konsole {#console-complements}

Einige Angebotsfunktionen sind noch nicht in der Web-Benutzeroberfläche verfügbar und müssen weiterhin über die Client-Konsole konfiguriert werden.

* **Angebotssimulation** – Das Modul **Simulation**, mit dem Sie die Verteilung von Angeboten vor dem Versand testen können. Siehe [Angebotssimulation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=de#offer-simulation){target="_blank"}.

* Verwaltung **vordefinierter Filter** – Wiederverwendbare Filterregeln, die von jedem Angebot aus referenziert werden können. Siehe [Verwalten vordefinierter Filter](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html?lang=de){target="_blank"}.

* **Angebotsverfolgung** – Konfiguration des Tracking von Angebotsvorschlägen zur Erfassung des Vorschlagsverlaufs. Siehe [Tracking von Angebotsvorschlägen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html?lang=de){target="_blank"}.

* **Benutzerrollen** – Zuweisung der Rechte des bzw. der Angebotsverantwortlichen/des bzw. der Versandverantwortlichen. Siehe [Benutzende des Interaction-Moduls](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html?lang=de){target="_blank"}.

* **Best Practices und Schlichtungsregeln für Interaction**. Siehe [Best Practices für Campaign Interaction](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=de){target="_blank"}.

* **Reporting** – Dedizierte Angebots- und Vorschlagsberichte sind noch nicht in der Web-Benutzeroberfläche verfügbar.