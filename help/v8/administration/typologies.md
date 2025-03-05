---
audience: end-user
title: Arbeiten mit Geschäftsregeln (Typologien)
description: Erfahren Sie, wie Sie mit Typologien und Typologieregeln arbeiten können, um den Versand von Sendungen zu steuern, zu filtern und zu überwachen.
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: ht
source-wordcount: '1449'
ht-degree: 100%

---

# Arbeiten mit Geschäftsregeln (Typologien) {#typologies}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Geschäftsregeln"
>abstract="Sie können jetzt Typologien und Typologieregeln in der Adobe Campaign Web-Benutzeroberfläche erstellen. Mit Typologien können Sie die Durchführung von Sendungen steuern, filtern und priorisieren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"


>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Typologien und Typologieregeln"
>abstract="Typologien ermöglichen es Ihnen, Geschäftspraktiken über alle Sendungen hinweg zu standardisieren. Eine Typologie ist eine Sammlung von Typologieregeln, mit denen der Versand von Sendungen gesteuert, gefiltert und priorisiert werden kann. Profile, die den Kriterien einer Typologieregel entsprechen, werden in der Vorbereitungsphase von den Versandzielgruppen ausgeschlossen."

## Über Typologien

Typologien ermöglichen es Ihnen, Geschäftspraktiken über alle Sendungen hinweg zu standardisieren. Eine **Typologie** ist eine Sammlung von **Typologieregeln**, mit denen die Durchführung von Sendungen gesteuert, gefiltert und priorisiert werden kann. Profile, die den Kriterien einer Typologieregel entsprechen, werden in der Vorbereitungsphase von den Versandzielgruppen ausgeschlossen.

Typologien stellen sicher, dass Ihre Sendungen immer bestimmte Elemente enthalten (z. B. einen Abmelde-Link oder eine Betreffzeile) oder Filterregeln, um bestimmte Zielgruppen auszuschließen. Dazu zählen etwa abgemeldete Abonnierende, Mitbewerbende oder Kundschaft, die nicht am Treueprogramm teilnimmt.

Auf Typologien können Sie über das Menü **[!UICONTROL Administration]** > **[!UICONTROL Geschäftsregeln]** zugreifen. Auf diesem Bildschirm können Sie auf alle vorhandenen Typologien und Typologieregeln zugreifen oder je nach Bedarf neue erstellen.

![](assets/business-rules-list.png)

>[!NOTE]
>
>Die Liste **[!UICONTROL Typologieregeln]** zeigt alle vorhandenen Regeln an, die bisher in der Web-Benutzeroberfläche oder der Client-Konsole erstellt wurden. Es können jedoch nur **Steuerungs**- und **Filterregeln** in der Web-Benutzeroberfläche erstellt werden. Verwenden Sie die Client-Konsole von Campaign v8, um andere Typen von Typologieregeln wie Druck- oder Kapazitätsregeln zu erstellen. [Erfahren Sie, wie Sie Typologieregeln in der Client-Konsole erstellen.](https://experienceleague.adobe.com/de/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

Die wichtigsten Schritte zum Anwenden von Typologien auf Ihre Nachrichten sind:

1. [Erstellen einer Typologie](#typology)
1. [Erstellen von Typologieregeln](#typology-rules)
1. [Referenzieren von Typologieregeln in der Typologie](#add-rules)
1. [Anwenden der Typologie auf Nachrichten](#message)

## Erstellen einer Typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Typologieeigenschaften"
>abstract="Definieren Sie die Eigenschaften der Typologie und erweitern Sie den Abschnitt **[!UICONTROL Weitere Optionen]**, um auf erweiterte Einstellungen zuzugreifen. Verwenden Sie das Feld **[!UICONTROL IP-Affinität]**, um IP-Affinitäten mit Typologien zu verknüpfen. Hierdurch können Sie den ausgehenden SMTP-Traffic besser steuern. Legen Sie dazu fest, welche IP-Adressen jeweils für die einzelnen Affinitäten verwendet werden können."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="IP-Affinität"
>abstract="Die Verwaltung der IP-Adressenaffinitäten ermöglicht eine bessere Steuerung des ausgehenden SMTP-Traffics, indem jedem Traffic-Typ je nach Versandtypologie unterschiedliche IP-Adressen zugewiesen werden."

Gehen Sie wie folgt vor, um eine Typologie zu erstellen:

1. Navigieren Sie zum Menü **[!UICONTROL Geschäftsregeln]** und wählen Sie dann die Registerkarte **[!UICONTROL Typologie]** aus.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Typologie erstellen]** und geben Sie einen **[!UICONTROL Titel]** für die Typologie ein.

1. Erweitern Sie den Abschnitt **[!UICONTROL Weitere Optionen]**, um erweiterte Einstellungen wie den internen Namen, den Speicherordner und die Beschreibung der Typologie zu definieren.

   ![](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >Mit dem Feld **[!UICONTROL IP-Affinität]** können Sie IP-Affinitäten mit Typologien verknüpfen. Hierdurch können Sie den ausgehenden SMTP-Traffic besser steuern. Legen Sie dazu fest, welche IP-Adressen jeweils für die einzelnen Affinitäten verwendet werden können. So können Sie beispielsweise eine Affinität pro Land oder Subdomain verwenden. Dann können Sie für jedes Land eine Typologie erstellen und jede Affinität mit der entsprechenden Typologie verbinden.

1. Klicken Sie auf **[!UICONTROL Erstellen]**, um die Erstellung der Typologie zu bestätigen.

Der Bildschirm mit den Typologiedetails wird geöffnet. Über diesen Bildschirm können Sie direkt auf vorhandene Typologieregeln verweisen. Sie können auch neue Typologieregeln erstellen und diese später in der Typologie referenzieren:
* [Erfahren Sie, wie Sie eine Typologieregel erstellen.](#add-rules)
* [Erfahren Sie, wie Sie Regeln in einer Typologie referenzieren.](#add-rules)

## Erstellen einer Typologieregel {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Eigenschaften einer Typologieregel"
>abstract="Definieren Sie die Eigenschaften der Typologieregel. Mit **Steuerungsregeln** werden vor dem Versand die Qualität und Gültigkeit der Nachrichten überprüft. **Filterregeln** dienen hingegen dazu, Segmente der Zielgruppe anhand bestimmter Kriterien auszuschließen.<br/><br/>Sie können auch die Anwendungsreihenfolge der Regel ändern, um die Anwendungsreihenfolge von Typologieregeln zu steuern, wenn mehrere Regeln desselben Typs während derselben Nachrichtenverarbeitungsphase ausgeführt werden."

Um eine Typologieregel zu erstellen, navigieren Sie zum Menü **[!UICONTROL Geschäftsregeln]** und wählen Sie dann die Registerkarte **[!UICONTROL Typologieregeln]** aus.

Klicken Sie auf **[!UICONTROL Typologieregel erstellen]** und führen Sie dann die folgenden Schritte aus.

### Definieren der Eigenschaften der Typologieregel {#properties}

So definieren Sie die Eigenschaften der Typologieregel:

1. Geben Sie einen **[!UICONTROL Titel]** für die Regel ein. 

   ![](assets/business-rules-control-rule.png)

1. Legen Sie den **[!UICONTROL Typ]** für die Typologieregel fest:

   * **Steuerungsregeln** stellen vor dem Versand die Qualität und Gültigkeit der Nachrichten sicher (z. B. Zeichenanzeige, SMS-Länge, Adressformat, URL-Verkürzung). Sie werden mithilfe einer Skripting-Oberfläche erstellt, um komplexe Logik für Inhaltsprüfungen und -änderungen zu definieren.

   * **Filterregeln** schließen Segmente der Zielgruppe anhand bestimmter Kriterien aus (z. B. Alter, Standort, Land, Telefonnummern). Diese Regeln sind mit einer Zielgruppendimension verknüpft.

   >[!NOTE]
   >
   >Vorerst können über die Web-Benutzeroberfläche nur Typologieregeln zur **Steuerung** und **Filterung** erstellt werden. Verwenden Sie zum Erstellen anderer Regeltypen die Client-Konsole. [Erfahren Sie, wie Sie Typologieregeln in der Client-Konsole erstellen.](https://experienceleague.adobe.com/de/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. Wählen Sie einen **[!UICONTROL Kanal]** aus, um ihn mit der Regel zu verknüpfen.

1. Schalten Sie die Option **[!UICONTROL Aktiv]** aus, wenn die Regel nicht direkt nach ihrer Erstellung aktiv sein soll.

1. Definieren Sie die **[!UICONTROL Anwendungsreihenfolge]** für die Regel.

   Standardmäßig ist diese Priorität einer Typologieregel auf 50 festgelegt. Sie können diesen Wert anpassen, um die Anwendungsreihenfolge von Typologieregeln zu steuern, wenn mehrere Regeln desselben Typs während derselben Nachrichtenverarbeitungsphase ausgeführt werden. Beispielsweise wird eine Filterregel mit einem Wert der Anwendungsreihenfolge von 20 vor einer Filterregel mit einem Wert von 30 ausgeführt.

1. Erweitern Sie den Abschnitt **[!UICONTROL Weitere Optionen]**, um auf erweiterte Einstellungen wie den internen Namen, den Speicherordner und die Beschreibung der Regel zuzugreifen.

1. Für Steuerungsregeln stehen in den weiteren Optionen zwei zusätzliche Regeln zur Verfügung. Damit können Sie festlegen, wann die Regel angewendet werden soll, und die Warnstufe bestimmen:

   * **[!UICONTROL Phase]**: In diesem Feld können Sie angeben, zu welchem Zeitpunkt des Versandlebenszyklus die Regel angewendet wird. Wählen Sie den anzuwendenden Wert in der Dropdown-Liste **[!UICONTROL Phase]** aus. Erweitern Sie den folgenden Abschnitt, um weitere Details zu den möglichen Werten zu erhalten:

   +++Phasen einer Steuerungsregel

   **[!UICONTROL Zu Beginn der Zielgruppenbestimmung]**: Die Steuerungsregel kann in dieser Phase angewandt werden, um im Falle eines Fehlers den Personalisierungsschritt nicht auszuführen.

   **[!UICONTROL Nach der Zielgruppenbestimmung]**: Wenn Sie die Größe der Zielgruppe kennen müssen, um die Steuerungsregel anzuwenden, wählen Sie diese Phase aus. Die Steuerungsregel „Prüfung der Testversandgröße“ beispielsweise wird zwingend nach der Phase der Zielgruppenbestimmung angewendet: Diese Regel verhindert eine Nachrichtenpersonalisierung, wenn die Zielgruppe des Testversands zu groß ist.

   **[!UICONTROL Zu Beginn der Personalisierung]**: Diese Phase muss ausgewählt werden, wenn die Steuerung die Validierung der Nachrichtenpersonalisierung betrifft. Die Nachrichtenpersonalisierung erfolgt während der Analysephase.

   **[!UICONTROL Am Ende der Analyse]**: Wenn eine Prüfung verlangt, dass die Nachrichtenpersonalisierung bereits abgeschlossen ist, wählen Sie diese Phase aus.

+++

   * **[!UICONTROL Ebene]**: Mit dieser Option können Sie die Warnstufe für die Regel angeben. Erweitern Sie die folgenden Abschnitte, um weitere Informationen zu erhalten.

   +++Ebenen einer Steuerungsregel:

   **[!UICONTROL Fehler]**: Die Nachrichtenvorbereitung wird angehalten.

   **[!UICONTROL Warnung]**: Es wird eine Warnung in den Vorbereitungs-Logs angezeigt.

   **[!UICONTROL Info]**: Es werden Informationen in den Vorbereitungs-Logs angezeigt.

   <!--**[!UICONTROL Status]**:-->

   **[!UICONTROL Verbose]**: Es werden Informationen in den Serverlogs angezeigt.

+++

### Erstellen des Regelinhalts {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtern"
>abstract="**Filterregeln** schließen Segmente der Zielgruppe anhand bestimmter Kriterien aus (z. B. Alter, Standort, Land, Telefonnummern). Wählen Sie die Zielgruppendimension der Typologieregel aus und klicken Sie auf die Schaltfläche **[!UICONTROL Regeln hinzufügen]**, um auf den Abfrage-Modeler zuzugreifen und die Regel zu erstellen."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Code"
>abstract="**Steuerungsregeln** überprüfen vor dem Versand die Qualität und Gültigkeit der Nachrichten (z. B. Zeichenanzeige, SMS-Länge, Adressformat, URL-Verkürzung). Sie werden mit JavaScript-Code erstellt."

Nachdem Sie die Eigenschaften der Typologieregel definiert haben, können Sie den Inhalt der Regel erstellen.

* Klicken Sie für **Steuerungsregeln** auf die Schaltfläche **Code bearbeiten** und geben Sie die Logik für die Regel mithilfe von JavaScript ein. Im folgenden Beispiel erstellen wir eine Regel, um eine Warnung in den Logs anzuzeigen, wenn das Ziel leer ist.

  ![](assets/business-rules-code.png)

* Wählen Sie für **Filterregeln** die Zielgruppendimension aus und klicken Sie auf die Schaltfläche **[!UICONTROL Regeln hinzufügen]**, um Filterkriterien mithilfe des [Abfrage-Modelers](../query/query-modeler-overview.md) zu definieren.

  ![](assets/business-rules-query.png)

Wenn Ihre Regel fertig ist, klicken Sie auf die Schaltfläche **[!UICONTROL Erstellen]**, um die Typologieregel zu erstellen. Sie können die Regel jetzt in einer Typologie referenzieren, um sie auf Nachrichten anzuwenden.

## Referenzieren von Typologieregeln in einer Typologie {#add-rules}

Gehen Sie wie folgt vor, um eine oder mehrere Regeln in einer Typologie zu referenzieren:

1. Navigieren Sie zur Registerkarte **[!UICONTROL Typologie]** und öffnen Sie die Typologie, in der Sie die Regel(n) referenzieren möchten.

1. Wählen Sie die **[!UICONTROL Typologieregeln]** und klicken Sie auf die Schaltfläche **[!UICONTROL Typologieregel(n) hinzufügen]**.

   ![](assets/business-rules-reference.png)

1. Wählen Sie eine oder mehrere Typologieregeln aus, die mit der Typologie verknüpft werden sollen, und bestätigen Sie sie.

   ![](assets/business-rules-typology-save.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

Sie können die Typologie jetzt auf Nachrichten anwenden. Daraufhin werden alle ausgewählten Typologieregeln ausgeführt, um die definierten Prüfungen durchzuführen.

## Anwenden von Typologien auf Nachrichten {#message}

Um eine Typologie auf eine Nachricht oder Nachrichtenvorlage anzuwenden, müssen Sie die Typologie in den Nachrichteneinstellungen auswählen. [Erfahren Sie, wie Sie Versandeinstellungen konfigurieren](../advanced-settings/delivery-settings.md#typology)

![](assets/business-rules-apply.png)

Anschließend werden die in der Typologie enthaltenen Typologieregeln ausgeführt, um die Versandgültigkeit während der Nachrichtenvorbereitung zu überprüfen. Profile, die den Kriterien einer Typologieregel entsprechen, werden dann von den Versandzielgruppen ausgeschlossen.
