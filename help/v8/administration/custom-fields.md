---
title: Benutzerdefinierte Felder
description: Informationen dazu, wie Sie benutzerdefinierte Felder konfigurieren können
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: ht
source-wordcount: '255'
ht-degree: 100%

---

# Konfigurieren benutzerdefinierter Felder {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Benutzerdefinierte Felder"
>abstract="Benutzerdefinierte Felder sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zu nativen Schemata hinzugefügt werden. Sie sind jetzt in der Web-Benutzeroberfläche verfügbar."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"



Benutzerdefinierte Felder sind zusätzliche Attribute, die über die Adobe Campaign-Konsole zu nativen Schemata hinzugefügt werden. Weitere Informationen finden Sie in der [Dokumentation zu Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=de){target="_blank"}.

Diese benutzerdefinierten Felder werden in verschiedenen Bildschirmen sichtbar, z. B. in den Details eines Profils oder eines Testprofils.

In der Web-Benutzeroberfläche können Sie zwar keine benutzerdefinierten Felder erstellen, dafür aber ihre Anzeige ändern. Diese Änderungen gelten für alle Campaign-Benutzenden.

>[!NOTE]
>
>Sie müssen über Administratorrechte verfügen, um benutzerdefinierte Felder zu ändern.

Benutzerdefinierte Felder sind in den folgenden Schemata verfügbar:

* Empfängende (nms)
* Kampagnen (nms)
* Sendungen (nms)
* Testadressen (nms)

Gehen Sie wie folgt vor, um benutzerdefinierte Felder zu konfigurieren:

1. Klicken Sie unter **Administration** auf **Schemata**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. Suchen Sie das gewünschte Schema, z. B. das Schema **Empfangende (nms)**.

   ![](assets/custom-fields2.png){zoomable="yes"}

1. Klicken Sie auf die Schaltfläche **Mehr Aktionen** und wählen Sie **Benutzerdefiniertes Detail bearbeiten**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   Auf dem Bildschirm **Benutzerdefiniertes Detail bearbeiten** werden alle benutzerdefinierten Felder und deren Typ angezeigt.

   ![](assets/custom-fields4.png){zoomable="yes"}

   Auf diesem Bildschirm können Sie die folgenden Aktionen durchführen:

   * Die Reihenfolge der verschiedenen Felder anhand der Nach-oben- und Nach-unten-Pfeile ändern
   * Das Feld obligatorisch machen: Aktivieren Sie das Kästchen **Obligatorisch**.
   * Das Feld sichtbar machen oder ausblenden: Klicken Sie auf die Schaltfläche **Sichtbar**.
   * Eine Sichtbarkeitsbedingung hinzufügen: Klicken Sie auf die Schaltfläche **Sichtbar, wenn** und schreiben Sie Ihren xtk-Ausdruck mit den verfügbaren xtk-Funktionen.

1. Navigieren Sie zu dem Bildschirm, auf dem das benutzerdefinierte Feld angezeigt wird. Im vorliegenden Beispiel handelt es sich um den Bildschirm mit den Profildetails.

   ![](assets/custom-fields5.png){zoomable="yes"}
