---
title: Arbeiten mit Empfängern und Zielgruppen
description: Erfahren Sie, wie Sie mit Empfängern im Campaign-Web arbeiten.
badge: label="Beta"
source-git-commit: 269cbb51f070b0f9f771691497ffa07bb94e2d49
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 19%

---


# Arbeiten mit Empfängern und Zielgruppen {#about-recipients}

## Empfänger {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Empfänger"
>abstract="Ein Empfänger ist ein Profil, das für den Empfang von Nachrichten bestimmt ist, die von Adobe Campaign gesendet werden. In Adobe Campaign sind Empfänger die Standardprofile für den Versand von Nachrichten (E-Mails, SMS). In dieser Liste können Sie das Empfängerprofil anhand Ihrer Berechtigungen anzeigen. Verwenden Sie die Filteroptionen, um diese Liste zu durchsuchen. Sie können eine kleine Gruppe von Empfängerattributen bearbeiten und aktualisieren."

Ein Empfänger ist ein Profil, das für den Empfang von Nachrichten bestimmt ist, die von Adobe Campaign gesendet werden. In Adobe Campaign sind die Standardprofile für Sendungen (E-Mails, SMS usw.) die Empfänger. Die in der Datenbank gespeicherten Empfängerdaten ermöglichen die Erstellung von Audiences, die einen bestimmten Versand erhalten, sowie das Hinzufügen von Personalisierungsdaten zu den Versandinhalten. Andere Typen von Profilen werden in der Datenbank gespeichert. Sie sind für unterschiedliche Verwendungszwecke konzipiert: Beispielsweise werden Testprofile erstellt, um Ihre Sendungen zu testen, bevor sie an die endgültige Audience gesendet werden.

Empfänger können nur über die Campaign-Clientkonsole hinzugefügt werden. Sie sind jedoch im Campaign-Web über die **Empfänger** Eintrag der linken Navigationsleiste.

Um die Empfängerdaten zu bearbeiten, klicken Sie auf die drei Punkte neben ihrem Namen und wählen Sie **Bearbeiten...**.

![Empfängerprofil bearbeiten](assets/recipient-edit.png)

Sie können eine begrenzte Anzahl von Attributen aktualisieren, nämlich: Vorname, Nachname, E-Mail-Adresse und Telefonnummer.

![Empfängerprofil aktualisieren](assets/recipient-update.png)

>[!NOTE]
>
>Dieses eingeschränkte Formular zur Profilbearbeitung wird nur für Beta-Programmtests bereitgestellt. Sie wird in der zukünftigen Version verbessert. Dadurch kann der Benutzer jedem Profil schnell eine E-Mail-Adresse und eine Telefonnummer hinzufügen, damit er die E-Mail- und SMS-Kanäle testen und die gesendeten Nachrichten empfangen kann.

Sie können die Empfänger mithilfe des Suchfelds über das **Filter anzeigen** Schaltfläche.

Empfänger können auch über die **Explorer** Anzeigen, Durchsuchen und Erstellen von Ordnern und Unterordnern sowie Überprüfen der zugehörigen Berechtigungen.

![Empfängerliste aus der Explorer-Ansicht](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Abhängig von Ihren Berechtigungen haben Sie möglicherweise keinen Zugriff auf die vollständige Liste der in der Datenbank gespeicherten Empfänger. Weiterführende Informationen zu Berechtigungen finden Sie in [diesem Abschnitt](../get-started/permissions.md).

Darüber hinaus können Sie die An- und Abmeldung Ihrer Empfänger für Dienste wie Newsletter verwalten. [Erfahren Sie, wie Sie mit Abonnementdiensten arbeiten können.](create-service.md)

## Zielgruppen {#audiences}

Die Zielgruppe ist das wichtigste Ziel Ihres Versands: die Empfängerinnen und Empfänger, die die Nachrichten erhalten. Der Zielgruppentyp hängt vom in der Versandvorlage definierten Zielgruppen-Mapping ab. [Versandvorlage erfahren](../msg/delivery-template.md).

Zur Bestimmung der Audience-Population haben Sie folgende Möglichkeiten:

* [Neue Zielgruppen erstellen](create-audience.md) aus dem **[!UICONTROL Zielgruppen]** Menü,
* [Existierende Zielgruppe auswählen](add-audience.md) als Liste in der Clientkonsole erstellt wurde,
* [Wählen Sie eine Adobe Experience Platform-Zielgruppe aus](aep-audience.md),
* [Erstellen Sie mit dem Regel-Builder eine neue Zielgruppe, indem Sie Filterkriterien definieren und kombinieren,](segment-builder.md)
* [Verwenden einer Audience aus einer externen Datei](file-audience.md). Diese Option ist nur für Einzelsendungen von E-Mails verfügbar und kann nicht in Kampagnensendungen verwendet werden.

Beim Targeting einer Audience können Sie auch **Kontrollgruppen** um zu vermeiden, dass Nachrichten an einen Teil Ihrer Audience gesendet werden, und messen Sie die Wirkung Ihrer Kampagnen. [Erfahren Sie, wie Sie eine Kontrollgruppe festlegen.](control-group.md)

>[!NOTE]
>
>Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Audience in einem bestimmten **Audience erstellen** Workflow-Aktivität. In diesem Zusammenhang ist es nicht möglich, eine Zielgruppe aus einer Datei für einen E-Mail-Versand zu laden. Die Zielgruppe wird nur in dieser dedizierten Aktivität definiert. [In diesem Abschnitt](../workflows/activities/build-audience.md) erfahren Sie, wie Sie die Zielgruppe Ihres Versands in einem Kampagnen-Workflow definieren
