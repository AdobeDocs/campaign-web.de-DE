---
audience: end-user
title: Erste Schritte mit dem KI-Assistenten
description: Erste Schritte mit dem KI-Assistenten
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Arbeiten mit dem KI-Assistenten {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="KI-Assistent"
>abstract="Nachdem Sie Ihren Versand erstellt und personalisiert haben, verwenden Sie den KI-Assistenten, um Ihre Inhalte zu verbessern. Diese Funktion vereinfacht die Personalisierung und Inhaltsverbesserung, da Sie den Inhalt durch eine Beschreibung dessen, was Sie generieren möchten, optimieren können."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext mit dem KI-Assistenten in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, aktivieren Sie den Umschalter **Mit aktuellem Inhalt verbessern** umschalten. Es können auch Marken-Assets hochgeladen werden, um sie als Quelle zu verwenden. Wenn der ausgewählte Inhalt nicht verwendet wird, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Bedingungen der generativen KI in Adobe"
>abstract="Der Zugriff auf diese Funktion ist abhängig von Ihrer Zustimmung zu den Benutzerrichtlinien für generative KI in Adobe Experience Cloud.  Prüfen Sie alle Ausgaben dieser Funktion auf ihre Richtigkeit und stellen Sie sicher, dass sie für den Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

>[!INFO]
>
>Nehmen Sie an unserer [Live-Funktionsvorstellung](https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator) teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.

Da die Marketing-Branche immer wettbewerbsintensiver wird, suchen Marken nach effizienten Wegen, um wirkungsvolle Inhalte schnell zu erstellen. Der KI-Assistent in Adobe Campaign Web basiert auf Microsoft Azure OpenAI und Adobe Firefly. Er ist das Angebot von Adobe zur KI-gestützten Generierung von Inhalten und transformiert die Erstellung professioneller und markenkonformer Inhalte für verschiedene Kanäle wie E-Mail, SMS und Push. Mit fortschrittlichen GenAI-Modellen und einem tiefgreifenden Verständnis der Markenrichtlinien generiert der KI-Assistent automatisch personalisierte, ansprechende und effektive Inhalte auf der Grundlage des Marketing-Ziels, wobei die Inhalte für die von der Marke vorgegebenen Stile, Layouts, die Tonalität und mehr optimiert sind.

Der KI-Assistent vereinfacht die Erstellung und Durchführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen, spart Zeit, erhöht die Effizienz und führt zu besseren Ergebnissen.

>[!IMPORTANT]
>
>* Bevor Sie diese Funktion verwenden, lesen Sie die entsprechenden Informationen unter [Schutzmechanismen und Einschränkungen](#generative-guardrails).
>
>* Sie müssen einer [Benutzervereinbarung](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) zustimmen, bevor Sie den KI-Assistenten in Adobe Campaign Web verwenden können. Weitere Informationen erhalten Sie beim Adobe-Support.

## Zugriff auf den KI-Assistenten {#generative-access}

Der KI-Assistent für E-Mails, Push-Benachrichtigungen und SMS ist nun allgemein für alle Benutzenden verfügbar. Die erforderlichen Berechtigungen und Schritte zum Gewähren des Zugriffs für Benutzende werden nachfolgend beschrieben.

+++ Erfahren Sie, wie Sie Berechtigungen für die Inhaltserstellung zuweisen

1. **Produktprofil erstellen**: Erstellen Sie in der [Admin Console](https://stage.adminconsole.adobe.com/) ein Produktprofil mit dem folgenden spezifischen Muster:
   `Campaign - <instance-name> - AIAssistant`

1. **Benutzende hinzufügen**: Fügen Sie diesem Produktprofil die erforderlichen Benutzenden hinzu\
   oder\
   **Benutzergruppe erstellen**: Fügen Sie dem Produktprofil diese Benutzergruppe und diesem Produktprofil Benutzende hinzu.

Informationen zum Definieren von Berechtigungen in Campaign finden Sie in [diesem Abschnitt](../get-started/permissions.md).

+++

## Schutzmechanismen und Einschränkungen {#generative-guardrails}

Im Folgenden sind die allgemeinen Richtlinien zur Verwendung des KI-Assistenten in Adobe Campaign Web zum Generieren von E-Mails aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. den von Ihnen definierten Prompt beeinflusst. Verwenden Sie einen gut definierten Prompt, den das GenAI-Modell genau interpretieren kann.
* Laden Sie Marken-Assets hoch, um genaue, markenkonforme Inhalte sicherzustellen. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB.  Größere Dateien oder viele Bilder können die Verarbeitungszeit erhöhen.
* Verwenden Sie [integrierte E-Mail-Vorlagen](../content/create-email-templates.md), markenspezifische Vorlagen oder benutzerdefinierte Vorlagen, um Ihre E-Mail-Inhalte mit dem KI-Assistenten zu erstellen. Es werden E-Mail-Vorlagen mit 8 bis 10 Bildern empfohlen.
* Melden Sie problematische Ausgaben, indem Sie bei der Auswahl von Varianten die Symbole mit dem Daumen nach oben, dem Daumen nach unten oder andere Kennzeichnungssymbole verwenden.
* Ihre Nutzung des KI-Assistenten unterliegt den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. [Weitere Informationen](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Adobe setzt sich für Transparenz bei der Verwendung generativer KI-Tools zur Medienerstellung ein und wendet daher Content Credentials an, wenn Inhalte oder Projekte mit Firefly-generierten Assets heruntergeladen oder exportiert werden. [Weitere Informationen](https://helpx.adobe.com/de/firefly/using/content-credentials.html).

Die folgenden Einschränkungen gelten für den KI-Assistenten in Adobe Campaign Web:

* Der KI-Assistent in Adobe Campaign Web wird derzeit nur auf Englisch unterstützt. Anderssprachige Eingaben können zu inkonsistenten oder fehlerhaften Ergebnissen führen. Probleme, die sich aus nicht englischen Antworten ergeben, werden derzeit weder behoben noch verbessert.
* Nur für den E-Mail-, Push- und SMS-Kanal verfügbar.
* GenAI-Inhalte sind möglicherweise nicht immer präzise. Teilen Sie ihr Feedback, damit Ingenieure und Ingenieurinnen die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden.

## Funktionen des KI-Assistenten zum Generieren von Inhalten {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Generierung von E-Mails mit dem KI-Assistenten]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generierung von E-Mails mit dem KI-Assistenten</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[Generierung von SMS mit dem KI-Assistenten]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generierung von SMS mit dem KI-Assistenten</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Generierung von Push-Benachrichtigungen mit dem KI-Assistenten]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generierung von Push-Benachrichtigungen mit dem KI-Assistenten</strong></a>
</div>
<p></td>
</tr></table>