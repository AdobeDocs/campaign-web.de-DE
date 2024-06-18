---
audience: end-user
title: Versandwarnung
description: Erfahren Sie, wie Sie mit Versandwarnungen arbeiten.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 17%

---

# Versandwarnungs-Dashboards {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Versandwarnungs-Dashboards"
>abstract="Versandwarnung ist ein Warnhinweissystem, mit dem Benutzergruppen automatisch E-Mail-Benachrichtigungen mit Informationen zu ihren Versandausführungen erhalten können. In Versandwarnungs-Dashboards können Sie festlegen, wer E-Mail-Warnungen erhalten soll, die Warnungsbedingungen zum Senden dieser Warnungen auswählen und konfigurieren sowie auf den Verlauf aller gesendeten Benachrichtigungen zugreifen."

In Versandwarnungs-Dashboards können Sie festlegen, wer E-Mail-Warnungen erhalten soll, die Warnungsbedingungen zum Senden dieser Warnungen auswählen und konfigurieren sowie auf den Verlauf aller gesendeten Benachrichtigungen zugreifen. Sie können über die **Versandwarnung** im linken Navigationsbereich unter dem **Dashboards** Registerkarte.

![](assets/alerting-dashboard-list.png)

## Versand-Dashboard erstellen {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Erstellen eines Versandwarnungs-Dashboards"
>abstract="Durch die Erstellung eines Versandwarnungs-Dashboards können Sie festlegen, wer E-Mail-Warnungen erhalten soll, die für den Versand dieser Warnungen zu verwendenden Warnungsbedingungen auswählen und konfigurieren sowie auf den Verlauf aller gesendeten Benachrichtigungen zugreifen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Allgemeine Parameter für die Versandwarnung"
>abstract="Geben Sie die allgemeinen Eigenschaften des Versandwarnungs-Dashboards an. Die **Wählen Sie eine Warngruppe aus.** -Feld können Sie die **Benutzergruppe** um die von diesem Dashboard gesendeten Warnungen zu erhalten."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Versandwarnungskriterien"
>abstract="Fügen Sie in diesem Abschnitt Kriterien hinzu, mit denen Sie Warnungen über dieses Dashboard senden möchten. Wählen Sie aus vordefinierten Kriterien oder erstellen Sie eigene Kriterien, um sie an bestimmte Anforderungen anzupassen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Bedingungsparameter"
>abstract="Kriterien verfügen über Standardparameter, die definieren, wie sie angewendet werden müssen. Sie können diese Werte entsprechend Ihren Anforderungen in diesem Abschnitt ändern."

Gehen Sie wie folgt vor, um ein Versand-Dashboard zu erstellen:

1. Navigieren Sie zum **Versandwarnung** Menü im linken Navigationsbereich und klicken Sie auf **Versand-Dashboard erstellen**.

   ![](assets/alerting-dashboard.png)

1. Benennen Sie Ihr Dashboard im **Titel** -Feld. Die **Interner Name** wird automatisch ausgefüllt und schreibgeschützt.

1. Im **Wählen Sie eine Warngruppe aus.** -Feld, geben Sie die **Benutzergruppe** um die von diesem Dashboard gesendeten Warnungen zu erhalten. Alle Mitglieder der ausgewählten Benutzergruppe erhalten die Warnungen.

   Weitere Informationen zu Berechtigungen und Benutzergruppen finden Sie im Abschnitt [Dokumentation zu Adobe Campaign v8 (Konsole)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. Im **Versandwarnungsbedingungen** -Abschnitt Kriterien hinzufügen, die Sie zum Senden von Warnungen verwenden möchten. Wählen Sie aus vordefinierten Kriterien oder erstellen Sie eigene Kriterien, um sie an bestimmte Anforderungen anzupassen. [Erfahren Sie, wie Sie mit Kriterien arbeiten.](../msg/delivery-alerting-criteria.md)

1. Kriterien verfügen über Standardparameter, die definieren, wie sie angewendet werden müssen. Sie können diese Werte anhand der Variablen **Bedingungsparameter** Abschnitt.

   ![](assets/alerting-criteria-parameters.png)

   Beispiel: Standardmäßig wird die **Mindestgröße der Versandzielgruppe** Der Kriterienparameter ist auf 50 gesetzt, d. h. ein Versand wird nur dann in die von diesem Dashboard gesendete Warnung aufgenommen, wenn er mindestens 50 Profile anspricht. Sie können diesen Parameter ändern, wenn Sie Sendungen mit weniger als 50 Profilen einbeziehen möchten.

   Erweitern Sie den folgenden Abschnitt, um weitere Informationen zu den einzelnen Kriterienparametern zu erhalten:

   ++ Verfügbare Kriterienparameter

   * **Mindestgröße der Versandzielgruppe**: Wenn Sie in diesem Feld beispielsweise 100 eingeben, wird eine Benachrichtigung nur für Sendungen gesendet, deren Zielgruppe mindestens 100 Empfänger umfasst. Dieser Parameter gilt für alle Bedingungen.
   * **Monitoring-Zeitraum vor und nach dem Kontaktdatum (in Stunden)**: Anzahl der Stunden vor und nach der aktuellen Zeit. Berücksichtigt werden nur Sendungen, deren Kontaktdatum in diesem Zeitraum liegt. Dieser Parameter gilt für alle Bedingungen. Standardmäßig ist der Wert dieses Feldes mit 24 Stunden festgelegt.
   * **Maximale Softbounce-Fehlerrate**: Eine Benachrichtigung wird für alle Sendungen gesendet, deren Softbounce-Fehlerrate über dem definierten Wert liegt. Standardmäßig ist der Wert dieses Feldes mit 0,05 (5 %) Stunden festgelegt.
   * **Maximale Hardbounce-Fehlerrate**: Eine Benachrichtigung wird für alle Sendungen gesendet, deren Hardbounce-Fehlerrate über dem definierten Wert liegt. Standardmäßig ist der Wert dieses Feldes mit 0,05 (5 %) Stunden festgelegt.
   * **Mindestzeitspanne für die Auslieferung im Status &quot;Start ausstehend&quot;(in Minuten)**: Eine Benachrichtigung wird für alle Sendungen gesendet, deren Status Start ausstehend die in diesem Feld angegebene Dauer überschreitet. Start ausstehend bedeutet, dass die Nachrichten vom System noch nicht berücksichtigt wurden.
   * **Mindestdauer für die Berechnung des Durchsatzes (in Minuten)**: Für die Bedingung Sendungen mit geringem Durchsatz werden nur die Sendungen berücksichtigt, die über die angegebene Dauer (mit Status Gestartet ) gestartet wurden.
   * **Maximaler Prozentsatz verarbeiteter Nachrichten zur Berechnung des Durchsatzes**: Nur Sendungen, deren Prozentsatz an verarbeiteten Nachrichten unter dem festgelegten Prozentsatz liegt, werden für die Bedingung Sendungen mit geringem Durchsatz berücksichtigt.
   * **Erwarteter Mindestdurchsatz (in gesendeten Nachrichten pro Stunde)**: Nur Sendungen mit einem Durchsatz, der unter dem angegebenen Wert liegt, werden für die Bedingung Sendungen mit geringem Durchsatz berücksichtigt.
   * **Für das Kriterium &quot;Gestartete Sendungen&quot;erforderliche Mindest-Verarbeitungsrate**: Nur Sendungen, deren Prozentsatz der verarbeiteten Nachrichten über dem festgelegten Prozentsatz liegt, werden berücksichtigt.

+++

1. Warnhinweis-Dashboards sind standardmäßig deaktiviert, d. h., mit diesem Dashboard verknüpfte E-Mail-Warnungen werden nicht gesendet. Um das Dashboard sofort zu aktivieren, schalten Sie die **Aktiviert** in der **Allgemein** neben dem Feld für die Warnungsgruppenauswahl.

   Sie können das Dashboard auch speichern und später aktivieren.

   ![](assets/alerting-dashboard-enable.png)

1. Um das Warnhinweis-Dashboard zu speichern, klicken Sie auf das **Speichern** Schaltfläche.

Das Warnungsdashboard wird mit leeren Daten geöffnet. Wenn Sie bereit sind, sie zu aktivieren und Benachrichtigungen zu senden, klicken Sie auf die Schaltfläche **Einstellungen** Schaltfläche und Umschalten **Aktiviert** , wenn Sie dies noch nicht getan haben.

Jedes Mal, wenn ein Versand die in diesem Dashboard definierten Kriterien erfüllt, wird eine Benachrichtigung zur Warnung an die angegebene Benutzergruppe gesendet.

## Warnungs-Dashboards verwalten

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Versandwarnungen gesendet"
>abstract="In diesem Abschnitt können Sie Informationen zu den zuletzt gesendeten Warnungen visualisieren."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Verlauf der Versandwarnungen"
>abstract="Die **Geschichte** enthält alle Warnungen, die von diesem Dashboard gesendet werden. Klicken Sie auf ein Element, um auf die entsprechenden Warnhinweise zuzugreifen, die zu dem jeweiligen Zeitpunkt gesendet wurden."

Alle erstellten Warnhinweis-Dashboards können über das Menü **Versandwarnung** im Menü **Dashboards** Registerkarte.

![](assets/alerting-dashboard-list.png)

Sie können ein Dashboard mit der Variablen **Mehr Aktionen** neben ihrem Namen.

Um eine detaillierte Ansicht eines Dashboards aufzurufen, klicken Sie in der Liste auf dessen Namen. In diesem Bildschirm können Sie den zuletzt gesendeten Warnhinweis visualisieren. Alle gesendeten Warnungen werden im linken Bereich aufgelistet. Klicken Sie auf ein Element, um auf die entsprechenden Warnhinweise zuzugreifen, die zu dem jeweiligen Zeitpunkt gesendet wurden.

![](assets/alerting-dashboard-details.png)

Um das Dashboard zu bearbeiten, klicken Sie auf die Schaltfläche **Einstellungen** in der oberen rechten Ecke und nehmen Sie die gewünschten Änderungen vor.
