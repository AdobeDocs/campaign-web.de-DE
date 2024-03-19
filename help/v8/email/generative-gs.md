---
audience: end-user
title: Erste Schritte mit dem Inhaltsassistenten
description: Erste Schritte mit dem Inhaltsassistenten
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 832f3da044810e81f3c46f7e3dfaba835c1fabb4
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 100%

---

# Erste Schritte mit dem Inhaltsassistenten {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Inhaltsassistent"
>abstract="Nachdem Sie Ihren Versand erstellt und personalisiert haben, können Sie den Inhaltsassistenten verwenden, um Ihre Inhalte zu verbessern. Diese Funktion vereinfacht den Prozess der Personalisierung und Inhaltsverbesserung, indem Sie den Inhalt durch eine Beschreibung dessen, was Sie generieren möchten, anpassen können."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext für die Inhaltserstellung"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, aktivieren Sie den Umschalter **Mit aktuellem Inhalt verbessern** umschalten. Sie können auch Ihre Marken-Assets hochladen, um sie als Quelle zu verwenden. Wenn Sie den ausgewählten Inhalt nicht verwenden, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe-Begriffe zu generativer KI"
>abstract="Der Zugriff auf diese Funktion unterliegt Ihrer Zustimmung zu den Adobe Experience Cloud-Benutzerrichtlinien für generative KI. Eingabeaufforderungen, Kontext, zusätzliche Informationen oder andere Eingaben, die Sie für diese Funktion bereitstellen, müssen an einen bestimmten Kontext gebunden sein, der Ihre Branding-Materialien, Website-Inhalte, Daten, Schemata für solche Daten, Vorlagen oder andere vertrauenswürdige Dokumente umfassen kann und keine personenbezogenen Daten enthalten darf („personenbezogenen Daten“ umfasst alles, was mit einer bestimmten Person in Verbindung gebracht werden kann). Sie sollten alle Ausgaben dieser Funktion auf ihre Richtigkeit hin überprüfen und sicherstellen, dass sie für Ihren Anwendungsfall geeignet sind"
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Benutzerrichtlinien für die generative KI von Adobe"


Der Inhaltsassistent, der auf generativer KI basiert, ist ein wertvolles Werkzeug zur Verbesserung von E-Mail-Inhalten. Er vereinfacht die Personalisierung und Inhaltsverbesserung und optimiert Ihre E-Mail-Sendungen, um besser auf Ihre Zielgruppe einzugehen.

Diese Funktion spart Zeit und gewährleistet konsistente Qualität, indem automatisch vollständige E-Mail-Inhalte generiert werden. Mit generativer KI können Sie mühelos ansprechende E-Mails erstellen und so die Effektivität und Effizienz Ihrer Kommunikation steigern.


Sie können den Campaign-Inhaltsassistenten in Ihren E-Mails für vielerlei verwenden: [Bilder generieren](generative-image.md), [Textinhalt generieren](generative-content.md), [Vollständigen HTML-Inhalt generieren](generative-email.md).

>[!NOTE]
>
>Diese Funktion ist in der Alpha-Version verfügbar und kann ohne vorherige Ankündigung geändert werden. Sie wird Anfang Oktober aktiviert.

## Schutzmechanismen und Begrenzungen {#generative-guardrails}

Im Folgenden sind die allgemeine Richtlinien zur Verwendung des Inhaltsassistenten für die E-Mail-Generierung aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. die von Ihnen definierte Eingabeaufforderung beeinflusst. Verwenden Sie eine gut definierte Eingabeaufforderung, damit das generative KI-Modell korrekt implementiert wird. 
* Laden Sie Marken-Assets hoch, um genaue Informationen zu Markeninhalten zu haben. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die empfohlene maximale Größe für hochgeladene Marken-Assets beträgt 10 MB. Größere Dateien oder viele Bilder können funktionieren, aber die Verarbeitungszeit verlängert sich.
* Verwenden Sie eine von Adobe Campaign erstellte E-Mail-Vorlage oder vorzugsweise [integrierte E-Mail-Vorlagen](../email/create-email-templates.md), um Ihren E-Mail-Inhalt zu erstellen. Es wird eine E-Mail-Vorlage mit 8 bis 10 Bildern empfohlen.


Es gelten die folgenden Einschränkungen für den Campaign-Inhaltsassistenten:

* Unterstützte Sprache ist nur Englisch
* Nur für den E-Mail-Kanal verfügbar
* Generative KI-Inhalte sind möglicherweise nicht immer genau: Teilen Sie uns bitte ggf. Ihr Feedback mit, damit unsere Ingenieurinnen und Ingenieure die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Textgenerierung" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Textgenerierung mit dem Inhaltsassistenten</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Bildgenerierung" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Bildgenerierung mit dem Inhaltsassistenten</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="E-Mail-Generierung" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>E-Mail-Generierung mit dem Inhaltsassistenten</strong></a>
</div>
<p></td>
</tr></table>
