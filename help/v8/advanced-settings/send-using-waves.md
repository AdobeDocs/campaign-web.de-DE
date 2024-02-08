---
audience: end-user
title: Versenden in Schüben
description: Erfahren Sie mehr über die Versandeinstellungen in Campaign Web
feature: Email
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 3f4f09ddae3a2e46adf99f288642acee561ce1f5
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 33%

---


# Versenden in Schüben {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Sendungen in mehrere Teilsendungen aufteilen"
>abstract="Erstellen Sie Schübe, um Sendungen in mehrere Teilsendungen zu unterteilen, anstatt gleichzeitig große Mengen von Nachrichten zu senden. Sie können mehrere Schübe derselben Größe konfigurieren oder einen Kalender für die verschiedenen Schübe festlegen, die gesendet werden sollen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Definieren der Größe jedes Schubs"
>abstract="Sie müssen für alle hinzugefügten Schübe eine Größe eingeben. Geben Sie entweder einen numerischen Wert (Anzahl der Nachrichten pro Schub) oder einen Prozentsatz (0-100 %) ein."

Um die Auslastung auszugleichen, können Sie E-Mail-Sendungen in mehrere Teilsendungen unterteilen. Konfigurieren Sie die Anzahl der Batches und ihren Anteil in Bezug auf den gesamten Versand sowie das Intervall zwischen zwei Schüben.

>[!NOTE]
>
>Sie können nur die Größe und die Verzögerung zwischen zwei aufeinander folgenden Schüben definieren. Die Auswahlkriterien der Empfänger für jeden Schub können nicht angepasst werden.

Gehen Sie wie folgt vor, um Sendungen in Schüben durchzuführen.

1. Öffnen Sie die [Versandeinstellungen](delivery-settings.md#retries).

1. Navigieren Sie zum **[!UICONTROL Versand]** Abschnitt.

1. Wählen Sie die **[!UICONTROL In mehreren Schüben versenden]** -Option.

1. Zur Konfiguration von Schüben haben Sie die folgenden Möglichkeiten:

   * [Mehrere Schübe gleicher Größe planen](#waves-same-size)
   * [Schübe nach einem Kalender planen](#waves-calendar)

1. Bereiten Sie Ihren Versand wie gewohnt vor und senden Sie ihn. [Weitere Informationen](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >Achten Sie darauf, dass die letzten Schübe nicht die in der Variablen [Gültigkeit](delivery-settings.md#validity) zuordnen, da andernfalls manche Nachrichten nicht gesendet werden. Eine spezifische Typologie-Kontrollregel (**[!UICONTROL Prüfung der Schub-Planung]**) stellt sicher, dass der letzte Schub vor dem Ablauf der Versandgültigkeit eingeplant ist. Weitere Informationen zu Kontrollregeln finden Sie in [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=de).
   >
   >Planen Sie bei der Konfiguration der letzten Schübe auch genügend Zeit für zusätzliche Versuche ein. [Weitere Informationen](delivery-settings.md#retries)

1. Um Ihre Sendungen zu überwachen, rufen Sie die [Versandlogs](../monitor/delivery-logs.md). Die Versandlogs enthalten die bereits in den verarbeiteten Schüben durchgeführten Sendungen (Status **[!UICONTROL Gesendet]**) sowie die in den restlichen Schüben durchzuführenden Sendungen (Status **[!UICONTROL Ausstehend]**).

## Mehrere Schübe gleicher Größe planen {#waves-same-size}

Wenn Sie diese Option wählen, haben alle Schübe dieselbe Größe (mit Ausnahme der letzten) und die Verzögerung zwischen jedem Schub ist immer gleich.

![](assets/waves-same-size.png)

* Geben Sie die Größe für alle Schübe an, in die Sie den Versand unterteilen. Sie können einen Prozentsatz oder einen numerischen Wert eingeben. Nur der letzte Schub kann variieren, da er die verbleibende Nachrichtenanzahl enthalten muss.

  Wenn Sie beispielsweise **[!UICONTROL 30 %]** im **[!UICONTROL Waagen-Größe]** eingeben, entsprechen die ersten drei Schübe 30 % aller im Versand enthaltenen Nachrichten, während die vierte die restlichen 10 % ausmacht.

* Geben Sie im Abschnitt **[!UICONTROL Intervall]** die Verzögerung zwischen dem Beginn von zwei aufeinanderfolgenden Wellen an. Wenn Sie beispielsweise **[!UICONTROL 2 Tage]**, beginnt der erste Schub sofort, der zweite Schub beginnt in zwei Tagen, der dritte in vier Tagen usw.

Ein gängiges Anwendungsbeispiel für die Verwendung mehrerer Schübe gleicher Größe ist der Einsatz eines Callcenters. Bei telefonischen Treuekampagnen verfügen Unternehmen oft über begrenzte Kapazitäten für die Verarbeitung der Anrufe an Abonnenten.

Mithilfe von Schüben kann die Anzahl der Nachrichten auf 20 pro Tag beschränkt werden, was der täglichen Verarbeitungskapazität eines Callcenters entspricht.

Wählen Sie dazu die Option **[!UICONTROL Mehrere Schübe derselben Größe planen]**. Eingabe **[!UICONTROL 20]** Größe der Schübe und **[!UICONTROL 1 Tag]** im **[!UICONTROL Intervall]** -Feld.

![](assets/waves-call-center.png)

## Schübe nach einem Kalender planen {#waves-calendar}

Wenn Sie diese Option auswählen, müssen Sie den Starttag/-zeitpunkt für jeden gesendeten Schub sowie die Größe jedes Schubs definieren.

* Im **[!UICONTROL Starten]** die Verzögerung zwischen dem Start zweier aufeinander folgender Schübe angeben.

* Geben Sie in der Spalte **[!UICONTROL Größe]** eine feste Zahl oder einen Prozentsatz ein.

Fügen Sie so viele Schübe hinzu, wie Sie möchten. Sie können sie nach Bedarf neu anordnen.

>[!NOTE]
>
>Wenn Sie Prozentsätze verwenden, sollte die Summe für alle Schübe 100 % nicht überschreiten.

Im folgenden Beispiel entspricht der erste Schub 25 % der Gesamtzahl der im Versand enthaltenen Nachrichten und beginnt sofort. Die nächsten beiden Schübe vervollständigen den Versand und starten in Intervallen von jeweils sechs Stunden.

![](assets/waves-calendar.png)

Ein gängiges Nutzungsszenario für die Verwendung mehrerer Schübe je nach Kalender ist die Anlaufphase.

Wenn E-Mails über eine neue Plattform versendet werden, sind ISPs normalerweise misstrauisch gegenüber den neuen IP-Adressen. Das plötzliche Versenden großer Mengen an E-Mails veranlasst ISPs oft dazu, sie als Spam zu qualifizieren.

Um zu verhindern, dass Ihre Sendungen als Spam eingestuft werden, können Sie das gesendete Volumen schrittweise mithilfe von Schüben erhöhen. Damit gewährleisten Sie eine problemlose Entwicklung in der Anfangsphase und die Verringerung der Anzahl der ungültigen Adressen.

Verwenden Sie dazu die **[!UICONTROL Schübe nach Kalenderangaben planen]** -Option. Setzen Sie beispielsweise den ersten Schub auf 10 %, den zweiten auf 15 %, den dritten auf 20 % usw.

![](assets/waves-ramp-up.png)



