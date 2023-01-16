---
audience: end-user
title: E-Mail-Bereitstellungseinstellungen
description: Erfahren Sie mehr über die Einstellungen für den E-Mail-Versand in der Web-Benutzeroberfläche von Campaign
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 46d8ac555e554faef91bcc817890466780387d0d
workflow-type: tm+mt
source-wordcount: '1468'
ht-degree: 55%

---

# E-Mail-Versandeinstellungen {#email-del-settings}

![Alpha-Version](../assets/do-not-localize/badge.png)

Diese Einstellungen sind **technische Versandparameter** die in der E-Mail-Vorlage definiert sind. Sie sind im **Konfigurieren der Versandeinstellungen** beim Bearbeiten eines E-Mail-Versands verfügbar ist.

## E-Mail-Versandeinstellungen {#email-delivery-settings}

>[!CAUTION]
>
> Diese Einstellungen werden nur für Ihre Informationen beschrieben. Einige davon hängen von Ihrer Konfiguration und Ihren Berechtigungen ab. Sie dürfen in dieser Version des Produkts nicht geändert werden.

## Typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="Mit einer Typologie können Sie die Durchführung von Sendungen steuern, filtern und überwachen."

Typologien sind Gruppen von **Typologieregeln**, die während der Nachrichtenanalyse ausgeführt werden. Damit können Sie sicherstellen, dass Ihre E-Mails immer bestimmte Elemente (z. B. einen Link zur Abmeldung oder eine Betreffzeile) oder Filterregeln enthalten, um Gruppen aus Ihrer beabsichtigten Zielgruppe auszuschließen (z. B. ehemalige Abonnenten, Konkurrenten oder Kunden, die nicht Mitglied im Treueprogramm sind).

Bei der Zuordnung einer Typologie zu einer Nachricht oder Nachrichtenvorlage werden die in der Typologie enthaltenen Typologieregeln ausgeführt, um die Gültigkeit der Nachricht während der Nachrichtenvorbereitung zu überprüfen.

![](assets/delivery-settings-1.png)


### Druckparameter {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Versandgewichtung"
>abstract="Die Versandgewichtung ermöglicht es Ihnen, im Rahmen der Druckverwaltung diejenigen Sendungen festzulegen, die vorrangig durchgeführt werden sollen. Die Nachrichten mit der höchsten Gewichtung haben Vorrang."

In diesem Abschnitt können Sie mithilfe von Druckparametern eine **Schwellenwert**. Dies ist die maximale Anzahl von Nachrichten, die an ein Profil in einem bestimmten Zeitraum gesendet werden können. Sobald diese Schwelle erreicht ist, können keine Sendungen mehr durchgeführt werden, bis der Zeitraum abgelaufen ist. Durch dieses Verfahren kann ein Profil aus einem Versand automatisch ausgeschlossen werden, wenn eine Nachricht die festgelegte Schwelle übersteigt. Dadurch wird verhindert, dass ein Profil zu oft angesprochen wird.

Schwellenwerte können konstant oder variabel sein. Das bedeutet, dass unterschiedliche Profile in einem bestimmten Zeitraum unterschiedliche Schwellen aufweisen können oder Schwellen sogar innerhalb desselben Profils variieren können.

Im Feld **Gewichtungstyp** stehen drei Optionen zur Verfügung:

* **Konstante**
* **Empfängerabhängig**
* **Wird in jeder Regel definiert**

Verwenden Sie die **Versandgewichtung** -Feld, um die Versandpriorität festzulegen. Jeder Versand hat eine Gewichtung, die seine Priorität darstellt. Standardmäßig ist die Gewichtung eines Versands auf 5 festgelegt. Mithilfe von Druckregeln können Sie die Gewichtung der Sendungen bestimmen, auf die sie angewendet werden. Die Gewichtung kann entweder mithilfe einer Formel festgelegt oder berechnet werden, um sie den Empfängern anzupassen. Sie können beispielsweise die Gewichtung eines Versands auf der Basis der Interessen des Empfängers festlegen.


Verwenden Sie die **Versandmodus** -Feld, um den Zielauswertungsmodus auszuwählen. Drei Modi sind verfügbar:

* **Zielgruppenschätzung und Nachrichtenpersonalisierung**
* **Schätzung und Validierung der geplanten Zielgruppe**
* **Zielgruppenevaluierung**

Die Ermüdungsverwaltung wird mit dem **Kampagnenoptimierung** -Add-on. Erfahren Sie mehr über Druckregeln und wie Sie die Ermüdungsverwaltung in [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=de){target="_blank"}.

### Kapazitätseinstellungen {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Wichtigkeit des Empfängers bzw. der Empfängerin"
>abstract="Mit der Wichtigkeit des Empfängers bzw. der Empfängerin wird festgelegt, welche Empfangenden im Falle einer Kapazitätsüberlastung der Typologieregeln beibehalten werden."

In diesem Bereich können Sie eine Kapazitätsregel auswählen, die in der Adobe Campaign v8-Konsole definiert ist. Diese Regel ist mit dem E-Mail-Kanal verknüpft.

Mit dem Feld **Wichtigkeit des Empfängers** wird festgelegt, welche Empfangenden im Falle einer Kapazitätsüberlastung der Typologieregeln beibehalten werden.

Erfahren Sie mehr über Konsistenz- und Kapazitätsregeln und deren Konfiguration in [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Audience {#audience}

In diesem Abschnitt können Sie eine **Zielgruppen-Mapping** unter denen, die verfügbar sind. Zielgruppen-Mappings werden in der Adobe Campaign v8-Konsole definiert.

Weitere Informationen zu Zielgruppen-Mappings finden Sie unter [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Versand {#delivery}

Versandparameter sind technische Einstellungen, die für Ihren Versand gelten.

* **Routing**: das externe Konto Integriertes E-Mail-Routing standardmäßig bereitgestellt wird. Es enthält die technischen Parameter, die es der Anwendung erlauben, E-Mails zu senden.

* **SMTP-Versand testen**: Diese Option wird zum Testen des Versands über SMTP verwendet. Der Versand wird bis zur Verbindung mit dem SMTP-Server verarbeitet, aber nicht gesendet: Für jeden Empfänger bzw. jede Empfängerin des Versands stellt Campaign eine Verbindung mit dem Server des SMTP-Anbieters her, führt den SMTP-Befehl RCPT TO aus und trennt die Verbindung vor dem SMTP-Befehl DATA.

* **E-Mail-BCC**: Diese Option wird verwendet, um E-Mails über BCC in einem externen System zu speichern, indem einfach eine BCC-E-Mail-Adresse zu Ihrer Versandzielgruppe hinzugefügt wird. Weitere Informationen zu E-Mail-BCC in [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### Weitere Zustellversuche {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximale Anzahl der weiteren Zustellversuche"
>abstract="Wenn die Zustellung einer Nachricht wegen eines vorübergehenden Fehlers fehlschlägt, werden während der Versandlaufzeit weitere Zustellversuche unternommen."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Erfahren Sie mehr über die Verwaltung von Wiederholungen in [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Validierung {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Validierungsmodus"
>abstract="Jeder Schritt eines Versands kann einer Validierung unterzogen werden, um eine vollständige Überwachung und Kontrolle der verschiedenen Prozesse zu gewährleisten."

Wenn bei der Versandvorbereitung Warnungen erzeugt werden, können Sie den Versand so konfigurieren, dass festgelegt wird, ob er weiterhin ausgeführt werden soll oder nicht. Standardmäßig muss der Benutzer den Nachrichtenversand am Ende der Analysephase bestätigen: dies ist **Handbuch** Validierung.

Sie können im entsprechenden Feld einen anderen Validierungsmodus auswählen. Verfügbare Modi sind:

* **Manuell**: Am Ende der Analysephase muss der Benutzer die Absendung bestätigen, um die Nachrichten abzuschicken.

* **Halbautomatisch**: Das Senden beginnt automatisch, wenn in der Analysephase keine Warnmeldungen erzeugt werden.

* **Automatisch**: Der Versand beginnt automatisch am Ende der Analysephase, unabhängig vom Ergebnis.


## Gültigkeit {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Versandlaufzeit"
>abstract="Im Feld „Versandlaufzeit“ können Sie die Zeitspanne angeben, in der erneute Zustellversuche unternommen werden sollen. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis nach Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Gültigkeit von Ressourcen"
>abstract="Das Feld „Gültigkeit von Ressourcen“ wird für hochgeladene Ressourcen verwendet, hauptsächlich für die Mirrorseite und Bilder. Die Gültigkeitsdauer der Ressourcen auf dieser Seite ist begrenzt."


Im Feld **Versandlaufzeit** können Sie die Zeitspanne angeben, in der erneute Zustellversuche unternommen werden. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis nach Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet.

Sie können alternativ auch ein genaues Ablaufdatum angeben. Kreuzen Sie in diesem Fall die Option **Gültigkeit explizit festlegen** an. Auf diese Weise kann auch eine bestimmte Uhrzeit konfiguriert werden. Standardmäßig ist dies die aktuelle Uhrzeit. Diese kann jedoch direkt im Eingabefeld angepasst werden.

**Gültigkeit der Ressourcen** wird für hochgeladene Ressourcen verwendet, hauptsächlich für die Mirrorseite und Bilder. Die Gültigkeitsdauer von Ressourcen auf dieser Seite ist begrenzt, um Speicherkapazität zu sparen.

![](assets/delivery-settings-2.png)


Erfahren Sie mehr über den Gültigkeitszeitraum eines Versands in [Dokumentation zu Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Verwaltung der Mirrorseite {#mirror}

Eine Mirrorseite ist eine HTML-Seite, die über einen Webbrowser online abgerufen werden kann und deren Inhalt mit dem der E-Mail identisch ist. Standardmäßig wird die Mirror­Seite automatisch generiert, wenn der entsprechende Link in den Inhalt der E-Mail eingefügt wurde.

Außerdem stehen die folgenden Modi zur Verfügung:

* **[!UICONTROL Mirrorseitenerzeugung forcieren]**: Erstellt eine Mirror-Seite, selbst wenn im Versandinhalt kein entsprechender Link enthalten ist.
* **[!UICONTROL Keine Mirrorseite erzeugen]**: Erstellt keine Mirror-Seite, selbst wenn im Versandinhalt der entsprechende Link enthalten ist.
* **[!UICONTROL Von der Nachrichtenkennung aus zugängliche Mirrorseite erzeugen]**: Diese Option ermöglicht den Zugriff auf den Inhalt der Mirror-Seite einschließlich aller Personalisierungsinformationen von den Versand-Logs aus. Klicken Sie hierfür nach Durchführung des Versands auf den Tab **[!UICONTROL Versand]** und wählen Sie die Zeile des Empfängers aus, dessen Mirror-Seite Sie ansehen möchten. Klicken Sie dann auf den Link **[!UICONTROL Mirrorseite dieser Nachricht anzeigen...]**.


### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Gültigkeitszeitraum"
>abstract="Diese Option definiert die Dauer, für die das Tracking in den URLs aktiv sein soll."

Tracking-Parameter werden im entsprechenden Abschnitt definiert. Mögliche Optionen sind:

**Gültigkeitsdauer des Trackings**: Verwenden Sie diese Option, um die Dauer zu ändern, für die das Tracking in den URLs aktiviert wird.

**Ersatz-URL für abgelaufene URLs**: Verwenden Sie diese Option, um eine Fallback-URL für eine Web-Seite einzugeben: Sie wird angezeigt, wenn das Tracking abgelaufen ist.

## Testeinstellungen {#test-setttings}

Sie können die Ausschlussparameter in diesem Abschnitt festlegen. Verfügbare Optionen sind:

* **Doppelte beibehalten** ermöglicht die Genehmigung mehrerer Sendungen an Empfänger, die verschiedenen Zielgruppenkriterien entsprechen.

* **auf die Blockierungsliste gesetzt Adressen beibehalten** verhindert, dass Profile, die nicht mehr in den Versand eingeschlossen sind, von der Zielgruppe ausgeschlossen werden, z. B. nach einer Abmeldung (Opt-out).

* **Quarantäne-Adressen beibehalten** ermöglicht es, alle Profile mit einer Adresse, die nicht reagiert, von der Zielgruppe fernzuhalten.

Sie können auch den Namen der Testsendungen anpassen.

Verwenden Sie die **Versandcode für den Testversand beibehalten** dem Testversand denselben Versandcode zuzuordnen, der für den Versand, auf den er sich bezieht, definiert ist.

Standardmäßig erhält der Betreff des Testversands das Präfix &quot;PROOF #&quot;, wobei # die Nummer des Testversands ist. Sie können dieses Präfix im **Titelpräfix** -Feld.