---
audience: end-user
title: Verwenden einer Trap-Gruppe
description: Erfahren Sie, wie Sie in der Campaign Web-Benutzeroberfläche eine Trap-Gruppe für Ihren Versand verwenden.
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 100%

---

# Verwenden einer Trap-Gruppe {#trap-group}

Eine **[!UICONTROL Trap-Gruppe]** (auch **[!UICONTROL Testadressenliste]** genannt) wird verwendet, um bestimmte Adressen in Ihre Sendungen einzubeziehen und den Verteilungsprozess zu überwachen und zu überprüfen, indem Sie Profile auswählen, die nicht den definierten Zielgruppenkriterien entsprechen. Auf diese Weise können Empfängerinnen und Empfänger, die außerhalb des Versandbereichs liegen, den Versand wie jede bzw. jeder andere Zielgruppenempfangende erhalten.

Eine **[!UICONTROL Fallen-Gruppe]** ist eine Gruppe von **[!UICONTROL Testadressen]** mit dem Titel **[!UICONTROL Testprofil]** in der Campaign Web-Benutzeroberfläche.

## Warum sollte eine Trap-Gruppe verwendet werden? {#why-trap-group}

Sie können eine **[!UICONTROL Fallen-Gruppe]** für Folgendes verwenden:

1. **Als Testversand**: Jedes Mitglied der **[!UICONTROL Fallen-Gruppe]** erhält den Versand so, als wäre er oder sie Teil der Zielgruppe.

1. **Zum Schutz Ihrer Mailing-Liste**: Da jedes **[!UICONTROL Testprofil]** der **[!UICONTROL Fallen-Gruppe]** das Gleiche erhält wie die Zielgruppe, fällt es auf, wenn die Mailing-Liste von Dritten verwendet wird.

>[!NOTE]
>
>Zusätzlich zum [Versenden von Testsendungen während der Erstellung des Versands](../email/create-email.md#preview-test) und von der [Kontrollgruppe](control-group.md) aus ist das Hinzufügen einer Trap-Gruppe eine gute Möglichkeit, Ihre Zielgruppe zu testen.

## Informationen zu Trap-Gruppen {#about-trap-group}

Testprofile werden aus Berichten zu folgenden Versandstatistiken automatisch ausgeschlossen: **Klicks**, **Öffnungen**, **Abmeldungen**. Die Berichte beziehen sich ausschließlich auf die tatsächliche Zielgruppe.

Beim E-Mail-Versand ist für die **[!UICONTROL Fallen-Gruppe]** nur die E-Mail-Adresse erforderlich. Die Personalisierung anderer Felder wird zufällig von Campaign ausgefüllt.

## Hinzufügen einer Trap-Gruppe zu einem Versand {#trap-group-in-delivery}

Navigieren Sie zum Einrichten einer **[!UICONTROL Fallen-Gruppe]** zu den **[!UICONTROL Zielgruppeneinstellungen]** Ihres Versands. Sie haben zwei Optionen:

* [Auswählen der Testprofile](#select-test-profiles)
* [Erstellen einer Bedingung](#create-condition)

[Screenshot der Benutzeroberfläche mit Einstellungen für die Fallen-Gruppen](assets/trap-group.png){zoomable="yes"}

### Auswählen der Testprofile {#select-test-profiles}

Wenn Sie **Testprofile auswählen** auswählen, können Sie die Schaltfläche **Testprofil(e) hinzufügen** verwenden, wie unten dargestellt:

[Screenshot der Schaltfläche „Testprofil hinzufügen“](assets/trap-no-test-profile.png){zoomable="yes"}

Wenn Sie auf die Schaltfläche klicken, erhalten Sie Zugriff auf die Testprofile, die Sie zu Ihrer **[!UICONTROL Fallen-Gruppe]** hinzufügen können. Wählen Sie diejenigen aus, die Sie verwenden möchten.

Sie können außerdem neue Testprofile erstellen. [Weitere Informationen](#create-seed)

[Screenshot der Benutzeroberfläche zur Auswahl der Testprofile](assets/trap-select-test-profiles.png){zoomable="yes"}

Prüfen Sie nach dem Bestätigen der Testprofile, ob unter **[!UICONTROL Fallen-Gruppe]** die richtige Anzahl angezeigt wird.

[Screenshot mit der Bestätigungs der Fallen-Gruppe](assets/trap-check.png){zoomable="yes"}

### Erstellen einer Bedingung {#create-condition}

Mit der Option **[!UICONTROL Bedingung erstellen]** erstellen Sie eine Abfrage, um die Testprofile zu definieren, die Sie verwenden möchten:

[Screenshot der Benutzeroberfläche zum Erstellen der Bedingung](assets/trap-create-condition.png){zoomable="yes"}

Ihre Abfrage wird unter **[!UICONTROL Trap-Gruppe]** angezeigt.

[Screenshot mit der Anzeige der Abfrage für die Fallen-Gruppe](assets/trap-custom.png){zoomable="yes"}

## Erstellen eines neuen Testprofils {#create-seed}

Sie können ein neues **[!UICONTROL Testprofil]** unter **[!UICONTROL Explorer]** > **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnenverwaltung]** > **[!UICONTROL Testempfänger]** erstellen.

[Screenshot mit der Navigation für das Erstellen von Testprofilen](assets/trap-create.png){zoomable="yes"}

Konfigurieren Sie alle Einstellungen für Ihr **[!UICONTROL Testprofil]** wie für jedes Profil:

[Screenshot mit der Konfiguration des Testprofils](assets/trap-create-contact.png){zoomable="yes"}