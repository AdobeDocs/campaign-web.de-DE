---
audience: end-user
title: Bearbeiten des E-Mail-Inhalts
description: Informationen dazu, wie Sie damit beginnen können, mit dem E-Mail-Designer in der Campaign Web-Benutzeroberfläche Inhalte zu erstellen
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 100%

---


# Erste Schritte mit dem E-Mail-Designer {#get-started-email-designer}

Nach der Erstellung einer E-Mail in Adobe Campaign müssen Sie deren Inhalt definieren.

Mit dem E-Mail-Designer können Sie über eine intuitive Drag-and-Drop-Oberfläche überzeugende, individuell zugeschnittene E-Mails erstellen. Egal, ob Sie bei null anfangen, vorhandene Inhalte importieren oder Vorlagen nutzen, Sie können für jede E-Mail alle Inhalte gestalten und präzisieren. Dies gilt sowohl für Promotions als auch für Transaktionen.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Verwenden Sie die Fähigkeiten zur E-Mail-Gestaltung von [!DNL Campaign], um auf einfache Weise responsive E-Mails zu erstellen. [Weitere Informationen](create-email-content.md)

* Verbessern Sie das Kundenerlebnis, indem Sie personalisierte Inhalte basierend auf den Profilattributen der Kundinnen und Kunden erstellen. [Weitere Informationen](../personalization/personalize.md)

* Konfigurieren Sie bedingte Inhaltsfelder, um eine dynamische Personalisierung basierend auf dem Empfängerprofil zu erstellen. [Weitere Informationen](../personalization/conditions.md)

## Best Practices für die E-Mail-Gestaltung {#best-practices}

Beachten Sie beim Senden von E-Mails, dass die Empfängerinnen und Empfänger sie weiterleiten könnten, was manchmal zu Problemen mit dem Rendering der E-Mail führen kann. Dies gilt insbesondere bei der Verwendung von CSS-Klassen, die vom E-Mail-Anbieter, über den die Weiterleitung läuft, möglicherweise nicht unterstützt werden. Wenn Sie beispielsweise die CSS-Klasse „is-desktop-hidden“ verwenden, um ein Bild auf Mobilgeräten auszublenden, wird es möglicherweise nicht korrekt gerendert.

Um diese Rendering-Probleme zu minimieren, empfehlen wir, die Struktur des E-Mail-Designs so einfach wie möglich zu halten. Versuchen Sie, ein einziges Design zu verwenden, das sowohl für Desktop- als auch für Mobilgeräte gut funktioniert, und vermeiden Sie die Verwendung komplexer CSS-Klassen oder anderer Design-Elemente, die möglicherweise nicht von allen E-Mail-Clients vollständig unterstützt werden. Vermeiden Sie in Ihren E-Mails Bilder, die größer als 2 MB sind, oder nutzen Sie kodierte Bild-Links.

Mithilfe dieser Best Practices können Sie sicherstellen, dass Ihre E-Mails konsistent gerendert werden, unabhängig davon, wie sie von Empfängerinnen und Empfängern angezeigt oder weitergeleitet werden.

## Beginnen mit der Inhaltserstellung {#start-authoring}

Gehen Sie im Dashboard des E-Mail-Versands durch den Bildschirm [Inhalt bearbeiten](edit-content.md), um die Startseite des E-Mail-Designers zu öffnen. Wählen Sie dort aus den folgenden Optionen aus, wie Sie Ihre E-Mail gestalten möchten:

* **E-Mail von Grund auf neu erstellen** über die Benutzeroberfläche des E-Mail-Designers. Erfahren Sie in [diesem Abschnitt](create-email-content.md), wie Sie E-Mail-Inhalte gestalten.

* **Codieren und Einfügen von rohen HTML-Zeilen** direkt in den E-Mail-Designer. Erfahren Sie in [diesem Abschnitt](code-content.md), wie Sie Ihre eigenen Inhalte codieren. 

* **Importieren von vorhandenen HTML-Inhalten** aus einer Datei oder einem ZIP-Ordner. In [diesem Abschnitt](existing-content.md) erfahren Sie, wie Sie E-Mail-Inhalte importieren.

* **Auswählen eines vorhandenen Inhalts** aus einer Liste integrierter oder benutzerdefinierter Vorlagen. In [diesem Abschnitt](../content/create-email-templates.md) erfahren Sie, wie Sie mit E-Mail-Vorlagen arbeiten.

  ![Optionen in der E-Mail-Designer-Benutzeroberfläche zum Erstellen von E-Mail-Inhalten](assets/email_designer_create_options.png){zoomable="yes"}
