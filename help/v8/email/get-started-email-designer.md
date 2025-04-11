---
audience: end-user
title: Bearbeiten des E-Mail-Inhalts
description: Informationen dazu, wie Sie damit beginnen können, mit dem E-Mail-Designer in der Campaign Web-Benutzeroberfläche Inhalte zu erstellen
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 45%

---


# Erste Schritte mit dem E-Mail-Designer {#get-started-email-designer}

Nachdem Sie eine E-Mail in Adobe Campaign erstellt haben, müssen Sie ihren Inhalt definieren.

Mit dem E-Mail-Designer können Sie über eine intuitive Drag-and-Drop-Oberfläche überzeugende, individuell zugeschnittene E-Mails erstellen. Egal, ob Sie bei null anfangen, vorhandene Inhalte importieren oder vorhandene Vorlagen nutzen, entwerfen und verfeinern Sie alle Inhalte für jede E-Mail, egal ob für Werbeaktionen oder Transaktionen.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Verwenden Sie die Fähigkeiten zur E-Mail-Gestaltung von [!DNL Campaign], um auf einfache Weise responsive E-Mails zu erstellen. [Weitere Informationen](create-email-content.md)

* Verbessern Sie das Kundenerlebnis, indem Sie personalisierte E-Mails auf der Basis von Kundenprofil-Attributen erstellen. [Weitere Informationen](../personalization/personalize.md)

* Konfigurieren Sie bedingte Inhaltsfelder, um eine dynamische Personalisierung basierend auf dem Empfängerprofil zu erstellen. [Weitere Informationen](../personalization/conditions.md)

## Best Practices für die E-Mail-Gestaltung {#best-practices}

Beachten Sie beim Senden von E-Mails, dass Empfängerinnen und Empfänger sie weiterleiten können, was manchmal zu Problemen mit dem Rendering der E-Mail führen kann. Dies gilt insbesondere bei der Verwendung von CSS-Klassen, die von dem für die Weiterleitung verwendeten E-Mail-Anbieter möglicherweise nicht unterstützt werden. Wenn Sie beispielsweise die CSS-Klasse „is-desktop-hidden“ verwenden, um ein Bild auf Mobilgeräten auszublenden, wird es möglicherweise nicht korrekt gerendert.

Um diese Rendering-Probleme zu minimieren, sollten Sie Ihre E-Mail-Design-Struktur so einfach wie möglich halten. Verwenden Sie ein einzelnes Design, das sowohl für Desktop- als auch für Mobilgeräte gut funktioniert, und vermeiden Sie die Verwendung komplexer CSS-Klassen oder anderer Design-Elemente, die möglicherweise nicht von allen E-Mail-Clients vollständig unterstützt werden. Mithilfe dieser Best Practices können Sie sicherstellen, dass Ihre E-Mails konsistent gerendert werden, unabhängig davon, wie sie von Empfängerinnen und Empfängern angezeigt oder weitergeleitet werden.

## Beginnen mit der Inhaltserstellung {#start-authoring}

Gehen Sie im Dashboard des E-Mail-Versands durch den Bildschirm [Inhalt bearbeiten](edit-content.md), um die Startseite des E-Mail-Designers zu öffnen. Wählen Sie dort aus den folgenden Optionen aus, wie Sie Ihre E-Mail gestalten möchten:

* **E-Mail von Grund auf neu erstellen** über die Benutzeroberfläche des E-Mail-Designers. Erfahren Sie in [diesem Abschnitt](create-email-content.md), wie Sie E-Mail-Inhalte gestalten.

* **Codieren und Einfügen von rohen HTML-Zeilen** direkt in den E-Mail-Designer. Erfahren Sie in [diesem Abschnitt](code-content.md), wie Sie Ihre eigenen Inhalte codieren. 

* **Importieren von vorhandenen HTML-Inhalten** aus einer Datei oder einem ZIP-Ordner. Erfahren Sie in ([ Abschnitt), wie Sie E-Mail-Inhalte ](existing-content.md).

* **Auswählen eines vorhandenen Inhalts** aus einer Liste integrierter oder benutzerdefinierter Vorlagen. In (diesem Abschnitt) erfahren Sie[ wie Sie mit E-](create-email-templates.md)-Vorlagen arbeiten.

  ![In der E-Mail-Designer-Benutzeroberfläche verfügbare Optionen zum Erstellen von E-Mail-Inhalten](assets/email_designer_create_options.png){zoomable="yes"}
