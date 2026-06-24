---
audience: end-user
title: Einrichten und Verwalten des Validierungsprozesses
description: Erfahren Sie, wie Sie Genehmigungen von Marketing-Kampagnen in Campaign Web verwalten.
feature: Approvals, Campaigns
exl-id: 8140f904-ec0a-44e1-981f-0e050d3c9cdb
TQID: https://experienceleague.adobe.com/Gpk7fY-VSFdgvgJo2STGjJ8-mHBkVZnp8cD-bFZrWpU
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616a
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 696
ht-degree: 100%

---

# Verwalten des Genehmigungsprozesses {#campaign-approvals}

>[!IMPORTANT]
>
>Validierungen sind nur für Sendungen verfügbar, die innerhalb einer Kampagne erstellt wurden. Dies gilt nicht für eigenständige Sendungen oder Sendungen, die in Workflows außerhalb eines Kampagnenkontexts erstellt wurden.

Der Validierungsprozess hilft, mehrere Stakeholder zu koordinieren, und stellt die Qualitätskontrolle vor dem Versand sicher. Verwenden Sie Validierungen, wenn Ihre Organisation die Validierung durch verschiedene Teams erfordert, z. B. durch das Marketing-Management, das Inhalte überprüft, oder durch das Datenanalyse-Team, das Zielgruppen validiert.

Wenn Validierungen aktiviert sind, müssen Sie Inhalte oder Zielgruppen zur Genehmigung einreichen. Designierte Validierungsverantwortliche erhalten E-Mail-Benachrichtigungen, in denen sie zur Validierung aufgefordert werden, und können diese direkt über die Web-Benutzeroberfläche genehmigen oder ablehnen. Sendungen können erst durchgeführt werden, wenn alle erforderlichen Genehmigungen erteilt wurden. Sie können Folgendes aktivieren:

* **Inhaltsvalidierung**: Validieren von Nachrichteninhalt, Design und Personalisierung
* **Zielgruppenvalidierung**: Validieren der Zielgruppe und der Zielgruppenkriterien
* **Versandbestätigung**: Vor dem Versand ist eine endgültige Bestätigung erforderlich.

## Konfigurieren von Validierungseinstellungen {#configure-approvals}

Validierungseinstellungen werden von der Kampagnenvorlage übernommen und können für einzelne Kampagnen geändert werden. Gehen Sie wie folgt vor, um die Validierungseinstellungen zu konfigurieren:

1. Öffnen Sie Ihre Kampagne oder Kampagnenvorlage oder erstellen Sie eine neue Kampagne über das Menü **[!UICONTROL Kampagnen]**.

1. Klicken Sie rechts oben im Kampagnen-Dashboard auf die Schaltfläche **[!UICONTROL Einstellungen]**.

1. Konfigurieren Sie im Abschnitt **[!UICONTROL Genehmigungen]** die beiden folgenden Optionen:

   ![Screenshot der Einstellungen zur Kampagnengenehmigung](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Inhaltsgenehmigung aktivieren]**: Bei Aktivierung muss der Versandinhalt vor dem Versand genehmigt werden. Klicken Sie auf das Ordnersymbol im Feld **[!UICONTROL Zu validieren von]**, um eine Person oder eine Benutzergruppe auszuwählen.

   * **[!UICONTROL Zielgruppengenehmigung aktivieren]** Wenn diese Option aktiviert ist, muss die Zielgruppe des Versands genehmigt werden. Klicken Sie auf das Ordnersymbol im Feld **[!UICONTROL Zu validieren von]**, um eine Person oder eine Benutzergruppe auszuwählen.

   * **[!UICONTROL Versand vor dem Senden bestätigen]**: Erfordert eine letzte manuelle Bestätigung vor dem Senden, selbst nachdem alle anderen Genehmigungen erfolgt sind.

>[!NOTE]
>
>* Wenn keine prüfende Person angegeben ist, wird die Kampagneneigentümerin bzw. der Kampagneneigentümer als prüfende Person zugewiesen.
>* Prüfende benötigen entsprechende Berechtigungen, um Sendungen zu genehmigen. Nur in der Liste der Prüfenden identifizierte Benutzende können genehmigen.

## Zur Validierung unterbreiten {#submit-approval}

Führen Sie nach der Erstellung des Versands die folgenden Schritte aus, um den Inhalt und die Zielgruppe zur Genehmigung einzureichen.

>[!NOTE]
>Genehmigungen sind sowohl in Kampagnen-Workflow-Sendungen als auch in eigenständigen Kampagnen-Sendungen verfügbar.

1. Klicken Sie im Versand-Dashboard auf die Schaltfläche **[!UICONTROL Inhalte übermitteln]**. Designierte Prüfende können genehmigen oder ablehnen. Weitere Informationen finden Sie in diesem [Abschnitt](#approve-reject).

   ![Screenshot der Schaltfläche „Inhalte übermitteln“](assets/approvals2.png){zoomable="yes"}

   Der Genehmigungsstatus ändert sich im Abschnitt **[!UICONTROL Eigenschaften]** des Versand-Dashboards in „Ausstehend“. Weitere Informationen finden Sie in diesem [Abschnitt](#rack-approvals).

1. Nachdem der Inhalt genehmigt wurde, klicken Sie auf die Schaltfläche **[!UICONTROL Vorbereiten]**, um das Versandziel vorzubereiten. Das System bereitet die Zielgruppen- und Zielgruppenkriterien vor.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe übermitteln]**. Designierte Prüfende können anschließend genehmigen oder ablehnen. Weitere Informationen finden Sie in diesem [Abschnitt](#approve-reject).

   ![Screenshot der Schaltfläche „Zielgruppe übermitteln“](assets/approvals5.png){zoomable="yes"}

   Der Genehmigungsstatus ändert sich in „Ausstehend“. Weitere Informationen finden Sie in diesem [Abschnitt](#rack-approvals).

1. Sobald die Zielgruppe genehmigt wurde, wird die Vorbereitung fortgesetzt und der Versand kann durchgeführt werden.

>[!NOTE]
>Wird eine Genehmigung abgelehnt, muss die Eigentümerin bzw. der Eigentümer des Versands alle erforderlichen Änderungen am Inhalt oder an der Zielgruppe vornehmen, die auf dem Feedback der prüfenden Person basieren, und den Versand erneut zur Genehmigung einreichen.

## Genehmigen oder ablehnen {#approve-reject}

Designierte prüfende Personen können Übermittlungen von Inhalten und Zielgruppen genehmigen oder ablehnen. Weitere Informationen finden Sie in diesem [Abschnitt](#submit-approval).

>[!NOTE]
>Damit die E-Mail-Benachrichtigung gesendet werden kann, muss die Adresse der prüfenden Person in der Instanz konfiguriert werden.

1. Wenn Sie die Benachrichtigungs-E-Mail erhalten, öffnen Sie den Versand, für den eine Genehmigung erforderlich ist, direkt über die Web-Benutzeroberfläche.

1. Überprüfen Sie die Inhalts- oder Zielinformationen.

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Inhalt genehmigen]** oder **[!UICONTROL Zielgruppe genehmigen]**.

   ![Screenshot der Schaltfläche „Inhalt genehmigen“ im Versand-Dashboard](assets/approvals3.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]**.

1. Fügen Sie optional einen **[!UICONTROL Kommentar]** hinzu, um Ihre Entscheidung zu erklären.

   ![Screenshot des Genehmigungs-Dialogfelds mit den Schaltflächen „Genehmigen“ und „Ablehnen“ und dem Feld „Kommentar“](assets/approvals4.png){zoomable="yes"}

1. Bestätigen Sie Ihre Entscheidung. Der Genehmigungsstatus wird sofort im Versand-Dashboard aktualisiert. Weitere Informationen finden Sie in diesem [Abschnitt](#rack-approvals).

## Nachverfolgen des Genehmigungsstatus {#track-approvals}

Der Genehmigungsstatus wird im Abschnitt **[!UICONTROL Eigenschaften]** des Versand-Dashboards angezeigt. Der Status zeigt an, welche Genehmigungen ausstehen und wie der aktuelle Status lautet:

![Screenshot mit Genehmigungsstatus](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL In Bearbeitung]**: Der Inhalt oder die Zielgruppe wurde noch nicht zur Genehmigung eingereicht
* **[!UICONTROL Genehmigung ausstehend]**: Der Inhalt oder die Zielgruppe wartet auf Überprüfung
* **[!UICONTROL Genehmigt]**: Der Inhalt oder die Zielgruppe wurde von der prüfenden Person genehmigt
* **[!UICONTROL Abgelehnt]**: Der Inhalt oder die Zielgruppe wurde von der prüfenden Person abgelehnt

Der Abschnitt „Genehmigung“ zeigt alle aktivierten Genehmigungen und Aktualisierungen in Echtzeit an, während die prüfenden Personen die einzelnen Schritte genehmigen oder ablehnen.

## Verwandte Themen {#related}

* [Erstellen von Kampagnen](create-campaigns.md)
* [Verwalten von Kampagnen](manage-campaigns.md)
