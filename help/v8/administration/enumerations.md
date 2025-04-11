---
title: Verwalten von Auflistungen
description: Erfahren Sie, wie Sie mit Auflistungen arbeiten.
exl-id: d2a30fef-2cc4-49af-9f5d-d42c6396a8ab
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 64%

---

# Verwalten von Auflistungen {#enumerations}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Erstellen von Auflistungen"
>abstract="Sie können Auflistungen nun direkt über die Adobe Campaign Web-Benutzeroberfläche erstellen. Eine Auflistung ist eine Liste von Werten, die vom System zum Auffüllen von Feldern vorgeschlagen werden."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=de" text="Siehe Versionshinweise"

>[!CONTEXTUALHELP]
>id="acw_enumerations_list"
>title="Auflistungen"
>abstract="Eine Auflistung ist eine Liste von Werten, die vom System zum Auffüllen von Feldern vorgeschlagen werden. Verwenden Sie Auflistungen, um die Werte dieser Felder zu standardisieren, die Dateneingabe zu unterstützen oder sie in Abfragen zu verwenden."

>[!CONTEXTUALHELP]
>id="acw_enumerations_properties"
>title="Eigenschaften"
>abstract="Definiert die Eigenschaften der Auflistung, z. B. ihren Namen, internen Namen und Typ. Auflistungen vom Typ **[!UICONTROL Geschlossen]** verfügen über eine feste Liste von Werten, die nur über das Menü **[!UICONTROL Auflistungen]** geändert werden kann. Auflistungen vom Typ **[!UICONTROL Offen]** ermöglichen es den Benutzenden, neue Werte direkt in die auf dieser Auflistung basierenden Felder einzufügen. Auflistungen vom Typ **[!UICONTROL System]** sind mit Systemfeldern verknüpft. Auflistungen vom Typ **[!UICONTROL Emoticon]** werden verwendet, um die Liste der Smileys zu aktualisieren. "

>[!CONTEXTUALHELP]
>id="acw_enumerations_values"
>title="Liste der Auflistungswerte"
>abstract="Um der Auflistung einen Wert hinzuzufügen, klicken Sie auf die Schaltfläche **[!UICONTROL Wert hinzufügen]** und konfigurieren Sie ihn dann nach Bedarf."

## Was sind Auflistungen? {#about}

Eine Auflistung ist eine Liste von Werten, die vom System zum Auffüllen von Feldern vorgeschlagen werden. Verwenden Sie Auflistungen, um die Werte dieser Felder zu standardisieren, die Dateneingabe zu unterstützen oder sie in Abfragen zu verwenden. Die Werteliste erscheint als Dropdown-Liste, aus der Sie den im Feld einzufügenden Wert auswählen können. Die Dropdown-Liste ermöglicht auch eine prädiktive Eingabe: Beim Eingeben der ersten Buchstaben füllt die Anwendung den Rest aus.

Die Werte für diesen Feldtyp werden über das Menü **[!UICONTROL Administration]** / **[!UICONTROL Auflistungen]** im linken Navigationsbereich definiert.

![Auflistungsliste im Menü Administration angezeigt](assets/enumeration-list.png)

## Erstellen einer Auflistung {#create}

Gehen Sie wie folgt vor, um eine Auflistung zu erstellen:

1. Navigieren Sie zum Menü **[!UICONTROL Auflistungen]** und klicken Sie dann auf die Schaltfläche **[!UICONTROL Auflistung erstellen]**.

1. Geben Sie einen **[!UICONTROL Titel]** und einen **[!UICONTROL internen Namen]** für die Auflistung ein.

   ![Auflistungsbildschirm mit Feldern für Titel und internen Namen erstellen](assets/enumeration-create.png)

1. Wählen Sie einen **[!UICONTROL Typ]** für die Auflistung aus:

   * **[!UICONTROL Geschlossene]** Auflistungen verfügen über eine feste Liste von Werten, die nur über das Menü **[!UICONTROL Auflistungen]** geändert werden kann.
   * Auflistungen vom Typ **[!UICONTROL Offen]** ermöglichen es den Benutzenden, neue Werte direkt in die auf dieser Auflistung basierenden Felder einzufügen.
   * **[!UICONTROL System]**-Auflistungen sind mit Systemfeldern verknüpft.
   * Auflistungen vom Typ **[!UICONTROL Emoticon]** werden verwendet, um die Liste der Smileys zu aktualisieren.

1. Klicken Sie auf **[!UICONTROL Erstellen]**. Die Auflistungsdetails werden angezeigt, sodass Sie der Liste Werte hinzufügen können.

   ![Bildschirm mit Auflistungsdetails mit Optionen zum Hinzufügen von Werten](assets/enumeration-details.png)

1. Um einen Wert hinzuzufügen, klicken Sie auf die Schaltfläche **[!UICONTROL Wert hinzufügen]** und konfigurieren Sie ihn dann nach Bedarf:

   * **[!UICONTROL Titel]**: Der in der Auflistung anzuzeigende Titel.
   * **[!UICONTROL Interner Name]**: Der interne Name des Werts (für Systemauflistungen).
   * **[!UICONTROL U+ (interner Name)]** (Emoticon-Auflistungen): Der Unicode-Code für den Smiley (für Emoticon-Auflistungen).

   ![Bildschirm „Wert hinzufügen“ mit Feldern für Beschriftung, internen Namen und Unicode](assets/enumeration-emoticon.png)

1. Speichern Sie Ihre Änderungen. Die Auflistung wird in den Bildschirmen aktualisiert, in denen sie verwendet wird.

## Anwendungsfall: Hinzufügen vordefinierter Werte zu einer Auflistung {#uc}

Standardmäßig können Benutzende im Feld „Herkunft“ im Bildschirm mit den Profildetails einen beliebigen Wert frei eingeben.

![Bildschirm mit den Profildetails mit dem Feld „Herkunft“](assets/enumeration-uc-profile.png)

Jedes Mal, wenn ein Benutzer einen Wert für das Feld eingibt, wird der Wert automatisch zur Auflistung „Herkunft“ hinzugefügt. Dies kann im Laufe der Zeit zu redundanten, inkonsistenten oder fehlerhaften Werten in der Werteliste führen.

![Origin-Auflistung mit inkonsistenten vom Benutzer eingegebenen Werten](assets/enumeration-uc-choice.png)

Um die Datenkonsistenz zu gewährleisten und Benutzende beim Ausfüllen des Felds zu unterstützen, definieren Sie einen Satz vordefinierter Werte. Gehen Sie dazu wie folgt vor:

1. Öffnen Sie im Menü **[!UICONTROL Auflistungen]** die Auflistung „Herkunft“.

2. Überprüfen Sie die Liste der benutzerseitig eingegebenen Werte und bereinigen Sie sie. Klicken Sie auf die Schaltfläche mit den Auslassungspunkten neben einem Wert, um ihn zu löschen. Wenn die Liste zu viele Inkonsistenzen enthält, löschen Sie die gesamte Auflistung und erstellen Sie sie von Grund auf neu.

   ![Bildschirm mit Optionen zum Bereinigen der vom Benutzer eingegebenen Werte](assets/enumeration-uc-clean.png)

3. Hinzufügen vordefinierter Werte Klicken Sie dazu auf die Schaltfläche **[!UICONTROL Wert hinzufügen]** und geben Sie die vordefinierten Werte ein, aus denen die Benutzenden wählen sollen.

   ![Bildschirm mit vordefinierten Werten, die der Auflistung hinzugefügt werden](assets/enumeration-uc-create.png)

4. Um Konsistenz zu erzwingen, wechseln Sie den Auflistungstyp zu **[!UICONTROL Geschlossen]**, wodurch Benutzer auf vordefinierte Werte beschränkt werden. Wenn eine Flexibilität erforderlich ist, belassen Sie **[!UICONTROL Offen]** als Typ, um neue Benutzereinträge zu ermöglichen.

5. Kehren Sie zum Bildschirm mit den Profildetails zurück. Das Feld „Herkunft“ zeigt nun die vordefinierten Werte zur Auswahl an.

   ![Bildschirm mit Profildetails mit vordefinierten Werten im Feld „Herkunft“](assets/enumeration-uc-populated.png)