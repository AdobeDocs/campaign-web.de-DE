---
audience: end-user
product: campaign
title: C2PA-Metadaten im E-Mail- und Landingpage-Designer
description: Erfahren Sie, was mit C2PA-Metadaten passiert, die bereits an ein Bild angehängt sind, wenn es den E-Mail- und Landingpage-Designer in der Web-Benutzeroberfläche von Adobe Campaign durchläuft.
topic: Content Management
role: User
level: Beginner
source-git-commit: 645352d9e2ba12d5430ddf1b62852077344c3016
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 100%
---

# C2PA-Metadaten im E-Mail- und Landingpage-Designer {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**Auf dieser Seite:** Erfahren Sie, was mit C2PA-Metadaten passiert, die bereits an ein Bild angehängt sind, wenn es den E-Mail- und Landingpage-Designer in der Web-Benutzeroberfläche von Adobe Campaign durchläuft.

>[!ENDSHADEBOX]

>[!INFO]
>
>In Bezug auf die Transparenz generativer KI entstehen laufend neue Gesetze und Adobe arbeitet daran, die geltenden Anforderungen in allen Gerichtsbarkeiten zu erfüllen. C2PA-Metadaten sind das Herkunfts-Tool, das Adobe verwendet, um die Anforderungen dieser Gesetze zu erfüllen.

Der E-Mail- und Landingpage-Designer generiert oder bearbeitet keine Bilder selbst. Er verweist auf Bilder, die bereits mit generativer KI in einem anderen Adobe-Tool, z. B. „Inhalt generieren“, Adobe Express oder Firefly, bzw. in einem Partnermodell generiert oder bearbeitet wurden. Bereits an diese Bilder angehängte C2PA-Metadaten bleiben beim Erstellen, Veröffentlichen und Senden unverändert.

## C2PA-Metadaten werden beim Erstellen und Senden beibehalten {#c2pa-preserved}

In der folgenden Tabelle ist zusammengefasst, was mit C2PA-Metadaten bei jedem Schritt des Erstellens und Sendens von Inhalten mit dem E-Mail- und Landingpage-Designer passiert.

| Aktion | Was passiert | C2PA-Metadaten beibehalten? | Beispiel |
| --- | --- | --- | --- |
| **Einfügen eines Bildes in eine Vorlage** | Der Designer fügt einen Verweis auf ein Bild hinzu, das bereits an anderer Stelle mit generativer KI generiert oder bearbeitet wurde, z. B. mit „Inhalt generieren“, Adobe Express, Firefly oder einem Partnermodell. Die Bilddatei selbst wird nicht geändert. | Ja, unverändert | Ein von Firefly generiertes Banner wird in eine E-Mail-Vorlage eingefügt. |
| **Ändern der Größe, Neupositionieren oder Hinzufügen von Alternativtext** | Es ändern sich nur die Anzeigeeigenschaften im HTML-Code der Vorlage. Die Bilddatei wird nicht neu codiert. | Ja, unverändert | Die Größe eines Bildes wird an ein Layout für Mobilgeräte angepasst und es wird Alternativtext hinzugefügt. |
| **Veröffentlichen** | Die E-Mail oder Landingpage wird veröffentlicht und das Bild wird für den Versand gespeichert. | Ja, unverändert | Eine Kampagne wird veröffentlicht und ihre Bilder werden zum Versand gespeichert. |
| **Senden einer E-Mail oder Anzeigen einer Landingpage** | Das Bild wird an den Posteingang der Empfängerin bzw. des Empfängers gesendet oder auf der Live-Seite angezeigt. | Ja, unverändert | Eine Empfängerin bzw. ein Empfänger öffnet die E-Mail und lädt das Bild herunter. Die Credentials stimmen weiterhin mit dem Original überein. |

## Inhaltstypen und ihr Umfang {#c2pa-content-types}

* **Bilder**: Abgedeckt. Bereits an ein Bild angehängte C2PA-Metadaten werden beim Einfügen, Anpassen, Veröffentlichen und Bereitstellen beibehalten, wie oben gezeigt.
* **Video, Audio, Text**: Nicht zutreffend. Der E-Mail- und Landingpage-Designer generiert oder bearbeitet diese Inhaltstypen nicht mit generativer KI.

## Was passiert, wenn Ihre Inhalte verschoben werden {#c2pa-content-moves}

C2PA-Metadaten bewegen sich mit dem Bild durch den E-Mail- und Landingpage-Designer in der Web-Benutzeroberfläche von Adobe Campaign und zwar von Ihrem Editor über den Speicher zum Posteingang der Empfängerin bzw. des Empfängers oder zur Live-Seite. Bei keinem dieser Schritte werden Credentials erstellt, geändert oder entfernt.

Wenn ein Bild keine C2PA-Metadaten für generative KI enthält, da es nicht mit generativer KI generiert oder bearbeitet wurde, werden hier keine Credentials angezeigt. Das ist das erwartete Verhalten und kein Fehler.

## Überprüfen von Credentials {#c2pa-checking-credential}

Es gibt noch keine Möglichkeit, Content Credentials direkt im E-Mail- oder Landingpage-Designer zu überprüfen.

## Zusätzliche Ressourcen

* [Arbeiten mit der Funktion „Inhalt generieren“](generative-gs.md)
* [Transparenz von Inhalten generativer KI](https://experienceleague.adobe.com/de/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)