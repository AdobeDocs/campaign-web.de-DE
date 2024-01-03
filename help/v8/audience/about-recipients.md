---
title: Profile überwachen und verwalten
description: Erfahren Sie, wie Sie Profile im Campaign Web überwachen und verwalten.
badge: label="Eingeschränkte Verfügbarkeit"
source-git-commit: 41c38ff3b18c28fbcb6fd07dd398600a207f53cb
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 9%

---

# Profile überwachen und verwalten {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360-Grad-Ansicht Ihrer Profile"
>abstract="Erstellen Sie neue Profile und überwachen Sie sie mithilfe leistungsstarker Berichte und Tools. Greifen Sie auf die Attribute, Interaktionen und Protokolle Ihrer Profile zu. Verwenden Sie die Filteroptionen, um die Profilliste zu durchsuchen, ihr Profil zu bearbeiten und zu aktualisieren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profile"
>abstract="Ein Profil ist ein Kontakt, der mit den von Adobe Campaign gesendeten Nachrichten angesprochen wird. In dieser Liste können Sie die Details der Profile anhand Ihrer Berechtigungen anzeigen. Die Filteroptionen verwenden, um diese Liste zu durchsuchen. Sie können eine kleine Gruppe von Profilattributen bearbeiten und aktualisieren."

## Erste Schritte mit Profilen {#gs}

Ein Profil im Adobe Campaign Web ist eine in der Datenbank gespeicherte Person, die als Schlüsselkomponente dient, um Zielgruppen für Sendungen zu erstellen und Ihrem Inhalt Personalisierungsdaten hinzuzufügen. Verschiedene Typen von Profilen werden in der Datenbank gespeichert, z. B. Testprofile, mit denen Ihre Sendungen getestet werden können, bevor sie an die endgültige Audience gesendet werden. [Erfahren Sie, wie Sie mit Testprofilen arbeiten.](test-profiles.md)

Profile können nur über die Campaign-Clientkonsole hinzugefügt werden. Sie sind jedoch im Adobe Campaign Web über die **Profile** in der linken Navigationsleiste. Sie können auch über die **Explorer** Ansicht, in der Sie die zugehörigen Berechtigungen durchsuchen, Ordner erstellen und Unterordner anzeigen können.

Sie können die Profilliste mithilfe des Suchfelds filtern oder die in der **Filter anzeigen** Schaltfläche.

![](assets/profiles-list.png)

>[!NOTE]
>
>Abhängig von Ihren Berechtigungen haben Sie möglicherweise keinen Zugriff auf die vollständige Liste der in der Datenbank gespeicherten Profile. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](../get-started/permissions.md).

## Profilattribute aufrufen und bearbeiten {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Grundlegende Details"
>abstract="Dieser Abschnitt bietet Einblicke in die grundlegenden Details des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Kontaktinformationen"
>abstract="Dieser Abschnitt bietet Einblicke in die Kontaktinformationen des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Adresse"
>abstract="Dieser Abschnitt bietet Einblicke in die Postanschrift des Profils und die Adressenqualität. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Kontodetails"
>abstract="Dieser Abschnitt bietet Einblicke in die Kontodetails des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Empfänger – Nicht mehr kontaktieren"
>abstract="Dieser Abschnitt bietet Einblicke in die Kontakteinstellungen des Profils. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Benutzerdefinierte Felder"
>abstract="Benutzerdefinierte Felder sind spezifische Attribute, die auf Ihre Anforderungen zugeschnitten sind und für Ihre Instanz konfiguriert wurden. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Sonstige"
>abstract="Dieser Abschnitt enthält zusätzliche integrierte Attribute. Um Informationen zu ändern, nehmen Sie die gewünschten Änderungen direkt im entsprechenden Feld vor und klicken Sie auf **Speichern** -Schaltfläche in der oberen rechten Ecke des Bildschirms."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Emfänger – Abonnementliste"
>abstract="Auf diesem Tab werden alle Dienste aufgelistet, für die das Profil angemeldet ist."

Um auf die Details eines Profils zuzugreifen, klicken Sie auf dessen Namen in der Profilliste.

![](assets/profiles-details.png)

Auf diesem Bildschirm können Sie auf detaillierte Informationen zum Profil zugreifen:

* Die **[!UICONTROL Details]** -Registerkarte können Sie die integrierten und benutzerdefinierten Attribute des Profils durchsuchen. Um ein Attribut zu bearbeiten, nehmen Sie Änderungen im gewünschten Feld vor und klicken Sie auf die Schaltfläche **[!UICONTROL Speichern]** Schaltfläche.
* Die **[!UICONTROL Abonnements]** enthält Informationen zu den Diensten, für die das Profil angemeldet ist. [Erfahren Sie, wie Sie mit Anmeldediensten arbeiten können](manage-services.md)
* Die **[!UICONTROL Protokolle]** über die Schaltfläche rechts oben im Bildschirm können Sie einen Verlauf der Interaktionen des Profils anzeigen, indem Sie Versand-, Ausschluss- und Trackinglogs sowie die dem Profil vorgeschlagenen Vorschläge anzeigen.
