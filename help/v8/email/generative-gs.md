---
audience: end-user
title: Erste Schritte mit dem KI-Assistenten
description: Erste Schritte mit dem KI-Assistenten
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 18%

---

# Arbeiten mit dem KI-Assistenten {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="KI-Assistent"
>abstract="Nachdem Sie Ihren Versand erstellt und personalisiert haben, verwenden Sie den KI-Assistenten, um Ihre Inhalte zu verbessern. Diese Funktion vereinfacht die Personalisierung und Inhaltsverbesserung, indem sie es Ihnen ermöglicht, den Inhalt durch die Beschreibung dessen, was Sie generieren möchten, fein abzustimmen."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext mit dem KI-Assistenten in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, aktivieren Sie den **Mit aktuellem Inhalt erweitern**. Es können auch Marken-Assets hochgeladen werden, um sie als Quelle zu verwenden. Wenn Sie die ausgewählten Inhalte nicht verwenden, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Bedingungen der generativen KI in Adobe"
>abstract="Der Zugriff auf diese Funktion hängt von Ihrer Zustimmung zu den Adobe Experience Cloud Generative AI-Benutzerrichtlinien ab. Überprüfen Sie alle Ausgaben aus dieser Funktion auf Genauigkeit und stellen Sie sicher, dass sie für Ihren Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

>[!INFO]
>
>Nehmen Sie an unserer [Live-Funktionsvorstellung](https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator) teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.

Da die Marketing-Branche wettbewerbsfähiger wird, suchen Marken nach effizienten Möglichkeiten, schnell wirkungsvolle Inhalte zu generieren. Der KI-Assistent in Adobe Campaign Web basiert auf Microsoft Azure OpenAI und Adobe Firefly und ist die KI-Inhaltsgenerierungsfunktion von Adobe, mit der Marketing-Experten professionelle und markenkonsistente Inhalte über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen hinweg erstellen können. Mit fortschrittlichen GenAI-Modellen und einem tiefen Verständnis der Markenrichtlinien generiert der KI-Assistent automatisch personalisierte, ansprechende und effektive Inhalte basierend auf dem Marketing-Ziel, wobei Inhalte für markenspezifische Stile, Layouts, Töne und mehr optimiert werden.

Der KI-Assistent vereinfacht die Erstellung und Ausführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen hinweg, spart Zeit, verbessert die Effizienz und erzielt bessere Ergebnisse.

>[!IMPORTANT]
>
>* Bevor Sie diese Funktion verwenden, lesen Sie die entsprechenden [Leitplanken und Einschränkungen](#generative-guardrails).
>
>* Sie müssen einer [Benutzervereinbarung“ zustimmen](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) bevor Sie den KI-Assistenten in Adobe Campaign Web verwenden. Weitere Informationen erhalten Sie vom Adobe-Support.

## Zugriff auf KI-Assistenten {#generative-access}

Der KI-Assistent für E-Mails, Push-Benachrichtigungen und SMS ist jetzt allgemein verfügbar (General Availability, GA) und steht allen Benutzern zur Verfügung. Die erforderlichen Berechtigungen und Schritte zum Gewähren des Zugriffs für Benutzende werden nachfolgend beschrieben.

+++ Erfahren Sie, wie Sie Berechtigungen zum Erstellen von Inhalten zuweisen

1. **Produktprofil erstellen** - Erstellen Sie in [Admin Console](https://stage.adminconsole.adobe.com/) ein Produktprofil mit dem folgenden spezifischen Muster:
   `Campaign - <instance-name> - AIAssistant`

1. **Benutzer hinzufügen** - Fügen Sie diesem Produktprofil den erforderlichen Benutzer hinzu,\
   oder\
   **Benutzergruppe erstellen** und diese Benutzergruppe zum Produktprofil hinzufügen und dann Benutzer zu diesem Produktprofil hinzufügen.

Informationen zum Definieren von Berechtigungen in Campaign finden Sie in [diesem Abschnitt](../get-started/permissions.md).

+++

## Schutzmechanismen und Einschränkungen {#generative-guardrails}

Allgemeine Richtlinien zur Verwendung des KI-Assistenten in Adobe Campaign Web für die E-Mail-Generierung finden Sie unten:

* Die Qualität der generierten Inhalte hängt stark von dem von Ihnen definierten Marketing-Ziel oder der von Ihnen definierten Eingabeaufforderung ab. Verwenden Sie eine klar definierte Eingabeaufforderung für das GenAI-Modell, um genau zu interpretieren.
* Laden Sie Marken-Assets hoch, um genaue, markeninterne Inhalte sicherzustellen. Andernfalls basiert der Inhalt auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann in den folgenden Formaten vorliegen: PDF, JPEG, PNG oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder eine Vielzahl von Bildern können die Verarbeitungszeit erhöhen.
* Verwenden Sie [integrierten E-Mail](../email/create-email-templates.md)Vorlagen), markenspezifische Vorlagen oder benutzerdefinierte Vorlagen, um Ihren E-Mail-Inhalt mithilfe des KI-Assistenten zu erstellen. E-Mail-Vorlagen mit bis zu 8-10 Bildern werden empfohlen.
* Melden Sie problematische Ausgaben mithilfe der Symbole „Daumen hoch“, „Daumen runter“ oder „Flag“ bei der Auswahl von Varianten.
* Ihre Verwendung des KI-Assistenten unterliegt den Adobe Experience Cloud Generative AI-Benutzerrichtlinien. [Weitere Informationen](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Als Teil des Engagements von Adobe für Transparenz bei der Verwendung von generativen KI-Tools bei der Medienerstellung wendet Adobe Content Credentials an, wenn Inhalte oder ein Projekt, das ein von Firefly generiertes Asset enthält, heruntergeladen oder exportiert werden. [Weitere Informationen](https://helpx.adobe.com/de/firefly/using/content-credentials.html).

Die folgenden Einschränkungen gelten für den KI-Assistenten in Adobe Campaign Web:

* Der KI-Assistent in Adobe Campaign Web wird derzeit nur auf Englisch unterstützt. Anderssprachige Eingaben können zu inkonsistenten oder fehlerhaften Ergebnissen führen. Probleme, die sich aus nicht englischen Antworten ergeben, werden derzeit nicht behandelt oder verbessert.
* Nur für die Kanäle E-Mail, Push und SMS verfügbar.
* GenAI-Inhalte sind möglicherweise nicht immer korrekt. Geben Sie ihr Feedback, damit Ingenieure die Modelle verfeinern können.
* Sie können mehrere Marken-Assets hochladen, aber nur eines für eine bestimmte Generation nutzen.

## Funktionen des KI-Assistenten zum Generieren von Inhalten {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[E-Mail-Erstellung mit KI-Assistenten]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>E-Mail-Generierung mit KI-Assistent</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[SMS-Generierung mit KI-Assistenten]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>SMS-Generierung mit dem KI-Assistenten</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Generieren von Push-Benachrichtigungen mit dem KI-Assistenten]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generieren von Push-Benachrichtigungen mit dem KI-Assistenten</strong></a>
</div>
<p></td>
</tr></table>