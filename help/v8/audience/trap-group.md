---
audience: end-user
title: Verwenden einer Trap-Gruppe
hide: true
hidefromtoc: true
description: Erfahren Sie, wie Sie in der Campaign Web-Benutzeroberfläche eine Trap-Gruppe für Ihren Versand verwenden.
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 48%

---

# Verwenden einer **[!UICONTROL Trap-Gruppe]** {#trap-group}

Eine **[!UICONTROL Fallen-Gruppe]** (auch **[!UICONTROL Testliste]** genannt) wird verwendet, um bestimmte Adressen in Ihre Sendungen einzubeziehen, um den Verteilungsprozess zu überwachen und zu überprüfen, indem Profile ausgewählt werden, die nicht den definierten Zielkriterien entsprechen. Auf diese Weise können Empfängerinnen und Empfänger, die außerhalb des Versandumfangs liegen, die Nachricht ebenso wie jede andere Person innerhalb der Zielgruppe erhalten.
Eine **[!UICONTROL Fallen-Gruppe]** ist eine Gruppe von **[!UICONTROL Testadressen]** mit dem Namen **[!UICONTROL Testprofil]** auf der AC-Web-Benutzeroberfläche.

## Warum **[!UICONTROL Trap group]** verwenden?

Sie können eine **[!UICONTROL Trap-Gruppe]** für Folgendes verwenden:

1. **Testversand**: Jedes Mitglied der **[!UICONTROL Trap-Gruppe]** erhält den Versand so, als wäre es Teil der Zielgruppe.


1. **Schutz Ihrer Mailingliste** : Durch den Empfang der Informationen, die die Zielgruppe erhalten wird, wird jedes **[!UICONTROL Testprofil]** der **[!UICONTROL Trap group]** bemerkt, wenn die Mailingliste von einem Drittanbieter verwendet wird.

>[!NOTE]
>
>Die Trap-Gruppe unterscheidet sich vom [Versand von Testsendungen während der Erstellung des Versands](../email/create-email.md#preview-test) und von der [Kontrollgruppe](control-group.md).


## Informationen zur **[!UICONTROL Trap-Gruppe]**

Testprofile werden aus Berichten zu folgenden Versandstatistiken automatisch ausgeschlossen: **Klicks**, **Öffnungen**, **Abmeldungen**. Die Berichte beziehen sich ausschließlich auf die tatsächliche Zielgruppe.

In E-Mail-Sendungen ist für die **[!UICONTROL Trap-Gruppe]** nur die E-Mail-Adresse erforderlich. Die Personalisierung anderer Felder wird zufällig von Campaign ausgefüllt.

## Einrichten einer **[!UICONTROL Trap-Gruppe]** im Versand

Navigieren Sie zum Einrichten einer **[!UICONTROL Trap-Gruppe]** zu den **[!UICONTROL Zielgruppeneinstellungen]** Ihres Versands. Sie haben zwei Optionen:
- [Testprofile auswählen](#select-test-profile)
- [Bedingung erstellen](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Testprofile auswählen {#select-test-profiles}

Wenn Sie sich für „Testprofile auswählen“ entscheiden, wird das Fenster wie unten dargestellt angezeigt. Dort werden Sie zum **[!UICONTROL Hinzufügen von Testprofilen]** aufgefordert:

![](assets/trap-no-test-profile.png){zoomable="yes"}

Wenn Sie auf die Schaltfläche klicken, haben Sie Zugriff auf die Testprofile, die Sie Ihrer **[!UICONTROL Fallen-Gruppe]** hinzufügen können. Kreuzen Sie diejenigen an, die Sie verwenden möchten.
Sie können neue Testprofile erstellen. [Weitere Informationen](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Wenn Sie Ihre Testprofile bestätigen, vergewissern Sie sich, dass unter **[!UICONTROL Trap group]** die richtige Zahl vorhanden ist.

![](assets/trap-check.png){zoomable="yes"}

### Bedingung erstellen {#create-condition}

Mit der Auswahl von **[!UICONTROL Bedingung erstellen]** erhalten Sie ein neues Fenster, in dem Sie eine Abfrage zur Definition der Testprofile, die Sie verwenden möchten, benutzerspezifisch einstellen können:

![](assets/trap-create-condition.png){zoomable="yes"}

Ihre Abfrage wird unter **[!UICONTROL Trap-Gruppe]** angezeigt.

![](assets/trap-custom.png){zoomable="yes"}

## Erstellen eines neuen **[!UICONTROL Testprofils]** {#create-seed}

Sie können ein neues **[!UICONTROL Testprofil]** in **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Testempfänger]** erstellen

![](assets/trap-create.png){zoomable="yes"}

Sie können alle Details zu Ihrem **[!UICONTROL Testprofil]** so vervollständigen, als wäre es ein Zielgruppenprofil :

![](assets/trap-create-contact.png){zoomable="yes"}