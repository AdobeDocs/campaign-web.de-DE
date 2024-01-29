---
audience: end-user
title: In Schüben versenden
description: Erfahren Sie mehr über die Versandeinstellungen in Campaign Web
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 1d3e2ccbf4db5eb23531351572a4400754982e2d
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 53%

---


# In Schüben versenden {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Waagen-Definition"
>abstract="Definieren Sie Schübe, um Sendungen in mehrere Teilsendungen zu unterteilen, anstatt große Mengen von Nachrichten gleichzeitig zu senden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Größe der Welle"
>abstract="Die Größe des Schubs ist erforderlich. Geben Sie entweder einen numerischen Wert (Anzahl Nachrichten) oder einen Prozentsatz (0-100 %) in das Feld &quot;Größe&quot;ein."

Um eine gleichmäßige Auslastung der Kapazitäten zu gewährleisten, können Sie Sendungen in mehrere Schübe unterteilen. Konfigurieren Sie die Anzahl der Schübe und ihre Größe in Bezug auf den gesamten Versand.

>[!NOTE]
>
>Sie können nur die Größe und die Zeitverzögerung zwischen zwei aufeinanderfolgenden Schüben definieren. Die Empfängerauswahlkriterien für jeden Schub können nicht konfiguriert werden.

1. Öffnen Sie die [Versandeinstellungen](delivery-settings.md#retries) und gehen Sie zu **[!UICONTROL Versand]** Registerkarte.
1. Wählen Sie die Option **[!UICONTROL In mehreren Schüben versenden]** aus und danach den Link **[!UICONTROL Definition der Schübe...]**.

1. Zur Konfiguration von Schüben haben Sie die folgenden Möglichkeiten:

   * **[!UICONTROL Mehrere Schübe derselben Größe planen]**. Wenn Sie beispielsweise **[!UICONTROL 30 %]** im entsprechenden Feld enthält jeder Schub 30 % der im Versand enthaltenen Nachrichten, mit Ausnahme des letzten Schubs, der 10 % der Nachrichten ausmacht.

     Im **[!UICONTROL Intervall]** den Zeitraum zwischen dem Start zweier aufeinander folgender Schübe festlegen. Wenn Sie beispielsweise **[!UICONTROL 2d]**, wird die erste Welle sofort starten, die zweite Welle wird in zwei Tagen starten, die dritte Welle in vier Tagen usw.

   * **[!UICONTROL Schübe nach Kalenderangaben planen]**.

     Im **[!UICONTROL Starten]** gibt die Verzögerung zwischen dem Start zweier aufeinander folgender Schübe an. Im **[!UICONTROL Größe]** eine feste Zahl oder einen Prozentsatz eingeben.

     Im unten stehenden Beispiel beinhaltet der erste Schub 25 % der Gesamtzahl der im Versand enthaltenen Nachrichten und beginnt unmittelbar. Die nächsten beiden Schübe vervollständigen den Versand und starten in Intervallen von je sechs Stunden.

     eine spezifische Typologieregel, **[!UICONTROL Prüfung der Wave Scheduling]**, stellt sicher, dass der letzte Schub vor der Gültigkeit des Versands geplant ist. Kampagnentypologien und ihre Regeln werden im Abschnitt **[!UICONTROL Typologie]** in den Versandeinstellungen. Weitere Informationen zu Kontrollregeln finden Sie in [Dokumentation zu Campaign v8 (Clientkonsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html)

     >[!IMPORTANT]
     >
     >Achten Sie darauf, dass die letzten Schübe nicht die in der Variablen **[!UICONTROL Gültigkeit]** Registerkarte. Andernfalls werden manche Nachrichten möglicherweise nicht gesendet. [Weitere Informationen](delivery-settings.md#validity)
     >
     >Planen Sie bei der Konfiguration der letzten Schübe auch genügend Zeit für zusätzliche Versuche ein. [Weitere Informationen](delivery-settings.md#retries)

1. Um Ihre Sendungen zu überwachen, rufen Sie die [Versandlogs](../monitor/delivery-logs.md).

Die Versandlogs enthalten die bereits in den verarbeiteten Schüben durchgeführten Sendungen (Status **[!UICONTROL Gesendet]**) sowie die in den restlichen Schüben durchzuführenden Sendungen (Status **[!UICONTROL Ausstehend]**).

Im Folgenden finden Sie die häufigsten Anwendungsbeispiele für Schübe.

* **In der Anfangsphase**

  Wenn E-Mails über eine neue Plattform versendet werden, sind ISPs normalerweise misstrauisch gegenüber den neuen IP-Adressen. Das plötzliche Versenden großer Mengen an E-Mails veranlasst ISPs oft dazu, sie als Spam zu qualifizieren.

  Um zu verhindern, dass Ihre Sendungen als Spam eingestuft werden, können Sie das gesendete Volumen schrittweise mithilfe von Schüben erhöhen. Damit gewährleisten Sie eine problemlose Entwicklung in der Anfangsphase und die Verringerung der Anzahl der ungültigen Adressen.

  Verwenden Sie dazu die Option **[!UICONTROL Schübe in einem Kalender definieren]**. Wählen Sie beispielsweise für den ersten Schub 10 %, für den zweiten 15 % usw.

* **Kampagnen, die ein Callcenter beinhalten**

  Bei telefonischen Treuekampagnen verfügen Unternehmen oft über begrenzte Kapazitäten für die Verarbeitung der Anrufe an Abonnenten.

  Mithilfe von Schüben kann die Anzahl der Nachrichten auf 20 pro Tag beschränkt werden, was der täglichen Verarbeitungskapazität eines Callcenters entspricht.

  Wählen Sie dazu die **[!UICONTROL Mehrere Schübe derselben Größe planen]** -Option. Eingabe **[!UICONTROL 20]** als Größe der Welle und **[!UICONTROL 1 T]** im **[!UICONTROL Zeitraum]** -Feld.