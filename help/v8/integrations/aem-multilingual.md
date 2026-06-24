---
audience: end-user
title: Erstellen mehrsprachiger E-Mails mit Adobe Experience Manager
description: Erfahren Sie, wie Sie in Campaign Web mehrsprachige E-Mail-Sendungen mit Adobe Experience Manager-Sprachkopien erstellen.
feature: Email
topic: Content Management
role: User
level: Intermediate
exl-id: 6fc6ff43-ac7f-46c7-aa1a-9489ffc45423
TQID: https://experienceleague.adobe.com/t7jTgugTG9NOGwqQ9OMcRCrLcr83sTI5cu-O-iYQsRk
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: d5ef99fa-df0c-4153-bf94-105ad0724167
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 527
ht-degree: 100%

---

# Erstellen mehrsprachiger E-Mails mit Adobe Experience Manager {#aem-multilingual}

Die Adobe Experience Manager-Integration ermöglicht es Ihnen, mehrsprachige E-Mail-Sendungen mit Adobe Experience Manager-Sprachkopien zu erstellen. Auf diese Weise können Sie Inhaltsvarianten in verschiedenen Sprachen verwalten und basierend auf den Voreinstellungen der Empfängersprache personalisierte E-Mails versenden.

## Voraussetzungen {#prerequisites}

Bevor Sie einen mehrsprachigen E-Mail-Versand erstellen, stellen Sie Folgendes sicher:

* Sie haben Zugriff auf eine Adobe Experience Manager-Instanz, die für die Integration der Adobe Campaign Web-Benutzeroberfläche konfiguriert ist.
* Adobe Experience Manager-Inhalte mit Sprachkopien wurden bereits erstellt und genehmigt. Weitere Informationen zum Sprachkopie-Assistenten finden Sie in der [Dokumentation zu Adobe Experience Manager](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard).
* Sie haben eine E-Mail-Versandvorlage, die für den Empfang von Adobe Experience Manager-Inhalten konfiguriert ist. In den Schritten im Abschnitt [Aktivieren des mehrsprachigen Modus](#enable-multilingual) finden Sie weitere Informationen.

## Erstellen eines mehrsprachigen Versands

Um einen mehrsprachigen E-Mail-Versand zu erstellen, müssen Sie zunächst die Option für Mehrsprachigkeit in den Versandeinstellungen aktivieren. Das System erkennt automatisch verfügbare Sprachkopien und ermöglicht die Auswahl der hinzuzufügenden Sprachkopien.

### Aktivieren des mehrsprachigen Modus {#enable-multilingual}

Erstellen Sie einen neuen Versand und aktivieren Sie die Option für Mehrsprachigkeit in den erweiterten Einstellungen.

1. Klicken Sie im Menü **[!UICONTROL Sendungen]** auf **[!UICONTROL Versand erstellen]**.

   ![](assets/lg-copy-1.png)

1. Wählen Sie die Vorlage **[!UICONTROL E-Mail-Versand mit AEM]** und klicken Sie auf **[!UICONTROL Versand erstellen]**.

   ![](assets/lg-copy-2.png)

1. Geben Sie ein Label für den Versand ein und konfigurieren Sie Ihre Zielgruppe. [Weitere Informationen](../email/create-email.md)

1. Rufen Sie die **[!UICONTROL Einstellungen]** für Ihren Versand auf und navigieren Sie dann zum Abschnitt **[!UICONTROL Erweitert]**.

1. Aktivieren Sie die Option **[!UICONTROL Mehrsprachige AEM-Version aktivieren]**.

   ![](assets/lg-copy-3.png)

1. Stellen Sie Folgendes sicher:

   * **[!UICONTROL Inhaltsbearbeitungsmodus]** ist auf **[!UICONTROL AEM]** eingestellt.
   * Das korrekte **[!UICONTROL Externe Konto]** von Adobe Experience Manager ist ausgewählt.

1. Klicken Sie auf **[!UICONTROL Speichern und schließen]**.

### Inhaltsvarianten erstellen {#create-variants}

Wählen Sie Ihre Adobe Experience Manager-Inhalte und die Sprachvarianten aus, die in den Versand aufgenommen werden sollen.

1. Klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**.

1. Wählen Sie **[!UICONTROL Inhaltsvariante erstellen]** aus.

   ![](assets/lg-copy-4.png)

1. Wählen Sie Ihren Adobe Experience Manager-Inhalt aus der Liste aus.

   ![](assets/lg-copy-5.png)

1. Das System erkennt alle Sprachkopien, die mit dem ausgewählten Inhalt verknüpft sind (Beziehung zwischen über- und untergeordneten Elementen). Wenn Ihr Adobe Experience Manager-Inhalt z. B. Varianten auf Französisch, Deutsch und Italienisch aufweist, können alle Varianten ausgewählt werden.

   Wählen Sie die Sprachvarianten aus, die Sie in Ihren Versand aufnehmen möchten.

   ![](assets/lg-copy-6.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

1. Überprüfen Sie Ihre Sprachvarianten im Inhaltseditor. Sie können jetzt [jede Variante einzeln verwalten](#manage-variants) oder [den Versand absenden](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Verwalten von Sprachvarianten {#manage-variants}

Nachdem Sie Inhaltsvarianten erstellt haben, können Sie sie direkt im Versand verwalten:

1. Um eine Standardsprache festzulegen, rufen Sie das erweiterte Menü für Ihre ausgewählte Variante auf und wählen Sie **[!UICONTROL Als Standard festlegen]** aus. Wenn die Spracheinstellung eines Profils nicht festgelegt ist oder mit keiner verfügbaren Variante übereinstimmt, wird die Standardsprache verwendet.

   Klicken Sie auf **[!UICONTROL Löschen]**, um alle Varianten aus Ihrem Versand zu entfernen.

   ![](assets/lg-copy-8.png)

1. Klicken Sie im erweiterten Menü der Inhaltsvarianten auf **[!UICONTROL Gebietsschemata verwalten]**, um weitere Gebietsschemata zu Ihrem Versand hinzuzufügen.

   ![](assets/lg-copy-9.png)

1. Wählen Sie zusätzliche Sprachkopien aus, um weitere Varianten einzuschließen, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/lg-copy-11.png)

1. Wenn der Inhalt in Adobe Experience Manager aktualisiert wird, klicken Sie auf **[!UICONTROL AEM-Inhalt aktualisieren]**, um alle Varianten mit der neuesten Version zu synchronisieren.

   ![](assets/lg-copy-10.png)

1. Klicken Sie auf **[!UICONTROL Verknüpfung von AEM-Inhalt aufheben]**, wenn Sie Inhalte direkt in Campaign bearbeiten oder die Verknüpfung mit Adobe Experience Manager aufheben möchten.

   >[!CAUTION]
   >
   >Nach dem Aufheben der Verknüpfung können Sie Inhalte nicht mehr aus Adobe Experience Manager aktualisieren oder neue Varianten erstellen. Der Inhalt ist dann unabhängig von Adobe Experience Manager.
