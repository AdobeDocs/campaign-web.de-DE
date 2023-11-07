---
title: Arbeiten mit Empfängerinnen bzw. Empfängern und Zielgruppen
description: Erfahren Sie, wie Sie mit Empfängerinnen und Empfängern in Campaign Web arbeiten.
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 332bcd3788ac137a60e7973d4e54b8cea22a9333
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 96%

---

# Arbeiten mit Empfängerinnen bzw. Empfängern und Zielgruppen {#about-recipients}

In Adobe Campaign ist die Zielpopulation eines Versands eine Zielgruppe. Eine Zielgruppe ist eine Gruppe von Personen, die ähnliche Verhaltensweisen und/oder Merkmale aufweisen. Diese Sammlung von Leuten kann entweder generiert, ausgewählt oder geladen werden, [wie im Folgenden beschrieben](#audiences). In den meisten Fällen besteht die Zielgruppe aus Profilen, die als [Empfängerinnen und Empfänger](#recipients) in Adobe Campaign gespeichert werden. Sie können auch mit anderen Zielgruppen-Mappings arbeiten, indem Sie die Dimension ändern, wie [in diesem Abschnitt](#targeting-dimensions) beschrieben.

## Was sind Empfängerinnen und Empfänger? {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Empfängerinnen und Empfänger"
>abstract="Eine Empfängerin bzw. ein Empfänger ist ein Profil, das für den Empfang von Nachrichten bestimmt ist, die von Adobe Campaign gesendet werden. In Adobe Campaign sind Empfängerinnen und Empfänger die Standardprofile, an die sich Sendungen richten (E-Mails oder SMS). In dieser Liste kann das Empfängerprofil anhand der Berechtigungen angezeigt werden. Die Filteroptionen verwenden, um diese Liste zu durchsuchen. Es kann eine kleine Gruppe von Empfängerattributen bearbeitet und aktualisiert werden."

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

Darüber hinaus können Sie die An- und Abmeldung Ihrer Empfängerinnen und Empfänger für Dienste wie beispielsweise Newsletter verwalten. Erfahren Sie, wie Sie mit Abonnementdiensten in arbeiten können. [diese Seite](manage-services.md)

Sie können Workflows erstellen, um Profile zu deduplizieren, anzureichern, zu kombinieren und Zielgruppen zu erstellen. Weiterführende Informationen finden Sie in [diesem Abschnitt](../workflows/gs-workflows.md).

## Was sind Zielgruppen? {#audiences}

Die Zielgruppe ist das wichtigste Ziel Ihres Versands: die Empfängerinnen und Empfänger, die die Nachrichten erhalten. Der Zielgruppentyp hängt vom in der Versandvorlage definierten Zielgruppen-Mapping ab. Weitere Informationen zu Versandvorlagen finden Sie in [diese Seite](../msg/delivery-template.md).

Um die Population Ihrer Zielgruppe zu bestimmen, können Sie:

* [neue Zielgruppen erstellen](create-audience.md) über das Menü **[!UICONTROL Zielgruppen]**,
* [eine vorhandene Zielgruppe auswählen](add-audience.md), die als Liste in der Client-Konsole erstellt wurde oder aus Adobe Experience Platform stammt,
* [mit dem Regel-Builder eine neue Zielgruppe erstellen](segment-builder.md), indem Sie Filterkriterien definieren und kombinieren,
* [eine Zielgruppe aus einer externen Datei verwenden](file-audience.md). Diese Option steht nur für eigenständige E-Mail-Sendungen zur Verfügung und kann nicht in Kampagnensendungen verwendet werden.

Wenn Sie eine Zielgruppe ansprechen, können Sie außerdem **Kontrollgruppen** definieren, um einen Teil Ihrer Zielgruppe vom Versand von Nachrichten auszuschließen und so die Wirkung Ihrer Kampagnen zu messen. [Erfahren Sie, wie Sie eine Kontrollgruppe festlegen](control-group.md)

>[!NOTE]
>
>Beim Versand von Nachrichten im Rahmen eines Kampagnen-Workflows wird die Zielgruppe in der speziellen Workflow-Aktivität **Zielgruppe erstellen** definiert. In diesem Zusammenhang ist es nicht möglich, eine Zielgruppe aus einer Datei für einen E-Mail-Versand zu laden. Die Zielgruppe wird nur in dieser dedizierten Aktivität definiert. Erfahren Sie, wie Sie die Audience Ihres Versands in einem Kampagnen-Workflow definieren können in [diesem Abschnitt](../workflows/activities/build-audience.md)

## Zielgruppendimensionen {#targeting-dimensions}

Die Zielgruppendimension, auch bekannt als Zielgruppen-Mapping, ist der Datentyp, den ein Vorgang verarbeitet. Sie ermöglicht die Bestimmung der Zielpopulation: Empfängerinnen und Empfänger, Vertragsbegünstigte, Benutzerinnen und Benutzer, Abonnentinnen und Abonnenten usw.

Die Zielgruppendimension eines Workflows wird durch die erste Aktivität **[!UICONTROL Zielgruppe erstellen]** definiert und wird bis zum Ende des Workflows für alle weiteren Aktivitäten verwendet. Wenn Sie beispielsweise eine Abfrage an die aus der Datenbank stammenden Empfängerinnen und Empfänger durchführen, enthält die ausgehende Transition Daten vom Typ Empfängerinnen und Empfänger und wird an die nächste Aktivität übermittelt.

Beachten Sie, dass Sie die Zielgruppendimension in einem Workflow mithilfe der Aktivität [Dimensionsaktivität ändern](../workflows/activities/change-dimension.md) wechseln können. Auf diese Weise können Sie beispielsweise die Datenbank in einer bestimmten Tabelle (z. B. zu Käufen oder Abonnements) abfragen und die Zielgruppendimension in Empfängerinnen und Empfänger ändern, um Sendungen an die entsprechenden Empfängerinnen und Empfänger durchzuführen.

Standardmäßig haben die E-Mail- und SMS-Versandvorlagen **[!UICONTROL Empfängerinnen und Empfänger]** als Zielgruppe. Ihr Zielgruppen-Mapping verwendet daher die Felder der Tabelle **nms:recipient**. Für Push-Benachrichtigungen ist die standardmäßige Zielgruppendimension **Abonnierte Anwendungen (nms:appSubscriptionRcp)**, das mit der Empfängertabelle verknüpft ist.

Sie können auch andere integrierte Zielgruppen-Mappings in Ihren Workflows und Sendungen verwenden, die unten aufgeführt sind:

| Name | Verwendung Verwendungszweck | Schema |
|---|---|---|
| Empfängerinnen und Empfänger | Versand an Empfänger (integrierte Empfängertabelle) | nms:recipient |
| Besucher | Versand an Besucher, deren Profile beispielsweise über Empfehlungen (Viral Marketing) erfasst wurden. | mns:visitor |
| Abonnements  | Versand richtet sich an Abonnenten eines Informationsdienstes wie z. B. einen Newsletter | nms:subscription |
| Besucher-Abonnements | Versand richtet sich an Besucher, die einen Informationsdienst beziehen | nms:visitorSub |
| Benutzer | Versand richtet sich an Adobe-Campaign-Benutzer | nms:operator |
| Externe Datei | Versand basiert auf einer Datei, die alle notwendigen Informationen enthält | Ohne Schema oder Zielgruppe |
| Abonnierte Anwendungen | Versand an Empfängerinnen und Empfänger, die eine Anwendung abonniert haben | nms:appSubscriptionRcp |

Zusätzlich können Sie je nach Bedarf ein neues Zielgruppen-Mapping erstellen. Dies erfolgt über die Client-Konsole. Weitere Informationen finden Sie in der [Dokumentation zu Campaign v8 (Client-Konsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=de#new-mapping){target="_blank"}.
