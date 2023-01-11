---
audience: end-user
title: Hinzufügen einer Audience
description: Web-Dokumentation zu Campaign v8
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 6d678442c0fe396f45a635c60837932f424d0763
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 86%

---

# Auswählen einer Audience {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Auswählen einer bestehenden Audience"
>abstract="Die Audiences werden in der Adobe Campaign v8-Konsole definiert. Wenn Sie über eine Adobe Experience Platform-Integration verfügen, sollten Sie auch in Platform definierte Audiences anzeigen können."

>[!NOTE]
>
>Diese Dokumentation wird derzeit erstellt und häufig aktualisiert. Die endgültige Version dieses Inhalts wird im Januar 2023 vorliegen.

In diesem Abschnitt wird beschrieben, wie Sie bei der Definition der Zielgruppe eines E-Mail-Versands eine bestehende Audience auswählen. Weiterführende Informationen zur Erstellung einer neuen Audience finden Sie in [diesem Abschnitt](segment-builder.md).

1. Klicken Sie im Abschnitt **Audience** des Assistenten zur Versanderstellung auf die Schaltfläche **[!UICONTROL Audience auswählen]**.

   ![](assets/create-audience.png)

1. Klicken Sie auf **[!UICONTROL Audience auswählen]**, um eine bestehende Audience zu verwenden. Um eine neue Audience zu erstellen, die in dieser E-Mail verwendet werden soll, wählen Sie **Eigene erstellen**. Näheres dazu finden Sie in [diesem Abschnitt](segment-builder.md).

   Auf diesem Bildschirm werden alle bestehenden Audiences angezeigt, die in der Adobe Campaign-Konsole oder durch Adobe Experience Platform definiert sind.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Um Adobe Experience Platform-Zielgruppen zu nutzen, müssen Sie die Integration mit Zielen konfigurieren. Siehe Abschnitt [Dokumentation zu Zielen](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=de).

1. Wählen Sie eine Audience aus und klicken Sie auf **Auswählen**.

1. Klicken Sie auf **Regeln bearbeiten**, wenn Sie Ihre Audience einschränken möchten.

   ![](assets/create-audience3.png)

1. Mithilfe des Regel-Builders können Sie Ihre Zielgruppe mit zusätzlichen Filtern oder durch die Kombination verschiedener Zielgruppen anreichern. Weitere Informationen finden Sie in [diesem Abschnitt](segment-builder.md).

   ![](assets/create-audience4.png)

1. Klicken Sie auf **Speichern**.

Sie können auch eine Kontrollgruppe einrichten, um die Wirkung Ihrer Kampagnen zu messen. Die Kontrollgruppe erhält die Nachricht nicht. Dadurch lässt sich das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen, die die Nachricht nicht erhalten haben. Siehe [diesen Abschnitt](control-group.md).