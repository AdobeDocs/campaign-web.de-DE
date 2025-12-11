---
title: Handbuch zur Erstellung von Prompts für die Inhaltsgenerierung mit dem KI-Assistenten
description: Erfahren Sie, wie Sie mit dem CO-STAR-Framework effektive Prompts zur KI-gestützten Inhaltsgenerierung erstellen können, um markenorientierte Marketing-Inhalte mit hoher Konversionsrate zu erstellen.
role: User
level: Intermediate
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: ht
source-wordcount: '2085'
ht-degree: 100%

---

# Best Practices für Prompts für den KI-Assistenten {#ai-assistant-prompting-guide}

Dieses Handbuch hilft Ihnen, Ihre Anfragen zu strukturieren, die Absicht klar zu kommunizieren und sicherzustellen, dass die KI Messaging erzeugt, das mit Ihren Markenrichtlinien, Zielgruppenanforderungen und Kampagnenzielen übereinstimmt.
Erfahren Sie, wie Sie effektive Prompts schreiben, mit denen der KI-Assistent hochwertige markenkonforme Marketing-Inhalte generieren kann, die auf Ihre Ziele zugeschnitten sind.

## Verwenden des CO-STAR-Frameworks {#costar-framework}

Um mit dem KI-Assistenten optimale Ergebnisse zu erzielen, sollten Sie Ihre Prompts mit dem CO-STAR-Framework organisieren. Dieser strukturierte Ansatz stellt sicher, dass die KI genau versteht, was Sie benötigen.

| Komponente | Was dies bedeutet | Warum dies wichtig ist |
|-|-|-|
| **C – Context (Kontext)** | Hintergrund der Kampagne, des Produkts oder der Situation | Hilft der KI, das Gesamtbild zu verstehen |
| **O – Objective (Ziel)** | Ihr konkretes Marketing-Ziel | Steuert, was der Inhalt erreichen sollte |
| **S – Style (Stil)** | Wie Sie kommunizieren möchten | Legt den Ansatz fest |
| **T – Tone (Ton)** | Emotionaler Stil und Ausdruck | Gestaltet die Stimmung Ihrer Nachricht |
| **A – Audience (Zielgruppe)** | Zielgruppe, die Sie ansprechen möchten | Stellt sicher, dass die Nachricht bei den richtigen Menschen Anklang findet |
| **R – Requirements (Anforderungen)** | Spezifische Einschränkungen oder Anforderungen, die erfüllt sein müssen | Definiert Grenzen und entscheidende Elemente |

## Wesentliche Bestandteile von KI-Prompts {#key-takeaways}


### Was Sie tun und nicht tun sollten


<table style="table-layout: fixed; width: 100%; border: 0;">
<thead style="border: 0; background-color: #FFFFFF;">
<tr>
<th>Tun Sie dies</th>
<th>Tun Sie dies nicht</th>
</tr>
</thead>
<tbody>
<tr style="border: 0;">
<td>
<p>Verwenden des CO-STAR-Frameworks als Struktur</p>
<p>Explizites Unterscheiden zwischen neuem und vorhandenem Inhalt</p>
<p>Fokussieren der Verwendung von Dokumenten mit konkreten Extraktionsanleitungen</p>
<p>Verwenden von Dropdown-Auswahlen für Ton, Strategie und Gebietsschema</p>
<p>Anpassen von Marketing-Zielen an Content-Typ-Funktionen</p>
<p>Generieren mehrerer Varianten für A/B-Tests</p>
</td>
<td>
<p>Anfordern von strukturellen Änderungen, Formatierung oder Bildbearbeitung in Prompts</p>
<p>Erwähnen von Ton/Strategie in Prompts, wenn diese in Dropdown-Menüs verfügbar sind</p>
<p>Vages Formulieren von Zielen wie „bewirb unser Produkt“</p>
<p>Anfordern von Auswahlen bedingter Elemente</p>
<p>Erwarten von Layout-Änderungen über Prompts</p>
</td>
</tr>
</tbody>
</table>

### Nicht in Prompts unterstützte Inhalte

>[!TIP]
>
>Verwenden Sie den **E-Mail-Editor** für visuelle Änderungen/Bildänderungen.

Diese Anfragen werden nicht unterstützt und sollten mit anderen Tools erledigt werden:

<table style="table-layout: fixed; border: 0;">
<thead style="border: 0; background-color: #FFFFFF">
<tr>
<th>✕ Änderungen an der E-Mail-Struktur</th>
<th>✕ Änderungen am visuellen Stil</th>
<th>✕ Bildbearbeitungsvorgänge</th>
</tr>
</thead>
<tbody>
<tr style="border: 0;">
<td>
<ul>
<li>Auswahl von bestimmten zu ändernden Abschnitten</li>
<li>Löschen oder Klonen von Elementen</li>
<li>Bedingte Auswahlen</li>
<li>Hinzufügen oder Entfernen von Layout-Abschnitten</li>
</ul>
</td>
<td>
<ul>
<li>Textformatierung (fett, kursiv, Schriftgrad)</li>
<li>Farbänderungen</li>
<li>Layout-Stile (Rahmen, Abstand, Ränder)</li>
<li>Visuelle Effekte (Schatten)</li>
</ul>
</td>
<td>
<ul>
<li>Hintergrundänderungen</li>
<li>Hinzufügen von Textüberlagerungen oder Logos</li>
<li>Zuschneiden von Bildern oder Größenänderungen</li>
<li>Farbkorrekturen</li>
<li>Austauschen von Bildern</li>
</ul>
</td>
</tr>
</tbody>
</table>

### Qualitäts-Checkliste {#quality-checklist}

Stellen Sie vor dem Generieren von Inhalten Folgendes sicher:

&amp;check; **Klares Ziel**: Gibt Aktion, Produkt/Dienst, Wert und Kontext klar an.

&amp;check; **Zielgruppe definiert**: Gibt Demografie, Rolle oder Segment an.

&amp;check; **Ausrichtung des Content-Typs**: Ziel entspricht dem ausgewählten Kanal oder Format.

&amp;check; **Dropdown-Auswahlen konfiguriert**: Ton, Strategie und Gebietsschema werden ausgewählt und sollen nicht im Prompt enthalten sein.

&amp;check; **Dokumentfokus festgelegt**: Markiert die Inhalte oder Abschnitte, auf die verwiesen werden soll.

&amp;check; **Marke angewendet**: Es sind passende Markenrichtlinien ausgewählt.

&amp;check; **Realistischer Umfang**: Vermeiden Sie das Anfordern von Layout-Änderungen, Formatierung oder strukturellen Bearbeitungen.

## Erstellen effektiver Marketing-Ziele {#marketing-objectives}

### Konkret und handlungsorientiert

Achten Sie bei der Formulierung von Marketing-Zielen darauf, dass diese klar, umsetzbar und messbar sind. Vermeiden Sie vage oder generische Aussagen.

**Beispiele für gute Ziele:**

&amp;check; „Steigere die Anmeldungen für unsere kostenlose 30-tägige Testversion des neuen KI-gestützten Analyse-Dashboards“

&amp;check; „Generiere Leads für unser B2B-Webinar zum Thema ,Reduzierung der Cloud-Kosten um 40 %‘, das am 15. März stattfindet“

&amp;check; „Bewirb unseren zeitlich begrenzten Feiertagsrabatt von 25 % auf Premium-Abonnements, der am 25. Dezember endet“

**Beispiele für zu vermeidende Ziele:**

✕ „Bewirb unser Produkt“ (zu vage)

✕ „Bring Menschen dazu, etwas zu kaufen“ (unklarer Wert)

✕ „E-Mail über neue Funktionen“ (Zweck fehlt)

### Strukturieren des Ziels

Geben Sie immer den Kontext und das Wertversprechen an, damit die KI relevante Inhalte generieren kann.
Verwenden Sie diese Formel, um effektive Ziele zu schreiben: **Aktion + Produkt/Dienst + Wert/Nutzen + Dringlichkeit/Kontext**

**Beispiele für gute Ziele:**

&amp;check; „Steigere die Downloads unserer neuen App, die Benutzenden hilft, nachhaltige Lebensgewohnheiten mit personalisierten umweltfreundlichen Empfehlungen zu verfolgen“

&amp;check; „Bewirb die Anmeldung für unseren exklusiven Workshop über fortschrittliche Datenvisualisierungstechniken für Marketing-Fachleute“

&amp;check; „Steigere die Teilnahme an unserer Produkteinführungsveranstaltung, auf der der revolutionäre KI-Schreibassistent vorgestellt wird, der mehr als 5 Stunden pro Woche einspart“

**Beispiele für zu vermeidende Formulierungen:**

✕ „Kündige die neue App an“ (Wertversprechen und Kontext fehlen)

✕ „Bring Menschen dazu, sich für den Workshop anzumelden“ (Spezifität bezüglich Zielgruppe und Nutzen fehlt)

✕ „Bewirb Veranstaltung“ (weder klare Aktion, klarer Wert noch klare Dringlichkeit)

## Erstellen neuer Inhalte im Vergleich zum Ändern vorhandener Inhalte {#new-vs-modify}

Geben Sie klar an, ob Ihre Anfrage auf das Generieren neuer Inhalte oder das Aktualisieren vorhandener Materialien abzielt. Diese Unterscheidung ist wichtig, da sie die KI bei der Auswahl des geeigneten Ansatzes anleitet und ein genaueres und nützlicheres Ergebnis sicherstellt.

### Erstellen neuer Inhalte

Wenden Sie diese Strategie an, wenn Sie Marketing-Kampagnen starten, neue Produkte vorstellen oder irgendeine Art von aktualisierter oder modernisierter Kommunikation initiieren. Sie stellt sicher, dass Ihre Nachricht über eine gute Grundlage verfügt und mit Ihren Zielen übereinstimmt.

**So sollte der Prompt aussehen** ➤ Konzentrieren Sie sich bei der Erstellung neuer Inhalte auf Ihr Marketing-Ziel und verweisen Sie nicht auf vorhandene Inhalte.

>[!BEGINSHADEBOX]

**Beispiele:**

* **SaaS-Testversion**: „Stelle unsere neue CRM-Software Kleinunternehen vor und betone dabei die Zeiteinsparungen von 50 %, die um 90 % schnellere Lead-Qualifizierung und das Angebot einer 30-tägigen kostenlosen Testversion mit personalisiertem Onboarding“
* **Funktionsankündigung**: „Kündige neue API-Integrationsfunktionen an, die die Entwicklungszeit für Unternehmenskundinnen und -kunden um 60 % verkürzen, und richte dich dabei an technische Entscheidungstragende“
* **Veranstaltungswerbung**: „Steigere die Anmeldungen für unser Webinar zum Thema ,Trends im Digital Marketing 2024‘ mit Fachleuten von Google, Meta und Adobe und betone dabei die verwertbaren Erkenntnisse und begrenzten Plätze (max. 500)“

>[!ENDSHADEBOX]

### Ändern von vorhandenen Inhalten

>[!TIP]
>
>Verwenden Sie für Standardänderungen wie Erklären, Zusammenfassen oder Vereinfachen von Inhalten die Funktion **Verfeinern**, anstatt benutzerdefinierte Prompts zu schreiben. [Weitere Informationen](generative-uc.md##refine)

Wenden Sie dies an, wenn Sie Ihre aktuellen Marketing-Kampagnen aktualisieren, modernisieren oder anpassen müssen. Diese Methode unterstützt inkrementelle Verbesserungen, um sicherzustellen, dass Ihr Messaging relevant bleibt, ohne dass Sie von Grund auf neu beginnen müssen.

**So sollte der Prompt aussehen** ➤ Geben Sie beim Ändern vorhandener Inhalte klar an, was Sie ändern und wie Sie es ändern möchten.

>[!BEGINSHADEBOX]

**Beispiele:**

* **Kampagnenaktualisierung**: „Ändere die Produkteinführungs-E-Mail, sodass sie sich auf Unternehmenssicherheitsfunktionen anstatt auf allgemeine Produktivitätsvorteile konzentriert und IT-Entscheidungstragende mit Compliance-Zertifizierungen anspricht“
* **Zielgruppenwechsel**: „Passe die Einladung zu unserer Software-Demo an, um gezielt das Gesundheitswesen anzusprechen, indem generische Beispiele durch Anwendungsfälle im Gesundheitswesen und HIPAA-konforme Vorteile ersetzt werden“
* **Saisonale Aktualisierung**: „Aktualisiere unsere Werbekampagne des 3. Quartals für den Weihnachtseinkauf im 4. Quartal, wobei der Fokus vom Schulbeginn auf die Geschenke für die Feiertage verlagert werden und ein Schwerpunkt auf schnellem Versand liegen soll“

>[!ENDSHADEBOX]

## Verbessern des Prompts mit erweiterten Einstellungen {#personalize-prompt}

### Kommunikationsstrategietypen

>[!TIP]
>
>Verwenden Sie das Dropdown-Menü „Kommunikationsstrategie“ im Menü „Texteinstellungen“, anstatt sie in Ihrem Prompt zu erwähnen, und stellen Sie so eine spezialisierte Verarbeitung sicher.

Ihre Kommunikationsstrategie bestimmt, wie Sie Ihre Nachricht so präsentieren, dass die größte Wirkung erzielt wird. Verschiedene Strategien funktionieren besser für verschiedene Ziele, sei es beim Erzeugen von Dringlichkeit, beim Aufbauen von Vertrauen oder beim Umsetzen sofortiger Maßnahmen. Wählen Sie die Strategie aus, die am besten zu Ihren Kampagnenzielen und der Denkweise Ihrer Zielgruppe passt.

| **Strategie** | **Am besten geeignet für** | **Nachrichtenstil** | **Beispiele** |
|--------------|--------------|------------------------|--------------|
| **Dringend** | Zeitkritische Angebote, Fristen, sofortiges Handeln | Erzeugt sofortigen Druck durch zeitbasierte Sprache | „Jetzt handeln: Angebot läuft um Mitternacht ab“ <br> „Heute registrieren, solange noch Plätze übrig sind“ <br> „48-stündiger Blitzverkauf beginnt jetzt“ |
| **FOMO (Fear of Missing Out – Angst, etwas zu verpassen)** | Eingeschränkte Angebote, Veranstaltungen, exklusiver Zugriff | Verwendet Hinweise auf Dringlichkeit, Knappheit und Zeitdruck | „Nur noch 24 Stunden! 40 % Rabatt auf ausgewählten Bestand“ <br> „Letzte Chance: Frühbucherpreis endet morgen“ <br> „Nur noch 100 Plätze im Beta-Programm übrig“ |
| **Social Proof** | Aufbau von Vertrauen, Erfahrungsberichte, beliebte Produkte | Nutzt die Erfahrungen und Bewertungen anderer Benutzender | „Schließen Sie sich mehr als 50.000 zufriedenen Kundinnen und Kunden an“ <br> „Von Branchenfachleuten mit 4,9/5 Sternen bewertet“ <br> „Von Fortune-500-Unternehmen als vertrauenswürdig eingestuft“ |
| **Knappheit** | Begrenzter Bestand, exklusive Versionen, Artikel mit hoher Nachfrage | Betont eingeschränkte Verfügbarkeit und Exklusivität | „Nur noch 5 Stück auf Lager“ <br> „Limitierte Auflage: 100 Stück verfügbar“ <br> „Exklusive Veröffentlichung: First come, first served“ |
| **Incentive** | Werbeaktionen, Prämienprogramme, Sonderangebote | Betont greifbare Vorteile und Prämien | „Erhalten Sie 20 % Rabatt auf Ihre erste Bestellung“ <br> „Sammeln Sie dieses Wochenende doppelte Punkte“ <br> „Kostenloser Versand bei Bestellungen über 50 €“ |
| **Exklusivität** | Premium-Produkte, VIP-Erlebnisse, exklusive Angebote für Mitglieder | Verwendet Premium-Positionierung und legt exklusiven Zugriff nahe | „Exklusive Einladung zu unserer privaten Vorschau“ <br> „Elite-Mitgliedschaft ermöglicht Zugang zu erweiterten Analysen“ <br> „Schließen Sie sich ausgewählten Fortune-500-Unternehmen an, die bereits mit uns arbeiten“ |
| **Gamification** | Interaktionskampagnen, Treueprogramme, interaktive Inhalte | Verwendet Spielmechanismen und weist auf Errungenschaften hin | „Entsperren Sie Ihre nächste Belohnungsstufe“ <br> „Schließen Sie Challenges ab, um Abzeichen zu erhalten“ <br> „Klettern Sie auf der Bestenliste nach oben, um exklusive Preise zu erhalten“ |
| **Informativ** | Bildung, Forschung, komplexe Produkte, Vordenkerrolle | Verwendet Fakten, Daten, Erkenntnisse und Erklärungen | „5 Erkenntnisse aus der Analyse von über 10.000 Interaktionen“ <br> „Neue Forschung offenbart 3 bahnbrechende Ansätze“ <br> „Vollständiger Leitfaden zur Implementierung von KI im Marketing“ |
| **Bildung und Erkenntnisse** | Lerninhalte, Branchen-Trends, Best Practices | Bietet wertvolles Wissen und verwertbare Erkenntnisse | „Lernen Sie fortschrittliche Techniken mit unserem fachlichen Leitfaden kennen“ <br> „Entdecken Sie 7 Strategien, die Top-Marketing-Fachleute verwenden“ <br> „Erfahren Sie, wie Sie Ihren Workflow in 5 Schritten optimieren können“ |

### Bestimmen des richtigen Tons {#tone}

>[!TIP]
>
>Verwenden Sie das Dropdown-Menü „Ton“ im Menü „Texteinstellungen“, anstatt ihn im Prompt anzugeben.

Der Ton bestimmt, wie Ihre Zielgruppe Ihre Nachricht wahrnimmt und auf sie reagiert. Wählen Sie immer einen Ton aus, der mit Ihrer Markensprache und der Phase der Profil-Journey übereinstimmt.

Verwenden Sie die nachstehende Tabelle, um Details zu jedem Ton zu erfahren, einschließlich wann er am besten funktioniert und Inhaltsbeispiele, die zum jeweiligen Stil passen.

| Tonalität | Am besten geeignet für | Inhaltsbeispiel |
|-|-|-|
| Professionell | B2B-Kommunikation, formelle Ankündigungen | „Wir freuen uns, unsere strategische Partnerschaft bekannt geben zu können …“ |
| Empathisch | Kunden-Support, sensible Themen | „Wir verstehen, wie frustrierend dies für Sie sein muss …“ |
| Humorvoll | Ansprechende Kampagnen, unbeschwerte Inhalte | „Warnung: Kann zu ernsthaften Produktivitätssteigerungen führen!“ |
| Aufregend | Produkteinführungen, Werbung für Veranstaltungen | „Das ist der Moment, auf den Sie gewartet haben!“ |
| Inspirierend | Motivationskampagnen, Markenzweck | „Gemeinsam können wir die Welt verändern …“ |
| Überzeugend | Verkaufskampagnen, Konversionen | „Verpassen Sie nicht diese zeitlich begrenzte Gelegenheit, um …“ |
| Freundlich | Kundeninteraktion, Willkommensnachrichten | „Wir sind so froh, Sie bei uns begrüßen zu können!“ |
| Förmlich | Rechtliche Kommunikation, amtliche Mitteilungen | „Wir benachrichtigen Sie hiermit über folgende Änderungen …“ |
| Entschuldigend | Wiederherstellung des Dienstes, Problembehebung | „Wir entschuldigen uns aufrichtig für eventuelle Unannehmlichkeiten …“ |
| Energisch | Anleitende Inhalte, autoritatives Messaging | „Sie müssen nun Folgendes tun …“ |
| Storytelling | Markengeschichten, emotionale Zusammenhänge | „Alles fing mit einer einfachen Frage an …“ |
| Dialogorientiert | Nurture-Kampagnen, Aufbau von Beziehungen | „Sprechen wir darüber, wie Ihnen das helfen kann …“ |

### Optimieren von Marken-Assets {#brand-assets}

>[!TIP]
>
>Wenn Sie bereits ein Marken-Asset über das Menü **Marken-Assets** hochgeladen haben, müssen Sie im Prompt nicht darauf verweisen. Das System verwendet automatisch alle ausgewählten Dokumente.

Marken-Assets bieten sachliche Informationen, die Ihre generierten Inhalte mit konkreten, genauen Details anreichern.
Wenn Sie umfangreiche Dokumente wie Produktbroschüren hochladen, fügen Sie Ihrem Prompt hinzu, auf welchen Teilen der Schwerpunkt liegen soll:

* **Anstelle von** _„Verwende die Produktbroschüre“_ **sollten Sie Folgendes verwenden:** _„Konzentriere dich auf die erweiterten Sicherheitsfunktionen und Compliance-Zertifizierungen, insbesondere auf die SOC-2-Konformität und die Datenverschlüsselung“_

* **Anstelle von** _„Referenziere die Fallstudien“_ **sollten Sie Folgendes verwenden:** _„Hebe die ROI-Ergebnisse von Kundinnen und Kunden im Gesundheitswesen hervor, insbesondere die Reduzierung der Kosten um 40 % im regionalen medizinischen Zentrum“_

* **Anstelle von** _„Beziehe technische Details ein“_ **sollten Sie Folgendes verwenden:** _„Betone die API-Integrationsfunktionen und die Vorteile für Entwickelnde und konzentriere dich dabei auf REST-API-Endpunkte und das SLA mit 99,9 % Verfügbarkeit“_

### Inhaltsverfeinerung

>[!TIP]
>
>Verwenden Sie anstelle von Prompts die Funktion „Verfeinern“, um vorhandene Inhalte ausführlich zu erklären, zusammenzufassen, zu vereinfachen, den Ton zu ändern oder zu übersetzen. [Weitere Informationen](generative-uc.md#refine)

Verwenden Sie nach Generieren des Inhalts die Funktion **Verfeinern**, um ihn zu iterieren und mit den folgenden Optionen zu erweitern:

| **Aktion** | **Anwendungsbeispiel** | **Prompt-Beispiel** |
|-|-|-|
| **Ausführlich** | Hinzufügen von Hintergrund und Details zu kurzen Inhalten | „Erläutere die technischen Vorteile unserer Sicherheitsfunktionen“ |
| **Zusammenfassen** | Zusammenfassen langer Inhalte für verschiedene Formate | „Fasse diesen Produktüberblick für einen Social-Media-Post zusammen“ |
| **Vereinfachen** | Näherbringen komplexer Inhalte | „Vereinfache diese technische Erklärung für eine allgemeine Zielgruppe“ |
| **Ton ändern** | Anpassen von Inhalten für verschiedene Zielgruppen | „Gestalte den Ton etwas lässiger für eine jüngere Zielgruppe“ |
| **Transkreieren** | Kulturelle Anpassung über die Übersetzung hinaus | „Transkreiere diese Kampagne für den japanischen Markt“ |

## Szenariobasierte Prompt-Beispiele

### Basierend auf Content-Typ {#content-type-practices}

<table style="table-layout: fixed; border: 0;">
<thead>
<tr style="border: 0;background-color: #FFFFFF;">
<th>Kanal</th>
<th>Beispiel</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>E-Mail</strong></td>
<td>„Wirb potenzielle Unternehmen an, indem du drei Kundenerfolgsgeschichten mit detaillierten ROI-Metriken präsentierst (IBM: 45 % Kostensenkung, Accenture: 200 % Lead-Steigerung, Microsoft: 60 % Zeitersparnis), und richte dich dabei an IT-Führungskräfte in Unternehmen mit mehr als 1.000 Mitarbeitenden.“</td>
</tr>
<tr>
<td><strong>SMS</strong></td>
<td>„Informiere VIP-Kundinnen und VIP-Kunden über den 4-stündigen Blitzverkauf bei Premium-Elektronik mit 40 % Rabatt, der auf die ersten 100 Kundinnen und Kunden beschränkt ist“</td>
</tr>
<tr>
<td><strong>Push-Benachrichtigungen</strong></td>
<td>„Nimm die Interaktion mit Benutzenden wieder auf, die die App seit 7 Tagen nicht geöffnet haben, und gib ihnen personalisierte Inhaltsempfehlungen auf Grundlage ihres Leseverlaufs“</td>
</tr>
<tr>
<td><strong>Landingpages</strong></td>
<td>„Konvertiere B2B-Besuchende in qualifizierte Leads durch Veranschaulichung, wie unsere Unternehmenssicherheitslösung 99,9 % der Cyber-Angriffe verhindert, und stelle dabei Fortune-500-Erfahrungsberichten und kostenlose Sicherheits-Audits zur Verfügung“</td>
</tr>
</tbody>
</table>

### Basierend auf branchenspezifischen Ansätzen {#industry-approaches}

<table style="table-layout: fixed; border-collapse: collapse; border: 0;">
<thead>
<tr style="border: 0;background-color: #FFFFFF;">
<th>Branche</th>
<th>Beispiel-Prompt</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>B2B-Technologie</strong></td>
<td>„Präsentiere den ROI und die technischen Spezifikationen, berücksichtige dabei auch Sicherheitsbedenken für IT-Entscheidungstragende, die unsere Cloud-Infrastrukturlösung evaluieren, und hebe das SLA mit 99,9 % Verfügbarkeit, die SOC-2-Konformität und die Kosteneinsparungen um 40 % hervor.“</td>
</tr>
<tr>
<td><strong>E-Commerce-Einzelhandel</strong></td>
<td>„Erzeuge Dringlichkeit im Bezug auf Feiertagsprodukte mit begrenztem Bestand, hebe gleichzeitig den kostenlosen Versand und die einfachen Rückgabebedingungen für Last-Minute-Kaufende hervor und betone dabei die begrenzten Mengen (weniger als 50 verbleibende Artikel) sowie das Ende des 24-Stunden-Versands.“</td>
</tr>
<tr>
<td><strong>Finanzdienstleistungen</strong></td>
<td>„Informiere Kundinnen und Kunden über Strategien zur Diversifizierung ihres Anlageportfolios, berücksichtige gleichzeitig die Einhaltung gesetzlicher Vorschriften und biete Erkenntnisse von zertifizierten Finanzberatenden und Haftungsausschlüsse zu Risiken.“</td>
</tr>
<tr>
<td><strong>Gesundheitswesen und Wellness</strong></td>
<td>„Bewirb Vorsorgeleistungen und jährliche Gesundheitsuntersuchungen, achte dabei auf medizinische Richtigkeit und biete Empfehlungen für zertifizierte Ärztinnen und Ärzte sowie Datenschutzgarantien für Patientinnen und Patienten.“</td>
</tr>
<tr>
<td><strong>Bildung und Schulungen</strong></td>
<td>„Weise auf Karrierefortschritte und Branchenzertifizierungen sowie die Expertise der Ausbildenden hin und hebe dabei die Stellenvermittlungsquote von 92 % und den projektbasierten Lehrplan hervor.“</td>
</tr>
<tr>
<td><strong>SaaS-Plattformen</strong></td>
<td>„Zeige Zeiteinsparungen und Automatisierungsvorteile mithilfe konkreter Metriken auf, gehe gleichzeitig auf Integrationsfragen ein und betone dabei die durchschnittlichen wöchentlichen Zeiteinsparungen von 25 Stunden sowie die Integration mit über 200 beliebten Tools.“</td>
</tr>
</tbody>
</table>
