---
title: Erstellen eines Profils
description: Erfahren Sie, wie Sie in Campaign Web ein Profil erstellen.
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 100%

---

# Erstellen eines Profils {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Grundlegende Details"
>abstract="Dieser Abschnitt bietet Erkenntnisse über grundlegende Profildetails. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Kontaktinformationen"
>abstract="Dieser Abschnitt bietet Erkenntnisse über die Kontaktinformationen des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Adresse"
>abstract="Dieser Abschnitt Erkenntnisse über die Postanschrift und die Adressenqualität des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Kontodetails"
>abstract="Dieser Abschnitt bietet Erkenntnisse über die Kontodetails des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Nicht mehr kontaktieren"
>abstract="Dieser Abschnitt bietet Erkenntnisse über die Kontakteinstellungen des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Benutzerdefinierte Felder"
>abstract="Benutzerdefinierte Felder sind spezifische Attribute, die auf die Anforderungen des jeweiligen Unternehmens zugeschnitten sind und für seine Instanz konfiguriert wurden. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Sonstige"
>abstract="Dieser Abschnitt enthält zusätzliche integrierte Attribute. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **Speichern**."

Gehen Sie wie folgt vor, um ein Profil zu erstellen:

1. Navigieren Sie zu **[!UICONTROL Kunden-Management]** > **[!UICONTROL Profile]** und klicken Sie oben rechts auf dem Bildschirm auf die Schaltfläche **[!UICONTROL Profil erstellen]**.

1. Die Liste der für die Profilanzeige verfügbaren Attribute, die in verschiedene Abschnitte unterteilt ist, ist in der folgenden Tabelle beschrieben.

   ![Screenshot mit der Liste der für das Profil verfügbaren Attribute, in Abschnitte unterteilt](assets/create-profile.png){zoomable="yes"}

   | Abschnitt „Attribute“ | Beschreibung |
   |  ---  |  ---  |
   | **Grundlegende Details** | Grundlegende Informationen zum Profil, z. B. Name oder Geburtsdatum.<br/>Standardmäßig werden Profile im Ordner **[!UICONTROL Empfänger]** gespeichert. Sie können ihn ändern, indem Sie zum gewünschten Speicherort navigieren. [Erfahren Sie mehr über die Arbeit mit Ordnern](../get-started/permissions.md#folders) |
   | **Kontaktinformationen** | Die Kontaktinformationen des Profils, z. B. die E-Mail-Adresse oder die Telefonnummer. |
   | **Adresse** | Die Postanschrift des Profils. Dieser Abschnitt enthält auch eine Bewertung der Adressqualität. Die Adresse eines Profils gilt als gültig, wenn die Felder „Nachname“, „Ort“ und „Postleitzahl“ angegeben sind. |
   | **Kontodetails** | Informationen zum Konto des Profils, z. B. dessen Status oder Kontonummer. |
   | **Nicht mehr kontaktieren** | Die Kontakteinstellungen des Profils. Wenn eine dieser Optionen ausgewählt ist, befindet sich das Profil auf der Blockierungsliste.<br/>Wenn die Empfängerin bzw. der Empfänger beispielsweise in einem Newsletter auf einen Abmelde-Link geklickt hat, werden diese Informationen zu den Kontaktdaten hinzugefügt. Eine solche Person gehört nicht mehr zur Zielgruppe für die ausgewählten Kanäle. Weitere Informationen zur Quarantäneverwaltung finden Sie in der [Dokumentation zu Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=de){target="_blank"}. |
   | **Benutzerdefinierte Felder** | Wenn benutzerdefinierte Felder konfiguriert wurden, werden sie in diesem Abschnitt angezeigt. Benutzerdefinierte Felder sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zum Schema **[!UICONTROL Profile]** hinzugefügt werden. Weitere Informationen finden Sie in der [Dokumentation zu Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=de){target="_blank"}. |
   | **Sonstige** | Zusätzliche integrierte Attribute. |

1. Nachdem Sie das Profil konfiguriert haben, klicken Sie auf **[!UICONTROL Erstellen]**, um es in der Datenbank zu speichern.

   Danach können Sie das Profil jederzeit bearbeiten, indem Sie es in der Profilliste öffnen. [Erfahren Sie, wie Sie die Profildetails erkunden können](profile-view.md).