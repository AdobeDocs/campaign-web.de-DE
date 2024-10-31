---
audience: end-user
title: Erste Schritte mit dem KI-Assistenten zur Beschleunigung von Inhalten
description: Erste Schritte mit dem KI-Assistenten zur Beschleunigung von Inhalten
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 87%

---

# Arbeiten mit dem Content Accelerator des KI-Assistenten  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Content Accelerator des KI-Assistenten"
>abstract="Der KI-Assistent macht die Erstellung und Durchführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push intuitiv, einfach und mühelos, spart gleichzeitig Zeit, erhöht die Effizienz und führt zu besseren Ergebnissen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="KI-Assistent"
>abstract="Nachdem der Versand erstellt und personalisiert wurde, kann der KI-Assistent verwendet werden, um die Inhalte zu verbessern. Diese Funktion vereinfacht den Prozess der Personalisierung und Verbesserung der Inhalte, da diese durch eine Beschreibung dessen, was generiert werden soll, genauer angepasst werden können."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext mit dem KI-Assistenten in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, den Umschalter **Mit aktuellem Inhalt verbessern** aktivieren. Es können auch Marken-Assets hochgeladen werden, um sie als Quelle zu verwenden. Wenn der ausgewählte Inhalt nicht verwendet wird, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Begriffe in Adobe Generative KI"
>abstract="Der Zugriff auf diese Funktion unterliegt der Zustimmung zu den Benutzerrichtlinien für generative KI in Adobe Experience Cloud.  Alle Ausgaben dieser Funktion auf ihre Richtigkeit überprüfen und sicherstellen, dass sie für den Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

>[!INFO]
>
>Nehmen Sie an unserer [Live-Funktionsvorstellung](https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator) teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.


Da die Marketing-Branche immer wettbewerbsintensiver wird, suchen Marken nach effizienten Wegen, um wirkungsvolle Inhalte schnell und effizient zu erstellen. Der AI Assistant Content Accelerator im Adobe Campaign Web, der von Microsoft Azure OpenAI und Adobe Firefly unterstützt wird, ist eine Funktion zur Erstellung von-Inhalten, die die Erstellung professioneller und markenkonsistenter Adobe-Inhalte auf verschiedenen Kanälen wie E-Mail, SMS oder Push-Benachrichtigungen revolutioniert. Mit fortschrittlichen GenAI-Modellen und einem tiefgreifenden Verständnis der Markenrichtlinien generiert der KI-Assistent automatisch personalisierte, ansprechende und effektive Inhalte auf der Grundlage des Marketing-Ziels, wobei die Inhalte für die von der Marke vorgegebenen Stile, Layouts, die Tonalität und mehr optimiert sind.

Der KI-Assistent macht die Erstellung und Durchführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push intuitiv, einfach und mühelos, spart gleichzeitig Zeit, erhöht die Effizienz und führt zu besseren Ergebnissen.

>[!IMPORTANT]
>
>* Bevor Sie mit der Verwendung dieser Funktion beginnen, lesen Sie die entsprechenden Informationen zu [Schutzmechanismen und Einschränkungen](#generative-guardrails).
>
>* Sie müssen einer [Benutzervereinbarung](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) zustimmen, bevor Sie den AI Assistant Content Accelerator im Adobe Campaign Web verwenden können. Weitere Informationen erhalten Sie beim Adobe-Support.

## Zugreifen auf den KI-Assistenten zur Beschleunigung von Inhalten {#generative-access}

Der KI-Assistent zur Beschleunigung von Inhalten für E-Mails, Push-Benachrichtigungen und SMS ist nun allgemein für alle Benutzenden verfügbar. Die erforderlichen Berechtigungen und Schritte zum Gewähren des Zugriffs für Benutzende werden nachfolgend beschrieben.

+++  Erfahren Sie, wie Sie Berechtigungen für die Inhaltserstellung zuweisen

1. **Produktprofil erstellen**: Erstellen Sie in der [Admin Console](https://stage.adminconsole.adobe.com/) ein Produktprofil mit dem folgenden spezifischen Muster:
   `Campaign - <instance-name> - AIAssistant`

1. **Benutzende hinzufügen**: Fügen Sie diesem Produktprofil die erforderlichen Benutzenden hinzu.
ODER
   **Benutzergruppe erstellen**: Fügen Sie dem Produktprofil diese Benutzergruppe und diesem Produktprofil Benutzende hinzu.

Informationen zum Definieren von Berechtigungen in Campaign finden Sie in [diesem Abschnitt](../get-started/permissions.md).

+++

## Schutzmechanismen und Einschränkungen {#generative-guardrails}

Die allgemeinen Richtlinien zur Verwendung des AI Assistant Content Accelerator im Adobe Campaign Web für die E-Mail-Generierung sind unten aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. die von Ihnen definierte Eingabeaufforderung beeinflusst. Verwenden Sie eine gut definierte Eingabeaufforderung, damit das generative KI-Modell korrekt implementiert wird. 
* Laden Sie Marken-Assets hoch, um genaue Informationen zu Markeninhalten zu haben. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder viele Bilder können funktionieren, aber die Verarbeitungszeit verlängert sich.
* Verwenden Sie [integrierte E-Mail-Vorlagen](../email/create-email-templates.md), markenspezifische Vorlagen oder benutzerdefinierte Vorlagen, um E-Mail-Inhalte mit der Funktion zur Beschleunigung von Inhalten zu erstellen. Es werden E-Mail-Vorlagen mit 8 bis 10 Bildern empfohlen.
* Denken Sie daran, problematische Ausgaben zu melden, indem Sie bei der Auswahl von Varianten die Symbole mit dem Daumen nach oben, dem Daumen nach unten oder andere Kennzeichnungssymbole verwenden.
* Ihre Nutzung des KI-Assistenten unterliegt den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. [Weitere Informationen](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Adobe setzt sich für Transparenz bei der Verwendung generativer KI-Tools zur Medienerstellung ein und wendet daher Inhaltsurhebernachweise an, wenn Inhalte oder Projekte mit Firefly-generierten Assets heruntergeladen oder exportiert werden. [Weitere Informationen](https://helpx.adobe.com/de/firefly/using/content-credentials.html)

Die folgenden Einschränkungen gelten für den AI Assistant Content Accelerator im Adobe Campaign Web:

* AI Assistant Content Accelerator in Adobe Campaign Web wird derzeit nur auf Englisch unterstützt. Anderssprachige Eingaben können zu inkonsistenten oder fehlerhaften Ergebnissen führen. Probleme, die sich aus nicht englischen Antworten ergeben, werden derzeit weder behoben noch verbessert.
* Nur für den E-Mail-, Push- und SMS-Kanal verfügbar.
* Generative KI-Inhalte sind möglicherweise nicht immer genau: Teilen Sie uns bitte ggf. Ihr Feedback mit, damit unsere Ingenieurinnen und Ingenieure die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden.

## Funktionen des KI-Assistenten zum Generieren von Inhalten {#generative-features}

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
