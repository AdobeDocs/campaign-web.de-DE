---
audience: end-user
title: Verwalten einer Marke
description: Erfahren Sie, wie Sie Ihre Markenrichtlinien erstellen und verwalten.
badge: label="Beta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: 61078f86bcd433b1bc3a995489f283eb709b3687
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 17%

---

# Erstellen und Verwalten Ihrer Marken {#brands}

>[!AVAILABILITY]
>
>Diese Funktion wird als private Betaversion veröffentlicht. Sie wird in kommenden Versionen schrittweise für alle Kunden verfügbar sein.

Markenrichtlinien sind ein umfassender Satz von Regeln und Standards, die die visuelle und verbale Identität einer Marke definieren. Sie dienen als Referenz, um eine konsistente Markendarstellung auf allen Marketing- und Kommunikationskanälen sicherzustellen.

In [!DNL Adobe Campaign Web] können Benutzer Markeninformationen manuell eingeben und organisieren oder Dokumente zu Markenrichtlinien hochladen, um die Daten automatisch zu extrahieren.

## Zugriff auf Marken {#generative-access}

Um auf das Menü **[!UICONTROL Marken]** in [!DNL Adobe Campaign Web] zugreifen zu können, müssen Benutzenden die Produktprofile **[!UICONTROL Administrator (]**) und **[!UICONTROL Brand Kit]** zugewiesen werden, um Marken zu erstellen und zu verwalten. Für den schreibgeschützten Zugriff benötigen Benutzende das Produktprofil [!UICONTROL KI]Assistent“.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Erfahren Sie, wie Sie markenbezogene Berechtigungen zuweisen

1. Greifen Sie auf der Startseite der [Admin Console](https://adminconsole.adobe.com/enterprise) auf Ihr Campaign-Produkt zu.

   ![Admin Console-Startseite mit Campaign-Produktzugriff](assets/brands_admin_1.png)

1. Wählen Sie die **[!DNL Product profile]** basierend auf der Berechtigungsstufe aus, die Sie Ihrem Benutzer gewähren möchten.

   ![Produktprofilauswahl in Admin Console](assets/brands_admin_2.png)

1. Klicken Sie zum Zuweisen des ausgewählten Produktprofils auf **[!DNL Add users]**.

   ![Option „Benutzer hinzufügen“ in Admin Console](assets/brands_admin_3.png)

1. Geben Sie den Namen, die Benutzergruppe oder die E-Mail-Adresse Ihres Benutzers ein.

1. Klicken Sie zum Anwenden der Änderungen auf **Speichern**.

Die Berechtigungen von Benutzenden, die dieser Rolle bereits zugewiesen sind, werden automatisch aktualisiert.

+++

## Erstellen Ihrer Marke {#create-brand-kit}

Gehen Sie wie folgt vor, um Ihre Markenrichtlinien zu erstellen und zu verwalten:

Benutzer können die Details entweder manuell eingeben oder ein Dokument mit Markenrichtlinien hochladen, um die Informationen automatisch zu extrahieren:

1. Klicken Sie im Menü **[!UICONTROL Marken]** auf **[!UICONTROL Marke erstellen]**.

   ![Menü „Marken“ mit der Option „Marke erstellen“](assets/brands-1.png)

1. Geben Sie einen **[!UICONTROL Namen]** für Ihre Marke ein.

1. Ziehen oder wählen Sie eine Datei, um Ihre Markenrichtlinien hochzuladen und automatisch relevante Markeninformationen zu extrahieren. Klicken Sie auf **[!UICONTROL Marke erstellen]**.

   Der Informationsextraktionsprozess beginnt jetzt. Beachten Sie, dass dieser Vorgang mehrere Minuten dauern kann.

   ![Datei-Upload für die Extraktion der Markenrichtlinien](assets/brands-2.png)

1. Ihre Standards für Content und visuelle Erstellung werden jetzt automatisch ausgefüllt. Durchsuchen Sie die verschiedenen Registerkarten, um die Informationen nach Bedarf anzupassen. [Weitere Informationen](#personalize)

1. Im erweiterten Menü jedes Abschnitts oder jeder Kategorie können Sie Verweise hinzufügen, um relevante Markeninformationen automatisch zu extrahieren.

   Um vorhandene Inhalte zu entfernen, verwenden Sie die Optionen **[!UICONTROL Abschnitt löschen]** oder **[!UICONTROL Kategorie löschen]**.

   ![](assets/brands-15.png)

1. Klicken Sie nach der Konfiguration **[!UICONTROL Speichern]** und anschließend **[!UICONTROL Veröffentlichen]**, um Ihre Markenrichtlinie im KI-Assistenten verfügbar zu machen.

1. Um Änderungen an Ihrer veröffentlichten Marke vorzunehmen, klicken Sie auf **[!UICONTROL Marke bearbeiten]**.

   >[!NOTE]
   >
   >Dadurch wird eine temporäre Kopie im Bearbeitungsmodus erstellt, die die Live-Version nach der Veröffentlichung ersetzt.

   ![Option „Marke bearbeiten“ im Menü „Marken“](assets/brands-8.png)

1. Öffnen Sie im Dashboard **[!UICONTROL Marken]** das erweiterte Menü, indem Sie auf das Symbol ![](assets/do-not-localize/Smock_More_18_N.svg) klicken, um Folgendes zu tun:

   * Marke anzeigen
   * Bearbeiten
   * Als Standardmarke markieren
   * Duplizieren
   * Veröffentlichen
   * Veröffentlichung aufheben
   * Löschen

   ![Erweiterte Menüoptionen im Marken-Dashboard](assets/brands-6.png)

Ihre Markenrichtlinien sind jetzt über die Dropdown-Liste **[!UICONTROL Marke]** im Menü KI-Assistent verfügbar. Dadurch kann der KI-Assistent Inhalte und Assets generieren, die mit Ihren Spezifikationen übereinstimmen. [Weitere Informationen zum KI-Assistenten](../email/generative-gs.md)

![KI-Assistenten-Menü mit Dropdown-Liste „Marke“](assets/brands_6.png)

### Festlegen einer Standardmarke {#default-brand}

Sie können eine Standardmarke festlegen, die bei der Erstellung von Inhalten und der Berechnung der Alignment-Bewertungen während der Kampagnenerstellung automatisch angewendet wird.

Um eine Standardmarke festzulegen, gehen Sie zum Dashboard **[!UICONTROL Marken]**. Öffnen Sie das erweiterte Menü, indem Sie auf das Symbol ![](assets/do-not-localize/Smock_More_18_N.svg) klicken und **[!UICONTROL Als Standardmarke markieren]** auswählen.

![Erweiterte Menüoptionen im Marken-Dashboard](assets/brands-6.png)

## Marke personalisieren {#personalize}

### Über die Marke {#about-brand}

Verwenden Sie die Registerkarte **[!UICONTROL Über die Marke]**, um die Kernidentität Ihrer Marke zu ermitteln und ihren Zweck, ihre Persönlichkeit, ihren Slogan und andere definierende Attribute zu umreißen.

1. Füllen Sie zunächst die grundlegenden Informationen für Ihre Marke in der Kategorie **[!UICONTROL Hauptdetails]** aus:

   * **[!UICONTROL Name des Brand Kits]**: Geben Sie den Namen Ihres Brand Kits ein.

   * **[!UICONTROL Verwendungszweck]**: Geben Sie Szenarien oder Kontexte an, in denen dieses Marken-Kit verwendet werden soll.

   * **[!UICONTROL Markenname]**: Geben Sie den offiziellen Namen der Marke ein.

   * **[!UICONTROL Markenbeschreibung]**: Bieten Sie einen Überblick darüber, was diese Marke darstellt.

   * **[!UICONTROL Standard-]**: Fügen Sie den primären Slogan hinzu, der der Marke zugeordnet ist.

     ![Kategorie der Schlüsseldetails](assets/brands-about-1.png)

1. Klären **[!UICONTROL in der Kategorie]** Leitprinzipien“ die Kernausrichtung und Philosophie Ihrer Marke:

   * **[!UICONTROL Mission]**: Beschreiben Sie den Zweck Ihrer Marke.

   * **[!UICONTROL Vision]**: Beschreiben Sie Ihr langfristiges Ziel oder Ihren gewünschten zukünftigen Status.

   * **[!UICONTROL Marktpositionierung]**: Erklären Sie, wie Ihre Marke auf dem Markt positioniert ist.

   ![Leitprinzipien-Kategorie](assets/brands-about-2.png)

1. Klicken Sie in der Kategorie **[!UICONTROL Markenwerte]** auf ![Bild in Alternativtext einblenden](assets/do-not-localize/Smock_Add_18_N.svg "Symbol hinzufügen"), um die Kernwerte der Marke hinzuzufügen und die Details auszufüllen:

   * **[!UICONTROL Wert]**: Benennen Sie einen Kern-Markenwert.

   * **[!UICONTROL Beschreibung]**: Erklären Sie, was dieser Wert für Ihre Marke bedeutet.

   * **[!UICONTROL Verhalten]**: Beschreiben Sie die Aktionen oder Einstellungen, die diesen Wert in der Praxis widerspiegeln.

   * **[!UICONTROL Manifestationen]**: Geben Sie Beispiele dafür, wie dieser Wert in der realen Markendarstellung ausgedrückt wird.

     ![](assets/brands-12.png)

1. Klicken Sie bei Bedarf auf das ![ALT-Text/Bearbeiten](assets/do-not-localize/Smock_Edit_18_N.svg "-")-Symbol für das Tauchbild, um einen Ihrer Kernmarkenwerte zu aktualisieren oder zu löschen.

   ![Wert bearbeiten](assets/brands-10.png)

Jetzt können Sie Ihre Marke weiter personalisieren oder [Ihre Marke veröffentlichen](#create-brand-kit).

### Schreibstil {#writing-style}

Im Abschnitt **[!UICONTROL Schreibstil]** werden die Standards für das Schreiben von Inhalten beschrieben. Außerdem wird erläutert, wie Sprache, Formatierung und Struktur verwendet werden sollten, um Klarheit, Kohärenz und Konsistenz über alle Materialien hinweg zu gewährleisten.

+++ Verfügbare Kategorie und Beispiele

<table>
  <thead>
    <tr>
      <th>Kategorie</th>
      <th>Unterkategorie</th>
      <th>Beispiel für Richtlinien</th>
      <th>Beispiel für Ausschlüsse</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Standards für die Inhaltserstellung</td>
      <td>Markenbotschaften - Standards</td>
      <td>Heben Sie Innovation und Customer-First-Messaging hervor.</td>
      <td>Versprechen Sie nicht zu viel Produktfunktionen.</td>
    </tr>
    <tr>
      <td>Verwendung von Slogan</td>
      <td>Platzieren Sie den Slogan unter dem Logo auf allen digitalen Marketing-Assets.</td>
      <td>Ändern oder übersetzen Sie den Slogan nicht.</td>
    </tr>
    <tr>
      <td>Kernbotschaft</td>
      <td>Heben Sie die wichtigsten Vorteile hervor, z. B. die gesteigerte Produktivität.</td>
      <td>Verwenden Sie keine nicht verwandten Wertvorschläge.</td>
    </tr>
    <tr>
      <td>Benennungsstandards</td>
      <td>Verwenden Sie einfache, beschreibende Namen wie „ProScheduler“.</td>
      <td>Verwenden Sie keine komplexen Begriffe oder Sonderzeichen.</td>
    </tr>
    <tr>
      <td rowspan="5">Markenkommunikationsstil</td>
      <td>Merkmale der Markenpersönlichkeit</td>
      <td>Freundlich und zugänglich.</td>
      <td>Sei nicht defätistisch.</td>
    </tr>
    <tr>
      <td>Schreibmechanik</td>
      <td>Halten Sie Sätze kurz und wirkungsvoll.</td>
      <td>Verwenden Sie keinen übermäßigen Jargon.</td>
    </tr>
    <tr>
      <td>situativer Ton</td>
      <td>Behalten Sie einen professionellen Ton in der Krisenkommunikation bei.</td>
      <td>Seien Sie in der Support-Kommunikation nicht abweisend.</td>
    </tr>
    <tr>
      <td>Word-Auswahlrichtlinien</td>
      <td>Verwende Wörter wie „innovativ“ und „intelligent“.</td>
      <td>Vermeide Wörter wie „billig“ oder „hack“.</td>
    </tr>
    <tr>
      <td>Sprachstandards</td>
      <td>Befolgen Sie die Konventionen für amerikanisches Englisch.</td>
      <td>Keine englische und amerikanische Schreibweise vermischen.</td>
    </tr>
    <tr>
      <td rowspan="3">Gesetzliche Compliance-Standards</td>
      <td>Markenstandards</td>
      <td>Verwenden Sie immer das ™- oder ®.</td>
      <td>Lassen Sie bei Bedarf keine Rechtssymbole weg.</td>
    </tr>
    <tr>
      <td>Urheberrechtsnormen</td>
      <td>Copyright-Hinweise auf Marketingmaterial einschließen.</td>
      <td>Verwenden Sie keine Inhalte von Drittanbietern ohne Erlaubnis.</td>
    </tr>
    <tr>
      <td>Haftungsausschluss-Standards</td>
      <td>Haftungsausschlüsse leserlich auf digitalen Assets anzeigen.</td>
      <td>Ausblenden von Haftungsausschlüssen in nicht sichtbaren Bereichen.</td>
    </tr>
</table>

+++

</br>

So personalisieren Sie **[!UICONTROL Schreibstil]**:

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Schreibstil“ auf ![](assets/do-not-localize/Smock_Add_18_N.svg) , um eine Richtlinie, einen Ausnahmefehler oder einen Ausschluss hinzuzufügen.

1. Geben Sie Richtlinie, Ausnahme oder Ausschluss ein und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/brands-3.png)

1. Wählen Sie eine der Richtlinien oder einen Ausschluss aus, die aktualisiert oder gelöscht werden sollen.

1. Klicken Sie auf ![ALT-Text/] (assets/do-not-localize/Smock_Edit_18_N.svg "), ") Ihr Beispiel zu bearbeiten, oder auf das ![Alternativtext für Tauchbild](assets/do-not-localize/Smock_Delete_18_N.svg "Löschen")Symbol, um es zu löschen.

   ![](assets/brands-11.png)

Jetzt können Sie Ihre Marke weiter personalisieren oder [Ihre Marke veröffentlichen](#create-brand-kit).

### Visueller Inhalt {#visual-content}

Im Abschnitt **[!UICONTROL Visuelle Inhalte]** werden die Standards für Bilder und Design definiert. Darin werden die Spezifikationen detailliert beschrieben, die für die Aufrechterhaltung eines einheitlichen und konsistenten Markenlooks erforderlich sind.

+++ Verfügbare Kategorien und Beispiele

<table>
  <thead>
    <tr>
      <th>Kategorie</th>
      <th>Beispiel für Richtlinien</th>
      <th>Beispiel für Ausschlüsse</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Fotografiestandards</td>
      <td>Verwenden Sie natürliche Beleuchtung für Außenaufnahmen.</td>
      <td>Vermeiden Sie übermäßig bearbeitete oder pixelige Bilder.</td>
    </tr>
    <tr>
      <td>Illustrationsstandards</td>
      <td>Verwenden Sie saubere, minimalistische Stile.</td>
      <td>Vermeiden Sie übermäßig komplexe Inhalte.</td>
    </tr>
    <tr>
      <td>Symbolstandards</td>
      <td>Verwenden Sie ein konsistentes 24px-Rastersystem.</td>
      <td>Keine Symbolabmessungen mischen, inkonsistente Strichgewichte verwenden oder von Rasterregeln abweichen.</td>
    </tr>
    <tr>
      <td>Nutzungsrichtlinien</td>
      <td>Wählen Sie Lifestyle-Bilder, die reale Kunden widerspiegeln, die das Produkt in professionellen Umgebungen verwenden.</td>
      <td>Verwenden Sie keine Bilder, die dem Markenton widersprechen oder aus dem Kontext gerissen erscheinen.</td>
    </tr>
</table>

+++

</br>

So personalisieren Sie **[!UICONTROL visuelle Inhalte]**:

1. Klicken Sie auf der Registerkarte **[!UICONTROL Visueller]**) auf ![](assets/do-not-localize/Smock_Add_18_N.svg) , um eine Richtlinie, einen Ausschluss oder ein Beispiel hinzuzufügen.

1. Geben Sie Ihre Richtlinie, Ihren Ausschluss oder Ihr Beispiel ein und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![Ausschluss oder Beispielschaltfläche hinzufügen](assets/brands-4.png)

1. Um ein Bild hinzuzufügen, das die korrekte Verwendung zeigt, wählen Sie **[!UICONTROL Beispiel]** und klicken Sie auf **[!UICONTROL Bild auswählen]**. Sie können auch ein Bild mit falscher Verwendung als Ausschlussbeispiel hinzufügen.

   ![Fügen Sie ein Bild als Beispiel hinzu](assets/brands-13.png)

1. Wählen Sie eine der Richtlinien oder einen Ausschluss aus, die aktualisiert oder gelöscht werden sollen.

1. Wählen Sie eine Richtlinie oder einen Ausschluss aus, um sie zu aktualisieren. Klicken Sie auf das ![Tauchbild-Alternativtext](assets/do-not-localize/Smock_Delete_18_N.svg "Löschen")-Symbol, um es zu löschen.

   ![Ausschluss oder Richtlinie löschen](assets/brands-14.png)

Jetzt können Sie Ihre Marke weiter personalisieren oder [Ihre Marke veröffentlichen](#create-brand-kit).
