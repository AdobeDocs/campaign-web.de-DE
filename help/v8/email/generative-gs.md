---
audience: end-user
title: Erste Schritte mit dem KI-Assistenten
description: Erste Schritte mit dem KI-Assistenten
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: ht
source-wordcount: '581'
ht-degree: 100%

---

# Erste Schritte mit dem KI-Assistenten {#generative-gs}

>[!BEGINSHADEBOX]

**Inhaltsverzeichnis**

* Erste Schritte mit dem KI-Assistenten
* [Generierung von E-Mails mit dem KI-Assistenten](generative-content.md)
* [Generierung von SMS mit dem KI-Assistenten](generative-sms.md)
* [Generierung von Push-Benachrichtigungen mit dem KI-Assistenten](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="KI-Assistent"
>abstract="Nachdem der Versand erstellt und personalisiert wurde, kann der KI-Assistent verwendet werden, um die Inhalte zu verbessern. Diese Funktion vereinfacht den Prozess der Personalisierung und Inhaltsverbesserung, da der Inhalt durch eine Beschreibung dessen, was generieret werden soll, angepasst werden kann."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext mit dem KI-Assistenten in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, den Umschalter **Mit aktuellem Inhalt verbessern** aktivieren. Es können auch Marken-Assets hochgeladen werden, um sie als Quelle zu verwenden. Wenn der ausgewählte Inhalt nicht verwendet wird, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Begriffe in Adobe Generative KI"
>abstract="Der Zugriff auf diese Funktion unterliegt Ihrer Zustimmung zu den Adobe Experience Cloud Generative KI-Benutzerrichtlinien.  Bitte überprüfen Sie alle Ausgaben dieser Funktion auf ihre Richtigkeit und stellen Sie sicher, dass sie für Ihren Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

Da die Marketing-Branche immer wettbewerbsintensiver wird, suchen Marken nach effizienten Wegen, um wirkungsvolle Inhalte schnell und effizient zu erstellen. Der KI-Assistent in Campaign basiert auf Azure OpenAI. Er ist das Angebot von Adobe zur KI-gestützten Generierung von Inhalten. Diese Funktion revolutioniert die Erstellung professioneller und markenkonformer Inhalte für verschiedene Kanäle wie E-Mail, SMS und Push. Mit fortschrittlichen GenAI-Modellen und einem tiefgreifenden Verständnis der Markenrichtlinien generiert der KI-Assistent automatisch personalisierte, ansprechende und effektive Inhalte auf der Grundlage des Marketing-Ziels, wobei die Inhalte für die von der Marke vorgegebenen Stile, Layouts, die Tonalität und mehr optimiert sind.

Der KI-Assistent macht die Erstellung und Durchführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push intuitiv, einfach und mühelos, während gleichzeitig Zeit gespart, die Effizienz gesteigert und bessere Ergebnisse erzielt werden.

>[!NOTE]
>
>Diese Funktion ist in der Beta-Version verfügbar und kann ohne vorherige Ankündigung geändert werden.

## Schutzmechanismen und Begrenzungen {#generative-guardrails}

Im Folgenden sind die allgemeinen Richtlinien zur Verwendung des KI-Assistenten für die E-Mail-Generierung aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. die von Ihnen definierte Eingabeaufforderung beeinflusst. Verwenden Sie eine gut definierte Eingabeaufforderung, damit das generative KI-Modell korrekt implementiert wird. 
* Laden Sie Marken-Assets hoch, um genaue Informationen zu Markeninhalten zu haben. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder viele Bilder können funktionieren, aber die Verarbeitungszeit verlängert sich.
* Verwenden Sie eine von Adobe Campaign erstellte E-Mail-Vorlage oder vorzugsweise eine der [integrierten E-Mail-Vorlagen](../email/create-email-templates.md), eine markenspezifische oder benutzerdefinierte Vorlage, um Ihren E-Mail-Inhalt zu erstellen. Es wird eine E-Mail-Vorlage mit 8 bis 10 Bildern empfohlen.
* Denken Sie daran, problematische Ausgaben zu melden, indem Sie bei der Auswahl von Varianten die Symbole mit dem Daumen nach oben, dem Daumen nach unten oder andere Kennzeichnungssymbole verwenden.
* Ihre Nutzung des KI-Assistenten unterliegt den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. [Weitere Informationen](https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

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
