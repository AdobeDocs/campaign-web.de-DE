---
title: Benutzerdefinierte Felder
description: Erfahren Sie, wie Sie benutzerdefinierte Felder konfigurieren
source-git-commit: 97769e885145d771685752f6367c5ea00831701d
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 8%

---

# Benutzerdefinierte Felder konfigurieren {#custom-fields}

Benutzerdefinierte Felder sind zusätzliche Attribute, die den nativen Schemas über die Adobe Campaign-Konsole hinzugefügt werden. Weitere Informationen finden Sie in der [Dokumentation zu Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=de){target="_blank"}.

Diese benutzerdefinierten Felder werden in verschiedenen Bildschirmen angezeigt, beispielsweise in den Details eines Profils oder eines Testprofils.

In der Web-Benutzeroberfläche können Sie keine benutzerdefinierten Felder erstellen, Sie können jedoch die Anzeige ändern. Änderungen gelten für alle Campaign-Benutzer.

>[!NOTE]
>
>Sie müssen über Administratorrechte verfügen, um benutzerdefinierte Felder zu ändern.

Benutzerdefinierte Felder sind in den folgenden Schemata verfügbar:

* Empfänger (nms)
* Kampagnen (nms)
* Sendungen (nms)
* Testadressen (nms)

Gehen Sie wie folgt vor, um benutzerdefinierte Felder zu konfigurieren:

1. under **Administration** klicken **Schemas**.

   ![](assets/custom-fields.png){zoomable=&quot;yes&quot;}

1. Suchen Sie das gewünschte Schema, z. B. das **Empfänger (nms)** Schema.

   ![](assets/custom-fields2.png){zoomable=&quot;yes&quot;}

1. Klicken Sie auf **Mehr Aktionen** Schaltfläche und wählen Sie **Benutzerdefiniertes Detail bearbeiten**.

   ![](assets/custom-fields3.png){zoomable=&quot;yes&quot;}

   Die **Benutzerdefiniertes Detail bearbeiten** zeigt alle benutzerdefinierten Felder und deren Typ an.

   ![](assets/custom-fields4.png){zoomable=&quot;yes&quot;}

   In diesem Bildschirm können Sie die folgenden Aktionen durchführen:

   * ändern Sie die Reihenfolge der verschiedenen Felder mithilfe der Nach-oben- und Nach-unten-Pfeile.
   * das Feld obligatorisch machen: Überprüfen Sie die **Obligatorisch** ankreuzen.
   * das Feld sichtbar machen oder ausblenden: Klicken Sie auf das **Sichtbar** Schaltfläche.
   * Hinzufügen einer Sichtbarkeitsbedingung: Klicken Sie auf die Schaltfläche **Sichtbar, wenn** und schreiben Sie Ihren xtk-Ausdruck mit den verfügbaren xtk-Funktionen.

1. Navigieren Sie zum Bildschirm, auf dem das benutzerdefinierte Feld angezeigt wird. Im vorliegenden Beispiel handelt es sich um den Bildschirm mit den Profildetails.

   ![](assets/custom-fields5.png){zoomable=&quot;yes&quot;}
