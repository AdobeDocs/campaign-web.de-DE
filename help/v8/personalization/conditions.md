---
title: Erstellen bedingter Inhalte
description: Erfahren Sie, wie Sie in der Web-Benutzeroberfläche von Adobe Campaign Bedingungen definieren, um Ihre Inhalte zu personalisieren
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: c977f8e3567a478fa46dc8914c329ca4e8dd3274
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 96%

---

# Bedingte Inhalte erstellen{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Erstellen bedingter Inhalte"
>abstract="Erstellen Sie bedingte Inhalte als Grundlage für dynamische Personalisierung anhand des Empfängerprofils und zur automatischen Ersetzung von Textblöcken und Bildern, wenn bestimmte Bedingungen erfüllt sind. Mit dieser Funktion bringen Sie Ihre Kampagnen auf eine neue Ebene und können zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen."



>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Hinzufügen bedingter Inhalte"
>abstract="Konfigurieren Sie bedingte Inhaltsfelder, um eine erweiterte dynamische Personalisierung basierend auf den Profildaten des Empfängers zu erstellen. Textblöcke, Links, Betreffzeile und/oder Bilder werden im Nachrichteninhalt ersetzt, wenn eine bestimmte Bedingung erfüllt ist."

Bedingter Inhalt ist eine leistungsstarke Funktion, mit der Sie eine dynamische Personalisierung erstellen können, die auf dem Empfängerprofil basiert. Dabei werden Textblöcke und Bilder automatisch ersetzt, wenn bestimmte Bedingungen erfüllt sind. Mit dieser Funktion bringen Sie Ihre Kampagnen auf eine neue Ebene und können zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen.

Durch die Konfiguration bedingter Inhaltsfelder können Sie beispielsweise eine erweiterte dynamische Personalisierung erstellen, die auf dem Empfängerprofil basiert. Textblöcke, Links, Betreffzeile und/oder Bilder werden im Nachrichteninhalt ersetzt, wenn eine bestimmte Bedingung erfüllt ist. Beispielsweise kann „Herr“ oder „Frau“ entsprechend dem Wert für das Feld „Geschlecht“ in der Adobe Campaign-Datenbank eingesetzt oder je nach bevorzugter Empfängersprache ein anderer Link eingefügt werden.

## Erstellen bedingter Inhalte

Um bedingte Inhalte zu erstellen, müssen Sie Bedingungen im **Ausdruckseditor** mithilfe spezifischer Hilfsfunktionen erstellen. Diese Methode steht für alle Versandkanäle in jedem Feld zur Verfügung, in dem Sie auf den Ausdruckseditor zugreifen können, z. B. Betreffzeile, E-Mail-Links oder Text-/Schaltflächen-Inhaltskomponenten. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen](gs-personalization.md/#access)

Zusätzlich zum Ausdruckseditor können beim Entwerfen einer E-Mail Sie einen speziellen **Builder für bedingte Inhalte** nutzen. So können Sie Bedingungen nur mithilfe von Profilattributen erstellen. [Erfahren Sie, wie Sie bedingte Inhalte in E-Mails erstellen](#condition-condition-builder)

## Erstellen von Bedingungen im Ausdruckseditor {#condition-perso-editor}

Gehen Sie wie folgt vor, um mit dem Ausdruckseditor bedingte Inhalte für einen Versand zu definieren. In diesem Beispiel möchten wir bedingte Inhalte basierend auf der Sprache der Empfängerinnen oder Empfänger (Französisch oder Englisch) erstellen.

1. Öffnen Sie einen Versand und navigieren Sie zum Abschnitt für die Inhaltsbearbeitung.

1. Suchen Sie das Feld, dem bedingte Inhalte hinzugefügt werden sollen. Beispielsweise können Sie einer SMS-Nachricht bedingte Inhalte hinzufügen.

1. Klicken Sie neben dem Feld auf **[!UICONTROL Personalisierungsdialog öffnen]**, um den Ausdruckseditor zu öffnen.

   ![](assets/open-perso-editor-sms.png)

1. Navigieren Sie im Personalisierungseditor zum Menü **[!UICONTROL Hilfsfunktionen]** auf der linken Seite.

1. Um mit der Erstellung Ihrer Bedingung zu beginnen, klicken Sie auf das Symbol „+“ neben der Funktion **Wenn**. Die folgende Zeile wird zum mittleren Bereich des Bildschirms hinzugefügt:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersetzen Sie `<FIELD>` durch ein Personalisierungsfeld, z. B. die Empfängersprache: `recipient.language`.
   * Ersetzen Sie `<VALUE>` durch den Wert, der erfüllt werden soll. Zum Beispiel `'French'`.
   * Ersetzen Sie `Ìnsert content here` durch den Inhalt, der für die Profile angezeigt werden soll, die die angegebene Bedingung erfüllen.

     ![](assets/condition-sample1.png){width="800" align="center"}

1. Geben Sie den Inhalt an, der angezeigt werden soll, wenn die Empfängerinnen bzw. Empfänger die Bedingung nicht erfüllen. Verwenden Sie dazu die Hilfsfunktion **Sonst**:

   1. Platzieren Sie den Cursor vor dem schließenden Tag des Ausdrucks `%>` und klicken Sie auf `+` neben der Funktion **Sonst**.

   1. Ersetzen Sie `Ìnsert content here` durch den Inhalt, der für die Profile angezeigt werden soll, die die Bedingung der Wenn-Funktion nicht erfüllen.

   ![](assets/condition-sample2.png){width="800" align="center"}

   Sie können auch die Hilfsfunktion **Sonst wenn** zum Erstellen von Bedingungen mit mehreren Inhaltsvarianten verwenden. Der folgende Ausdruck zeigt beispielsweise drei Varianten einer Nachricht in Abhängigkeit von der Sprache der Empfängerinnen oder Empfänger:

   ![](assets/condition-sample3.png){width="800" align="center"}

   >[!NOTE]
   >
   >Jedes Mal, wenn eine Hilfsfunktion hinzugefügt wird, werden öffnende (`<%`) und schließende (`%>`) Tags vor und nach der Funktion automatisch hinzugefügt.
   >
   >Beispiel nach dem Hinzufügen einer Hilfsfunktion „Sonst“ innerhalb eines Ausdrucks: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Entfernen Sie diese Tags, um Syntaxfehler zu vermeiden. In diesem Beispiel lautet der korrigierte Ausdruck nach dem Entfernen der Tags der Funktion **Sonst**:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Sobald Ihre Bedingung fertig ist, können Sie Ihren Inhalt speichern und das Rendering überprüfen, indem Sie Ihren Inhalt simulieren.

## Erstellen von bedingten Inhalten in E-Mails {#condition-condition-builder}

Bedingte Inhalte in E-Mails können auf zwei Arten erstellt werden:
* Im Ausdruckseditor durch Erstellen einer Bedingung mit Hilfsfunktionen
* In einem speziellen Builder für bedingte Inhalte, auf den Sie beim Entwerfen einer E-Mail zugreifen können

Detaillierte Informationen zum Erstellen von Bedingungen mithilfe des Ausdruckseditors finden Sie [hier](#condition-perso-editor). Im folgenden Abschnitt finden Sie eine schrittweise Anleitung zum Erstellen von Bedingungen mithilfe der Funktion für bedingte Inhalte des E-Mail-Designers. In diesem Beispiel möchten wir eine E-Mail-Nachricht mit mehreren Varianten erstellen, die auf der Empfängersprache basieren. Führen Sie folgende Schritte aus:

1. Erstellen oder öffnen Sie einen E-Mail-Versand, bearbeiten Sie den Inhalt und klicken Sie auf die Schaltfläche **[!UICONTROL E-Mail-Text bearbeiten]**, um den Arbeitsbereich zum Entwerfen von E-Mails zu öffnen.

1. Wählen Sie eine Inhaltskomponente aus und klicken Sie auf das Symbol **[!UICONTROL Bedingten Inhalt aktivieren]**.

   ![](assets/condition-email-enable.png){width="800" align="center"}

1. Der Bereich **[!UICONTROL Bedingter Inhalt]** wird auf der linken Bildschirmseite geöffnet. In diesem Bereich können Sie mithilfe von Bedingungen mehrere Varianten der ausgewählten Inhaltskomponente erstellen.

1. Konfigurieren Sie Ihre erste Variante. Bewegen Sie den Mauszeiger über **[!UICONTROL Variante - 1]** im Bereich **[!UICONTROL Bedingter Inhalt]** und klicken Sie auf das Symbol **[!UICONTROL Bedingung hinzufügen]**.

1. Ein Regel-Builder wird angezeigt. Verwenden Sie Profilattribute, um die Bedingung für die erste Variante der Nachricht zu erstellen, und klicken Sie auf **[!UICONTROL Bestätigen]**. In diesem Beispiel wird eine Regel erstellt, die sich an Empfängerinnen und Empfänger richtet, deren Sprache „Französisch“ ist.

   ![](assets/condition-email-rule.png){width="800" align="center"}

1. Die Regel ist nun mit der Variante verknüpft. Um die Lesbarkeit zu verbessern, wird empfohlen, die Variante umzubenennen, indem Sie auf das Menü mit den Auslassungspunkten klicken.

1. Konfigurieren Sie, wie die Komponente angezeigt werden soll, wenn die Regel beim Senden der Nachricht erfüllt ist. In diesem Beispiel soll der Text auf Französisch angezeigt werden, wenn dies die bevorzugte Sprache der Empfängerin bzw. des Empfängers ist.

   ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Fügen Sie so viele Varianten hinzu, wie für die Inhaltskomponente erforderlich sind. Sie können jederzeit zwischen den Varianten wechseln, um zu überprüfen, wie die Inhaltskomponente basierend auf ihren bedingten Regeln angezeigt wird.

   >[!NOTE]
   >Wenn keine der in den Varianten definierten Regeln beim Senden der Nachricht erfüllt ist, zeigt die Inhaltskomponente den Inhalt an, der für die **[!UICONTROL Standardvariante]** im Bereich **[!UICONTROL Bedingter Inhalt]** definiert ist.
