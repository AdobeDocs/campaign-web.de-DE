---
audience: end-user
title: Verwenden einer Trap-Gruppe
description: Erfahren Sie, wie Sie in der Campaign Web-Benutzeroberfläche eine Trap-Gruppe für Ihren Versand verwenden.
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 35%

---

# Verwenden einer Trap-Gruppe {#trap-group}

Eine **[!UICONTROL Trap-Gruppe]** (auch **[!UICONTROL Testadressenliste]** genannt) wird verwendet, um bestimmte Adressen in Ihre Sendungen einzubeziehen und den Verteilungsprozess zu überwachen und zu überprüfen, indem Sie Profile auswählen, die nicht den definierten Zielgruppenkriterien entsprechen. Auf diese Weise können Empfänger, die außerhalb des Versandbereichs liegen, den Versand wie jede andere Zielgruppe erhalten.

Eine **[!UICONTROL Trap-Gruppe]** ist eine Gruppe von **[!UICONTROL Testadressen]** mit dem Namen **[!UICONTROL Testprofil]** auf der Web-Benutzeroberfläche von Campaign.

## Warum sollte eine Trap-Gruppe verwendet werden? {#why-trap-group}

Sie können eine **[!UICONTROL Trap-Gruppe“]**:

1. **Als Testversand**: Jedes Mitglied der **[!UICONTROL Trap-Gruppe]** erhält den Versand als ob es Teil der Audience wäre.

1. **Zum Schutz Ihrer Mailing-Liste**: Durch den Empfang der Informationen, die die Audience erhält **[!UICONTROL wird jedes Testprofil]** der **[!UICONTROL Trap-Gruppe]** bemerkt, wenn die Mailing-Liste von einem Drittanbieter verwendet wird.

>[!NOTE]
>
>Zusätzlich zum [Versenden von Testsendungen während der Erstellung des Versands](../email/create-email.md#preview-test) und von der [Kontrollgruppe](control-group.md) aus ist das Hinzufügen einer Trap-Gruppe eine gute Möglichkeit, Ihre Zielgruppe zu testen.

## Informationen zu Trap-Gruppen {#about-trap-group}

Testprofile werden aus Berichten zu folgenden Versandstatistiken automatisch ausgeschlossen: **Klicks**, **Öffnungen**, **Abmeldungen**. Die Berichte konzentrieren sich nur auf die tatsächliche Zielgruppe.

Für einen E-Mail-Versand ist für die Gruppe „Trap **[!UICONTROL nur die E-Mail-Adresse]**. Die Personalisierung anderer Felder wird von Campaign nach dem Zufallsprinzip ausgewählt.

## Hinzufügen einer Trap-Gruppe zu einem Versand {#trap-group-in-delivery}

Um eine **[!UICONTROL Trap-Gruppe]** einzurichten, gehen Sie zu den **[!UICONTROL Audience]**-Einstellungen Ihres Versands. Sie haben zwei Möglichkeiten:

* [Testprofile auswählen](#select-test-profiles)
* [Erstellen einer Bedingung](#create-condition)

[Screenshot der Oberfläche für Trap-Gruppeneinstellungen](assets/trap-group.png){zoomable="yes"}

### Testprofile auswählen {#select-test-profiles}

Wenn Sie **Testprofile auswählen** verwenden Sie die Schaltfläche **Testprofil(e) hinzufügen** wie unten dargestellt:

[Screenshot der Schaltfläche „Testprofil hinzufügen“](assets/trap-no-test-profile.png){zoomable="yes"}

Wenn Sie auf die Schaltfläche klicken, können Sie auf die Testprofile zugreifen, die Sie Ihrer **[!UICONTROL Trap-Gruppe“ hinzufügen]**. Wählen Sie diejenigen aus, die Sie verwenden möchten.

Sie können außerdem neue Testprofile erstellen. [Weitere Informationen](#create-seed)

[Screenshot der Benutzeroberfläche für Testprofile auswählen](assets/trap-select-test-profiles.png){zoomable="yes"}

Nachdem Sie die Testprofile bestätigt haben, überprüfen Sie, ob unter „Trap-Gruppe **[!UICONTROL die richtige Anzahl angezeigt]**.

[Bestätigungs-Screenshot der Trap-Gruppe](assets/trap-check.png){zoomable="yes"}

### Erstellen einer Bedingung {#create-condition}

Erstellen Sie mit **[!UICONTROL Option „Bedingung]**&quot; eine Abfrage, um die Testprofile zu definieren, die Sie verwenden möchten:

[Screenshot der Bedingungsschnittstelle erstellen](assets/trap-create-condition.png){zoomable="yes"}

Ihre Abfrage wird unter **[!UICONTROL Trap-Gruppe]** angezeigt.

[Screenshot der Trap-Gruppen-Abfrage](assets/trap-custom.png){zoomable="yes"}

## Erstellen eines neuen Testprofils {#create-seed}

Sie können ein neues **[!UICONTROL Testprofil]** im Ordner **[!UICONTROL Explorer]** > **[!UICONTROL Ressourcen]** > **[!UICONTROL Kampagnen-Management]** > **[!UICONTROL Testmitglieder]** erstellen.

[Screenshot zur Navigation bei Testprofilen erstellen](assets/trap-create.png){zoomable="yes"}

Konfigurieren Sie alle Einstellungen für Ihr **[!UICONTROL Testprofil]** so, wie Sie es für jedes Profil tun würden:

[Screenshot zur Testprofilkonfiguration](assets/trap-create-contact.png){zoomable="yes"}