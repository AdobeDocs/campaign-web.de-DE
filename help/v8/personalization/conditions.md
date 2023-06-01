---
title: Bedingte Inhalte erstellen
description: Erfahren Sie, wie Sie Bedingungen zur Personalisierung Ihres Inhalts in der Adobe Campaign-Web-Benutzeroberfläche definieren.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 5598a82bf745659b8c1db8cb51b1a82cfd184093
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 3%

---

# Bedingten Inhalt erstellen{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Bedingte Inhalte erstellen"
>abstract="Erstellen bedingter Inhalte zur Definition einer dynamischen Personalisierung basierend auf dem Empfängerprofil und zum automatischen Ersetzen von Textbausteinen und Bildern, wenn bestimmte Bedingungen erfüllt sind. Diese Funktion kann Ihre Kampagnen auf neue Höhen bringen und zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen."


Bedingter Inhalt ist eine leistungsstarke Funktion, mit der Sie eine dynamische Personalisierung erstellen können, die auf dem Empfängerprofil basiert. Dabei werden Textbausteine und Bilder automatisch ersetzt, wenn bestimmte Bedingungen erfüllt sind. Diese Funktion kann Ihre Kampagnen auf neue Höhen bringen und zielgerichtete, personalisierte Erlebnisse für Ihre Zielgruppe bereitstellen.

Durch die Konfiguration bedingter Inhaltsfelder können Sie beispielsweise eine erweiterte dynamische Personalisierung erstellen, die auf dem Empfängerprofil basiert. Textbausteine, Links, Betreffzeile und/oder Bilder werden im Nachrichteninhalt ersetzt, wenn eine bestimmte Bedingung erfüllt ist. Beispielsweise können Sie &quot;Herr&quot;oder &quot;Frau&quot;entsprechend dem Wert des Felds &quot;Geschlecht&quot;in der Adobe Campaign-Datenbank anzeigen oder je nach bevorzugter Sprache einen anderen Link einfügen.

## Personalisierungssyntax{#perso-syntax}



## Arbeiten mit Bedingungen im Personalisierungs-Editor{#condition-perso-editor}

So definieren Sie bedingte Inhalte für einen Versand:

1. Öffnen Sie einen Versand und bearbeiten Sie den Inhalt.
1. Klicken Sie auf **[!UICONTROL Personalisierungsdialogfeld öffnen]** beispielsweise für SMS rechts neben dem Feld Nachricht .

   ![](assets/open-perso-editor-sms.png)

1. Navigieren Sie im Personalisierungs-Editor zu **[!UICONTROL Hilfsfunktionen]**.
1. Klicken Sie auf das &quot;+&quot;-Symbol neben dem **Wenn** -Funktion. Die folgende Zeile wird zum mittleren Bildschirm hinzugefügt:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Ersetzen `<FIELD>` durch ein Personalisierungsfeld. Beispiel: das Unternehmen des Empfängers: `recipient.company`.
1. Ersetzen `<VALUE>` durch einen Wert, der erfüllt werden soll. Beispiel, `ADOBE`.




## Beispiel: Bedingte Betreffzeile für SMS{#condition-subject-line}

Gehen Sie wie folgt vor, um eine bedingte Betreffzeile für eine SMS-Nachricht zu erstellen:

1. Öffnen Sie einen Versand und bearbeiten Sie den Inhalt.
1. Klicken Sie rechts neben der Betreffzeile auf das Symbol Personalisierungsdialogfeld öffnen .
1. Navigieren Sie im Personalisierungs-Editor zu


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
