---
title: Erstellen bedingter Inhalte
description: Erfahren Sie, wie Sie in der Web-Benutzeroberfläche von Adobe Campaign Bedingungen definieren, um Ihre Inhalte zu personalisieren
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 1dfd557b22de9888ab8d3a1f0479b45d59a86f93
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 3%

---

# Bedingten Inhalt erstellen{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Erstellen bedingter Inhalte"
>abstract="Erstellen bedingter Inhalte zur Definition einer dynamischen Personalisierung basierend auf dem Empfängerprofil und zum automatischen Ersetzen von Textbausteinen und Bildern, wenn bestimmte Bedingungen erfüllt sind. Diese Funktion kann Ihre Kampagnen auf neue Höhen bringen und zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen."

Bedingter Inhalt ist eine leistungsstarke Funktion, mit der Sie eine dynamische Personalisierung erstellen können, die auf dem Empfängerprofil basiert. Dabei werden Textbausteine und Bilder automatisch ersetzt, wenn bestimmte Bedingungen erfüllt sind. Diese Funktion kann Ihre Kampagnen auf neue Höhen bringen und zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen.

Durch die Konfiguration bedingter Inhaltsfelder können Sie beispielsweise eine erweiterte dynamische Personalisierung erstellen, die auf dem Empfängerprofil basiert. Textbausteine, Links, Betreffzeile und/oder Bilder werden im Nachrichteninhalt ersetzt, wenn eine bestimmte Bedingung erfüllt ist. Beispielsweise können Sie &quot;Herr&quot;oder &quot;Frau&quot;entsprechend dem Wert des Felds &quot;Geschlecht&quot;in der Adobe Campaign-Datenbank anzeigen oder je nach bevorzugter Sprache einen anderen Link einfügen.

## Erstellen bedingter Inhalte

Um bedingte Inhalte zu erstellen, müssen Sie Bedingungen im Ausdruckseditor mithilfe einer bestimmten Hilfsfunktion erstellen. Diese Methode ist für alle Versandkanäle verfügbar, und zwar in allen Feldern, in denen Sie auf den Ausdruckseditor zugreifen können, z. B. im Betreffzeilenfeld oder in E-Mail-Links und Text-/Schaltflächeninhaltskomponenten. [Erfahren Sie, wo dynamische Inhalte hinzugefügt werden](gs-personalization.md/#access)

Zusätzlich zum Ausdruckseditor können Sie einen dedizierten Builder für bedingte Inhalte bei der Erstellung einer E-Mail verwenden, mit der Sie Bedingungen mithilfe von Profilattributen erstellen können.

## Erstellen von Bedingungen im Ausdruckseditor {#condition-perso-editor}

Gehen Sie wie folgt vor, um einen bedingten Inhalt für einen Versand zu definieren: In diesem Beispiel möchten wir bedingte Inhalte basierend auf der Sprache der Empfänger (Französisch oder Englisch) erstellen.

1. Öffnen Sie einen Versand und bearbeiten Sie den Inhalt.

1. Suchen Sie das Feld, dem bedingte Inhalte hinzugefügt werden sollen, und klicken Sie auf die Schaltfläche **[!UICONTROL Personalisierungsdialogfeld öffnen]** -Symbol, um den Ausdruckseditor zu öffnen. In diesem Beispiel möchten wir einer SMS-Nachricht bedingten Inhalt hinzufügen:

   ![](assets/open-perso-editor-sms.png)

1. Navigieren Sie im Personalisierungs-Editor zum **[!UICONTROL Hilfsfunktionen]** Menü links.

1. Klicken Sie auf das &quot;+&quot;-Symbol neben dem **Wenn** -Funktion, um Ihre Bedingung zu starten. Die folgende Zeile wird zum mittleren Bildschirm hinzugefügt:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Ersetzen `<FIELD>` durch ein Personalisierungsfeld. Beispielsweise die Sprache des Empfängers: `recipient.language`.
   * Ersetzen `<VALUE>` durch den Wert, der erfüllt werden soll. Beispiel, `'French'`.
   * Ersetzen `Ìnsert content here` durch den Inhalt, den Sie den Profilen anzeigen möchten, die die oben angegebene Bedingung erfüllen.

     ![](assets/condition-sample1.png)

1. Geben Sie den Inhalt an, der angezeigt werden soll, wenn die Empfänger die Bedingung nicht erfüllen. Gehen Sie dazu wie folgt vor:

   1. Hinzufügen einer **else** Hilfsfunktion: Platzieren Sie den Cursor vor dem schließenden -Tag des Ausdrucks `%>` und klicken Sie auf `+` neben dem **Else** -Funktion.

      >[!NOTE]
      >
      >Jedes Mal, wenn eine Hilfsfunktion hinzugefügt wird, öffnen Sie (`<%`) und schließen (`%>`)-Tags werden vor und nach der Funktion automatisch hinzugefügt. Beispiel nach dem Hinzufügen einer Hilfsfunktion &quot;Else&quot;innerhalb eines Ausdrucks:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
      >
      >Entfernen Sie diese Tags unbedingt, um Syntaxfehler zu vermeiden. In diesem Beispiel wurde der Ausdruck nach dem Entfernen der **Else** -Funktions-Tags:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

   1. Ersetzen `Ìnsert content here` durch den Inhalt, den Sie den Profilen anzeigen möchten, die die Bedingung nicht erfüllen.

      ![](assets/condition-sample2.png)

   Sie können auch die **else if** Hilfsfunktion zum Erstellen von Bedingungen mit mehreren Inhaltsvarianten. Der folgende Ausdruck zeigt beispielsweise drei Varianten einer Nachricht in Abhängigkeit von der Sprache der Empfänger:

   ![](assets/condition-sample3.png)

1. Sobald Ihre Bedingung fertig ist, können Sie Ihren Inhalt speichern und sein Rendering überprüfen, indem Sie Ihren Inhalt simulieren.

## Bedingten Inhalt in E-Mails erstellen  {#condition-condition-builder}

Bedingte Inhalte in E-Mails können auf zwei Arten erstellt werden:
* Im Ausdruckseditor durch Erstellen einer Bedingung mithilfe von Hilfsfunktionen,
* In einem dedizierten Builder für bedingte Inhalte, auf den beim Entwerfen einer E-Mail zugegriffen werden kann.

Detaillierte Informationen zum Erstellen von Bedingungen mithilfe des Ausdruckseditors finden Sie unter [here](#condition-perso-editor).

Der folgende Abschnitt führt Sie durch die Schritte zum Erstellen von Bedingungen mithilfe des Builders für bedingte Inhalte für E-Mail-Designer. In diesem Beispiel erstellen wir eine E-Mail-Nachricht, die je nach Sprache der Empfänger mehrere Varianten enthält. Gehen Sie dazu wie folgt vor:

1. Erstellen oder öffnen Sie einen E-Mail-Versand, bearbeiten Sie seinen Inhalt und klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten des E-Mail-Hauptteils]** -Schaltfläche, um den Arbeitsbereich zum Erstellen von E-Mails zu öffnen.

1. Wählen Sie eine Inhaltskomponente aus und klicken Sie auf **[!UICONTROL Bedingten Inhalt aktivieren]**.

   ![](assets/condition-email-enable.png)

1. Die **[!UICONTROL Bedingter Inhalt]** wird auf der linken Bildschirmseite geöffnet. In diesem Bereich können Sie mithilfe von Bedingungen mehrere Varianten der ausgewählten Inhaltskomponente erstellen.

1. Konfigurieren Sie Ihre erste Variante. Bewegen Sie dazu den Mauszeiger über **[!UICONTROL Variante - 1]** im **[!UICONTROL Bedingter Inhalt]** und klicken Sie auf **[!UICONTROL Bedingung hinzufügen]** Symbol.

1. Ein Regel-Builder wird angezeigt. Verwenden Sie die Profilattribute, um die Bedingung für die erste Variante der Nachricht zu erstellen, und klicken Sie auf **[!UICONTROL Bestätigen]**. In diesem Beispiel wird eine Regel erstellt, die sich an Empfänger richtet, deren Sprache &#39;Französisch&#39; lautet.

   ![](assets/condition-email-rule.png)

1. Die Regel ist nun mit der Variante verknüpft. Um die Lesbarkeit zu verbessern, wird empfohlen, die Variante umzubenennen, indem Sie auf das Menü mit den Auslassungspunkten klicken.

   Konfigurieren Sie jetzt, wie die Komponente angezeigt werden soll, wenn die Regel beim Senden der Nachricht erfüllt ist. In diesem Beispiel soll der Text auf Französisch angezeigt werden, wenn er die bevorzugte Sprache des Empfängers ist.

   ![](assets/condition-email-variant1.png)

1. Fügen Sie so viele Varianten hinzu, wie für die Inhaltskomponente erforderlich sind. Sie können jederzeit zwischen den verschiedenen Varianten wechseln, um zu überprüfen, wie die Inhaltskomponente je nach den bedingten Regeln dargestellt wird.

   >[!NOTE]
   >Wenn keine der in den Varianten definierten Regeln beim Versand der Nachricht erfüllt ist, zeigt die Inhaltskomponente den in der Variablen **[!UICONTROL Standardvariante]** von **[!UICONTROL Bedingter Inhalt]** -Bereich.
