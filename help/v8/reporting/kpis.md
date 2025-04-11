---
title: Wichtige Performance-Indikatoren
description: Lernen Sie, die wichtigsten Performance-Indikatoren zu verstehen.
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 37%

---

# Wichtige Leistungsindikatoren {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Wichtige Performance-Indikatoren"
>abstract="Mit dem Abschnitt **Wichtige Performance-Indikatoren** können Sie die Effektivität Ihrer Plattform anhand gängiger KPIs überprüfen."

<!-- à enlever? -->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="Spam-KPI"

Navigieren Sie zur Startseite, um die wichtigsten Performance-Indikatoren für Ihre Plattform zu überprüfen. Diese Indikatoren zeigen die Anzahl und den Prozentsatz der zugestellten, geöffneten, geklickten Nachrichten, Abmeldungen und Fehlerquoten an.

Metriken werden standardmäßig für die Sendungen berechnet, die in den letzten sieben Tagen durchgeführt wurden. Sie können den Punkt aus der Dropdown-Liste oben rechts auf der Karte ändern. Nachrichten, die an Testprofile gesendet werden, sind ausgeschlossen.

Sie können den anzuzeigenden Kanal auswählen. Standardmäßig beziehen sich diese Indikatoren auf Metriken für den E-Mail-Kanal.

![Screenshot der KPI-Karte mit Metriken für den E-Mail-Kanal.](assets/kpi.png){zoomable="yes"}

## Nachricht zugestellt {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Zugestellt"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller erfolgreich verarbeiteten Nachrichten und den Prozentsatz der erfolgreich zugestellten Nachrichten im Vergleich zur Gesamtzahl der gesendeten Nachrichten an."

Die Anzahl der zugestellten Nachrichten spiegelt Ihre Zustellbarkeit wider. Es kann aus den folgenden Gründen nie 100 % sein: Einige Adressen oder Telefonnummern können falsch sein, Spam-Blocker bei E-Mail-Anbietern können Ihre Nachrichten ablehnen, oder es können Probleme mit der Zustellbarkeit auftreten.

Der **Zugestellt** zeigt für jeden Kanal die folgenden KPIs an:

* Prozentsatz der erfolgreich zugestellten Nachrichten im Vergleich zur Gesamtzahl der gesendeten Nachrichten.

* Summe aller erfolgreich verarbeiteten Nachrichten.

In Adobe Campaign lautet die Regel, nach der eine Nachricht als „zugestellt“ gilt, wie folgt:

Anzahl der Nachrichten, für die das Feld „Testadresse“ gleich „Nein“ und mit dem Status „Vom Dienstleister berücksichtigt“ (für SMS), „Gesendet“ (für E-Mails) oder „Auf dem Mobiltelefon empfangen“ (für Push-Benachrichtigungen) ist.

## Öffnungen insgesamt {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Öffnungen"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller geöffneten Nachrichten und den Prozentsatz der geöffneten Nachrichten im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Die Öffnungen insgesamt werden berechnet, indem verfolgt wird, wie oft eine Nachricht insgesamt geöffnet wird, unabhängig davon, wie viele einzelne Empfänger diese Öffnungen erzeugen. Dieser Indikator ist nur für E-Mails verfügbar.

Die Anzeige **Öffnungen** zeigt für jeden Kanal die folgenden KPIs an:

* Prozentualer Anteil der geöffneten Nachrichten im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten.

* Summe aller geöffneten Nachrichten pro Kanal.

Adobe Campaign erkennt das Öffnen einer Nachricht, wenn die Empfängerin bzw. der Empfänger die Bilder in der E-Mail herunterlädt. HTML und Multipart/Alternative-E-Mails enthalten ein Bild mit 0 Pixeln, mit dem Sie geöffnete Nachrichten erkennen können. Da Nachrichten im Textformat keine Bilder enthalten, ist es unmöglich festzustellen, ob sie geöffnet wurden. Bei Werten, die auf der Grundlage der Öffnungen von Nachrichten berechnet werden, handelt es sich immer um Schätzungen aufgrund der mit der Bildanzeige verknüpften Fehlermarge.

## Clickthrough-Rate {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Klicks"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller in Nachrichten angeklickten URLs und den Prozentsatz der Klicks im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Fügen Sie URLs in Ihrem Nachrichteninhalt hinzu, um Empfänger zu einer bestimmten Seite weiterzuleiten. Die Klickrate misst die Anzahl und den Prozentsatz der Empfänger, die auf einen Link in der Nachricht geklickt haben.

Die Anzeige **Klicks** zeigt für jeden Kanal die folgenden KPIs an:

* Prozentualer Anteil der Klicks in Bezug auf die Gesamtzahl der erfolgreich zugestellten Nachrichten.

* Anzahl unterschiedlicher Personen, die mindestens einmal auf einen Versand geklickt haben. Abmelde-Links und Links zur E-Mail-Mirrorseite sind ausgeschlossen.

Diese Metriken basieren auf der konsolidierten Tracking-Tabelle (`nms:trackingStats`). Diese aggregierte Tabelle wird aus Leistungsgründen bei der Anzeige von Berichten anstelle der Tabelle der Empfänger-Trackinglogs (`nms:trackingLogRcp`) verwendet. Er wird nicht in Echtzeit berechnet. Die Tabelle wird einige Minuten nach dem Abrufen der Trackinglogs generiert.

## Abo-Raten {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Abonnements    "
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller Abonnements für einen Dienst und den Prozentsatz der Abonnements im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Empfänger können sich für E-Mail- und SMS-Nachrichten anmelden.

Der **Abonnements** zeigt für jeden Kanal die folgenden KPIs an:

* Prozentualer Anteil der Abonnements an der Gesamtzahl der erfolgreich zugestellten Nachrichten.

>[!NOTE]
>
> Die KPIs für An- und Abmeldung variieren je nach Diensttyp. E-Mail-Abonnements und -Abmeldungen umfassen beispielsweise alle E-Mail-bezogenen Dienste, unabhängig davon, ob sie aus manuellen Aktionen oder Web-Formularen resultieren. Es ist wichtig, diesen Ansatz von der Abmeldemetrik auf Versandebene zu unterscheiden, die Klicks auf Abmelde-Links statt tatsächlich abgemeldeten Benutzenden verfolgt.

## Abmelderaten {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Abmeldungen"
>abstract="Diese Metrik zeigt für den ausgewählten Kanal die Summe aller Abmeldungen von einem Dienst und den Prozentsatz der Abmeldungen im Vergleich zur Gesamtzahl der erfolgreich zugestellten Nachrichten an."

Empfänger müssen in der Lage sein, sich von E-Mail und SMS über einen speziellen Abmelde-Link im E-Mail-Inhalt oder durch Antwort auf eine SMS abzumelden.

Der Indikator **Abmeldungen** zeigt die folgenden KPIs für jeden Kanal an:

* Prozentualer Anteil der Abmeldungen in Bezug auf die Gesamtzahl der erfolgreich zugestellten Nachrichten.

* Summe aller Klicks auf einen Abmelde-Link, d. h. mit einer URL-Kategorie, die gleich „Opt-out“ ist.

>[!NOTE]
>
> Die KPIs für An- und Abmeldung variieren je nach Diensttyp. E-Mail-Abonnements und -Abmeldungen umfassen beispielsweise alle E-Mail-bezogenen Dienste, unabhängig davon, ob sie aus manuellen Aktionen oder Web-Formularen resultieren. Es ist wichtig, diesen Ansatz von der Abmeldemetrik auf Versandebene zu unterscheiden, die Klicks auf Abmelde-Links statt tatsächlich abgemeldeten Benutzenden verfolgt.

## Fehlerquoten {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Fehler"
>abstract="Gesamtzahl an Fehlern in Sendungen und der automatischen Bounce-Verarbeitung. Die zugehörige Rate wird in Bezug auf die Anzahl der zu versendenden Nachrichten berechnet."

Einige von Ihrer Adobe Campaign-Plattform gesendete Nachrichten erreichen möglicherweise nicht ihr Ziel. Dies kann vorkommen, wenn die Benutzeradresse oder die Telefonnummer Tippfehler enthält, der Empfänger seine E-Mail-Adresse geändert hat oder sein Postfach voll ist. Wenn eine Nachricht nicht an ein Profil gesendet werden kann, sendet der Remote-Server automatisch eine Fehlermeldung an Adobe Campaign. Dieser Fehler wird qualifiziert, um festzustellen, ob die E-Mail-Adresse, die Telefonnummer oder das Gerät unter Quarantäne gestellt werden soll.

Überprüfen und aktualisieren Sie Ihre Datenbank regelmäßig und stellen Sie sicher, dass alle Profile aktiv und echt sind. Versandfehler können temporär oder dauerhaft sein - Soft- oder Hardbounce - je nachdem, warum die Nachricht nicht zugestellt wurde.

Der **Fehler** zeigt für jeden Kanal die folgenden KPIs an:

* Prozentualer Anteil der fehlerhaften Nachrichten in Bezug auf die Gesamtzahl der zu sendenden Nachrichten.

* Gesamtzahl an Fehlern in Sendungen und der automatischen Bounce-Verarbeitung.

## Nachricht gesendet {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Gesendet"
>abstract="Diese Metrik zeigt für den Briefpost-Kanal die Summe aller gesendeten Nachrichten und den Prozentsatz der an den Anbieter gesendeten Nachrichten im Vergleich zur Gesamtzahl der während der Versandvorbereitungsphase vorbereiteten Nachrichten an."

Während der Vorbereitungsphase wird die Briefpost-Extraktionsdatei zwar generiert, aber die Empfängerinformationen (Versandlogs) werden nicht aktualisiert. Der Status eines Versands wechselt von Ausstehender Versand zu Gesendet , wenn der Campaign-Benutzer den Versand bestätigt. Dann wird der Status des Versands in „Abgeschlossen“ geändert.

Der Anteil der gesendeten Nachrichten kann nie 100 % betragen im Vergleich zur Gesamtzahl der vorbereiteten Nachrichten, da einige Adressen fehlen oder unvollständig sind.

Die Anzeige **Gesendet** zeigt die folgenden KPIs für den Briefpostkanal an:

* Prozentualer Anteil der gesendeten Nachrichten im Vergleich zur Gesamtzahl der vorbereiteten Nachrichten.

* Summe aller gesendeten Nachrichten.