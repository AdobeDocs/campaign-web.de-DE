---
audience: end-user
title: Erstellen eines SMS-Versands
description: Erfahren Sie, wie Sie SMS mit Adobe Campaign Web erstellen und senden
badge: label="Alpha" type="Positive"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: 0463bc48bcee20b9f97d5b98053b77956dc4ef53
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 100%

---

# Erstellen eines SMS-Versands {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Eigenschaften des SMS-Versands"
>abstract="Die Eigenschaften umfassen die üblichen Versandparameter, nach denen Sie Ihren Versand benennen und klassifizieren können. Wenn Ihr Versand auf einem erweiterten Schema basiert, stehen spezifische Felder für benutzerdefinierte Optionen zur Verfügung."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definieren der SMS-Zielgruppe"
>abstract="Wählen Sie die beste Zielgruppe für Ihre SMS-Nachricht aus."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Auswahl von SMS-Vorlagen"
>abstract="Wählen Sie eine vordefinierte Vorlage aus, um Ihren SMS-Versand zu starten."

1. Klicken Sie auf der **[!UICONTROL Sendungen]**-Startseite auf **[!UICONTROL Versand erstellen]**.

1. Wählen Sie im Abschnitt **[!UICONTROL Kanal]** den Kanal SMS aus und wählen Sie eine Vorlage aus. [Weitere Informationen zu Vorlagen](../msg/delivery-template.md)

1. Klicken Sie zur Bestätigung auf **[!UICONTROL Versand erstellen]**.

   ![](assets/sms_create_1.png)

1. Geben Sie eine **[!UICONTROL Kennzeichnung]** für den Versand ein und greifen Sie auf die Dropdown-Liste **[!UICONTROL Zusätzliche Optionen]** zu.

   +++Konfigurieren Sie die folgenden Einstellungen entsprechend Ihren Anforderungen.
   * **[!UICONTROL Interner Name]**: Weisen Sie dem Versand eine eindeutige Kennung zu.
   * **[!UICONTROL Ordner]**: Speichern Sie den Versand in einem bestimmten Ordner.
   * **[!UICONTROL Versand-Code]**: Verwenden Sie dieses Feld, um Ihre Sendungen basierend auf Ihrer eigenen Namenskonvention zu organisieren.
   * **[!UICONTROL Beschreibung]**: Geben Sie eine Beschreibung für den Versand an.
   * **[!UICONTROL Art]**: Geben Sie die Art der E-Mail zu Klassifizierungszwecken an.
+++

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Zielgruppe auswählen]**, um eine vorhandene Zielgruppe anzusprechen oder eine eigene zu erstellen. [Weitere Informationen](../audience/about-audiences.md).

   ![](assets/sms_create_2.png)

1. Schalten Sie die Gruppenoption **[!UICONTROL Kontrollgruppe aktivieren]** ein, um zur Messung der Wirkung Ihres Versands eine Kontrollgruppe einzurichten, durch die Sie das Verhalten der Population, die die Nachricht erhalten hat, mit dem Verhalten der Kontakte vergleichen können, die die Nachricht nicht erhalten haben. [Weitere Informationen](../audience/control-group.md)

1. Klicken Sie auf **[!UICONTROL Inhalt bearbeiten]**, um mit der Erstellung des Inhalts Ihrer SMS-Nachricht zu beginnen.

1. Um den Versand für ein bestimmtes Datum und eine bestimmte Uhrzeit zu planen, aktivieren Sie die Option **[!UICONTROL Zeitplan aktivieren]**. Nachdem der Versand initiiert wurde, wird die Nachricht automatisch an dem Datum und zu der Uhrzeit gesendet, die Sie für die Empfängerin bzw. den Empfänger festgelegt haben.
