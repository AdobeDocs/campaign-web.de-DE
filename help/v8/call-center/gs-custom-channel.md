---
audience: end-user
title: Erste Schritte mit benutzerdefinierten externen Kanälen
description: Erfahren Sie, wie Sie mit Adobe Campaign Web Sendungen über benutzerdefinierte externe Kanäle erstellen und durchführen.
exl-id: b4336a0a-d845-4024-a06b-400fce1316a4
source-git-commit: ded0942ef4a145189007e3ce428f1cd7594bc347
workflow-type: ht
source-wordcount: '550'
ht-degree: 100%

---

# Erste Schritte mit benutzerdefinierten externen Kanälen {#gs-custom-channel}

Sie können Sendungen direkt über die Adobe Campaign Web-Benutzeroberfläche orchestrieren und auf Grundlage benutzerdefinierter externer, mit Drittanbietern integrierter Kanäle ausführen. Die Erstellung des benutzerdefinierten externen Kanals erfolgt in der Client-Konsole.

Sie können Sendungen über benutzerdefinierte externe Kanäle in Workflows oder als eigenständige Sendungen konfigurieren, Ihre Zielgruppe definieren und anpassbare Exportdateien mit allen erforderlichen Kontakt- und Personalisierungsdaten generieren.

>[!NOTE]
>
>Die Reporting-Funktion ist in der Web-Benutzeroberfläche für Sendungen über benutzerdefinierte externe Kanäle nicht verfügbar. Sie müssen zur Client-Konsole wechseln, um auf Berichte zuzugreifen.

Die folgenden Schritte beschreiben die Vorgehensweise beim Erstellen eines eigenständigen (einmaligen) Versands. Die meisten Schritte ähneln denen von Callcenter-Sendungen. Weitere Informationen finden Sie auf dieser [Seite](../call-center/create-call-center.md).

Befolgen Sie die Hinweise in den nachfolgenden Punkten, um einen neuen, eigenständigen, benutzerdefinierten externen Versand zu erstellen und durchzuführen:

1. [Weitere Informationen](#create-channel) zum Erstellen des benutzerdefinierten externen Kanals
1. [Weitere Informationen](#create-delivery) zum Erstellen eines Versands
1. [Weitere Informationen](#select-audience) zum Definieren einer Zielgruppe
1. [Weitere Informationen](#edit-content) zum Bearbeiten des Inhalts
1. [Weitere Informationen](#preview-send) zum Anzeigen einer Vorschau und zum Senden eines Versands

## Erstellen des benutzerdefinierten externen Kanals{#create-channel}

Zunächst müssen Sie den benutzerdefinierten externen Kanal konfigurieren. Im Folgenden finden Sie die wichtigsten Schritte, die in der Client-Konsole ausgeführt werden müssen:

1. Konfigurieren Sie das Schema, um den neuen Kanal zur Liste der verfügbaren Kanäle hinzuzufügen.
1. Erstellen Sie ein neues externes Routing-Konto.
1. Erstellen Sie eine neue Versandvorlage, die mit dem neuen Kanal verknüpft ist.

Weitere Informationen finden Sie in der [Dokumentation zur Client-Konsole](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html?lang=de).

## Erstellen des Versands{#create-delivery}

Führen Sie die folgenden Schritte aus, um den Versand zu erstellen und seine Eigenschaften zu konfigurieren:

1. Wählen Sie das Menü **[!UICONTROL Sendungen]** aus und klicken Sie auf die Schaltfläche **[!UICONTROL Versand erstellen]**.

1. Wählen Sie den gewünschten benutzerdefinierten externen Kanal und die zugehörige Vorlage aus. Klicken Sie dann zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![Screenshot zur Erstellung eines benutzerdefinierten Versands](assets/cus-create.png){zoomable="yes"}


1. Geben Sie unter **[!UICONTROL Eigenschaften]** ein **[!UICONTROL Label]** für den Versand ein. 

   ![Screenshot zur Konfiguration der Eigenschaften für einen benutzerdefinierten Versand](assets/cus-properties.png){zoomable="yes"}

Weitere Informationen zum Erstellen eines Versands finden Sie in der [Dokumentation](../call-center/create-call-center.md#create-delivery) zum Callcenter.

## Definieren der Zielgruppe{#select-audience}

Definieren Sie nun die Zielgruppe für die Extraktionsdatei.

1. Klicken Sie im Abschnitt **[!UICONTROL Zielgruppe]** der Versandseite auf **[!UICONTROL Zielgruppe auswählen]**.

1. Wählen Sie eine vorhandene Zielgruppe oder erstellen Sie eine eigene.

   ![Screenshot zur Zielgruppenauswahl für einen benutzerdefinierten Versand](assets/cc-audience2.png){zoomable="yes"}

Weitere Informationen zum Definieren von Zielgruppen finden Sie in der [Dokumentation](../call-center/create-call-center.md#select-audience) zum Callcenter.

## Bearbeiten des Inhalts{#edit-content}

Nun wird der Inhalt der Extraktionsdatei bearbeitet, die im Rahmen des Versands über den benutzerdefinierten Kanal generiert wird.

1. Klicken Sie auf der Versandseite auf die Schaltfläche **[!UICONTROL Inhalt bearbeiten]**.

1. Geben Sie einen **[!UICONTROL Dateinamen]** an, wählen Sie ein **[!UICONTROL Dateiformat]** aus und fügen Sie so viele Spalten hinzu, wie Sie für Ihre Extraktionsdatei benötigen.

   ![Screenshot mit den Konfigurationsoptionen für Attribute für die Extraktionsdatei](assets/cc-content-attributes.png)

Weitere Informationen zum Bearbeiten von Inhalten finden Sie in der [Dokumentation](../call-center/create-call-center.md#edit-content) zum Callcenter.

## Vorschau und Durchführen des Versands{#preview-send}

Wenn der Versandinhalt fertig ist, können Sie ihn mithilfe von Testprofilen in der Vorschau anzeigen und einen Testversand durchführen. Sie können dann den Versand durchführen, um die Extraktionsdatei zu generieren.

1. Klicken Sie auf der Seite mit dem Versandinhalt auf die Schaltfläche **[!UICONTROL Inhalte simulieren]** und wählen Sie „Testprofile“ aus.

   ![Screenshot mit der Option „Inhalte simulieren“ auf der Seite für den Versandinhalt](assets/cus-simulate.png){zoomable="yes"}

1. Klicken Sie auf der Versandseite auf **[!UICONTROL Überprüfen und senden]** und dann auf **[!UICONTROL Vorbereiten]**. Bestätigen Sie anschließend.

   ![Screenshot mit der Option „Vorbereiten“ und dem Menü „Logs“](assets/cus-prepare.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Senden]**, um mit dem endgültigen Sendevorgang fortzufahren, und bestätigen Sie dann.

Weitere Informationen zum Anzeigen in der Vorschau und Senden finden Sie in der [Dokumentation](../call-center/create-call-center.md#preview-send) zum Callcenter.
