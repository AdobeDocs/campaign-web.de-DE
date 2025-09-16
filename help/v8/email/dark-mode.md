---
title: Wechseln zum dunklen Modus
description: Erfahren Sie, wie Sie den Dunkelmodus in der Adobe Campaign Email Designer verwenden.
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: Dunkler Modus, E-Mail, Farbe, Editor
hide: true
hidefromtoc: true
source-git-commit: b85a78cf89586679630398f5f3c7d732a59711fd
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 4%

---

# Verwalten von Inhalten für den dunklen Modus {#dark-mode}

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode"
>title="Wechseln zum dunklen Modus"
>abstract="Wechseln Sie in den Dunkelmodus, in dem Sie eine Vorschau des Renderings anzeigen und spezifische benutzerdefinierte Einstellungen definieren können. <br>Das endgültige Rendering hängt vom E-Mail-Client des Empfängers ab. Beachten Sie, dass nicht alle E-Mail-Clients den benutzerdefinierten Dunkelmodus unterstützen."

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode_preview"
>title="Wechseln zum dunklen Modus"
>abstract="Wechseln Sie zum dunklen Modus, um eine Vorschau des Renderings auf unterstützenden E-Mail-Clients anzuzeigen. <br>Das endgültige Rendering hängt vom E-Mail-Client des Empfängers ab. Beachten Sie, dass alle E-Mail-Clients den Dunkelmodus nicht unterstützen."

Designer Beim Entwerfen Ihrer E-Mails können Sie mit [!DNL Adobe Campaign] [E-Mail-](get-started-email-designer.md)) zur Ansicht **[!UICONTROL Dunkelmodus]** wechseln.

In dieser Ansicht <!--Email Designer -->Dunkelmodus“ können Sie auch spezifische benutzerdefinierte Einstellungen definieren, die von den unterstützenden E-Mail-Clients angezeigt werden, wenn ihr Dunkelmodus aktiviert ist.

## Was ist der Dunkelmodus? {#what-is-dark-mode}

Die Art und Weise, wie der Dunkelmodus in den verschiedenen E-Mail-Clients gerendert wird, ist komplex. Definieren wir zunächst den Dunkelmodus.

Der Dunkelmodus ermöglicht es den unterstützenden E-Mail-Clients und -Programmen, E-Mails mit dunkleren Hintergründen und helleren Farben für Text, Schaltflächen und andere Benutzeroberflächenelemente anzuzeigen. Dadurch werden die Augen entlastet, die Akkulaufzeit verkürzt und die Lesbarkeit in schwach beleuchteten Umgebungen verbessert, sodass das Betrachten angenehmer wird.

Aufgrund des wachsenden Trends bei den wichtigsten Betriebssystemen und Apps <!-- (Apple Mail, Gmail, Outlook, Twitter, Slack)--> es eine wichtige Überlegung im modernen E-Mail-Design, sicherzustellen, dass Inhalte für alle Benutzer lesbar und visuell ansprechend bleiben.

## Schutzmechanismen {#guardrails}

Die Erwartungen in Bezug auf das Rendering im Dunkelmodus müssen mit Vorsicht berücksichtigt werden, da die Art und Weise, wie sie von den verschiedenen E-Mail-Clients angewendet wird, stark variieren kann.

<!--The dark mode final rendering depends on the recipient's email client. It is not possible to guarantee that your email will look the same in dark mode across all devices.-->

Bevor Sie den Dunkelmodus in der [!DNL Adobe Campaign] E-Mail-Designer verwenden, müssen Sie wissen, wie die wichtigsten E-Mail-Clients damit umgehen. Es gibt drei Fälle, in denen unterschieden werden muss:

<!--
* Check out the list of [email clients supporting dark mode](https://www.caniemail.com/search/?s=dark){target="_blank"}

* Learn more on Dark mode in this [Litmus blog post](https://www.litmus.com/blog/the-ultimate-guide-to-dark-mode-for-email-marketers){target="_blank"}
-->

### Clients unterstützen keinen Dunkelmodus {#not-supporting}

Einige E-Mail-Clients unterstützen diese Funktion überhaupt nicht, z. B.:

* Yahoo!Mail
* AOL

Unabhängig davon, ob Sie benutzerdefinierte Einstellungen für den Dunkelmodus in der E-Mail-Designer definieren oder nicht, zeigen diese E-Mail-Clients nie Rendering im Dunkelmodus an. <!--Regardless of whether the interface is in light or dark mode, your email will render the same.-->

### Clients, die ihren eigenen Dunkelmodus anwenden {#default-support}

Einige E-Mail-Clients wenden systematisch ihren eigenen standardmäßigen Dunkelmodus auf alle empfangenen E-Mails an. Farben, Hintergründe, Bilder usw. werden automatisch mit den für den E-Mail-Client spezifischen Einstellungen für den Dunkelmodus angepasst, was bedeutet, dass keine externe Änderung möglich ist.

<!--It is important to note that less than 25% of email clients offer customization options for dark mode. Clients such as Gmail implement their own dark mode rendering, which is not subject to external modification.-->

Diese Clients sind zum Beispiel:

* Gmail (Desktop-Webmail, iOS, Android, mobile Webmail)
* Outlook-Fenster
* Outlook Windows Mail

Wenn Sie in diesem Fall benutzerdefinierte Einstellungen für den Dunkelmodus in der E-Mail-Designer definieren, werden diese Einstellungen mit den E-Mail-Client-Einstellungen überschrieben.

Es ist wichtig zu verstehen, dass diese E-Mail-Clients den Dunkelmodus verarbeiten, aber Ihr spezifisches Design für den Dunkelmodus wird nicht gerendert.

### Clients, die den benutzerdefinierten Dunkelmodus unterstützen {#custom-support}

Andere E-Mail-Clients bieten die Option, den benutzerdefinierten Dunkelmodus mit der `@media (prefers-color-scheme: dark)`-Abfrage zu rendern, was die von der [!DNL Journey Optimizer] E-Mail-Designer verwendete Methode ist.

Im Folgenden finden Sie eine Liste der wichtigsten Clients, die diese Option handhaben:

* Apple Mail macOS
* Apple Mail iOS
* Outlook macOS
* Outlook.com
* Outlook iOS
* Outlook Android

In diesem Fall sollten die spezifischen Einstellungen angezeigt werden, die Sie in der E-Mail-Designer definieren.

>[!NOTE]
>
>In diesem Abschnitt erfahren Sie, wie Sie mit der E-Mail-Designer benutzerdefinierte Einstellungen für [ Dunkelmodus ](#define-custom-dark-mode).

Je nach E-Mail-Client können jedoch einige Einschränkungen gelten. Beispielsweise erzeugen einige Clients wie Apple Mail 16 (macOs 13) keinen Dunkelmodus, wenn im E-Mail-Inhalt Bilder vorhanden sind.

Um optimale Ergebnisse zu erzielen, testen Sie Ihren Inhalt mit den anvisierten E-Mail-Clients. Um eine Simulation anzuzeigen, die dem Endergebnis für jeden Client so nahe wie möglich kommt, verwenden Sie die Option [E-Mail-Rendering](../preview-test/email-rendering.md) in der E-Mail-Designer.

## Dunkler Modus in der E-Mail-Designer {#dark-mode-email-designer}

Beim Dunkelmodus in der E-Mail-Designer sind zwei Aspekte zu berücksichtigen:

* Sie können eine Vorschau davon erhalten, wie der standardmäßige Dunkelmodus in den meisten unterstützenden E-Mail-Clients gerendert wird. [Weitere Informationen](#preview-dark-mode)

* Wenn Sie die Standardeinstellungen von E-Mail-Clients ([ benutzerdefinierten Dunkelmodus unterstützen) ](#custom-support) möchten, können Sie benutzerdefinierte Einstellungen für die E-Mail definieren, die Sie bearbeiten. [Weitere Informationen](#define-custom-dark-mode)

### Vorschau des standardmäßigen Dunkelmodus {#preview-dark-mode}

Gehen Sie wie folgt vor, um auf den Dunkelmodus in der E-Mail-Designer zuzugreifen und eine Vorschau der Standardeinstellungen für den Dunkelmodus zu erhalten.

1. Wählen Sie auf der Startseite von Email Designer die Option **[!UICONTROL Erstellen von neuen Inhalten]** aus. [Weitere Informationen](create-email-content.md)

1. Fügen Sie [Strukturen](create-email-content.md) und [Inhaltskomponenten) ](content-components.md) Inhalt hinzu.

1. Schalten Sie oben rechts auf der zentralen Arbeitsfläche den Umschalter in den **[!UICONTROL Dunkelmodus]**.

   ![](assets/light-mode-toggle.png)

1. Die standardmäßige Vorschau des Dunkelmodus wird angezeigt.

   ![](assets/dark-mode-default.png)

Standardmäßig wendet die Vorschau des Dunkelmodus-Modus von Email Designer das Farbschema „Vollfarbinvertierung“ auf alle Elemente außer Bildern und Symbolen an.

Das bedeutet, dass Bereiche mit hellen und dunklen Elementen erkannt und invertiert werden, sodass helle Hintergründe dunkel und dunkler Text hell werden, während dunkle Hintergründe hell und heller Text dunkel werden.

>[!CAUTION]
>
>Das endgültige Rendering kann je nach E-Mail-Client des Empfängers variieren. Um für jeden E-Mail-Client eine Simulation anzuzeigen, die dem Endergebnis möglichst nahe kommt, verwenden Sie die Option [E-Mail-Rendering](../preview-test/email-rendering.md).

### Definieren des benutzerdefinierten Dunkelmodus {#define-custom-dark-mode}

>[!CONTEXTUALHELP]
>id="ac_edition_darkmode_image"
>title="Verwenden eines bestimmten Bildes für den dunklen Modus"
>abstract="Es kann ein anderes Bild ausgewählt werden, das angezeigt wird, wenn der dunkle Modus aktiviert ist. <br>Das Hinzufügen eines bestimmten Bildes für den Dunkelmodus garantiert nicht, dass es in allen E-Mail-Clients korrekt gerendert wird. Beachten Sie, dass nicht alle E-Mail-Clients den benutzerdefinierten Dunkelmodus unterstützen."

Nach dem Wechsel **[!UICONTROL Dunkler Modus]** können Sie bestimmte Stilelemente Ihres Inhalts bearbeiten, die nur angezeigt werden, wenn der Dunkle Modus im E-Mail-Client des Empfängers aktiviert ist - vorausgesetzt, diese Funktion wird unterstützt.

>[!WARNING]
>
>Das endgültige Rendering im Dunkelmodus hängt von jedem E-Mail-Client ab, sodass die Ergebnisse von einem zum anderen variieren können. [Weitere Informationen](#guardrails)

<!--
>[!WARNING]
>
>Not all email clients support dark mode. Moreover, some email clients only apply their own default dark mode for all emails that are received. In both cases, the custom settings that you defined in the Email Designer cannot be rendered.-->

Um den benutzerdefinierten Dunkelmodus-Stil von E-Mail-Designer zu nutzen, verwendet Journey Optimizer den<!-- `@media (prefers-color-scheme: dark)` method--> `@media (prefers-color-scheme: dark)` CSS-Abfrage, die erkennt, ob der E-Mail-Client des Benutzers auf den Dunkelmodus eingestellt ist, und das in Ihrer E-Mail definierte Design mit dunklem Design anwendet.

Gehen Sie wie folgt vor, um benutzerdefinierte Einstellungen für den Dunkelmodus zu definieren.

1. Stellen Sie sicher, dass Sie in der E **[!UICONTROL Mail-Designer in den]** Dunkelmodus“ wechseln. [Weitere Informationen](#preview-dark-mode)

1. Bearbeiten Sie alle Stilattribute wie Text, Hintergrund, Schaltfläche usw.

1. Sie können die Farben von Bildern und Symbolen nicht ändern, aber Sie können bestimmte Assets nur für den Dunkelmodus definieren.

   Wählen Sie dazu ein Bild aus. Wechseln Sie **[!UICONTROL Dunkler Modus]** über den entsprechenden Umschalter im Bereich **[!UICONTROL Einstellungen]** und wählen Sie ein anderes Asset aus.

   ![](assets/dark-mode-image.png)

   <!--![](assets/dark-mode-custom.png)-->

1. Sie können jederzeit **[!UICONTROL Zur Live-Ansicht wechseln]** um zu überprüfen, wie Ihre Inhalte auf verschiedenen Gerätegrößen gerendert werden können. Wählen Sie in dieser Ansicht den Umschalter für den Dunkelmodus oben auf dem Bildschirm aus, um eine Vorschau der Dunkelmodusversion Ihres Inhalts auf den verschiedenen Geräten anzuzeigen.

   ![](assets/dark-mode-live-view.png){width="80%" align="center"}

   >[!CAUTION]
   >
   >Die Live-Ansicht ist eine allgemeine Vorschau, die vergleicht, wie das Rendering über verschiedene Gerätegrößen hinweg aussehen könnte. Das endgültige Rendering kann je nach E-Mail-Client des Empfängers variieren.

1. Wenn Sie mit den Änderungen für den Dunkelmodus zufrieden sind, klicken Sie auf **[!UICONTROL Inhalt simulieren]**.

   ![](assets/dark-mode-simulate.png)

1. Wählen Sie **[!UICONTROL E-Mail rendern]** und verbinden Sie sich mit Ihrem Litmus-Konto. Sie können das endgültige Rendering des Dunkelmodus für verschiedene E-Mail-Clients sehen. Weitere Informationen zu [E-Mail-Rendering](../preview-test/email-rendering.md).

   >[!WARNING]
   >
   >Während die Simulation dem Aussehen von E-Mails im Dunkelmodus sehr nahe kommt, kann das tatsächliche Rendering aufgrund von Variationen bei E-Mail-Service-Anbietern oder Einstellungen auf Geräteebene unterschiedlich sein.

## Best Practices {#best-practices}

Da die Akzeptanz des Dunkelmodus in den wichtigsten E-Mail-Clients zunimmt, ist es wichtig zu berücksichtigen, wie Ihre E-Mails in hellen und dunklen Umgebungen gerendert werden - unabhängig davon, ob [ den benutzerdefinierten Dunkelmodus ](#define-custom-dark-mode) oder nicht.

Der Dunkelmodus kann Farben, Hintergründe und Bilder verändern - und manchmal die Designentscheidungen überschreiben. Befolgen Sie die unten aufgeführten Best Practices, um visuelle Konsistenz, Barrierefreiheit und Markenintegrität sicherzustellen.

**Optimieren Sie Ihre Bilder und Logos**

* Speichern Sie Logos und Symbole als PNGs mit transparentem Hintergrund, um sichtbare weiße Kästchen im Dunkelmodus zu vermeiden.

* Vermeiden Sie Bilder mit hartcodierten weißen oder hellen Hintergründen.

* Wenn Transparenz nicht möglich ist, platzieren Sie Bilder auf einem einfarbigen Hintergrund in Ihrem Design, um unangenehme Farbinversionen zu verhindern.

**Achten Sie auf Ihre Hintergründe**

* Sicherstellen von ausreichendem Kontrast zwischen Text- und Hintergrundfarben für bessere Lesbarkeit im hellen und dunklen Modus.

* Vermeiden Sie es, sich bei kritischen Inhalten allein auf Hintergrundfarben zu verlassen. Einige Clients überschreiben Hintergrundfarben im Dunkelmodus, sodass Sie sicherstellen müssen, dass wichtige Informationen weiterhin sichtbar sind.

<!--**Inline critical styles**

Inline CSS helps maintain more control over styling, as some clients strip external styles in dark mode.-->

**Entwerfen barrierefreier Inhalte im Dunkelmodus**

<!--KEEP dark mode accessibility best practices IN ONE SINGLE LOCATION - for now listed on this page.
If needed, it can be moved to the Design accessible content page:
The best practices for designing accesible content in dark mode are listed in [this section](accessible-content.md#dark-mode).-->

* Verwenden Sie Farbkombinationen, die für Menschen mit Farbenblindheit leicht zu unterscheiden sind.

* Verwenden Sie eine Mitteltonpalette, um Kontrast sowohl vor hellen als auch vor dunklen Hintergründen sicherzustellen.

* Verwenden Sie barrierefreie Farbkombinationen mit hohem Kontrast, um die Lesbarkeit zu verbessern und die WCAG-Standards (Web Content Accessibility Guidelines) zu erfüllen. Verwenden Sie Tools wie den Kontrast-Checker von WebAIM, um den Farbkontrast zu überprüfen.

* Vermeiden Sie dünne Schriftarten, da sie die Lesbarkeit beeinträchtigen können. Wenn für Ihre Marke eine dünne Schriftart erforderlich ist, fett formatieren Sie sie im dunklen Modus.

* Überspringen Sie reines Weiß auf reinem Schwarz, da es zu Augenbelastungen führen kann und von einigen E-Mail-Clients automatisch invertiert werden kann.

* Wenn der Dunkelmodus nicht unterstützt wird, können barrierefreie Ausweich-Stile bereitgestellt werden.

**Testen Sie Ihre E-Mails in einer Umgebung im dunklen Modus**

* Verwenden Sie die E-Mail[Designer-Vorschau ](#preview-dark-mode) Dunkelmodus, die invertierte Farbschemata verwendet, um Probleme frühzeitig zu erkennen.

* Verwenden Sie die Option [E-Mail-Rendering](../preview-test/email-rendering.md), die Litmus nutzt, um Ihre Designs in wichtigen E-Mail-Clients (Apple Mail, Gmail, Outlook) zu simulieren und zu sehen, wie sich Farben und Bilder im Dunkelmodus verhalten.
