---
audience: end-user
title: Erste Schritte mit dem AI-Assistenten - Content Accelerator
description: Erste Schritte mit dem AI-Assistenten - Content Accelerator
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 55b726961149e7eb19ee326f1b702e6b75976dae
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 57%

---

# Arbeiten mit dem AI Assistant - Content Accelerator  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="AI Assistant Content Accelerator"
>abstract="Der KI-Assistent macht die Erstellung und Durchführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push intuitiv, einfach und mühelos, während gleichzeitig Zeit gespart, die Effizienz gesteigert und bessere Ergebnisse erzielt werden."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"


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

>[!INFO]
>
>Machen Sie sich mit [unserer interaktiven Demo](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator) vertraut, die es Ihnen ermöglicht, die Funktionen selbst zu erforschen und deren Funktionen vollständig zu verstehen.


Da die Marketing-Branche immer wettbewerbsintensiver wird, suchen Marken nach effizienten Wegen, um wirkungsvolle Inhalte schnell und effizient zu erstellen. Der AI-Assistent im Adobe Campaign Web für Content Acceleration, der von Microsoft Azure OpenAI und Adobe Firefly unterstützt wird, ist eine Funktion zur Erstellung von AI-Inhalten, die die Art und Weise revolutioniert, wie Marketingexperten professionelle und markenkonsistente Adobe-Inhalte über verschiedene Kanäle wie E-Mail, SMS und Push erstellen. Mit fortschrittlichen GenAI-Modellen und einem tiefgreifenden Verständnis der Markenrichtlinien generiert der KI-Assistent automatisch personalisierte, ansprechende und effektive Inhalte auf der Grundlage des Marketing-Ziels, wobei die Inhalte für die von der Marke vorgegebenen Stile, Layouts, die Tonalität und mehr optimiert sind.

Der KI-Assistent macht die Erstellung und Durchführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push intuitiv, einfach und mühelos, während gleichzeitig Zeit gespart, die Effizienz gesteigert und bessere Ergebnisse erzielt werden.

>[!IMPORTANT]
>
>* Bevor Sie mit der Verwendung dieser Funktion beginnen, lesen Sie die entsprechenden Informationen zu [Schutzmechanismen und Begrenzungen](#generative-guardrails).
>
>* Sie müssen einer [Benutzervereinbarung](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) zustimmen, bevor Sie den AI-Assistenten in Adobe Campaign Web for Content Acceleration verwenden können. Weitere Informationen erhalten Sie von Ihrer Adobe-Kontaktperson.

## Zugriff auf den AI Assistant - Content Accelerator {#generative-access}

AI-Assistent - Content Accelerator für E-Mails, Push-Benachrichtigungen und SMS ist jetzt allgemein verfügbar und für alle Benutzer verfügbar. Die erforderlichen Berechtigungen und Schritte zum Gewähren des Zugriffs für Benutzer werden nachfolgend beschrieben.

+++  Erfahren Sie, wie Sie Berechtigungen zur Inhaltserstellung zuweisen.

1. **Produktprofil erstellen** - Erstellen Sie in [Admin Console](https://stage.adminconsole.adobe.com/) ein Produktprofil mit dem folgenden spezifischen Muster:
   `Campaign - <instance-name> - AIAssistant`

1. **Benutzer hinzufügen** - Fügen Sie diesem Produktprofil den erforderlichen Benutzer hinzu.
oder
   **Benutzergruppe erstellen** , diese Benutzergruppe zum Produktprofil hinzufügen und diesem Produktprofil Benutzer hinzufügen.

In [diesem Abschnitt](../get-started/permissions.md) erfahren Sie, wie Sie Berechtigungen in Campaign definieren.

+++

## Schutzmechanismen und Einschränkungen {#generative-guardrails}

Die allgemeinen Richtlinien für die Verwendung des AI-Assistenten in Adobe Campaign Web for Content Acceleration zur E-Mail-Generierung sind unten aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. die von Ihnen definierte Eingabeaufforderung beeinflusst. Verwenden Sie eine gut definierte Eingabeaufforderung, damit das generative KI-Modell korrekt implementiert wird. 
* Laden Sie Marken-Assets hoch, um genaue Informationen zu Markeninhalten zu haben. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder viele Bilder können funktionieren, aber die Verarbeitungszeit verlängert sich.
* Verwenden Sie [ integrierte E-Mail-Vorlagen](../email/create-email-templates.md), markenspezifische Vorlagen oder benutzerdefinierte Vorlagen, um E-Mail-Inhalte mit Content Accelerator zu erstellen. E-Mail-Vorlagen mit bis zu 8 bis 10 Bildern werden empfohlen.
* Denken Sie daran, problematische Ausgaben zu melden, indem Sie bei der Auswahl von Varianten die Symbole mit dem Daumen nach oben, dem Daumen nach unten oder andere Kennzeichnungssymbole verwenden.
* Ihre Nutzung des KI-Assistenten unterliegt den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. [Weitere Informationen](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Als Teil der Verpflichtung von Adobe zur Förderung der Transparenz bei der Verwendung generativer KI-Tools bei der Medienerstellung wendet Adobe Content credentials an, wenn Inhalte oder ein Projekt, das ein Firefly-generiertes Asset enthält, heruntergeladen oder exportiert werden. [Weitere Informationen](https://helpx.adobe.com/firefly/using/content-credentials.html)

Die folgenden Einschränkungen gelten für den AI-Assistenten in Adobe Campaign Web for Content Acceleration:

* Der AI-Assistent in Adobe Campaign Web for Content Acceleration wird derzeit nur auf Englisch unterstützt. Nicht-englische Eingaben können zu inkonsistenten oder fehlerhaften Ergebnissen führen. Probleme, die sich aus nicht englischsprachigen Antworten ergeben, werden derzeit weder behoben noch verbessert.
* Nur für den E-Mail-, Push- und SMS-Kanal verfügbar.
* Generative KI-Inhalte sind möglicherweise nicht immer genau: Teilen Sie uns bitte ggf. Ihr Feedback mit, damit unsere Ingenieurinnen und Ingenieure die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden.

## Funktionen zur Inhaltserstellung für AI Assistant {#generative-features}

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
