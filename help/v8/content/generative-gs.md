---
audience: end-user
title: Erste Schritte mit der Inhaltserstellung
description: Erste Schritte mit der Inhaltserstellung
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
TQID: https://experienceleague.adobe.com/jpw4u-Vy7M2Q9qRyQ2J3rJ-Mr8UKLUpxhw39tglbbNc
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 887
ht-degree: 63%

---

# Arbeiten mit generierten Inhalten {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Inhalt generieren"
>abstract="Nachdem Sie Ihren Versand erstellt und personalisiert haben, verwenden Sie KI , um Ihre Inhalte zu verbessern. Diese Funktion vereinfacht die Personalisierung und Inhaltsverbesserung, da Sie den Inhalt durch eine Beschreibung dessen, was Sie generieren möchten, optimieren können."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definieren des Kontexts mit dem Generate Content in Campaign"
>abstract="Um den ausgewählten Inhalt als Eingabe für die Inhaltserstellung zu verwenden, aktivieren Sie den Umschalter **Mit aktuellem Inhalt verbessern** umschalten. Es können auch Marken-Assets hochgeladen werden, um sie als Quelle zu verwenden. Wenn der ausgewählte Inhalt nicht verwendet wird, ist das Hochladen und Auswählen von Marken-Assets obligatorisch."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Bedingungen der generativen KI in Adobe"
>abstract="Der Zugriff auf diese Funktion ist abhängig von der Zustimmung zu den Benutzerrichtlinien für generative KI in Adobe Experience Cloud. Alle Ausgaben dieser Funktion auf ihre Richtigkeit prüfen und sicherstellen, dass sie für den Anwendungsfall geeignet sind."
>additional-url="https://www.adobe.com/de/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative KI – Benutzungsrichtlinien"

>[!INFO]
>
>Nehmen Sie an unserer [Live-Funktionsvorstellung](https://experienceleague.adobe.com/de/apps/journey-optimizer/ai-assistant-content-accelerator) teil, um die Funktionen in der Praxis selbst zu erkunden und die vielfältigen Einsatzmöglichkeiten zu verstehen.

Da die Marketing-Branche immer wettbewerbsintensiver wird, suchen Marken nach effizienten Wegen, um wirkungsvolle Inhalte schnell zu erstellen. Generieren von Inhalten in Adobe Campaign Web, unterstützt durch Microsoft Azure OpenAI und Adobe Firefly, ist Adobes KI-Inhaltsgenerierungsfunktion, die die Erstellung professioneller und markenkonsistenter Inhalte auf Kanälen wie E-Mail, SMS und Push-Benachrichtigungen transformiert. Mit fortschrittlichen GenAI-Modellen und einem tiefen Verständnis der Markenrichtlinien generiert Generate Content automatisch personalisierte, ansprechende und effektive Inhalte basierend auf dem Marketing-Ziel, die Optimierung von Inhalten für markendefinierte Stile, Layouts, Ton und mehr.

Inhaltserstellung unterstützt die Erstellung von **(in mehreren Sprachen** wodurch Sie unterschiedliche globale Zielgruppen erreichen und ansprechen können. Generate Content ist in den folgenden Sprachen verfügbar:

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

„Inhalt generieren“ vereinfacht die Erstellung und Ausführung von Marketing-Kampagnen über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen hinweg, spart Zeit, verbessert die Effizienz und erzielt bessere Ergebnisse.

>[!IMPORTANT]
>
>* Bevor Sie diese Funktion verwenden, lesen Sie die entsprechenden Informationen unter [Schutzmechanismen und Einschränkungen](#generative-guardrails).
>
>* Sie müssen einer [Benutzervereinbarung“ zustimmen, &#x200B;](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) KI zum Generieren von Inhalten in Adobe Campaign Web verwenden zu können. Weitere Informationen erhalten Sie beim Adobe-Support.

## Zugriff auf generierten Inhalt {#generative-access}

Die Generierung von Inhalten für E-Mails, Push-Benachrichtigungen, Landingpages und SMS ist jetzt allgemein verfügbar (General Availability, GA) und steht allen Benutzern zur Verfügung. Die erforderlichen Berechtigungen und Schritte zum Gewähren des Zugriffs für Benutzende werden nachfolgend beschrieben.

+++ Erfahren Sie, wie Sie Berechtigungen für die Inhaltserstellung zuweisen

1. **Rufen Sie die [Admin Console](https://adminconsole.adobe.com/)** auf, navigieren Sie zum Menü **Produkte** und wählen Sie dann **Adobe Campaign Managed Cloud** aus.

1. Greifen Sie auf die Instanz zu, für die Sie Berechtigungen erteilen möchten, und klicken Sie dann auf **Neues Profil**, um ein neues Produktprofil mit dem folgenden spezifischen Produktprofilnamen zu erstellen:

   `Campaign - <instance-name> - AIAssistant`

1. Richten Sie das Produktprofil mit den erforderlichen Berechtigungen für den Zugriff auf „Inhalt generieren“ ein.

1. **Fügen Sie Benutzende oder Benutzergruppen hinzu**. Wählen Sie eine der folgenden Optionen:
   * **Einzelne Benutzer hinzufügen:** Fügen Sie diesem Produktprofil die erforderlichen Benutzenden direkt hinzu.
   * **Benutzergruppen hinzufügen:** Erstellen Sie eine Benutzergruppe, fügen Sie dieser Gruppe Benutzende hinzu und fügen Sie die Benutzergruppe dann dem Produktprofil hinzu.

Informationen zum Definieren von Berechtigungen in Campaign finden Sie in [diesem Abschnitt](../get-started/permissions.md).

+++

## Schutzmechanismen und Einschränkungen {#generative-guardrails}

Im Folgenden finden Sie allgemeine Richtlinien für die Verwendung von KI zum Generieren von Inhalten in Adobe Campaign Web für die E-Mail-Generierung:

* Die Qualität des generierten Inhalts wird stark durch das von Ihnen definierte Marketing-Ziel bzw. den von Ihnen definierten Prompt beeinflusst. Verwenden Sie einen gut definierten Prompt, den das GenAI-Modell genau interpretieren kann.
* Laden Sie Marken-Assets hoch, um genaue, markenkonforme Inhalte sicherzustellen. Andernfalls basieren Inhalte auf öffentlich verfügbaren Informationen. Der hochgeladene Inhalt kann folgende Formate haben: PDF-, JPEG-, PNG- oder ZIP-Dateien (mit unterstützten Dateiformaten).
* Die maximale Größe für hochgeladene Marken-Assets beträgt 50 MB. Größere Dateien oder viele Bilder können die Verarbeitungszeit erhöhen.
* Verwenden [integrierte E-Mail](../content/create-email-templates.md)Vorlagen), markenspezifische Vorlagen oder benutzerdefinierte Vorlagen, um Ihren E-Mail-Inhalt mithilfe von KI zu erstellen. Es werden E-Mail-Vorlagen mit 8 bis 10 Bildern empfohlen.
* Melden Sie problematische Ausgaben, indem Sie bei der Auswahl von Varianten die Symbole mit dem Daumen nach oben, dem Daumen nach unten oder andere Kennzeichnungssymbole verwenden.
* Ihre Verwendung von Inhalt generieren unterliegt den Benutzerrichtlinien für generative KI von Adobe Experience Cloud. [Weitere Informationen](https://www.adobe.com/de/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Adobe setzt sich für Transparenz bei der Verwendung generativer KI-Tools zur Medienerstellung ein und wendet daher Content Credentials an, wenn Inhalte oder Projekte mit Firefly-generierten Assets heruntergeladen oder exportiert werden. [Weitere Informationen](https://helpx.adobe.com/de/firefly/using/content-credentials.html).

Die folgenden Einschränkungen gelten für das Generieren von Inhalten in Adobe Campaign Web:

* Das Generieren von Inhalten in Adobe Campaign Web wird derzeit nur auf Englisch unterstützt. Anderssprachige Eingaben können zu inkonsistenten oder fehlerhaften Ergebnissen führen. Probleme, die sich aus nicht englischen Antworten ergeben, werden derzeit weder behoben noch verbessert.
* Nur für den E-Mail-, Push- und SMS-Kanal verfügbar.
* GenAI-Inhalte sind möglicherweise nicht immer präzise. Teilen Sie ihr Feedback, damit Ingenieure und Ingenieurinnen die Modelle präzisieren können.
* Sie können mehrere Marken-Assets hochladen, jedoch für eine bestimmte Generierung nur eines verwenden.

## Funktionen zur Inhaltserstellung {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Vollständige Inhaltserstellung mit Inhalt generieren]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Vollständige Inhaltserstellung mit „Inhalt generieren“</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Generieren von Textinhalten mit Inhalt generieren]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Textgenerierung mit Inhalt generieren</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Bilderstellung mit Inhalt generieren]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Bildgenerierung mit Inhalt generieren</strong></a>
</div>
<p></td>
</tr></table>