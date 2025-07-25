---
title: Branding
description: Informationen zum Konfigurieren Ihrer Marke
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 2b4a818c819ae598d5555c1a2d64447b0793b5b8
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 100%

---

# Konfigurieren von Marken {#branding-configure}

>[!IMPORTANT]
>
>Marken können von Endnutzenden nicht erstellt oder geändert werden. Diese Tätigkeiten müssen von technischen Adobe Campaign-Admins vorgenommen werden. Bei Fragen wenden Sie sich an die Adobe-Kundenunterstützung.

In Adobe Campaign V8 finden Sie Marken im Menü **[!UICONTROL Administration > Plattform > Branding]**.

Eine **[!UICONTROL Marke]** wird durch die folgenden Eigenschaften definiert:

* eine **[!UICONTROL Identität]**, durch die Ihre Marke definiert und personalisiert wird. Dieser Abschnitt weist folgende Felder auf:

   * **[!UICONTROL Titel]** (in der Benutzeroberfläche sichtbar)
   * **[!UICONTROL Kennung]**
   * **[!UICONTROL Markenname]**
   * **[!UICONTROL URL]** und **[!UICONTROL Titel]** der Marken-Website
   * **[!UICONTROL Markenlogo]**

  ![](assets/branding_1.png)

* **[!UICONTROL In Header-Parameter für ausgehende E-Mails]** kann der Inhalt für die Empfänger Ihrer Kampagnen personalisiert werden. Dieser Abschnitt weist folgende Felder auf:

   * **[!UICONTROL Absender (E-Mail)]** mit der E-Mail-Adresse der Marke.
   * **[!UICONTROL Absender (Name)]** mit dem Namen der Marke.
   * **[!UICONTROL Antwortadresse (E-Mail)]** mit der E-Mail-Adresse, an die der Kunde eine Antwort senden kann.
   * **[!UICONTROL Antwortadresse (Name)]** mit dem Namen der Marke.
   * **[!UICONTROL Fehler (E-Mail)]** mit der E-Mail-Adresse, die im Falle eines Fehlers verwendet werden soll.

  >[!IMPORTANT]
  >
  >Sollten nach der Aktualisierung der E-Mail-Header-Parameter Name und E-Mail-Adresse des Absenders in einer neuen, auf dieser Vorlage basierenden E-Mail nicht geändert sein, überprüfen Sie die erweiterten Parameter der Vorlage.

  ![](assets/branding_2.png)

* Über **[!UICONTROL Markenkonfigurationen]** werden die Server definiert, die für das Tracking sowie den Zugriff auf Landingpages verwendet werden. Dieser Abschnitt weist folgende Felder auf:

   * **[!UICONTROL Marken-Subdomain]** bezieht sich auf die für diese Marke spezifische designierte Subdomain-URL, die von Adobe delegiert werden soll.

  Beachten Sie, dass die Konfiguration für Tracking-, Mirror- und Anwendungs-Server in separaten externen Konten gespeichert ist, die mit dem Routing verbunden sind. Diese Einstellungen werden während der Bereitstellung angewendet und sollten nicht geändert werden. Um URLs anzuzeigen, greifen Sie über Ihr externes Konto auf die Registerkarte **[!UICONTROL Branding-Präfixe]** zu.

  ![](assets/branding_3.png)

* Über das Menü **[!UICONTROL Konfiguration der Tracking-URL]** können Sie das URL-Tracking verbessern, indem Sie zusätzliche Parameter für die Integration mit Web-Analyse-Tools wie Adobe Analytics und Google Analytics definieren.

  Verwenden Sie das Menü **[!UICONTROL Zusätzliche URL-Parameter]**, um zusätzliche Parameter als Schlüssel-Wert-Paare zusammen mit ihren Anwendungsbedingungen zu erstellen. Alle Parameternamen müssen eindeutig und dürfen nicht leer sein. Alle Parameterwerte dürfen nicht leer sein. Die Anwendungsbedingung kann leer sein, aber keiner dieser Werte darf JST-Tags enthalten.

  Diese Parameter werden auf getrackte URLs angewendet, die mit einem in der **[!UICONTROL Liste der Domain-Namen]** angegebenen Domain-Namen übereinstimmen, der reguläre Ausdrücke enthalten kann.
