---
audience: end-user
title: Arbeiten mit Geschäftsregeln (Typologien)
description: Erfahren Sie, wie Sie mit Typologien und Typologieregeln arbeiten können, um den Versand von Sendungen zu steuern, zu filtern und zu überwachen.
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: 4444fc6742754137d1d73d7ea8bc12388ce1bc7d
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 39%

---

# Arbeiten mit Geschäftsregeln (Typologien) {#typologies}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Geschäftsregeln"
>abstract="Sie können jetzt Typologien und Typologieregeln in der Adobe Campaign Web-Benutzeroberfläche erstellen. Mit Typologien können Sie die Durchführung von Sendungen steuern, filtern und priorisieren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Typologien und Typologieregeln"
>abstract="Mit Typologien können Sie Geschäftspraktiken für alle Sendungen standardisieren. Eine Typologie ist eine Sammlung von Typologieregeln, mit denen Sie den Versand von Nachrichten steuern, filtern und priorisieren können. Profile, die den Kriterien einer Typologieregel entsprechen, werden während der Vorbereitungsphase aus den Versand-Audiences ausgeschlossen."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_type"
>title="Filtern"
>abstract=" Es stehen zwei Arten von Typologieregeln zur Verfügung: <br/><br/>**Kontrolle** Regeln, die die Qualität und Gültigkeit von Nachrichten vor dem Senden sicherstellen, z. B. Zeichenanzeige, SMS-Länge, Adressformat oder URL-Verkürzung. <br/><br/>**Filterregeln** die Segmente der Zielgruppe basierend auf bestimmten Kriterien wie Alter, Standort, Land oder Telefonnummern ausschließen."

## Über Typologien

Mit Typologien können Sie Geschäftspraktiken für alle Sendungen standardisieren. Eine **Typologie** ist eine Sammlung von **Typologieregeln** mit denen Sie den Versand von Sendungen steuern, filtern und priorisieren können. Profile, die den Kriterien einer Typologieregel entsprechen, werden während der Vorbereitungsphase aus den Versand-Audiences ausgeschlossen.

Typologien stellen sicher, dass Ihre Sendungen immer bestimmte Elemente enthalten, z. B. einen Abmelde-Link oder eine Betreffzeile, oder Filterregeln, um Gruppen aus Ihrer Zielgruppe auszuschließen, z. B. Abonnenten, Konkurrenten oder Kunden, die nicht Mitglied im Treueprogramm sind.

Auf Typologien können Sie über das Menü **[!UICONTROL Administration]** > **[!UICONTROL Geschäftsregeln]** zugreifen. Greifen Sie auf diesem Bildschirm auf alle vorhandenen Typologien und Typologieregeln zu oder erstellen Sie neue, Ihren Anforderungen entsprechende Typologien.

![Liste der Geschäftsregeln in der Benutzeroberfläche](assets/business-rules-list.png)

>[!NOTE]
>
>Die Liste **[!UICONTROL Typologieregeln]** zeigt alle vorhandenen Regeln an, die bisher in der Web-Benutzeroberfläche oder der Client-Konsole erstellt wurden. Es können jedoch nur **Steuerungs**- und **Filterregeln** in der Web-Benutzeroberfläche erstellt werden. Verwenden Sie die Client-Konsole von Campaign v8, um andere Typen von Typologieregeln wie Druck- oder Kapazitätsregeln zu erstellen. [Erfahren Sie, wie Sie Typologieregeln in der Client-Konsole erstellen](https://experienceleague.adobe.com/de/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

Die wichtigsten Schritte zum Anwenden von Typologien auf Ihre Nachrichten sind:

1. [Erstellen einer Typologie](#typology)
1. [Erstellen von Typologieregeln](#typology-rules)
1. [Referenzieren von Typologieregeln in der Typologie](#add-rules)
1. [Anwenden der Typologie auf Nachrichten](#message)

## Erstellen einer Typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Typologieeigenschaften"
>abstract="Definieren Sie die Eigenschaften der Typologie und erweitern Sie den Abschnitt **[!UICONTROL Weitere Optionen]**, um auf erweiterte Einstellungen zuzugreifen. Verwenden Sie das Feld **[!UICONTROL IP-Affinität]**, um IP-Affinitäten mit Typologien zu verknüpfen. Auf diese Weise können Sie den ausgehenden SMTP-Traffic besser kontrollieren, indem Sie festlegen, welche spezifischen IP-Adressen für jede Affinität verwendet werden können."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="IP-Affinität"
>abstract="Die Verwaltung der IP-Adressenaffinitäten ermöglicht eine bessere Steuerung des ausgehenden SMTP-Traffics, indem jedem Traffic-Typ je nach Versandtypologie unterschiedliche IP-Adressen zugewiesen werden."

Gehen Sie wie folgt vor, um eine Typologie zu erstellen:

1. Navigieren Sie zum Menü **[!UICONTROL Geschäftsregeln]** und wählen Sie dann die Registerkarte **[!UICONTROL Typologie]** aus.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Typologie erstellen]** und geben Sie einen **[!UICONTROL Titel]** für die Typologie ein.

1. Erweitern Sie den Abschnitt **[!UICONTROL Zusätzliche Optionen]**, um erweiterte Einstellungen wie den internen Namen der Typologie, den Speicherordner und die Beschreibung zu definieren.

   ![Typologieerstellungsschnittstelle](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >Mit dem Feld **[!UICONTROL IP-Affinität]** können Sie IP-Affinitäten mit Typologien verknüpfen. Dies ermöglicht eine bessere Steuerung des ausgehenden SMTP-Traffics, indem festgelegt wird, welche spezifischen IP-Adressen für jede Affinität verwendet werden können. So können Sie beispielsweise eine Affinität pro Land oder Subdomain verwenden. Dann können Sie für jedes Land eine Typologie erstellen und jede Affinität mit der entsprechenden Typologie verbinden.

1. Klicken Sie auf **[!UICONTROL Erstellen]**, um die Erstellung der Typologie zu bestätigen.

Die Typologiedetails werden geöffnet. Verweisen Sie auf diesem Bildschirm direkt auf vorhandene Typologieregeln oder erstellen Sie neue Typologieregeln, auf die Sie später verweisen können:
* [Erfahren Sie, wie Sie eine Typologieregel erstellen.](#add-rules)
* [Erfahren Sie, wie Sie Regeln in einer Typologie referenzieren.](#add-rules)

## Erstellen einer Typologieregel {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Eigenschaften einer Typologieregel"
>abstract="Definieren Sie die Eigenschaften der Typologieregel. Mit **Steuerungsregeln** werden vor dem Versand die Qualität und Gültigkeit der Nachrichten überprüft. **Filterregeln** dienen hingegen dazu, Segmente der Zielgruppe anhand bestimmter Kriterien auszuschließen.<br/><br/>Sie können auch die Ausführungsreihenfolge der Regel ändern, um die Reihenfolge zu verwalten, in der Typologieregeln ausgeführt werden, wenn mehrere Regeln desselben Typs während derselben Nachrichtenverarbeitungsphase ausgeführt werden."

Um eine Typologieregel zu erstellen, navigieren Sie zum Menü **[!UICONTROL Geschäftsregeln]** und wählen Sie dann die Registerkarte **[!UICONTROL Typologieregeln]** aus.

Klicken Sie auf **[!UICONTROL Typologieregel erstellen]** und führen Sie dann die folgenden Schritte aus.

### Definieren der Eigenschaften der Typologieregel {#properties}

So definieren Sie die Eigenschaften der Typologieregel:

1. Geben Sie einen **[!UICONTROL Titel]** für die Regel ein. 

   ![Schnittstelle zur Regelerstellung](assets/business-rules-control-rule.png)

1. Legen Sie den **[!UICONTROL Typ]** für die Typologieregel fest:

   * **Kontrolle**: Stellt die Qualität und Gültigkeit der Nachrichten vor dem Senden sicher, z. B. die Zeichenanzeige, die SMS-Länge, das Adressformat oder die URL-Verkürzung. Diese Regeln werden mithilfe einer Skriptoberfläche erstellt, um komplexe Logik für Inhaltsprüfungen und -änderungen zu definieren.

   * **Filtern**: Schließt Segmente der Zielgruppe basierend auf bestimmten Kriterien wie Alter, Standort, Land oder Telefonnummern aus. Diese Regeln sind mit einer Zielgruppendimension verknüpft.

   >[!NOTE]
   >
   >Derzeit können nur **Kontrolle** und **Filterung** Typologieregeln über die Web-Benutzeroberfläche erstellt werden. Verwenden Sie zum Erstellen anderer Regeltypen die Client-Konsole. [Erfahren Sie, wie Sie Typologieregeln in der Client-Konsole erstellen](https://experienceleague.adobe.com/de/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. Wählen Sie einen **[!UICONTROL Kanal]** aus, um ihn mit der Regel zu verknüpfen.

1. Schalten Sie die Option **[!UICONTROL Aktiv]** aus, wenn die Regel nicht sofort nach ihrer Erstellung aktiv sein soll.

1. Definieren Sie die **[!UICONTROL der Regel]**.

   Standardmäßig ist diese Priorität einer Typologieregel auf 50 festgelegt. Passen Sie diesen Wert an, um die Reihenfolge zu verwalten, in der Typologieregeln ausgeführt werden, wenn mehrere Regeln desselben Typs während derselben Nachrichtenverarbeitungsphase ausgeführt werden. Beispielsweise wird eine Filterregel mit einem Wert der Anwendungsreihenfolge von 20 vor einer Filterregel mit einem Wert von 30 ausgeführt.

1. Erweitern Sie den Abschnitt **[!UICONTROL Zusätzliche Optionen]**, um auf erweiterte Einstellungen wie den internen Namen der Regel, den Ordnerspeicher und die Beschreibung zuzugreifen.

1. Für Kontrollregeln stehen in den zusätzlichen Optionen zwei zusätzliche Felder zur Verfügung. Geben Sie an, wann die Regel angewendet werden soll und wie hoch die Warnstufe sein soll:

   * **[!UICONTROL Phase]**: Geben Sie an, zu welchem Zeitpunkt des Versandlebenszyklus die Regel angewendet wird. Wählen Sie den Wert in der Dropdown **[!UICONTROL Liste]** Phase“ aus. Erweitern Sie den folgenden Abschnitt, um weitere Details zu den möglichen Werten zu erhalten:

   +++Phasen einer Steuerungsregel

   **[!UICONTROL Zu Beginn der Zielgruppenbestimmung]**: Verhindern Sie, dass der Personalisierungsschritt im Fehlerfall ausgeführt wird.

   **[!UICONTROL Nach der Zielgruppenbestimmung]**: Wählen Sie diese Phase aus, wenn Sie das Volumen der Zielgruppe kennen müssen, um die Kontrollregel anwenden zu können. Beispielsweise gilt nach jedem **[!UICONTROL die Regel]** Größe des Testversands überprüfen. Diese Regel verhindert die Personalisierung von Nachrichten, wenn zu viele Testversand-Empfänger vorhanden sind.

   **[!UICONTROL Zu Beginn der Personalisierung]**: Wählen Sie diese Phase, wenn das Steuerelement die Validierung der Nachrichtenpersonalisierung betrifft. Die Nachrichtenpersonalisierung erfolgt während der Analysephase.

   **[!UICONTROL Am Ende der Analyse]**: Übernehmen Sie Prüfungen, für die eine vollständige Nachrichtenpersonalisierung erforderlich ist.

   +++

   * **[!UICONTROL Level]**: Geben Sie die Warnstufe für die Regel an. Erweitern Sie die folgenden Abschnitte, um weitere Informationen zu erhalten.

   +++Ebenen einer Steuerungsregel:

   **[!UICONTROL Fehler]**: Die Nachrichtenvorbereitung wird angehalten.

   **[!UICONTROL Warnung]**: Es wird eine Warnung in den Vorbereitungs-Logs angezeigt.

   **[!UICONTROL Info]**: Es werden Informationen in den Vorbereitungs-Logs angezeigt.

   **[!UICONTROL Verbose]**: Es werden Informationen in den Serverlogs angezeigt.

   +++

### Erstellen des Regelinhalts {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtern"
>abstract="**Filterregeln** schließen Segmente der Zielgruppe basierend auf bestimmten Kriterien aus, z. B. Alter, Standort, Land oder Telefonnummern. Wählen Sie die Zielgruppendimension der Typologieregel aus und klicken Sie auf die Schaltfläche **[!UICONTROL Regeln hinzufügen]**, um auf den Abfrage-Modeler zuzugreifen und die Regel zu erstellen."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Code"
>abstract="**Kontrollregeln** überprüfen die Qualität und Gültigkeit der Nachrichten vor dem Versand, z. B. die Zeichenanzeige, die SMS-Länge, das Adressformat oder die URL-Verkürzung. Diese Regeln werden mit JavaScript-Code erstellt."

Nachdem die Eigenschaften der Typologieregel definiert wurden, erstellen Sie den Inhalt der Regel.

* Klicken Sie für **Steuerungsregeln** auf die Schaltfläche **Code bearbeiten** und geben Sie die Logik für die Regel mithilfe von JavaScript ein. Im folgenden Beispiel wird eine Regel erstellt, die eine Warnung in den Protokollen anzeigt, wenn das Ziel leer ist.

  ![Regeleditor](assets/business-rules-code.png)

* Wählen Sie für **Filterregeln** die Zielgruppendimension aus und klicken Sie auf die Schaltfläche **[!UICONTROL Regeln hinzufügen]**, um Filterkriterien mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) zu definieren.

  ![Filterregel-Abfragemodellierer](assets/business-rules-query.png)

Wenn Ihre Regel fertig ist, klicken Sie auf die Schaltfläche **[!UICONTROL Erstellen]**, um die Typologieregel zu erstellen. Referenzieren Sie die Regel in einer Typologie, um sie auf Nachrichten anzuwenden.

## Referenzieren von Typologieregeln in einer Typologie {#add-rules}

Gehen Sie wie folgt vor, um auf eine oder mehrere Regeln in einer Typologie zu verweisen:

1. Navigieren Sie zur Registerkarte **[!UICONTROL Typologie]** und öffnen Sie die Typologie, in der Sie die Regel(n) referenzieren möchten.

1. Wählen Sie die **[!UICONTROL Typologieregeln]** und klicken Sie auf die Schaltfläche **[!UICONTROL Typologieregel(n) hinzufügen]**.

   ![Oberfläche für Typologieregeln hinzufügen](assets/business-rules-reference.png)

1. Eine oder mehrere Typologieregeln auswählen, die mit der Typologie verknüpft werden sollen, und bestätigen.

   ![Oberfläche für Typologieregeln speichern](assets/business-rules-typology-save.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Sie können die Typologie jetzt auf Nachrichten anwenden. Daraufhin werden alle ausgewählten Typologieregeln ausgeführt, um die definierten Prüfungen durchzuführen.

## Anwenden von Typologien auf Nachrichten {#message}

Um eine Typologie auf eine Nachricht oder Nachrichtenvorlage anzuwenden, wählen Sie die Typologie in den Nachrichteneinstellungen aus. [Erfahren Sie, wie Sie Versandeinstellungen konfigurieren](../advanced-settings/delivery-settings.md#typology)

![Anwenden der Typologie auf die Nachrichtenschnittstelle](assets/business-rules-apply.png)

Nach der Anwendung werden die in der Typologie enthaltenen Typologieregeln ausgeführt, um die Versandgültigkeit während der Nachrichtenvorbereitung zu überprüfen. Profile, die den Kriterien einer Typologieregel entsprechen, werden aus den Versand-Audiences ausgeschlossen.