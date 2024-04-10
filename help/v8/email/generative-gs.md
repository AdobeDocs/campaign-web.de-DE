---
audience: end-user
title: Erste Schritte mit dem KI-Assistenten
description: Erste Schritte mit dem KI-Assistenten
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: ht
source-wordcount: '551'
ht-degree: 100%

---

# Erste Schritte mit dem KI-Assistenten {#generative-gs}

>[!BEGINSHADEBOX]

**Inhaltsverzeichnis**

* **[Erste Schritte mit dem KI-Assistenten](generative-gs.md)**
* [Generierung von E-Mails mit dem KI-Assistenten](generative-content.md)
* [Generierung von SMS mit dem KI-Assistenten](generative-sms.md)
* [Generierung von Push-Benachrichtigungen mit dem KI-Assistenten](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="KI-Assistent"
>abstract="Nachdem Sie Ihren Versand erstellt und personalisiert haben, können Sie den KI-Assistenten verwenden, um Ihre Inhalte zu verbessern. Diese Funktion vereinfacht den Prozess der Personalisierung und Inhaltsverbesserung, da Sie den Inhalt durch eine Beschreibung dessen, was Sie generieren möchten, anpassen können."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext mit dem KI-Assistenten in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, aktivieren Sie den Umschalter **Mit aktuellem Inhalt verbessern** umschalten. Sie können auch Ihre Marken-Assets hochladen, um sie als Quelle zu verwenden. Wenn Sie den ausgewählten Inhalt nicht verwenden, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Begriffe in Adobe Generative KI"
>abstract="Der Zugriff auf diese Funktion unterliegt Ihrer Zustimmung zu den Adobe Experience Cloud Generative KI-Benutzerrichtlinien.  Eingabeaufforderungen, Kontextdaten, zusätzliche Informationen oder andere Eingaben, die Sie für diese Funktion bereitstellen, müssen an einen bestimmten Kontext gebunden sein, der Ihre Branding-Materialien, Website-Inhalte, Daten, Schemata für solche Daten, Vorlagen oder andere vertrauenswürdige Dokumente umfassen kann und keine personenbezogenen Daten enthalten darf (personenbezogene Daten umfassen alles, was mit einer bestimmten Person verknüpft werden kann). Sie sollten alle Ausgaben dieser Funktion auf ihre Richtigkeit hin überprüfen und sicherstellen, dass sie für Ihren Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

Der KI-Assistent ist ein wertvolles Werkzeug zur Verbesserung von E-Mail-Inhalten. Er vereinfacht die Personalisierung und Inhaltsverbesserung und optimiert Ihre E-Mail-Sendungen, um besser auf Ihre Zielgruppe einzugehen.

Diese Funktion spart Zeit und gewährleistet konsistente Qualität, indem automatisch vollständige E-Mail-Inhalte generiert werden. Mit generativer KI können Sie mühelos ansprechende E-Mails erstellen und so die Effektivität und Effizienz Ihrer Kommunikation steigern.

>[!NOTE]
>
>Diese Funktion ist in der Alpha-Version verfügbar und kann ohne vorherige Ankündigung geändert werden. Sie wird Anfang Oktober aktiviert.

## Schutzmechanismen und Begrenzungen {#generative-guardrails}

Im Folgenden sind die allgemeinen Richtlinien zur Verwendung des KI-Assistenten für die E-Mail-Generierung aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. die von Ihnen definierte Eingabeaufforderung beeinflusst. Verwenden Sie eine gut definierte Eingabeaufforderung, damit das generative KI-Modell korrekt implementiert wird. 
* Laden Sie Marken-Assets hoch, um genaue Informationen zu Markeninhalten zu haben. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die empfohlene maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder viele Bilder können funktionieren, aber die Verarbeitungszeit verlängert sich.
* Verwenden Sie eine von Adobe Campaign erstellte E-Mail-Vorlage oder vorzugsweise eine der [integrierten E-Mail-Vorlagen](../email/create-email-templates.md), eine markenspezifische oder benutzerdefinierte Vorlage, um Ihren E-Mail-Inhalt zu erstellen. Es wird eine E-Mail-Vorlage mit 8 bis 10 Bildern empfohlen.


Die folgenden Einschränkungen gelten für den KI-Assistenten in Campaign:

* Unterstützte Sprache ist nur Englisch.
* Nur für den E-Mail-, Push- und SMS-Kanal verfügbar.
* Generative KI-Inhalte sind möglicherweise nicht immer genau: Teilen Sie uns bitte ggf. Ihr Feedback mit, damit unsere Ingenieurinnen und Ingenieure die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden.



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Generierung von E-Mails" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generierung von E-Mails mit dem KI-Assistenten</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="Generierung von SMS" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generierung von SMS mit dem KI-Assistenten</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Generierung von Push-Benachrichtungen" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generierung von Push-Benachrichtigungen mit dem KI-Assistenten</strong></a>
</div>
<p></td>
</tr></table>
