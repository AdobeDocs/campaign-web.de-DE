---
audience: end-user
title: Verwalten einer Marke
description: Erfahren Sie, wie Sie Ihre Markenrichtlinien erstellen und verwalten.
hide: true
hidefromtoc: true
badge: label="Beta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 41%

---

# Erstellen und Verwalten Ihrer Marken {#brands}

>[!AVAILABILITY]
>
>Diese Funktion wird als private Betaversion veröffentlicht. Sie wird in kommenden Versionen schrittweise für alle Kunden verfügbar sein.

Markenrichtlinien sind ein umfassender Satz von Regeln und Standards, die die visuelle und verbale Identität einer Marke definieren. Sie dienen als Referenz, um eine konsistente Markendarstellung auf allen Marketing- und Kommunikationskanälen sicherzustellen.

In [!DNL Adobe Campaign Web] können Benutzer Markeninformationen manuell eingeben und organisieren oder Dokumente zu Markenrichtlinien hochladen, um die Daten automatisch zu extrahieren.

## Zugriff auf Marken {#generative-access}

Um auf das Menü **[!UICONTROL Marken]** in [!DNL Adobe Campaign Web] zugreifen zu können, müssen Benutzenden die Produktprofile **[!UICONTROL Administrator (]**) und **[!UICONTROL Brand Kit]** zugewiesen werden, um Marken zu erstellen und zu verwalten. Für den schreibgeschützten Zugriff benötigen Benutzende das Produktprofil [!UICONTROL KI]Assistent“.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Erfahren Sie, wie Sie markenbezogene Berechtigungen zuweisen

1. Greifen Sie auf der Startseite der [Admin Console](https://adminconsole.adobe.com/enterprise) auf Ihr Campaign-Produkt zu.

   ![Admin Console-Startseite mit Campaign-Produktzugriff](assets/brands_admin_1.png)

1. Wählen Sie die **[!DNL Product profile]** basierend auf der Berechtigungsstufe aus, die Sie Ihrem Benutzer gewähren möchten.

   ![Produktprofilauswahl in Admin Console](assets/brands_admin_2.png)

1. Klicken Sie zum Zuweisen des ausgewählten Produktprofils auf **[!DNL Add users]**.

   ![Option „Benutzer hinzufügen“ in Admin Console](assets/brands_admin_3.png)

1. Geben Sie den Namen, die Benutzergruppe oder die E-Mail-Adresse Ihres Benutzers ein.

1. Klicken Sie zum Anwenden der Änderungen auf **Speichern**.

Die Berechtigungen von Benutzenden, die dieser Rolle bereits zugewiesen sind, werden automatisch aktualisiert.

+++

## Erstellen Ihrer Marke {#create-brand-kit}

Gehen Sie wie folgt vor, um Ihre Markenrichtlinien zu erstellen und zu verwalten:

Benutzer können die Details entweder manuell eingeben oder ein Dokument mit Markenrichtlinien hochladen, um die Informationen automatisch zu extrahieren:

1. Wählen Sie im Menü **[!UICONTROL Content-Management]** die Option **[!UICONTROL Marken]** aus.

1. Klicken Sie im Menü **[!UICONTROL Marken]** auf **[!UICONTROL Marke erstellen]**.

   ![Menü „Marken“ mit der Option „Marke erstellen“](assets/brands_1.png)

1. Geben Sie einen **[!UICONTROL Namen]** für Ihre Marke ein.

1. Datei per Drag-and-Drop ziehen oder auswählen, um Ihre Markenrichtlinien hochzuladen und relevante Markeninformationen automatisch zu extrahieren. Klicken Sie auf **[!UICONTROL Marke erstellen]**.

   Der Informationsextraktionsprozess beginnt. Beachten Sie, dass dieser Vorgang mehrere Minuten dauern kann.

   ![Datei-Upload für die Extraktion der Markenrichtlinien](assets/brands_7.png)

1. Ihre Standards für Inhalt und visuelle Erstellung werden automatisch ausgefüllt. Durchsuchen Sie die verschiedenen Registerkarten, um die Informationen nach Bedarf anzupassen.

1. Klicken Sie auf der **[!UICONTROL Schreibstil]** auf ![Symbol hinzufügen](assets/do-not-localize/Smock_Add_18_N.svg), um eine Richtlinie oder einen Ausschluss einschließlich Beispiele hinzuzufügen.

   ![Registerkarte „Schreibstil“ mit der Option „Richtlinie hinzufügen“](assets/brands_2.png)

1. Klicken Sie auf der Registerkarte **[!UICONTROL Visueller Inhalt]** auf ![Symbol hinzufügen](assets/do-not-localize/Smock_Add_18_N.svg), um eine weitere Richtlinie oder einen Ausschluss hinzuzufügen.

1. Um ein Bild hinzuzufügen, das die korrekte Verwendung zeigt, wählen Sie **[!UICONTROL Beispiele]** und klicken Sie auf **[!UICONTROL Bild auswählen]**. Sie können auch ein Bild mit falscher Verwendung als Ausschlussbeispiel hinzufügen.

   ![Registerkarte „Visueller Inhalt“ mit Beispielbildoptionen](assets/brands_3.png)

1. Klicken Sie nach der Konfiguration auf **[!UICONTROL Speichern]** und dann auf **[!UICONTROL Veröffentlichen]**, um Ihre Markenrichtlinie im KI-Assistenten verfügbar zu machen.

1. Um Ihre veröffentlichte Marke zu ändern, klicken Sie auf **[!UICONTROL Marke bearbeiten]**.

   >[!NOTE]
   >
   >Dadurch wird eine temporäre Kopie im Bearbeitungsmodus erstellt, die die Live-Version nach der Veröffentlichung ersetzt.

   ![Option „Marke bearbeiten“ im Menü „Marken“](assets/brands_4.png)

1. Öffnen Sie im Dashboard **[!UICONTROL Marken]** das erweiterte Menü, indem Sie auf das Symbol ![Weitere Optionen](assets/do-not-localize/Smock_More_18_N.svg) klicken, um:

   * Marke anzeigen
   * Bearbeiten
   * Duplizieren
   * Veröffentlichen
   * Veröffentlichung aufheben
   * Löschen

   ![Erweiterte Menüoptionen im Marken-Dashboard](assets/brands_5.png)

Ihre Markenrichtlinien sind jetzt über die Dropdown-Liste **[!UICONTROL Marke]** im Menü KI-Assistent verfügbar. Dadurch kann der KI-Assistent Inhalte und Assets generieren, die mit Ihren Spezifikationen übereinstimmen. [Erfahren Sie mehr über den KI-Assistenten](../email/generative-gs.md)

![KI-Assistenten-Menü mit Dropdown-Liste „Marke“](assets/brands_6.png)