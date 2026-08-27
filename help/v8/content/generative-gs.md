---
audience: end-user
title: Erste Schritte mit der Funktion „Inhalt erzeugen“
description: Erste Schritte mit der Funktion „Inhalt erzeugen“
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
TQID: https://experienceleague.adobe.com/jpw4u-Vy7M2Q9qRyQ2J3rJ-Mr8UKLUpxhw39tglbbNc
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 887
ht-degree: 100%

---

# Arbeiten mit der Funktion „Inhalt erzeugen“ {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Erzeugen von Inhalt"
>abstract="Nachdem Sie Ihren Versand erstellt und personalisiert haben, verwenden Sie KI, um Ihre Inhalte zu verbessern. Diese Funktion vereinfacht die Personalisierung und Inhaltsverbesserung, da Sie den Inhalt durch eine Beschreibung dessen, was Sie generieren möchten, optimieren können."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren von Kontext mit „Inhalt erzeugen“ in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, aktivieren Sie den Umschalter **Mit aktuellem Inhalt verbessern** umschalten. Es können auch Marken-Assets hochgeladen werden, um sie als Quelle zu verwenden. Wenn der ausgewählte Inhalt nicht verwendet wird, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Bedingungen der generativen KI in Adobe"
>abstract="Der Zugriff auf diese Funktion ist abhängig von der Zustimmung zu den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. Alle Ausgaben dieser Funktion auf ihre Richtigkeit prüfen und sicherstellen, dass sie für den Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

>[!INFO]
>
>Nehmen Sie an unserer [Live-Funktionsvorstellung](https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator) teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.

Da die Marketing-Branche immer wettbewerbsintensiver wird, suchen Marken nach effizienten Wegen, um wirkungsvolle Inhalte schnell zu erstellen. Die Funktion „Inhalt erzeugen“ in Adobe Campaign Web basiert auf Microsoft Azure OpenAI und Adobe Firefly. Sie ist das Angebot von Adobe zur KI-gestützten Inhaltsgenerierung und transformiert die Erstellung professioneller und markenkonformer Inhalte für verschiedene Kanäle wie E-Mail, SMS und Push-Benachrichtigungen. Mit fortschrittlichen GenAI-Modellen und einem tiefgreifenden Verständnis der Markenrichtlinien generiert die Funktion „Inhalt erzeugen“ automatisch personalisierte, ansprechende und effektive Inhalte auf der Grundlage des Marketing-Ziels, wobei die Inhalte für die von der Marke vorgegebenen Stile, Layouts, die Tonalität und mehr optimiert sind.

Die Funktion „Inhalt erzeugen“ unterstützt die Generierung **in mehreren Sprachen**, sodass Sie unterschiedliche globale Zielgruppen erreichen und ansprechen können. „Inhalt erzeugen“ ist in den folgenden Sprachen verfügbar:

<table style="table-layout:fixed; margin-top: 0px; margin-bottom: 0px;">
  <tbody>
    <tr style="border: 0;background-color: #FFFFFF;">
      <td>
        <ul>
          <li>Chinesisch (Hongkong)</li>
          <li>Chinesisch (vereinfacht)</li>
          <li>Chinesisch (Taiwan)</li>
          <li>Niederländisch</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Französisch</li>
          <li>Deutsch</li>
          <li>Italienisch</li>
          <li>Japanisch</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Norwegisch</li>
          <li>Portugiesisch</li>
          <li>Spanisch</li>
          <li>Schwedisch</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

„Inhalt erzeugen“ vereinfacht die Erstellung und Ausführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen hinweg, spart Zeit, erhöht die Effizienz und führt zu besseren Ergebnissen.

>[!IMPORTANT]
>
>* Bevor Sie diese Funktion verwenden, lesen Sie die entsprechenden Informationen unter [Schutzmechanismen und Einschränkungen](#generative-guardrails).
>
>* Sie müssen einer [Benutzervereinbarung](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) zustimmen, bevor Sie KI zum Generieren von Inhalten in Adobe Campaign Web verwenden können. Weitere Informationen erhalten Sie beim Adobe-Support.

## Zugreifen auf „Inhalt erzeugen“ {#generative-access}

Die Funktion „Inhalt erzeugen“ zum Erstellen von Inhalten für E-Mails, Push-Benachrichtigungen, Landingpages und SMS ist jetzt allgemein für alle Benutzenden verfügbar. Die erforderlichen Berechtigungen und Schritte zum Gewähren des Zugriffs für Benutzende werden nachfolgend beschrieben.

+++ Erfahren Sie, wie Sie Berechtigungen für die Inhaltserstellung zuweisen

1. **Rufen Sie die [Admin Console](https://adminconsole.adobe.com/)** auf, navigieren Sie zum Menü **Produkte** und wählen Sie dann **Adobe Campaign Managed Cloud** aus.

1. Greifen Sie auf die Instanz zu, für die Sie Berechtigungen erteilen möchten, und klicken Sie dann auf **Neues Profil**, um ein neues Produktprofil mit dem folgenden spezifischen Produktprofilnamen zu erstellen:

   `Campaign - <instance-name> - AIAssistant`

1. Richten Sie das Produktprofil mit den erforderlichen Berechtigungen für den Zugriff auf die Funktion „Inhalt erzeugen“ ein.

1. **Fügen Sie Benutzende oder Benutzergruppen hinzu**. Wählen Sie eine der folgenden Optionen:
   * **Einzelne Benutzer hinzufügen:** Fügen Sie diesem Produktprofil die erforderlichen Benutzenden direkt hinzu.
   * **Benutzergruppen hinzufügen:** Erstellen Sie eine Benutzergruppe, fügen Sie dieser Gruppe Benutzende hinzu und fügen Sie die Benutzergruppe dann dem Produktprofil hinzu.

Informationen zum Definieren von Berechtigungen in Campaign finden Sie in [diesem Abschnitt](../get-started/permissions.md).

+++

## Schutzmechanismen und Einschränkungen {#generative-guardrails}

Im Folgenden sind die allgemeinen Richtlinien für die Verwendung von KI zum Generieren von Inhalten in Adobe Campaign Web für die E-Mail-Erstellung aufgeführt:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. den von Ihnen definierten Prompt beeinflusst. Verwenden Sie einen gut definierten Prompt, den das GenAI-Modell genau interpretieren kann.
* Laden Sie Marken-Assets hoch, um genaue, markenkonforme Inhalte sicherzustellen. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder viele Bilder können die Verarbeitungszeit erhöhen.
* Verwenden Sie [integrierte E-Mail-Vorlagen](../content/create-email-templates.md), markenspezifische Vorlagen oder benutzerdefinierte Vorlagen, um Ihre E-Mail-Inhalte mithilfe von KI zu erstellen. Es werden E-Mail-Vorlagen mit 8 bis 10 Bildern empfohlen.
* Melden Sie problematische Ausgaben, indem Sie bei der Auswahl von Varianten die Symbole mit dem Daumen nach oben, dem Daumen nach unten oder andere Kennzeichnungssymbole verwenden.
* Ihre Nutzung der Funktion „Inhalt erzeugen“ unterliegt den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. [Weitere Informationen](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Adobe setzt sich für Transparenz bei der Verwendung generativer KI-Tools zur Medienerstellung ein und wendet daher Content Credentials an, wenn Inhalte oder Projekte mit Firefly-generierten Assets heruntergeladen oder exportiert werden. [Weitere Informationen](https://helpx.adobe.com/de/firefly/using/content-credentials.html).

Die folgenden Einschränkungen gelten für die Funktion „Inhalt erzeugen“ in Adobe Campaign Web:

* Die Funktion „Inhalt erzeugen“ in Adobe Campaign Web wird derzeit nur auf Englisch unterstützt. Anderssprachige Eingaben können zu inkonsistenten oder fehlerhaften Ergebnissen führen. Probleme, die sich aus nicht englischen Antworten ergeben, werden derzeit weder behoben noch verbessert.
* Nur für den E-Mail-, Push- und SMS-Kanal verfügbar.
* GenAI-Inhalte sind möglicherweise nicht immer präzise. Teilen Sie ihr Feedback, damit Ingenieure und Ingenieurinnen die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden.

## Funktionen von „Inhalt erzeugen“ {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Vollständige Inhaltsgenerierung mit „Inhalt erzeugen“]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Vollständige Inhaltsgenerierung mit „Inhalt erzeugen“</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Generierung von Textinhalten mit „Inhalt erzeugen“]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Textgenerierung mit „Inhalt erzeugen“</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Bildgenerierung mit „Inhalt erzeugen“]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Bildgenerierung mit „Inhalt erzeugen“</strong></a>
</div>
<p></td>
</tr></table>