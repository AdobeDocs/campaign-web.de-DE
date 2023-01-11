---
audience: end-user
title: Erweiterte Einstellungen
description: Web-Dokumentation zu Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 96d5ee712131ba314ef25736e421efe436d5170a
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 51%

---

# Erweiterte Parameter {#advanced-settings}

![](../assets/do-not-localize/badge.png)

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

Diese Einstellungen sind **technische Versandparameter** die in der E-Mail-Vorlage definiert sind. Wenn Sie einen Versand ändern möchten, ist Vorsicht geboten.

## E-Mail-Versandeinstellungen {#email-delivery-settings}

>[!NOTE]
>
> Nur Einstellungen ändern, keine neue Erstellung erlaubt. Vorbehaltlich der Zugriffsrechte.

## Typology {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typology"
>abstract="Mit der Typologie können Sie den Versand von Nachrichten steuern, filtern und überwachen."

Typologien sind Gruppen von **Typologieregeln**, die während der Nachrichtenanalyse ausgeführt werden. Damit können Sie sicherstellen, dass Ihre E-Mails immer bestimmte Elemente (z. B. einen Link zur Abmeldung oder eine Betreffzeile) oder Filterregeln enthalten, um Gruppen aus Ihrer beabsichtigten Zielgruppe auszuschließen (z. B. ehemalige Abonnenten, Konkurrenten oder Kunden, die nicht Mitglied im Treueprogramm sind).

Wenn Sie eine Typologie mit einer Nachricht oder Nachrichtenvorlage verknüpfen, werden die in der Typologie enthaltenen Typologieregeln ausgeführt, um die Gültigkeit der Nachricht zu überprüfen.

### Druckparameter {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Versandgewichtung"
>abstract="Die Versandgewichtung ermöglicht es Ihnen, im Rahmen der Druckverwaltung diejenigen Sendungen festzulegen, die vorrangig durchgeführt werden sollen. Die Nachrichten mit der höchsten Gewichtung haben Vorrang."

In diesem Abschnitt können Sie mithilfe von Druckparametern eine **Schwellenwert**. Dies ist die maximale Anzahl von Nachrichten, die an ein Profil in einem bestimmten Zeitraum gesendet werden können. Sobald diese Schwelle erreicht ist, können keine Sendungen mehr durchgeführt werden, bis der Zeitraum abgelaufen ist. Durch dieses Verfahren kann ein Profil aus einem Versand automatisch ausgeschlossen werden, wenn eine Nachricht die festgelegte Schwelle übersteigt. Dadurch wird verhindert, dass ein Profil zu oft angesprochen wird.

Schwellenwerte können konstant oder variabel sein. Das bedeutet, dass unterschiedliche Profile in einem bestimmten Zeitraum unterschiedliche Schwellen aufweisen können oder Schwellen sogar innerhalb desselben Profils variieren können.

Im **Gewichtungstyp** -Feld stehen drei Optionen zur Verfügung: (fehlende Formel je nach Option..)

* **Konstante**
* **Empfängerabhängig**
* **Wird in jeder Regel definiert**

Die **Versandgewichtung** field : Jeder Versand hat eine Gewichtung, die seine Priorität darstellt. Standardmäßig ist die Gewichtung eines Versands auf 5 festgelegt. Mithilfe von Druckregeln können Sie die Gewichtung der Sendungen bestimmen, auf die sie angewendet werden. Die Gewichtung kann entweder mithilfe einer Formel festgelegt oder berechnet werden, um sie den Empfängern anzupassen. Sie können beispielsweise die Gewichtung eines Versands auf der Basis der Interessen des Empfängers festlegen.

Die **Versandmodus** Feld. ??

* **Zielgruppenschätzung und Nachrichtenpersonalisierung**
* **Schätzung und Validierung der geplanten Zielgruppe**
* **Zielgruppenevaluierung**

### Kapazitätseinstellungen {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Wichtigkeit des Empfängers"
>abstract="Die Wichtigkeit des Empfängers ist eine Formel, mit der bestimmt wird, welche Empfänger bei Überschreitung der Typologieregeln beibehalten werden."

In diesem Abschnitt können Sie eine Kapazitätsregel auswählen, die in der Adobe Campaign v8-Konsole definiert ist. Diese Regel ist mit dem E-Mail-Kanal verknüpft.

Die **Bedeutung des Empfängers** -Feld ist eine Formel, mit der bestimmt wird, welche Empfänger bei Überschreitung der Typologieregeln zur Kapazität beibehalten werden.

## Audience {#audience}

In diesem Abschnitt können Sie eine **Zielgruppen-Mapping** definiert in der Adobe Campaign v8-Konsole. Die Zielgruppen-Mapping-Erstellung ist erforderlich, wenn Sie eine andere als die von Adobe Campaign bereitgestellte Empfängertabelle verwenden.

## Versand {#delivery}

**Routing** selection: Das externe Konto Integriertes E-Mail-Routing wird standardmäßig bereitgestellt. Es enthält die technischen Parameter, die es der Anwendung erlauben, E-Mails zu senden.

**SMTP-Versand testen**: Verwenden Sie diese Option, um den Versand per SMTP zu testen. Der Versand wird bis zur Verbindung mit dem SMTP-Server verarbeitet, aber nicht gesendet: Für jeden Empfänger des Versands stellt Campaign eine Verbindung mit dem Server des SMTP-Anbieters her, führt den SMTP-Befehl RCPT TO aus und schließt die Verbindung vor dem SMTP-Befehl DATA.

**E-Mail-BCC**: Mit dieser Option können Sie mit der BCC-Funktion E-Mails in einem externen System speichern, indem Sie einfach eine E-Mail-Adresse als BCC zu Ihrer Versandzielgruppe hinzufügen.

### Weitere Zustellversuche {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximale Anzahl der Wiederholungsversuche"
>abstract="Wenn die Zustellung einer Nachricht wegen eines vorübergehenden Fehlers fehlschlägt, werden während der Versandlaufzeit weitere Zustellversuche unternommen."

Vorübergehend nicht zugestellte Nachrichten aufgrund eines Softbounce oder eines ignorierten Fehlers werden automatisch erneut versucht. Standardmäßig sind innerhalb der ersten 24 Stunden des Versands fünf erneute Versuche im Abstand von mindestens einer Stunde vorgesehen. An den folgenden Tagen und bis zum Ablauf der Versandgültigkeit, die im Tab Gültigkeit angegeben wird, wird jeweils ein Zustellversuch unternommen.

## Validierung {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Validierung mode"
>abstract="Jeder Schritt eines Versands kann einer Validierung unterzogen werden, um eine vollständige Überwachung und Kontrolle der verschiedenen Prozesse zu gewährleisten."

**Manuell**: Am Ende der Analysephase muss der Benutzer die Absendung bestätigen, um die Nachrichten abzuschicken.

**Halbautomatisch**: Das Senden beginnt automatisch, wenn in der Analysephase keine Warnmeldungen erzeugt werden.

**Automatisch**: Die Nachrichten werden unabhängig vom Ergebnis der Analysephase automatisch abgeschickt.


## Gültigkeit {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Versandlaufzeit"
>abstract="Im Feld Versandlaufzeit können Sie die Zeitspanne angeben, in der erneute Zustellversuche unternommen werden. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis nach Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Ressourcengültigkeit"
>abstract="Das Feld Gültigkeit wird für hochgeladene Ressourcen verwendet, insbesondere für Mirrorseite und Bilder. Die Ressourcen auf dieser Seite sind für eine begrenzte Zeit gültig."


Im Feld **Versandlaufzeit** können Sie die Zeitspanne angeben, in der erneute Zustellversuche unternommen werden. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis nach Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet.

Sie können alternativ auch ein genaues Ablaufdatum angeben. Kreuzen Sie in diesem Fall die Option **Gültigkeit explizit festlegen** an. Auf diese Weise kann auch eine bestimmte Uhrzeit konfiguriert werden. Standardmäßig ist dies die aktuelle Uhrzeit. Diese kann jedoch direkt im Eingabefeld angepasst werden.

**Gültigkeit der Ressourcen** wird für hochgeladene Ressourcen verwendet, hauptsächlich für die Mirrorseite und Bilder. Die Gültigkeitsdauer der Ressourcen auf dieser Seite ist begrenzt, um Speicherkapazität zu sparen.

### Verwaltung der Mirrorseite {#mirror}

**Verwaltung der Mirrorseite** enthält vier Optionen:

* **Mirrorseite erzeugen, wenn im E-Mail-Inhalt ein Mirrorlink angezeigt wird**: Die Mirrorseite wird erzeugt, wenn der Link in den E-Mail-Inhalt eingefügt wird.
* **Mirrorseitenerzeugung forcieren**: Erstellt eine Mirrorseite, selbst wenn im Versandinhalt kein entsprechender Link enthalten ist.
* **Keine Mirrorseite erzeugen**: Generiert keine Mirrorseite, selbst wenn in den Nachrichten der entsprechende Link enthalten ist.
* **Erzeugt eine Mirrorseite, auf die nur die Nachrichtenkennung zugreifen kann**: Diese Option ermöglicht den Zugriff auf den Inhalt der Mirrorseite mit Personalisierungsinformationen im Versandlog-Fenster.


### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Gültigkeitszeitraum"
>abstract="Diese Option definiert die Dauer, für die das Tracking in den URLs aktiviert wird."

**Gültigkeitsdauer des Trackings**: Diese Option definiert die Dauer, für die das Tracking in den URLs aktiviert wird.

**Ersatz-URL für abgelaufene URLs**: Verwenden Sie diese Option, um eine Fallback-URL für eine Web-Seite einzugeben: Sie wird angezeigt, wenn das Tracking abgelaufen ist.


## Testeinstellungen {#test-setttings}

**Doppelte beibehalten** ermöglicht die Genehmigung mehrerer Sendungen an Empfänger, die verschiedenen Zielgruppenkriterien entsprechen.

**auf die Blockierungsliste gesetzt Adressen beibehalten** verhindert, dass Profile, die nicht mehr in den Versand eingeschlossen sind, von der Zielgruppe ausgeschlossen werden, z. B. nach einer Abmeldung (Opt-out).

**Quarantäne-Adressen beibehalten** ermöglicht es, alle Profile mit einer Adresse, die nicht reagiert, von der Zielgruppe fernzuhalten.

**Versandcode für den Testversand beibehalten** den gleichen Versandcode wie der für den Versand, auf den er sich bezieht, verwenden.

Standardmäßig erhält der Betreff des Testversands das Präfix &quot;Proof #&quot;, wobei # die Nummer des Testversands ist. Sie können dieses Präfix im **Titelpräfix** -Feld.