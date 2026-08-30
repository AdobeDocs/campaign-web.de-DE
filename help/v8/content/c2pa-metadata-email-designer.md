---
audience: end-user
product: campaign
title: C2PA-Metadaten in E-Mail und Landingpage-Designer
description: Erfahren Sie, was mit C2PA-Metadaten passiert, die bereits an ein Bild angehängt sind, wenn es durch den E-Mail- und Landingpage-Designer in der Web-Benutzeroberfläche von Adobe Campaign navigiert.
topic: Content Management
role: User
level: Beginner
source-git-commit: 645352d9e2ba12d5430ddf1b62852077344c3016
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---


# C2PA-Metadaten in E-Mail und Landingpage-Designer {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**Auf dieser Seite:** Erfahren Sie, was mit C2PA-Metadaten passiert, die bereits an ein Bild angehängt sind, wenn es durch den E-Mail- und Landingpage-Designer in der Web-Benutzeroberfläche von Adobe Campaign navigiert.

>[!ENDSHADEBOX]

>[!INFO]
>
>Im Bereich der generativen KI-Transparenz entstehen neue Gesetze, und Adobe arbeitet daran, die geltenden Anforderungen in allen Rechtssystemen zu erfüllen. C2PA-Metadaten sind das Herkunftstool, das Adobe verwendet, um die Anforderungen dieser Gesetze zu erfüllen.

Der E-Mail- und Landingpage-Designer generiert oder bearbeitet keine Bilder selbst. Sie verweist auf Bilder, die bereits mit generativer KI in einem anderen Adobe-Tool, z. B. „Inhalt generieren“, &quot;Adobe Express&quot; oder &quot;Firefly&quot;, oder in einem Partnermodell generiert oder bearbeitet wurden. An diese Bilder bereits angehängte C2PA-Metadaten bleiben beim Erstellen, Veröffentlichen und Senden unverändert.

## C2PA-Metadaten werden beim Erstellen und Senden beibehalten {#c2pa-preserved}

In der folgenden Tabelle ist zusammengefasst, was mit C2PA-Metadaten bei jedem Schritt des Erstellens und Sendens von Inhalten mit dem E-Mail- und Landingpage-Designer passiert.

| Aktion | Was passiert? | C2PA-Metadaten beibehalten? | Beispiel |
| --- | --- | --- | --- |
| **Einfügen eines Bildes in eine Vorlage** | Der Designer fügt einen Verweis auf ein Bild hinzu, das bereits an anderer Stelle mit generativer KI generiert oder bearbeitet wurde, z. B. „Inhalt generieren“, Adobe Express, Firefly oder ein Partnermodell. Die Bilddatei selbst wird nicht geändert. | Ja, unverändert | Ein von Firefly generiertes Banner wird in eine E-Mail-Vorlage eingefügt. |
| **Größe ändern, neu positionieren oder alternativen Text hinzufügen** | Nur Eigenschaften anzeigen, die sich in der HTML-Änderung der Vorlage befinden. Die Bilddatei wird nicht neu kodiert. | Ja, unverändert | Die Größe eines Bildes wird an ein Layout für Mobilgeräte angepasst, und es wird Alternativtext angegeben. |
| **Veröffentlichen** | Die E-Mail oder Landingpage wird veröffentlicht und das Bild wird für den Versand gespeichert. | Ja, unverändert | Eine Kampagne wird veröffentlicht und ihre Bilder werden zum Versand gespeichert. |
| **Senden einer E-Mail oder Anzeigen einer Landingpage** | Das Bild wird an den Posteingang der Empfängerin bzw. des Empfängers gesendet oder auf der Live-Seite angezeigt. | Ja, unverändert | Ein Empfänger öffnet die E-Mail und lädt das Bild herunter. Die Anmeldedaten stimmen weiterhin mit dem Original überein. |

## Inhaltstypen und ihr Umfang {#c2pa-content-types}

* **Bilder**: Überdeckt. Bereits an ein Bild angehängte C2PA-Metadaten werden beim Einfügen, Anpassen, Veröffentlichen und Bereitstellen beibehalten, wie oben gezeigt.
* **Video, Audio, Text**: Nicht zutreffend. Der E-Mail- und Landingpage-Designer generiert oder bearbeitet diese Inhaltstypen nicht mit generativer KI.

## Was passiert, wenn Inhalte verschoben werden? {#c2pa-content-moves}

C2PA-Metadaten bewegen sich mit dem Bild durch den E-Mail- und Landingpage-Designer in der Adobe Campaign-Web-Benutzeroberfläche, von Ihrem Editor über die Speicherung zum Posteingang der Empfängerin oder zur Live-Seite. Bei keinem dieser Schritte werden Anmeldeinformationen erstellt, geändert oder entfernt.

Wenn ein Bild keine C2PA-Metadaten für generative KI enthält, da es nicht mit generativer KI generiert oder bearbeitet wurde, werden hier keine Anmeldeinformationen angezeigt. Dies ist ein erwarteter Fehler, kein Fehler.

## Überprüfen einer Berechtigung {#c2pa-checking-credential}

Es gibt noch keine Möglichkeit, eine Content Credential direkt im E-Mail- oder Landingpage-Designer zu überprüfen.

## Zusätzliche Ressourcen

* [Arbeiten mit der Funktion „Inhalt erzeugen“](generative-gs.md)
* [Transparenz des generativen KI-Inhalts](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)