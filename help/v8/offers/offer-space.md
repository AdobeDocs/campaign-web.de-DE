---
audience: end-user
title: Erstellen und Verwalten von Platzierungen
description: Erfahren Sie, wie Sie Platzierungen in Campaign Web erstellen, konfigurieren, bereitstellen und in der Vorschau anzeigen.
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 921
ht-degree: 0%

---

# Erstellen und Verwalten von Platzierungen {#offer-space}

Eine **Platzierung** definiert, wo und wie ein Angebot einem Kontakt angezeigt wird: welchen Kanal es verwendet (E-Mail, Briefpost, SMS, eingehendes Web usw.), welche Inhaltsfelder das Angebot verwenden kann und wie die endgültige Darstellung erstellt wird. Eine Umgebung kann mehrere Platzierungen enthalten - eine für jeden Ausstellungspunkt.

Eine Platzierung ist kein Kanal an sich. Es stellt eine bestimmte Position dar, an der das Angebot auf einem Kanal angezeigt wird. Zwei Banner auf derselben Web-Seite entsprechen in der Regel zwei verschiedenen Platzierungen. Das vollständige Konzeptmodell finden Sie in der Dokumentation zu [ v8 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}.

## Platzierung erstellen oder ändern{#create-offer-space}

Platzierungen werden im Ordner der Angebotsumgebung gespeichert. Um die auf Ihrer Plattform verfügbaren Platzierungen zu durchsuchen, öffnen Sie den **[!UICONTROL Explorer]**, navigieren Sie zur Angebotsumgebung und wählen Sie den Unterordner aus, der sie enthält.

![Screenshot der Platzierungsliste.](assets/offers-space.png){zoomable="yes"}

Dort können Sie eine vorhandene Platzierung öffnen oder durch Klicken auf „Platzierung erstellen **[!UICONTROL eine neue]** erstellen.

![Screenshot mit dem Bildschirm für die Platzierung.](assets/offers-space-1.png){zoomable="yes"}

### Definieren der Eigenschaften {#properties}

In diesem Abschnitt haben Sie folgende Möglichkeiten:

* Geben Sie **[!UICONTROL Platzierung]** Titel“ ein.
* Wählen Sie den **[!UICONTROL Kanal]** aus, der dem Expositionspunkt entspricht (E-Mail, Briefpost, SMS, Web usw.).
* Wählen Sie **[!UICONTROL Einzelmodus aktivieren]**, wenn diese Platzierung zusätzlich zu den Massenversand-Aufrufen auch Einzelaufrufe an das Angebotsmodul (Echtzeit, Einzelangebot) unterstützen muss.

### Definieren der Inhaltsfelder {#content-fields}

In den Inhaltsfeldern werden die Attribute aufgelistet, die auf Angebotsebene bearbeitet und von der Rendering-Funktion wiederverwendet werden können. Die Reihenfolge, in der Sie die Felder in der Platzierung hinzufügen, bestimmt die Reihenfolge, in der sie im Abschnitt **[!UICONTROL Inhalt]** verfügbar gemacht werden.

Standardmäßig ist jedes Angebot mit den folgenden vordefinierten Inhaltsfeldern ausgeliefert: **[!UICONTROL Titel]**, **[!UICONTROL Ziel-URL]**, **[!UICONTROL Bild-URL]**, **[!UICONTROL HTML-]** und **[!UICONTROL Text]**. Sie können diese Liste mit jedem benutzerdefinierten Feld erweitern, das Sie für das Rendering benötigen, z. B. **kurzer Inhalt**, eine **getrackte URL** oder jedes Attribut, das über die Schemaerweiterung hinzugefügt wurde.

Klicken Sie **[!UICONTROL Inhaltsfeld hinzufügen]** und wählen Sie dann im Angebotsschema das Attribut aus, das angezeigt werden soll, oder klicken Sie auf **[!UICONTROL Ausdruck bearbeiten]**, um stattdessen einen benutzerdefinierten Ausdruck zu definieren.

>[!IMPORTANT]
>
>Damit ein benutzerdefiniertes Attribut aus dem Abschnitt Angebot **[!UICONTROL Inhalt]** bearbeitet werden kann, muss das Attribut auch im Abschnitt **[!UICONTROL Angebotsinhalt]** des [!DNL nms:offer]-Schemas deklariert werden. Weitere Informationen finden Sie unter [Arbeiten mit Schemata](../administration/schemas.md).

### Rendering-Funktionen konfigurieren {#rendering}

Die Rendering-Funktionen erstellen die endgültige Angebotsdarstellung aus den Inhaltsfeldern. Sie können zwischen dem Standard-Rendering, bei dem der Inhalt einfach unverändert ausgegeben wird, und einer benutzerdefinierten Funktion wählen, die die Felder mit HTML, XML oder Text kombiniert.

Wählen Sie die Registerkarte **[!UICONTROL HTML]**, **[!UICONTROL XML]** oder **[!UICONTROL Text-Rendering]** aus und aktivieren Sie **[!UICONTROL Überschreiben der Rendering-Funktion]**, um sie zu aktivieren.

Verwenden Sie den Ausdruckseditor, um die Rendering-Funktion zu schreiben. Sie können auf die in der Platzierung definierten Inhaltsfelder, die Angebotsattribute und jede beliebige Funktion im [Ausdruckseditor“ ](../query/expression-editor.md).

>[!NOTE]
>
>Wenn keine Rendering-Funktion definiert ist, wird der Angebotsinhalt mit den nativen Attributen unverändert zurückgegeben. Die XML-Rendering-Funktion kann nur verwendet werden, wenn **[!UICONTROL Einzelmodus aktivieren]** in der Platzierung ausgewählt ist.

### Konfigurieren des Speicher- und Vorschlagsstatus {#storage}

In diesem Abschnitt können Sie steuern, wie Vorschläge, die durch diesen Bereich generiert wurden, beibehalten werden und wie sich ihr Status während ihres Lebenszyklus verändert:

* **[!UICONTROL Einfügen von Vorschlägen deaktivieren]** - Verhindert, dass über diese Platzierung erstellte Vorschläge in die Vorschlagstabelle eingefügt werden.

* **[!UICONTROL Status]** bei Vorschlag - Status, der auf den Vorschlag angewendet wird, sobald das Angebotsmodul ihn zurückgibt (normalerweise **[!UICONTROL Unterbreitet]** bei ausgehenden Sendungen).

* **[!UICONTROL Status]** bei Annahme - Status, der angewendet wird, wenn der Empfänger mit dem Angebot interagiert (normalerweise **[!UICONTROL Akzeptiert]**).

Die verfügbaren Statuswerte entsprechen der von der Client-Konsole verwendeten Liste. Weitere Informationen finden Sie in der [ zu Campaign v8 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"} der Konsolendokumentation.

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### Konfigurieren der erweiterten Einstellungen {#advanced}

In diesem Abschnitt können Sie die &quot;**[!UICONTROL &quot;]**. Klicken Sie auf **[!UICONTROL Hinzufügen]** und wählen Sie ein oder mehrere **[!UICONTROL Empfänger]**-Attribute aus oder klicken Sie **[!UICONTROL Ausdruck bearbeiten]**, um stattdessen einen benutzerdefinierten Ausdruck zu definieren. Diese Einstellung ist für eine einfache Platzierung optional. Die vollständigen Informationen und das Verhalten finden Sie in der [ zu Campaign v8 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}.

Platzierungen, die im **eingehenden Web-Kanal** erstellt wurden, erfordern außerdem, dass die Website so konfiguriert ist, dass das Angebot angezeigt und das Angebotsmodul aufgerufen wird. Diese Integration erfolgt in der Client-Konsole - siehe [Angebote in Echtzeit ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"} und [Integration des Angebotsmoduls konfigurieren](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"} in der Dokumentation zu Campaign v8.

## Platzierung bereitstellen {#deploy}

Eine Platzierung muss bereitgestellt werden, bevor sie in einem Versand verwendet werden kann. Platzierung speichern und auf „Bereitstellen **** klicken Der Status der Bereitstellung wird in der Platzierung angezeigt.

![Screenshot zur Bereitstellung des Angebots.](assets/offers-space-2.png){zoomable="yes"}

## Vorschau der Platzierung {#preview}

In der Vorschau können Sie simulieren, wie ein Angebot für eine bestimmte Zielgruppe ausgewählt und gerendert wird.

1. Wählen Sie in der Platzierung die Registerkarte **[!UICONTROL Vorschau]** neben **[!UICONTROL Übersicht]**.

   ![Screenshot der Angebotsvorschau.](assets/offers-space-3.png){zoomable="yes"}

1. Wählen Sie ein Zielprofil aus und starten Sie die Vorschau. Die übereinstimmenden Angebote werden mit der von der Rendering-Funktion erstellten Darstellung zurückgegeben.

>[!NOTE]
>
>Wenn keine Vorschläge zurückgegeben werden, überprüfen Sie die Eignungsregeln der Angebote und die Konfiguration der Platzierung.

Als Nächstes [ Sie im ](create-offer.md) ein Angebot erstellen und es dieser Platzierung zuweisen.
