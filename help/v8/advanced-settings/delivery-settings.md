---
audience: end-user
title: Versandeinstellungen
description: Erfahren Sie mehr über die Versandeinstellungen in Campaign Web
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 96aec85933a47c1289549ba0696874a5f82e7fd5
workflow-type: tm+mt
source-wordcount: '2316'
ht-degree: 99%

---


# E-Mail-Versandeinstellungen {#email-del-settings}

E-Mail-Versandeinstellungen sind **technische Versandparameter**, die in der E-Mail-Vorlage definiert sind. Sie können bei jedem Versand überschrieben werden.

Diese Einstellungen sind über die Schaltfläche **Einstellungen** verfügbar, wenn ein E-Mail-Versand oder eine E-Mail-Versandvorlage bearbeitet wird.

## E-Mail-Versandeinstellungen {#email-delivery-settings}

>[!CAUTION]
>
>Diese Einstellungen werden hier nur zur Information beschrieben. Einige sind von Ihrer Konfiguration und Ihren Berechtigungen abhängig. Sie dürfen in dieser Version des Produkts nicht geändert werden.

## Typologieeinstellungen {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="Typologieregeln ermöglichen es Marketing-Fachleuten, Geschäftspraktiken für alle Sendungen zu standardisieren. Eine Typologie ist eine Sammlung von Typologieregeln, mit denen der Versand von Sendungen gesteuert, gefiltert und priorisiert werden kann. Profile, die den Kriterien einer Typologieregel entsprechen, werden in der Vorbereitungsphase von den Versandzielgruppen ausgeschlossen. Typologien und Typologieregeln werden in der Campaign-Client-Konsole erstellt."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologieeinstellungen für den Versand"
>abstract="Typologieregeln ermöglichen es Marketing-Fachleuten, Geschäftspraktiken für alle Sendungen zu standardisieren. Eine Typologie ist eine Sammlung von Typologieregeln, mit denen der Versand von Sendungen gesteuert, gefiltert und priorisiert werden kann. Profile, die den Kriterien einer Typologieregel entsprechen, werden in der Vorbereitungsphase von den Versandzielgruppen ausgeschlossen. Typologien und Typologieregeln werden in der Campaign-Client-Konsole erstellt."


Typologien sind Gruppen von **Typologieregeln**, die während der Vorbereitungsphase ausgeführt werden, um auf einfache Weise mehrere Filterregeln gleichzeitig auf einen Versand anwenden zu können. Sie ermöglichen es Marketing-Fachleuten, ihre Geschäftspraktiken für alle Sendungen zu standardisieren, da sie den Versand von Sendungen kontrollieren, filtern und priorisieren können.

Wenn Sie eine Typologie mit einer Nachricht oder Nachrichtenvorlage verknüpfen, werden die in der Typologie enthaltenen Typologieregeln ausgeführt, um die Gültigkeit des Versands während der Nachrichtenvorbereitung zu überprüfen. Profile, die den Kriterien einer Typologieregel entsprechen, werden dann von den Versandzielgruppen ausgeschlossen.

Typologien ermöglichen es Ihnen sicherzustellen, dass Ihre E-Mails immer bestimmte Elemente enthalten (wie beispielsweise einen Abmelde-Link oder eine Betreffzeile), oder Filterregeln anzuwenden, um Gruppen aus Ihrer Zielgruppe auszuschließen (wie abgemeldete Abonnentinnen und Abonnenten, die Konkurrenz oder die Kundschaft, die nicht Mitglied im Treueprogramm sind).

![](assets/delivery-settings-typology.png)

>[!NOTE]
>
>Typologien und Typologieregeln werden in der Campaign-Client-Konsole erstellt. Weitere Informationen über Druckregeln und die Konfiguration der Ermüdungsverwaltung finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=de){target="_blank"}.

### Druckparameter {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Druckparameter für den Versand"
>abstract="Die Versandgewichtung ermöglicht die Identifizierung von Sendungen mit der höchsten Priorität im Rahmen der Ermüdungsverwaltung. Nachrichten mit der höchsten Gewichtung haben Priorität."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Versandgewichtung"
>abstract="Die Versandgewichtung ermöglicht es Ihnen, im Rahmen der Druckverwaltung diejenigen Sendungen festzulegen, die vorrangig durchgeführt werden sollen. Die Nachrichten mit der höchsten Gewichtung haben Vorrang."

In diesem Abschnitt können Sie mithilfe von Druckparametern einen **Schwellenwert** definieren, um Regeln für die Ermüdungsverwaltung einzurichten, d. h. die maximale Anzahl von Nachrichten, die in einem bestimmten Zeitraum an ein Profil gesendet werden können.

Sobald diese Schwelle erreicht ist, können keine Sendungen mehr durchgeführt werden, bis der Zeitraum abgelaufen ist. Durch dieses Verfahren kann ein Profil aus einem Versand automatisch ausgeschlossen werden, wenn eine Nachricht die festgelegte Schwelle übersteigt. Dadurch wird verhindert, dass ein Profil zu oft angesprochen wird.

Schwellenwerte können konstant oder variabel sein. Das bedeutet, dass unterschiedliche Profile in einem bestimmten Zeitraum unterschiedliche Schwellen aufweisen können oder Schwellen sogar innerhalb desselben Profils variieren können.

Im Feld **[!UICONTROL Gewichtungstyp]** stehen drei Optionen zur Verfügung:

* **[!UICONTROL Konstante]**
* **[!UICONTROL Empfängerabhängig]**
* **[!UICONTROL Wird in jeder Regel definiert]**

Verwenden Sie das Feld **[!UICONTROL Versandgewichtung]**, um die Versandpriorität zu definieren. Jeder Versand verfügt über eine Gewichtung, die die jeweilige Priorität darstellt. Standardmäßig ist die Versandgewichtung auf den Wert 5 festgelegt. Mit Druckregeln können Sie die Gewichtung der Sendungen festlegen, auf die sie angewendet werden. Die Gewichtung kann konstant sein oder mithilfe einer Formel empfängerabhängig berechnet werden. Beispielsweise kann die Gewichtung eines Versands den Interessen eines Empfängers bzw. einer Empfängerin entsprechend bestimmt werden.

Verwenden Sie das Feld **[!UICONTROL Versandmodus]**, um den Zielgruppenauswertungsmodus auszuwählen. Drei Modi sind verfügbar:

* **[!UICONTROL Zielgruppenschätzung und Nachrichtenpersonalisierung]**
* **[!UICONTROL Schätzung und Validierung der geplanten Zielgruppe]**
* **[!UICONTROL Zielgruppenauswertung]**

>[!NOTE]
>
>Die Ermüdungsverwaltung wird in der Campaign-Client-Konsole konfiguriert. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=de){target="_blank"}.

### Kapazitätseinstellungen {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Kapazitätseinstellungen für den Versand"
>abstract="Stellen Sie vor dem Versand von Nachrichten mithilfe von Kapazitätsregeln sicher, dass Ihr Unternehmen den Versand, die durch den Versand möglicherweise erzeugten eingehenden Nachrichten und die Anzahl der Anrufe, die beispielsweise an die Abonnentinnen und Abonnenten zu richten sind, verarbeiten kann. Die Kapazitätsregeln sind in der Adobe Campaign v8-Konsole definiert. Wählen Sie in diesem Bildschirm eine Regel aus, die dem E-Mail-Kanal zugeordnet ist."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Wichtigkeit des Empfängers bzw. der Empfängerin"
>abstract="Mit der Wichtigkeit des Empfängers bzw. der Empfängerin wird festgelegt, welche Empfangenden im Falle einer Kapazitätsüberlastung der Typologieregeln beibehalten werden."


In diesem Abschnitt können Sie eine Kapazitätsregel auswählen, die in der Adobe Campaign v8-Konsole definiert ist. Diese Regel ist dem E-Mail-Kanal zugeordnet.

Das Feld **[!UICONTROL Wichtigkeit der bzw. des Empfangenden]** ist eine Formel, mit der definiert wird, welche Empfängerinnen und Empfänger bei Überschreitung der Kapazitätstypologie-Regeln behalten werden.

>[!NOTE]
>
>Typologieregeln werden in der Campaign-Client-Konsole konfiguriert. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=de){target="_blank"}.

## Zielgruppeneinstellungen {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Zielgruppeneinstellungen für den Versand"
>abstract="Ein **Zielgruppen-Mapping** unter den verfügbaren Optionen auswählen. Zielgruppen-Mappings werden in der Adobe Campaign v8-Konsole definiert. Außerdem können die Ausschlussparameter für den Versand festgelegt werden. "

In diesem Abschnitt können Sie ein verfügbares **Zielgruppen-Mapping** auswählen. Zielgruppen-Mappings werden in der Adobe Campaign v8-Konsole definiert. Zielgruppen-Mapping ist der Datentyp, den ein Vorgang verarbeitet. Sie ermöglicht die Bestimmung der Zielpopulation: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw.

Weitere Informationen über Zielgruppen-Mapping finden Sie in [diesem Abschnitt](../audience/targeting-dimensions.md).

Im Feld **[!UICONTROL Ausschluss]** können Sie Empfängerinnen und Empfänger ausschließen, die nicht mehr kontaktiert werden möchten oder sich in Quarantäne befinden. [Weitere Informationen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=de){target="_blank"}

## Versand {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Versandeinstellungen für den Versand"
>abstract="Versandparameter sind technische Einstellungen, die für Ihren Versand gelten. Für den Versand kann BCC aktiviert und die Versand- sowie die Routinemodi können geändert werden. Diese Optionen sind erfahrenen Benutzerinnen und Benutzern vorbehalten."

**[!UICONTROL Versandparameter]** sind technische Einstellungen, die für Ihren Versand gelten.

Das externe Konto **[!UICONTROL Integriertes E-Mail-Routing]** wird standardmäßig bereitgestellt. Es enthält die technischen Parameter, die es der Anwendung erlauben, E-Mails zu senden.

Sie können folgende **[!UICONTROL Versandeinstellungen]** definieren:

* **[!UICONTROL SMTP-Versand testen]**: Diese Option wird verwendet, um den Versand über SMTP zu testen. Der Versand wird bis zur Verbindung mit dem SMTP-Server verarbeitet, jedoch nicht gesendet: Für jeden Empfänger bzw. jede Empfängerin des Versands stellt Campaign eine Verbindung mit dem Server des SMTP-Anbieters her, führt den SMTP-Befehl „RCPT TO“ aus und trennt die Verbindung vor dem SMTP-Befehl „DATA“.

* **[!UICONTROL E-Mail-BCC]**: Diese Option wird verwendet, um mit der BCC-Funktion E-Mails in einem externen System zu speichern, indem einfach eine E-Mail-Adresse als BCC zu Ihrer Nachrichtzielgruppe hinzugefügt wird. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=de){target="_blank"}.

* **[!UICONTROL In mehreren Schüben versenden]**: Sie können das gesendete Volumen mithilfe von Schüben schrittweise erhöhen. Dadurch wird verhindert, dass Ihre Nachrichten als Spam gekennzeichnet werden, oder Sie können die Anzahl der pro Tag versendeten Nachrichten beschränken. Mit Schüben können Sie Sendungen in mehrere Teilsendungen unterteilen, anstatt große Mengen von Nachrichten gleichzeitig zu senden. [Weitere Informationen](send-using-waves.md)

Sie können auch das Format der gesendeten E-Mail-Nachrichten ändern:

* **[!UICONTROL Empfängerangaben berücksichtigen]** (Standardmodus)

  Das Nachrichtenformat wird auf der Grundlage der im Empfängerprofil gespeicherten Daten definiert. Falls eine Empfängerin bzw. ein Empfänger Nachrichten in einem bestimmten Format erhalten möchte, werden sie in diesem Format gesendet. Ohne Angabe in diesem Feld wird eine Nachricht vom Typ „Multipart-Alternative“ gesendet, wie im Anschluss erläutert.

* **[!UICONTROL E-Mail-Programm des Empfängers das beste Format wählen lassen]**

  Die Nachricht enthält beide Formate: Text und HTML. Das beim Empfänger angezeigte Format hängt von der Konfiguration des E-Mail-Programms ab (Multipart-Alternative).

  >[!IMPORTANT]
  >
  >Bei dieser Option werden beide Versionen des Dokuments gesendet. Der hierdurch erhöhte Kapazitätsverbrauch kann den Versanddurchsatz beeinträchtigen.

* **[!UICONTROL Alle Nachrichten im Textformat senden]**

  Die Nachricht wird im Textformat gesendet. Das HTML-Format wird nicht gesendet, sondern lediglich für die Mirrorseite verwendet, wenn der Empfänger auf die Nachricht klickt.

## Web-Analyse {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Web-Analyse-Einstellungen für den Versand"
>abstract="Ein Web-Analyse-Konto auswählen. Dieses Konto wird in der Campaign-Client-Konsole konfiguriert. Außerdem können die Tags definiert werden, die für das verwendete Analyse-Tool freigegeben wurden."

In diesem Abschnitt können Sie ein Web-Analyse-Konto auswählen. Dieses Konto wird in der Campaign-Client-Konsole konfiguriert.

Außerdem können die Tags definiert werden, die für das verwendete Analyse-Tool freigegeben wurden.

>[!NOTE]
>
>Web-Analyse-Funktionen werden in der Campaign-Client-Konsole konfiguriert. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=de#external-account-ac){target="_blank"}.

## Weitere Zustellversuche {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Maximale Anzahl der weiteren Zustellversuche"
>abstract="Wenn ein Nachrichtenversand aufgrund eines temporären Fehlers fehlschlägt, werden weitere Zustellversuche bis zum Ende der Versandlaufzeit durchgeführt."

<!--Currently not visible in UI > ??-->

Sendungen von vorübergehend nicht zugestellten Nachrichten aufgrund eines Softbounce oder eines Ignoriert-Fehlers werden automatisch wiederholt. Standardmäßig sind innerhalb der ersten 24 Stunden des Versands fünf erneute Zustellversuche im Abstand von mindestens einer Stunde vorgesehen.

Weitere Informationen zur Verwaltung von weiteren Zustellversuchen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=de){target="_blank"}.

## Validierung {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Genehmigungsmodus für den Versand"
>abstract="Den Genehmigungsmodus auswählen. Wenn bei der Versandvorbereitung Warnungen erzeugt werden, kann der Versand so konfiguriert werden, dass definiert wird, ob er trotzdem ausgeführt werden soll."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Genehmigungsmodus für Sendungen"
>abstract="Wählen Sie den Genehmigungsmodus für Sendungen aus, die auf dieser Vorlage basieren. Wenn bei der Versandvorbereitung Warnungen erzeugt werden, kann der Versand so konfiguriert werden, dass definiert wird, ob er trotzdem ausgeführt werden soll."

Wenn bei der Versandvorbereitung Warnungen erzeugt werden, kann der Versand so konfiguriert werden, dass definiert wird, ob er trotzdem ausgeführt werden soll. Standardmäßig müssen Benutzende den Nachrichtenversand am Ende der Analysephase bestätigen: Hierbei handelt es sich um eine **manuelle** Validierung.

Sie können im entsprechenden Feld einen anderen Validierungsmodus auswählen. Folgende Modi sind verfügbar: 

* ****[!UICONTROL Manuell]****: Am Ende der Analysephase muss der Benutzer bzw. die Benutzerin den Versand bestätigen, um die Nachrichten abzuschicken.

* **[!UICONTROL Halbautomatisch]**: Die Nachrichten werden automatisch gesendet, wenn die Analysephase ohne Warnhinweise abgeschlossen wird.

* **[!UICONTROL Automatisch]**: Die Nachrichten werden unabhängig vom Ergebnis der Analysephase automatisch gesendet.

## Gültigkeit {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Gültigkeit der Einstellungen"
>abstract="Im Feld **Versandlaufzeit** können Sie die Zeitspanne angeben, während der erneute Zustellversuche unternommen werden. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis zum Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet.<br>Das Feld **Gültigkeit von Ressourcen** wird für hochgeladene Ressourcen verwendet, wie etwa die Mirrorseite oder Bilder. Nach Erreichen des Grenzwerts sind keine Ressourcen mehr verfügbar."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Gültigkeit von Ressourcen"
>abstract="Das Feld **Gültigkeit von Ressourcen** wird für Ressourcen verwendet, die online verfügbar sind, insbesondere für die Mirrorseite und Bilder. Diese Ressourcen sind für eine begrenzte Zeit gültig: Nach Erreichen des Grenzwerts sind keine Ressourcen mehr verfügbar."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Versandlaufzeit"
>abstract="Im Feld **Versandlaufzeit** können Sie die Zeitspanne angeben, während der erneute Zustellversuche unternommen werden. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis zum Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### Gültigkeitszeitraum {#validity-period}

Im Feld **[!UICONTROL Versandlaufzeit]** kann die Zeitspanne angegeben werden, in der erneute globale Zustellversuche unternommen werden. Dies bedeutet konkret, dass Adobe Campaign die Nachrichten ab dem Startdatum versendet und bis zum Ablauf der angegebenen Spanne nicht zustellbare Nachrichten in regelmäßigen Abständen erneut sendet.

Sie können alternativ auch ein genaues Datum angeben. Markieren Sie dazu die Option **[!UICONTROL Gültigkeit explizit festlegen]**. In diesem Fall kann mit den Versand- und Gültigkeitsdaten auch eine bestimmte Uhrzeit konfiguriert werden. Standardmäßig wird die aktuelle Uhrzeit eingesetzt, sie kann jedoch direkt im Eingabefeld angepasst werden.

Das Feld **[!UICONTROL Gültigkeit von Ressourcen]** wird für hochgeladene Ressourcen verwendet, insbesondere für die Mirrorseite und Bilder. Die Gültigkeitsdauer von Ressourcen auf dieser Seite ist begrenzt, um Speicherkapazität zu sparen. Nach diesem Limit sind diese Ressourcen nicht mehr verfügbar.

![](assets/delivery-settings-validity.png)

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

Weitere Informationen zur Gültigkeitsdauer des Versands finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=de#validity-period){target="_blank"}.

### Verwaltung der Mirror-Seite {#mirror}

Eine Mirror-Seite ist eine HTML-Seite, die über einen Webbrowser online abgerufen werden kann und deren Inhalt mit dem der E-Mail identisch ist. Standardmäßig wird die Mirror-Seite automatisch generiert, wenn der entsprechende Link in den Inhalt der E-Mail eingefügt wurde.

Zusätzlich zum Standardmodus stehen die folgenden Optionen zur Verfügung:

* **[!UICONTROL Mirrorseitenerzeugung forcieren]**: Verwenden Sie diesen Modus, um die Mirrorseite zu erstellen, selbst wenn im Versand kein Link zur Mirrorseite eingefügt wurde.
* **[!UICONTROL Keine Mirrorseite erzeugen]**: Verwenden Sie diesen Modus, um die Erstellung einer Mirrorseite zu vermeiden, selbst wenn der Link im Versand vorhanden ist.
* **[!UICONTROL Von der Nachrichtenkennung aus zugängliche Mirrorseite erzeugen]**: Wenn der Mirrorseite-Link nicht im E-Mail-Inhalt vorhanden ist, verwenden Sie diese Option, um den Zugriff auf den Inhalt der Mirrorseite im Versandlog-Fenster über die Client-Konsole zu aktivieren.


### Tracking {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Gültigkeitszeitraum"
>abstract="Der Gültigkeitszeitraum legt die Dauer fest, für die das Tracking in den Nachrichten-URLs aktiviert ist."

**[!UICONTROL Trackingparameter]** werden im entsprechenden Abschnitt definiert. Mögliche Optionen sind:

**[!UICONTROL Tracking-Gültigkeit]**: Verwenden Sie diese Option, um die Dauer zu ändern, für die das Tracking für die URLs aktiviert ist.

**[!UICONTROL Ersatz-URL für abgelaufene URLs]**: Verwenden Sie diese Option, um eine Fallback-URL für eine Web-Seite einzugeben: Sie wird angezeigt, wenn das Tracking abgelaufen ist.

## Testversandeinstellungen {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Definieren der Testversandparameter für den Versand"
>abstract="Wählen Sie die Ausschlussparameter aus und passen Sie den Titel der Testsendungen an."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

Sie können die Ausschlussparameter in diesem Abschnitt festlegen. Folgende Optionen sind verfügbar: 

* ****[!UICONTROL Dubletten beibehalten]****: Ermöglicht es, mehrere Sendungen an Empfängerinnen und Empfänger zu genehmigen, die mehrere Zielgruppenbestimmungskriterien erfüllen.

* **[!UICONTROL Adressen auf der Blockierungsliste behalten]**: Ermöglicht es, Zielgruppenprofile, die nicht mehr in den Versand eingeschlossen sind, beizubehalten, z. B. nach einer Abmeldung (Opt-out).

* **[!UICONTROL Quarantäneadressen beibehalten]**: Ermöglicht es, Zielgruppenprofile mit einer Adresse beizubehalten, über die keine Reaktion erfolgt.

Sie können auch den Namen der Testsendungen anpassen:

* Verwenden Sie die Option **[!UICONTROL Versandcode für den Testversand beibehalten]**, um den Testversand mit demselben Versand-Code zu verknüpfen, der für den Versand, auf den er sich bezieht, definiert ist.

* Standardmäßig wird dem Betreff des Testversands „TESTVERSAND #“ vorangestellt, wobei # die Nummer des Testversands ist. Sie können dieses Präfix im Feld **[!UICONTROL Titelpräfix]** ändern.