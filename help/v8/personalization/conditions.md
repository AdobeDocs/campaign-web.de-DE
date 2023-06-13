---
title: Erstellen bedingter Inhalte
description: Erfahren Sie, wie Sie in der Web-Benutzeroberfläche von Adobe Campaign Bedingungen definieren, um Ihre Inhalte zu personalisieren
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 2%

---

# Bedingten Inhalt erstellen{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Erstellen bedingter Inhalte"
>abstract="Erstellen bedingter Inhalte zur Definition einer dynamischen Personalisierung basierend auf dem Empfängerprofil und zum automatischen Ersetzen von Textbausteinen und Bildern, wenn bestimmte Bedingungen erfüllt sind. Diese Funktion kann Ihre Kampagnen auf neue Höhen bringen und zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen."

Bedingter Inhalt ist eine leistungsstarke Funktion, mit der Sie eine dynamische Personalisierung erstellen können, die auf dem Empfängerprofil basiert. Dabei werden Textbausteine und Bilder automatisch ersetzt, wenn bestimmte Bedingungen erfüllt sind. Diese Funktion kann Ihre Kampagnen auf neue Höhen bringen und zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen.

Durch die Konfiguration bedingter Inhaltsfelder können Sie beispielsweise eine erweiterte dynamische Personalisierung erstellen, die auf dem Empfängerprofil basiert. Textbausteine, Links, Betreffzeile und/oder Bilder werden im Nachrichteninhalt ersetzt, wenn eine bestimmte Bedingung erfüllt ist. Beispielsweise können Sie &quot;Herr&quot;oder &quot;Frau&quot;entsprechend dem Wert des Felds &quot;Geschlecht&quot;in der Adobe Campaign-Datenbank anzeigen oder je nach bevorzugter Sprache einen anderen Link einfügen.

## Erstellen bedingter Inhalte

Um bedingte Inhalte zu erstellen, müssen Sie Bedingungen im **Ausdruckseditor** Verwendung spezifischer Hilfsfunktionen. Diese Methode steht für alle Versandkanäle zur Verfügung und steht in jedem Feld zur Verfügung, in dem Sie auf den Ausdruckseditor zugreifen können, z. B. die Betreffzeile oder E-Mail-Links und Text-/Schaltflächeninhaltskomponenten. [Erfahren Sie, wie Sie auf den Ausdruckseditor zugreifen können.](gs-personalization.md/#access)

Zusätzlich zum Ausdruckseditor können Sie eine dedizierte **Bedingter Content Builder** beim Entwerfen einer E-Mail, die es Ihnen ermöglicht, Bedingungen nur mithilfe von Profilattributen zu erstellen. [Erfahren Sie, wie Sie bedingte Inhalte in E-Mails erstellen](#condition-condition-builder)

## Erstellen von Bedingungen im Ausdruckseditor {#condition-perso-editor}

Gehen Sie wie folgt vor, um bedingte Inhalte für einen Versand mit dem Ausdruckseditor zu definieren. In diesem Beispiel möchten wir bedingte Inhalte basierend auf der Sprache der Empfänger (Französisch oder Englisch) erstellen.

1. Öffnen Sie einen Versand und navigieren Sie zum Abschnitt Inhaltsbearbeitung .

1. Suchen Sie das Feld, dem bedingte Inhalte hinzugefügt werden sollen. Beispielsweise können Sie einer SMS-Nachricht bedingte Inhalte hinzufügen.

1. Klicken Sie auf **[!UICONTROL Personalisierungsdialogfeld öffnen]** neben dem Feld, um den Ausdruckseditor zu öffnen.

   ![](assets/open-perso-editor-sms.png)

1. Navigieren Sie im Personalisierungs-Editor zum **[!UICONTROL Hilfsfunktionen]** auf der linken Seite.

1. Um mit der Erstellung Ihrer Bedingung zu beginnen, klicken Sie auf das &quot;+&quot;-Symbol neben dem **Wenn** -Funktion. Die folgende Zeile wird zum mittleren Bildschirm hinzugefügt:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersetzen `<FIELD>` mit einem Personalisierungsfeld, z. B. der Sprache des Empfängers: `recipient.language`.
   * Ersetzen `<VALUE>` mit dem Wert, der erfüllt werden soll. Beispiel, `'French'`.
   * Ersetzen `Ìnsert content here` mit dem Inhalt, den Sie den Profilen anzeigen möchten, die die angegebene Bedingung erfüllen.

     ![](assets/condition-sample1.png){width="800" align="center"}

1. Geben Sie den Inhalt an, der angezeigt werden soll, wenn die Empfänger die Bedingung nicht erfüllen. Verwenden Sie dazu **else** Hilfsfunktion:

   1. Platzieren Sie den Cursor vor dem schließenden -Tag des Ausdrucks `%>` und klicken Sie auf `+` neben dem **Else** -Funktion.

   1. Ersetzen `Ìnsert content here` mit dem Inhalt, den Sie den Profilen anzeigen möchten, die die If -Funktion-Bedingung nicht erfüllen.

   ![](assets/condition-sample2.png){width="800" align="center"}

   Sie können auch die **else if** Hilfsfunktion zum Erstellen von Bedingungen mit mehreren Inhaltsvarianten. Der folgende Ausdruck zeigt beispielsweise drei Varianten einer Nachricht in Abhängigkeit von der Sprache der Empfänger:

   ![](assets/condition-sample3.png){width="800" align="center"}

   >[!NOTE]
   >
   >Jedes Mal, wenn eine Hilfsfunktion hinzugefügt wird, öffnen Sie (`<%`) und schließen (`%>`)-Tags werden vor und nach der Funktion automatisch hinzugefügt.
   >
   >Beispiel nach dem Hinzufügen einer Hilfsfunktion &quot;Else&quot;innerhalb eines Ausdrucks: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Entfernen Sie diese Tags, um Syntaxfehler zu vermeiden. In diesem Beispiel wurde der korrigierte Ausdruck nach dem Entfernen der **else** -Funktions-Tags:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Sobald Ihre Bedingung fertig ist, können Sie Ihren Inhalt speichern und sein Rendering überprüfen, indem Sie Ihren Inhalt simulieren.

## Bedingten Inhalt in E-Mails erstellen {#condition-condition-builder}

Bedingte Inhalte in E-Mails können auf zwei Arten erstellt werden:
* Im Ausdruckseditor durch Erstellen einer Bedingung mit Hilfsfunktionen,
* In einem dedizierten Builder für bedingte Inhalte, auf den beim Entwerfen einer E-Mail zugegriffen werden kann.

Detaillierte Informationen zum Erstellen von Bedingungen mithilfe des Ausdruckseditors finden Sie unter [here](#condition-perso-editor). Im folgenden Abschnitt finden Sie eine schrittweise Anleitung zum Erstellen von Bedingungen mithilfe der Funktion für bedingte Inhalte des E-Mail-Designers. In diesem Beispiel möchten wir eine E-Mail-Nachricht mit mehreren Varianten erstellen, die auf der Sprache der Empfänger basieren. Führen Sie folgende Schritte aus:

1. Erstellen oder öffnen Sie einen E-Mail-Versand, bearbeiten Sie seinen Inhalt und klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten des E-Mail-Hauptteils]** -Schaltfläche, um den Arbeitsbereich zum Erstellen von E-Mails zu öffnen.

1. Wählen Sie eine Inhaltskomponente aus und klicken Sie auf die **[!UICONTROL Bedingten Inhalt aktivieren]** Symbol.

   ![](assets/condition-email-enable.png){width="800" align="center"}

1. Die **[!UICONTROL Bedingter Inhalt]** wird auf der linken Bildschirmseite geöffnet. In diesem Bereich können Sie mithilfe von Bedingungen mehrere Varianten der ausgewählten Inhaltskomponente erstellen.

1. Konfigurieren Sie Ihre erste Variante. Bewegen **[!UICONTROL Variante - 1]** im **[!UICONTROL Bedingter Inhalt]** und klicken Sie auf **[!UICONTROL Bedingung hinzufügen]** Symbol.

1. Ein Regel-Builder wird angezeigt. Verwenden Sie Profilattribute, um die Bedingung für die erste Variante der Nachricht zu erstellen, und klicken Sie auf **[!UICONTROL Bestätigen]**. In diesem Beispiel wird eine Regel erstellt, die sich an Empfänger richtet, deren Sprache &#39;Französisch&#39; lautet.

   ![](assets/condition-email-rule.png){width="800" align="center"}

1. Die Regel ist nun mit der Variante verknüpft. Um die Lesbarkeit zu verbessern, wird empfohlen, die Variante umzubenennen, indem Sie auf das Suchmenü klicken.

1. Konfigurieren Sie, wie die Komponente angezeigt werden soll, wenn die Regel beim Senden der Nachricht erfüllt ist. In diesem Beispiel soll der Text auf Französisch angezeigt werden, wenn er die bevorzugte Sprache des Empfängers ist.

   ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Fügen Sie so viele Varianten hinzu, wie für die Inhaltskomponente erforderlich sind. Sie können jederzeit zwischen den Varianten wechseln, um zu überprüfen, wie die Inhaltskomponente basierend auf ihren bedingten Regeln angezeigt wird.

   >[!NOTE]
   >Wenn keine der in den Varianten definierten Regeln beim Versand der Nachricht erfüllt ist, zeigt die Inhaltskomponente den in der Variablen **[!UICONTROL Standardvariante]** von **[!UICONTROL Bedingter Inhalt]** -Bereich.
