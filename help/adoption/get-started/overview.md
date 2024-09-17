---
title: Erste Schritte mit Adobe Campaign v8 nach der Umstellung vom Campaign Standard
description: Erfahren Sie, welche Schritte für die ersten Schritte mit Ihrer neuen Campaign v8-Anwendung erforderlich sind.
role: User, Admin, Developer
level: Beginner
source-git-commit: a1c16a9ba5e5ca844eaf82ed3b587f4f7a0b0873
workflow-type: tm+mt
source-wordcount: '1560'
ht-degree: 35%

---


# Von Campaign Standard zu v8 {#ac-acs}

Herzlich willkommen bei Adobe Campaign v8!

Wenn ein Benutzer von Campaign Standard auf Campaign v8 umstellt, ist dieses Referenzhandbuch für Sie gedacht. Dies hilft Ihnen, sich mit Ihrer neuen Campaign-Umgebung vertraut zu machen und Sie durch die Schritte zu führen, die zum Einstieg in Ihre Rolle erforderlich sind.

1. Beginnen Sie mit dem Erlernen von [neuen Funktionen in Adobe Campaign v8](#new).

1. Als Nächstes verstehen Sie [die Erlebnisunterschiede zwischen Adobe Campaign Standard und Adobe Campaign v8 gemäß Ihrer Rolle](#experiences).

## Neue Funktionen {#new}

Verschaffen Sie sich auf dieser Seite einen Überblick über die neuesten Verbesserungen in der Adobe Campaign-Web-Benutzeroberfläche. Eine umfassende Liste der wichtigsten Funktionen und Funktionen zur Aktualisierung von Versionen finden Sie in [diesem Abschnitt](../../v8/rn/whats-new.md).

### Verbesserungen mit Campaign v8 {#ac-enhancements}

Die wichtigsten Verbesserungen von Adobe Campaign v8 sind unten aufgeführt.

* **Web-Benutzeroberfläche**

  Adobe Campaign v8 bietet sowohl eine Client-Konsole als auch eine Web-Benutzeroberfläche, die unterschiedlichen Benutzervorlieben und Anforderungen gerecht wird. Die Client-Konsole bietet ein leistungsstarkes Desktop-Programm-Erlebnis, während die Web-Benutzeroberfläche intuitiv und barrierefrei gestaltet ist, sodass sie für Marketingexperten, die mit Adobe Campaign Standard vertraut sind, ideal geeignet ist.

  Die Webbenutzeroberfläche weist viele Ähnlichkeiten mit Adobe Campaign Standard auf, auch wenn einige Begriffe unterschiedlich sein können.

  Weitere Informationen zur Adobe Campaign-Webbenutzeroberfläche finden Sie hier ](../../v8/campaign-web-home.md).[

  ![](assets/home.png){zoomable="yes"}

  Alle neuen Funktionen und Verbesserungen sind in den [Versionshinweisen](../../v8/rn/release-notes.md) aufgeführt. Die Versionen der Adobe Campaign Web-Benutzeroberfläche basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren, schrittweisen Ansatz für die Implementierung von Funktionen ermöglicht. Dementsprechend werden diese Versionshinweise mehrmals im Monat aktualisiert. Sie sollten daher regelmäßig nachschauen.


* **Leistung**

  Adobe Campaign v8 nutzt fortschrittliche Cloud-basierte Datenbanktechnologien, was zu einer deutlich verbesserten Leistung und Effizienz führt. Diese neu gestaltete Architektur bietet mehrere wesentliche Vorteile:

   * *Skalierung*: Das System unterstützt jetzt eine erhebliche Erweiterung der Verarbeitungsfunktionen, wobei der Batch-Verarbeitungsdurchsatz bis zu **20 Millionen Vorgänge pro Stunde** erreicht. Mit dieser neuen Architektur können noch höhere Profile mit vorhersehbarer Leistung verwaltet werden.
   * *Geschwindigkeit*: Das System wurde für jede Marketing-Aktivität verbessert: Segmentierung, Versandvorbereitung oder Durchsatz für Transaktionsnachrichten, der jetzt **1 Million pro Stunde** beträgt.

  Die vollständig verwalteten Cloud Services bieten Benutzern Folgendes:

   * Datenanalyse in Echtzeit: Sie können sofort auf Daten zugreifen und diese analysieren, um schnelle Einblicke zu erhalten und fundiertere Entscheidungen zu treffen.

   * Schnelles Erstellen von Zielgruppen: Einfaches Erstellen zielgerichteter Zielgruppen innerhalb von Minuten für eine effizientere Kampagnensegmentierung.

  Die robuste Architektur von Adobe Campaign v8 bietet eine leistungsstarke Grundlage für die Verwaltung umfangreicher und komplexer Marketingkampagnen mit verbesserter Geschwindigkeit und Effizienz.

### Neue Funktionen in Adobe Campaign v8 {#ac-new-features}

Als Campaign Standard, der zu Adobe Campaign v8 wechselt, stehen Ihnen jetzt die folgenden Funktionen zur Verfügung:

* **Rich push**

  Adobe Campaign v8 bietet die Möglichkeit, Rich-Push-Benachrichtigungen zu versenden, um die Aufmerksamkeit der Benutzer zu erfassen und sie zu Maßnahmen zu ermutigen. Diese Benachrichtigungen können eine Vielzahl von Elementen umfassen, wie Text, Bilder, Schaltflächen, Countdown-Timer, Töne usw.

  ![](../../v8/push/assets/rich_push.png){zoomable="yes"}

  Um die Erstellung dieser Rich-Benachrichtigungen zu erleichtern, stellt Adobe Campaign v8 verschiedene Vorlagen bereit, mit denen Sie den Inhalt komplexer Benachrichtigungen, wie Karussells oder Timer, entwerfen und anpassen können.

  Sie können Ihre Benachrichtigungen nach dem System des Kunden anpassen:

   * Für [Android](../../v8/push/rich-push.md)-Vorlagen

   * Für [iOS](../../v8/push/rich-push.md)-Vorlagen

  Push-Benachrichtigungen sind ein wichtiges Tool, um Benutzer mobiler Apps anzusprechen und zu erreichen, selbst wenn sie Ihre App nicht aktiv verwenden.

* **Adobe Experience Manager as a Cloud Service**

  Adobe Campaign v8 ist nahtlos in Adobe Experience Manager as a Cloud Service integriert, sodass Sie Ihren Kunden personalisierte und inhaltsreiche Erlebnisse bieten können. Diese native Integration optimiert das Content Management und nutzt die robusten Funktionen von Adobe Experience Manager zur Optimierung Ihrer Marketing-Maßnahmen.

  Im Folgenden finden Sie die wichtigsten Funktionen, die durch diese Integration aktiviert werden:

   * *Asset-Verwaltung*: In Adobe Campaign v8 bietet der E-Mail-Designer eine Auswahl für den Zugriff auf und die Verwaltung von Assets. Diese Funktion vereinfacht die Integration von Elementen aus Adobe Experience Manager in Ihre Bereitstellung und sorgt so für eine effizientere Verwaltung von Inhalten. [Weitere Informationen zur Asset-Verwaltung](../../v8/integrations/aem-assets.md)

     ![](../../v8/integrations/assets/assets_6.png){zoomable="yes"}

   * *Import von E-Mail-Vorlagen*: Mit Adobe Campaign v8 können Sie E-Mail-Vorlagen aus Adobe Experience Manager direkt in Campaign durchsuchen und importieren. [Weitere Informationen zum Import von E-Mail-Vorlagen](../../v8/integrations/aem-content.md)

     ![](../../v8/integrations/assets/aem_6.png){zoomable="yes"}

  Adobe Experience Manager as a Cloud Service bietet Cloud-native Agilität, mit der Sie Ihre Wertschöpfungszeit verkürzen und sich an die sich wandelnden Geschäftsanforderungen anpassen können. Diese Integration verbessert nicht nur Ihre Content-Management-Funktionen, sondern ermöglicht Ihnen auch, Ihren Kunden personalisiertere und ansprechendere Erlebnisse an allen Touchpoints bereitzustellen.

* **AI-Assistent - Content Accelerator**

  Der Campaign-KI-Assistent ermöglicht die Erstellung und Ausführung von Marketingkampagnen über verschiedene Kanäle wie E-Mail, SMS und Push hinweg intuitiv, einfach und unkompliziert, während gleichzeitig Zeit eingespart, die Effizienz verbessert und bessere Ergebnisse erzielt werden.

  ![](../../v8/email/assets/full-email-1.png){zoomable="yes"}

  Der AI-Assistent revolutioniert die kanalübergreifende Erstellung professioneller und markenkonsistenter Inhalte. Mit fortschrittlichen GenAI-Modellen und einem tiefen Verständnis Ihrer Markenrichtlinien generiert der KI-Assistent automatisch personalisierte, ansprechende und effektive Inhalte basierend auf dem Marketingziel. Die Inhalte sind für markenumrissene Stile, Layouts, Ton und mehr optimiert.

  Der KI-Assistent ermöglicht die intuitive, einfache und unkomplizierte Erstellung und Ausführung von Marketing-Kampagnen, spart Zeit, verbessert die Effizienz und sorgt für bessere Ergebnisse.

  ![](../../v8/email/assets/full-email-2.png){zoomable="yes"}

  Es bietet eine Reihe von E-Mail-Vorlagen und erzeugt und erzeugt Bilder neu. Weitere Informationen zum AI-Assistenten - Content Accelerator finden Sie in [diesem Abschnitt](../../v8/email/generative-content.md). Adobe Campaign v8 verfügt über einen KI-Assistenten für [E-Mail](../../v8/email/generative-content.md), [SMS](../../v8/email/generative-sms.md) und [Push](../../v8/email/generative-push.md).

* **Aktualisierte SMS-Infrastruktur - SMS v2.0**

  Dank der Einfachheit und der einfachen Bedienung von SMS ist SMS ein sehr wertvoller Kommunikationskanal, der neben seiner Robustheit und der unübertroffenen Kompatibilität gegenüber Milliarden von Terminals sehr wertvoll ist.

  Adobe Campaign v8 verfügt über eine neue Infrastruktur, die den SMS-Versand verbessert. [Erfahren Sie mehr über die neuen SMS-Einstellungen](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.

* **Aktualisierte Push-Infrastruktur**

  Adobe Campaign v8 führt den neuesten Push-Benachrichtigungsdienst ein, der auf einem robusten Framework basiert, das auf modernster Technologie basiert. Dieser Dienst wurde entwickelt, um neue Ebenen der Skalierbarkeit zu erschließen und sicherzustellen, dass Ihre Benachrichtigungen eine größere Zielgruppe mit nahtloser Effizienz erreichen können. Mit unserer verbesserten Infrastruktur und optimierten Prozessen können Sie höhere Skalierbarkeit und Zuverlässigkeit erwarten, die es Ihnen ermöglicht, mit Ihren App-Nutzenden wie nie zuvor in Kontakt zu treten und Verbindungen herzustellen.

  [Erfahren Sie mehr über die aktualisierte Push-Infrastruktur](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.


## Managed Services {#ac-managed-services}

Adobe Campaign v8 ist als Managed Cloud Service verfügbar und bietet proaktive Überwachung, zeitgerechte Warnmeldungen und Service-Governance. Adobe Managed Cloud Service bietet Marketing-Experten eine agilere, sicherere und skalierbarere Lösung für das Cross-Channel-Kampagnen-Management mit niedrigen Gesamtbetriebskosten. Das neue Angebot kombiniert Services mit einer proaktiven Überwachung und rechtzeitigen Warnmeldungen.

## Campaign Standard-Funktionen hinzugefügt in v8 {#ac-v8-added}

Damit Sie reibungslos zu Campaign v8 wechseln können, wurden wichtige Funktionen von Campaign Standard in Campaign v8 aufgenommen. Weitere Informationen dazu finden Sie in [dieser Dokumentation](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de){target="_blank"}.

* **Dynamisches Reporting**: Das dynamische Reporting ermöglicht vollständig anpassbare und in Echtzeit aktualisierte Berichte, um die Wirkung Ihrer Marketing-Aktivitäten zu messen. Durch diese Funktion kann auf Profildaten zugegriffen werden, was die demografische Analyse nach Profildimensionen wie Geschlecht, Stadt und Alter sowie nach Daten von E-Mail-Kampagnen wie Öffnungen und Klicks ermöglicht. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=de){target="_blank"}.

* **Zentrales Branding**: Jedes Unternehmen hat seine Richtlinien bezüglich der Darstellung und technischen Charakteristika seiner Marken. Mit Adobe Campaign können Sie Spezifikationen festlegen, um Ihre Marke Ihren Kundinnen und Kunden einheitlich zu präsentieren, angefangen bei den Logos bis hin zu technischen Aspekten wie E-Mail-Absenderinnen und -Absendern, URLs oder Domains. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=de)

* **Rest-APIs**: Wenn Sie von Campaign Standard migriert sind, können Sie REST-APIs verwenden, um Integrationen für Adobe Campaign zu erstellen und Ihr eigenes Ökosystem zu erstellen, indem Sie Adobe Campaign mit den von Ihnen verwendeten Technologien verbinden. [Weitere Informationen](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=de){target="_blank"}.

* **Landingpages**: An den Landingpages von Campaign v8 wurden einige Verbesserungen vorgenommen, damit die Funktionen mit denen von Campaign Standard vergleichbar sind. Weitere Informationen finden Sie in den [Versionshinweisen](../../v8/rn/release-notes.md#new-24-4) und in der [Dokumentation](../../v8/landing-pages/get-started-lp.md) zu Landingpages.

* **Visuelle Fragmente**: Visuelle Fragmente sind wiederverwendbare visuelle Komponenten, die in einer oder mehreren E-Mail-Sendungen oder in Inhaltsvorlagen referenziert werden können. Wenn Sie ein Fragment ändern, wird jeder Inhalt, der dieses Fragment verwendet, aktualisiert. Diese Funktionalität ermöglicht es, mehrere benutzerdefinierte Inhaltsbausteine vorab zu erstellen, die anschließend von Benutzenden aus dem Bereich Marketing verwendet werden können, um NachrichtenInhalte in einem verbesserten Designprozess schnell zusammenzustellen. [Weitere Informationen](../../v8//content/use-visual-fragments.md)

## Wichtige Unterschiede zwischen Campaign Standard und Campaign v8 {#experiences}

Die meisten Konzepte sind zwischen Adobe Campaign v8 und Adobe Campaign Standard ähnlich. Es gibt jedoch einige Unterschiede, wie unten beschrieben.

### Terminologieänderungen {#terminology-changes}

Nachstehend finden Sie einige terminologische Unterschiede zwischen Campaign Standard und Campaign v8.

* Benutzerdefinierte Ressourcen sind **Schemata**
* Nachrichten werden als **Sendungen** bezeichnet
* Benutzende des Produkts bleiben **Benutzende**. (Im Englischen wird jedoch zwischen „Users“ und „Operators“ unterschieden.)
* Rollen werden mit **spezifischen Berechtigungen** konfiguriert
* Sicherheitsgruppen sind **Benutzergruppen**
* Organisationseinheiten werden über **Ordnerberechtigungen** verwaltet

Beachten Sie außerdem, dass als bestehender Campaign-Benutzer einige Konzepte in Übereinstimmung mit den neuesten Terminologiestandards umbenannt wurden. Diese Änderungen betreffen nur die Campaign Web-Benutzeroberfläche, nicht aber die Client-Konsole. Sie sind unten zusammengefasst.

* Empfängerinnen und Empfänger werden jetzt als **Profile** bezeichnet. [Weitere Informationen](../../v8/audience/gs-audiences-recipients.md).
* Testadressen werden jetzt als **Testprofile** bezeichnet. [Weitere Informationen](../../v8/preview-test/test-deliveries.md).
* Die Versandanalyse heißt jetzt **Versandvorbereitung**. Wenn Sie die Vorbereitung von Nachrichten starten möchten, klicken Sie auf die Schaltfläche **Vorbereiten**.  [Weitere Informationen](../../v8/monitor/prepare-send.md).
* Die E-Mail-Vorschau ist jetzt über die Schaltfläche **Inhalt simulieren** verfügbar. [Weitere Informationen](../../v8/preview-test/preview-test.md)
* Listen heißen jetzt **Zielgruppen**. [Weitere Informationen](../../v8/audience/gs-audiences-recipients.md).

## Neues Benutzererlebnis

Rufen Sie das entsprechende Referenzhandbuch für Ihre Rolle auf, um das neue Benutzererlebnis mit Adobe Campaign v8 kennenzulernen.

<table>
<tr>
  <td>
    <a href="marketers.md">
      <img alt="Kampagnenverantwortliche Benutzerinnen und Benutzer"src="./assets/digital_marketing.jpeg"/>
    </a>
    <div>
  </td>
  <td>
  <a href="admin-developers.md">
    <img alt="Admins oder Entwicklerinnen bzw. Entwickler" src="./assets/admin.jpeg"/>
    </a>
    <div>
  </td>
  </tr>
  <tr>
    <td>
    <a href="marketers.md">
    <strong>Marketing-Fachleute</strong>
    </a>
    </td>
    <td>
      <a href="admin-developers.md">
      <strong>Admins oder Entwicklerinnen bzw. Entwickler</strong>
      </a>
    </td>
  </tr>
    <td>
    <em>Kampagnen-Managerinnen und -Manager, Fachleute für Medien-Marketing</em>
    </td>
    <td>
      <em> Systemadmins, Fachleute für technisches Marketing</em>
    </td>
  <tr>
    <td>
    <b>Zu den wichtigsten Aufgaben/Verantwortlichkeiten gehören:</b>
    </td>
      <td>
    <b>Zu den wichtigsten Aufgaben/Verantwortlichkeiten gehören:</b>
    </td>
  </tr>
  <tr>
    <td>
      <li>Erstellen von Marketing-Kampagnen
      <li>Entwerfen von Workflows
      <li>Testen und Ausführen von Kampagnen
      <li>Bereitstellen von Multi-Channel-Kampagnen
      <li>Optimieren von Kampagnen
      <li>Optimieren von automatisierten Kampagnen
    </td>
    <td>
        <li>Zugriffsverwaltung 
        <li>Systemkonfiguration
        <li>Systemanpassung
    </td>
</tr>
</table>
</div>

<!--
## Deprecated items

Adobe constantly evaluates product capabilities to identify older features that should be replaced with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility.

Please refer to [this documentation for information on deprecated items](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features).-->

