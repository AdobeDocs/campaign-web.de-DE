---
title: Erste Schritte mit dynamischen Inhalten
description: Erfahren Sie, wie Sie Ihren Inhalt mit Personalisierung, bedingtem Inhalt und integrierten Inhaltsbausteinen dynamisch gestalten können.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 39%

---


# Erste Schritte mit dynamischen Inhalten

Um jede Marketing-Kampagne optimal zu nutzen, bietet Ihnen Adobe Campaign eine Möglichkeit, benutzerdefinierte dynamische Inhalte bereitzustellen, die Kunden auf ihrer Ebene ansprechen. Verwenden Sie auf der Basis von Profildaten Personalisierungsfunktionen, um ein benutzerdefiniertes Erlebnis für verschiedene Gruppen und Personen zu erstellen: Sie können Ihre Nachrichten an jeden einzelnen Empfänger anpassen, indem Sie die vorhandenen Daten und Informationen nutzen. Dies können Vornamen, Interessen, Wohnorte, bisherige Käufe und vieles mehr sein.

Verwenden Sie Campaign, um dynamische Inhalte zu erstellen und personalisierte Nachrichten zu versenden. Personalisierungsfunktionen können kombiniert werden, um Ihre Nachrichten zu verbessern und ein individuelles Benutzererlebnis zu schaffen.

Der Nachrichteninhalt kann dynamisch gestaltet werden, indem Sie Folgendes einfügen:

* **Personalisierungsfelder**

   Personalisierungsfelder werden für die oberste Ebene der Nachrichtenpersonalisierung verwendet. Sie können jedes in der Datenbank verfügbare Feld aus dem Personalisierungseditor auswählen. Für einen Versand können Sie jedes Feld auswählen, das sich auf die Empfängerin oder den Empfänger, die Nachricht oder den Versand bezieht. Diese Personalisierungsattribute können in die Betreffzeile oder in den Text Ihrer Nachrichten eingefügt werden.

   ![](assets/perso-subject-line.png)

   Mit der folgenden Syntax wird die Stadt des Empfängers bzw. der Empfängerin in Ihren Inhalt eingefügt: &lt;%= recipient.location.city %>.

* **Bedingte Inhalte**

   Konfigurieren Sie bedingte Inhalte, um beispielsweise eine dynamische Personalisierung basierend auf dem Empfängerprofil hinzuzufügen. Textblöcke und/oder Bilder werden eingefügt, wenn eine bestimmte Bedingung erfüllt ist. Sie können die alternative Version des Inhalts definieren, wenn die Bedingung nicht wahr ist.

* **Integrierte Inhaltsbausteine**

   Campaign verfügt über eine Reihe von Gestaltungsbausteinen, die ein bestimmtes Rendering ermöglichen, das Sie in Ihre Sendungen einfügen können. Sie können beispielsweise ein Logo, eine Grußnachricht oder einen Link zur Mirrorseite einer E-Mail-Nachricht hinzufügen. Inhaltsbausteine sind über einen eigenen Eintrag im Personalisierungs-Editor verfügbar.

   ![](assets/perso-content-blocks.png)

## Wo kann ich dynamische Inhalte hinzufügen?

Adobe Campaign V8 Web bietet einen Ausdruckseditor, in dem Sie alle Daten auswählen, anordnen, anpassen und validieren können, um ein benutzerdefiniertes Erlebnis für Ihren Inhalt zu erstellen.

Der Ausdruckseditor ist für alle Kanäle und in allen Feldern mit dem Symbol Personalisierungsdialogfeld öffnen verfügbar, z. B. im Betreffzeilenfeld oder in den Komponenten für Text- und Schaltflächeninhalte in E-Mails.

![](assets/expression-editor-access.png)

![](assets/expression-editor-access-email.png)

Darüber hinaus steht beim Entwerfen einer E-Mail ein dedizierter Builder für bedingte Inhalte zur Verfügung. [Erfahren Sie, wie Sie bedingte Inhalte in E-Mails erstellen](conditions.md)

## Tauchen wir tiefer in die Materie ein

Nachdem Sie nun wissen, wie Sie Ihren Inhalt dynamisch gestalten können, ist es an der Zeit, diese Dokumentationsabschnitte näher zu untersuchen, um mit der Funktion zu beginnen.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Personalisieren von Inhalten" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Hinzufügen von Personalisierung</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Lead" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Hinzufügen bedingter Inhalte</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Gelegentlich" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Hinzufügen integrierter Inhaltsbausteine</strong></a>
</div>
<p></td>
</tr></table>
