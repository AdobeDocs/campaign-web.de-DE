---
audience: end-user
title: Hinzufügen einer bearbeitbaren Liste zum Angebotsschema
description: Erfahren Sie, wie Sie einen benutzerdefinierten Sammlungs-Link als bearbeitbare Liste direkt im Detailbildschirm des Angebots anzeigen können.
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: ht
source-wordcount: 449
ht-degree: 100%

---

# Hinzufügen einer bearbeitbaren Liste zum Angebotsschema {#offer-editable-list}

Wenn Sie das [ [!DNL nms:offer] Schema](../administration/schemas.md) mit einem benutzerdefinierten Sammlungs-Link erweitern, z. B. mit einer Reihe von Segmenten, die mit einem Angebot verknüpft sind, können Sie es direkt im Abschnitt **[!UICONTROL Benutzerdefinierte Optionen]** des Angebots als bearbeitbare Liste anzeigen. Anstatt die zugehörigen Einträge über einen separaten Bildschirm zu verwalten, wird die Sammlung als Liste in den Angebotsdetails gerendert, und Sie können neue zugehörige Einträge direkt über ein spezielles Dialogfeld erstellen.

>[!NOTE]
>
>Diese Funktion ist derzeit nur für das Angebotsschema verfügbar.

## Hinzufügen eines Sammlungs-Link-Felds {#add-field}

1. Erweitern Sie das [!DNL nms:offer]-Schema mit Ihrer benutzerdefinierten Sammlung, navigieren Sie zum Menü **[!UICONTROL Schemata]**, öffnen Sie das Schema **[!UICONTROL Marketing-Angebote]** und klicken Sie auf **[!UICONTROL Bildschirmbearbeitung]**. [Weitere Informationen](../administration/schemas-browse-access.md#screen-def).

   ![Screenshot mit der Schaltfläche „Bildschirmdefinition“.](assets/offers-editable-list.png){zoomable="yes"}

1. Klicken Sie im Abschnitt **[!UICONTROL Konfiguration des Detailbildschirms]** auf das Symbol mit den Auslassungspunkten über der Tabelle **[!UICONTROL Liste der benutzerdefinierten Felder]** und wählen Sie **[!UICONTROL Attribute auswählen]** aus. [Weitere Informationen](../administration/schemas-custom-fields.md).

   ![Screenshot der Schaltfläche „Bildschirmdefinition“.](assets/offers-editable-list-0.png){zoomable="yes"}

1. Durchsuchen Sie die Attribute und wählen Sie Ihren benutzerdefinierten Sammlungs-Link aus, der durch das Sammlungssymbol gekennzeichnet ist.

   ![Screenshot der Attributauswahl mit einem Sammlungs-Link-Attribut.](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >Sammlungs-Link-Felder können nicht als Pflichtfelder festgelegt werden und unterstützen keine Unterattribute. Standardmäßig erstrecken sie sich über zwei Spalten im Formular.

1. Bestätigen Sie Ihre Auswahl. Der Sammlungs-Link wird der Tabelle **[!UICONTROL Liste der benutzerdefinierten Felder]** hinzugefügt, wobei **[!UICONTROL collection]** der Typ ist.

   ![Screenshot der hinzugefügten Attribute.](assets/offers-editable-list-2.png){zoomable="yes"}

## Konfigurieren der bearbeitbaren Liste der Sammlung {#configure-list}

1. Klicken Sie auf das Symbol mit den Auslassungspunkten in der Zeile des Sammlungsfelds und wählen Sie **[!UICONTROL Bearbeiten]** aus, um das Dialogfeld **[!UICONTROL Einstellungen für Sammlungs-Links]** zu öffnen.

   ![Screenshot der Bearbeitungsschaltfläche.](assets/offers-editable-list-3.png){zoomable="yes"}

1. Legen Sie auf der Registerkarte **[!UICONTROL Allgemein]** optional die Bedingung **[!UICONTROL In folgenden Fällen sichtbar]** fest oder aktivieren Sie die Option **[!UICONTROL Schreibgeschützt]**.

   ![Screenshot des Bearbeitungsbildschirms.](assets/offers-editable-list-4.png){zoomable="yes"}

1. Klicken Sie auf der Registerkarte **[!UICONTROL Bildschirmkonfiguration]** auf **[!UICONTROL Attribute auswählen]** und wählen Sie die Attribute aus, die beim Hinzufügen eines neuen Elements zur Liste verwendet werden sollen, z. B. einen Segmentnamen und ein benutzerdefiniertes Feld.

   ![Screenshot der Registerkarte für die Bildschirmkonfiguration des Dialogfelds für Sammlungs-Link-Einstellungen.](assets/offers-editable-list-5.png){zoomable="yes"}

1. Auf der Registerkarte **[!UICONTROL Layout]** können Sie die Option **[!UICONTROL Zwei Spalten umfassen]** aktivieren oder deaktivieren.

1. Wählen Sie **[!UICONTROL Bestätigen]** und danach **[!UICONTROL Speichern]** für die Bildschirmdefinition aus.

## Verwenden der bearbeitbaren Liste in einem Angebot {#use-list}

1. Klicken Sie im linken Menü auf **Angebote** und öffnen Sie ein Angebot. [Weitere Informationen](create-offer.md#create)

   ![Screenshot des Angebotsbildschirms.](assets/offers-editable-list-7.png){zoomable="yes"}

1. Öffnen Sie die Angebotseigenschaften. Die Sammlung wird als Liste im Abschnitt **Benutzerdefinierte Optionen** gerendert.

   ![Screenshot, der die Darstellung der bearbeitbaren Liste im Bildschirm mit den Angebotsdetails zeigt.](assets/offers-editable-list-6.png){zoomable="yes"}

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**, um die konfigurierten Attribute anzuzeigen, füllen Sie sie aus und klicken Sie auf **[!UICONTROL Bestätigen]**. Das neue Element wird der Liste hinzugefügt.

   Sie können derselben Liste mehrere Elemente hinzufügen, und die Angebotsdetails können mehr als eine bearbeitbare Liste enthalten.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->