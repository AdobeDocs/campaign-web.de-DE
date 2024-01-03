---
title: Arbeiten mit Empfängerinnen bzw. Empfängern und Zielgruppen
description: Erfahren Sie, wie Sie mit Empfängerinnen und Empfängern in Campaign Web arbeiten.
badge: label="Beta"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 93%

---

# Arbeiten mit Empfängerinnen bzw. Empfängern und Zielgruppen {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360 Ansicht Ihrer Empfänger"
>abstract="Erstellen Sie neue Empfängerinnen und Empfänger und überwachen Sie sie mithilfe leistungsstarker Berichte und Tools. Zugriff auf die Attribute, Interaktionen und Protokolle Ihres Empfängers. Verwenden Sie die Filteroptionen, um die Empfängerliste zu durchsuchen, ihr Profil zu bearbeiten und zu aktualisieren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Siehe Versionshinweise"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profile"
>abstract="Ein Profil ist ein Kontakt, der mit den von Adobe Campaign gesendeten Nachrichten angesprochen wird. In Adobe Campaign sind Empfängerinnen und Empfänger die Standardprofile, an die sich Sendungen richten (E-Mails oder SMS). In dieser Liste kann das Empfängerprofil anhand der Berechtigungen angezeigt werden. Die Filteroptionen verwenden, um diese Liste zu durchsuchen. Es kann eine kleine Gruppe von Empfängerattributen bearbeitet und aktualisiert werden."

Eine Empfängerin bzw. ein Empfänger ist ein Profil, das für den Empfang von Nachrichten bestimmt ist, die von Adobe Campaign gesendet werden. In Adobe Campaign sind Empfängerinnen und Empfänger die Standardprofile, an die sich Sendungen richten (E-Mails, SMS usw.). Mit den in der Datenbank gespeicherten Empfängerdaten können Sie die Zielgruppen erstellen, die einen bestimmten Versand erhalten sollen, und Personalisierungsdaten in die Versandinhalte einfügen. In der Datenbank sind weitere Arten von Profilen gespeichert. Sie sind für unterschiedliche Verwendungszwecke konzipiert: Beispielsweise werden Testprofile erstellt, um Ihre Sendungen zu testen, bevor sie an die endgültige Zielgruppe gesendet werden.

Empfängerinnen und Empfänger können nur über die Campaign-Client-Konsole hinzugefügt werden. Sie sind jedoch in Campaign Web über den Eintrag **Empfänger** in der linken Navigationsleiste sichtbar. Sie können die Attribute der Empfängerin bzw. des Empfängers auch von diesem Bildschirm aus bearbeiten.

Um die Empfängerdaten zu bearbeiten, klicken Sie auf die drei Punkte neben einem Namen und wählen Sie **Bearbeiten…**.

![Bearbeiten eines Empfängerprofils](assets/recipient-edit.png)

Sie können einen begrenzten Satz von Attributen aktualisieren, nämlich: Vorname, Nachname, E-Mail-Adresse und Telefonnummer.

![Aktualisieren eines Empfängerprofils](assets/recipient-update.png)

>[!NOTE]
>
>Dieses eingeschränkte Formular zur Profilbearbeitung wird nur für Beta-Programmtests bereitgestellt. Es wird in der zukünftigen Version verbessert. Dadurch kann die Benutzerin bzw. der Benutzer jedem Profil schnell eine E-Mail-Adresse und eine Telefonnummer hinzufügen, damit sie bzw. er die E-Mail- und SMS-Kanäle testen und die gesendeten Nachrichten empfangen kann.

Sie können die Empfängerinnen und Empfänger mithilfe des Suchfelds über die Schaltfläche **Filter anzeigen** filtern.

Sie können über die **Explorer**-Ansicht außerdem auf Empfängerinnen und Empfänger zugreifen, Ordner und Unterordner durchsuchen und erstellen und zugehörige Berechtigungen überprüfen.

![Empfängerliste aus der Explorer-Ansicht](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Abhängig von Ihren Berechtigungen haben Sie möglicherweise keinen Zugriff auf die vollständige Liste der in der Datenbank gespeicherten Empfängerinnen und Empfänger. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](../get-started/permissions.md).

Darüber hinaus können Sie die An- und Abmeldung Ihrer Empfängerinnen und Empfänger für Dienste wie beispielsweise Newsletter verwalten. Auf [dieser Seite](manage-services.md) erfahren Sie, wie Sie mit Anmeldediensten arbeiten

Sie können Workflows erstellen, um Profile zu deduplizieren, anzureichern, zu kombinieren und Zielgruppen zu erstellen. Weiterführende Informationen finden Sie in [diesem Abschnitt](../workflows/gs-workflows.md).
