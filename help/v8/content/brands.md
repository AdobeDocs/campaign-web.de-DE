---
audience: end-user
title: Verwalten einer Marke
description: Erfahren Sie, wie Sie Ihre Markenrichtlinien erstellen und verwalten.
hide: true
hidefromtoc: true
badge: label="Beta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: a62c0277bc6bbc9f6d14fd82c96b1e5cee77c63c
workflow-type: ht
source-wordcount: '455'
ht-degree: 100%

---

# Erstellen und Verwalten Ihrer Marken {#brands}

>[!AVAILABILITY]
>
>Diese Funktion wird als private Betaversion veröffentlicht. Sie wird in zukünftigen Versionen nach und nach allen Kundinnen und Kunden zur Verfügung stehen.

Markenrichtlinien sind ein umfassender Satz von Regeln und Standards, die die visuelle und verbale Identität einer Marke definieren. Sie dienen als Referenz, um eine konsistente Markendarstellung auf allen Marketing- und Kommunikationskanälen sicherzustellen.

In [!DNL Adobe Campaign Web] können Sie Ihre Markeninformationen jetzt manuell eingeben und organisieren oder Dokumente zu Markenrichtlinien hochladen, um die Daten automatisch zu extrahieren.

## Zugriff auf Marken {#generative-access}

Für den Zugriff auf das Menü **[!UICONTROL Marken]** in [!DNL Adobe Campaign Web] müssen Benutzenden die Produktprofile **[!UICONTROL Administrator (admin)]** und **[!UICONTROL Marken-Kit]** zugewiesen werden, damit sie Marken erstellen und verwalten können. Für den schreibgeschützten Zugriff benötigen Benutzende das Produktprofil [!UICONTROL KI-Assistent].

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++  Erfahren Sie, wie Sie markenbezogene Berechtigungen zuweisen.

1. Greifen Sie auf der Startseite der [Admin Console](https://adminconsole.adobe.com/enterprise) auf Ihr Campaign-Produkt zu.

   ![](assets/brands_admin_1.png)

1. Wählen Sie das **[!DNL Product profile]** abhängig von der Berechtigungsstufe aus, die Sie Ihrer Benutzerin oder Ihrem Benutzer gewähren möchten.

   ![](assets/brands_admin_2.png)

1. Klicken Sie zum Zuweisen des ausgewählten Produktprofils auf **[!DNL Add users]**.

   ![](assets/brands_admin_3.png)

1. Geben Sie den Namen, die Benutzergruppe oder die E-Mail-Adresse der Benutzerin oder des Benutzers ein.

1. Klicken Sie zum Anwenden der Änderungen auf **Speichern**.

Für alle Benutzenden, die dieser Rolle bereits zugewiesen sind, werden die Berechtigungen automatisch aktualisiert.

+++

## Erstellen Ihrer Marke {#create-brand-kit}

Gehen Sie wie folgt vor, um Ihre Markenrichtlinien zu erstellen und zu verwalten:

Um Ihre Markenrichtlinie zu erstellen und zu verwalten, können Sie die Details entweder selbst eingeben oder Ihr Dokument mit den Markenrichtlinien hochladen, damit die Informationen automatisch extrahiert werden:


1. Wählen Sie im Menü **[!UICONTROL Content-Management]** die Option **[!UICONTROL Marken]** aus.

1. Klicken Sie im Menü **[!UICONTROL Marken]** auf **[!UICONTROL Marke erstellen]**.

   ![](assets/brands_1.png)

1. Geben Sie einen **[!UICONTROL Namen]** für Ihre Marke ein.

1. Ziehen oder wählen Sie eine Datei, um Ihre Markenrichtlinien hochzuladen und automatisch relevante Markeninformationen zu extrahieren. Klicken Sie auf **[!UICONTROL Marke erstellen]**.

   Der Informationsextraktionsprozess beginnt jetzt. Beachten Sie, dass dieser Vorgang mehrere Minuten dauern kann.

   ![](assets/brands_7.png)

1. Ihre Standards für Content und visuelle Erstellung werden jetzt automatisch ausgefüllt. Durchsuchen Sie die verschiedenen Registerkarten, um die Informationen nach Bedarf anzupassen.

1. Klicken Sie auf der Registerkarte **[!UICONTROL Schreibstil]** auf ![](assets/do-not-localize/Smock_Add_18_N.svg), um eine Richtlinie oder einen Ausschluss einschließlich Beispielen hinzuzufügen.

   ![](assets/brands_2.png)

1. Klicken Sie auf der Registerkarte **[!UICONTROL Visueller Inhalt]** auf ![](assets/do-not-localize/Smock_Add_18_N.svg), um eine weitere Richtlinie oder einen Ausschluss hinzuzufügen.

1. Um ein Bild hinzuzufügen, das die korrekte Verwendung zeigt, wählen Sie **[!UICONTROL Beispiele]** und klicken Sie auf **[!UICONTROL Bild auswählen]**. Sie können auch ein Bild mit falscher Verwendung als Ausschlussbeispiel hinzufügen.

   ![](assets/brands_3.png)

1. Klicken Sie nach der Konfiguration auf **[!UICONTROL Speichern]** und dann auf **[!UICONTROL Veröffentlichen]**, um Ihre Markenrichtlinie im KI-Assistenten verfügbar zu machen.

1. Um Änderungen an Ihrer veröffentlichten Marke vorzunehmen, klicken Sie auf **[!UICONTROL Marke bearbeiten]**.

   >[!NOTE]
   >
   >Dadurch wird eine temporäre Kopie im Bearbeitungsmodus erstellt, die die Live-Version nach der Veröffentlichung ersetzt.

   ![](assets/brands_4.png)

1. Öffnen Sie im Dashboard **[!UICONTROL Marken]** das erweiterte Menü, indem Sie auf das Symbol ![](assets/do-not-localize/Smock_More_18_N.svg) klicken, um Folgendes zu tun:

   * Marke anzeigen
   * Bearbeiten
   * Duplizieren
   * Veröffentlichen
   * Veröffentlichung aufheben
   * Löschen

   ![](assets/brands_5.png)

Ihre Markenrichtlinien sind jetzt über die Dropdown-Liste **[!UICONTROL Marke]** im Menü des KI-Assistenten verfügbar, sodass Inhalte und Assets generiert werden können, die mit Ihren Spezifikationen übereinstimmen. [Erfahren Sie mehr über den KI-Assistenten](../email/generative-gs.md)

![](assets/brands_6.png)
