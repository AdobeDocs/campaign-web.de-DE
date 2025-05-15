---
title: 'Konfigurieren von Optionen in [!DNL Campaign] '
description: Erfahren Sie, wie Sie Campaign-Optionen konfigurieren und Ihre eigenen benutzerdefinierten Optionen erstellen.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: 10a43da9df57a32f987b3d4c51bea91da10cbf92
workflow-type: ht
source-wordcount: '431'
ht-degree: 100%

---

# Konfigurieren von Optionen in [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Optionen"
>abstract="Optionen"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Option „Erstellen“"
>abstract="Option „Erstellen“"

Adobe Campaign Web verfügt über technische Optionen, mit denen Sie die Anwendung genauer konfigurieren können. Einige dieser Optionen sind schon integriert, während andere bei Bedarf manuell hinzugefügt werden können.

>[!IMPORTANT]
>Die integrierten Optionen sind vorkonfiguriert und sollten nur von erfahrenen Benutzenden geändert werden. Wenden Sie sich bei Fragen oder Wünschen an den Adobe-Support.

## Zugriff auf Campaign-Optionen {#access}

Optionen sind im Menü **[!UICONTROL Administration]** > **[!UICONTROL Optionen]** verfügbar. Verwenden Sie den Filterbereich, um die Liste einzugrenzen und schnell die benötigte Option zu finden.

![](assets/options-list.png)\
[Optionsliste, die im Menü „Administration“ > „Optionen“ angezeigt wird]

>[!NOTE]
>Obwohl die Position des Menüs „Optionen“ in der Adobe Campaign-Konsole im Vergleich zur Web-Benutzeroberfläche abweicht, ist die Liste identisch und agiert wie ein Spiegel. Weitere Informationen zu den verfügbaren Optionen finden Sie in der Optionsliste in der [Dokumentation zu Campaign v7](https://experienceleague.adobe.com/de/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}.

Über die Optionsliste haben Sie folgende Möglichkeiten:

* **Option duplizieren oder löschen**: Klicken Sie auf die Schaltfläche mit den Auslassungspunkten und wählen Sie die gewünschte Aktion aus.
* **Option ändern**: Klicken Sie auf den Namen der Option, um ihre Eigenschaften zu öffnen. Nehmen Sie Ihre Änderungen vor und speichern Sie sie.
* **Benutzerdefinierte Option erstellen**: Klicken Sie auf die Schaltfläche **[!UICONTROL Option erstellen]**.

## Erstellen einer Option {#create}

Die Adobe Campaign Web-Benutzeroberfläche ermöglicht es Ihnen, benutzerdefinierte Optionen für Ihre Anforderungen zu erstellen. Dies ist besonders nützlich, wenn Sie mit Workflow-Aktivitäten arbeiten, die **[!UICONTROL JavaScript-Code]** verwenden, um Zwischenergebnisse zu speichern.

So erstellen Sie eine Option:

1. Greifen Sie auf die Optionsliste zu und klicken Sie auf **[!UICONTROL Option erstellen]**.
1. Geben Sie einen Namen für die Option ein, wählen Sie ihren Typ aus und legen Sie den gewünschten Wert fest.
1. Klicken Sie auf **[!UICONTROL Erstellen]**, um die Option zu erstellen. 

![Benutzeroberfläche „Option erstellen“ mit Feldern für Name, Typ und Wert](assets/options-create.png)

Optionen können als temporärer Speicherplatz für Daten dienen und bieten die folgenden Vorteile:

* Eingegebene Werte: Optionen unterstützen bestimmte Datentypen, z. B. Datumsangaben, Ganzzahlen, Strings usw.
* Flexibilität: Mit Optionen können die Benutzenden Daten effizient speichern und abrufen, ohne Datenbanktabellen aufwändig verwalten zu müssen.

Im folgenden Beispiel wird eine benutzerdefinierte Option namens `sampleOption` mit dem Anfangswert „a“ erstellt. Die Aktivität **[!UICONTROL JavaScript-Code]** in einem Workflow ändert den Wert dieser Option und speichert ihn in einer Variablen. Der aktualisierte Wert wird in den Workflow-Protokollen angezeigt und im Menü **[!UICONTROL Optionen]** angezeigt.

1. Erstellen Sie die Option.

   ![Benutzeroberfläche zur Erstellung einer benutzerdefinierten Option namens `sampleOption` mit dem Anfangswert „a“](assets/options-sample-create.png)

1. Konfigurieren Sie eine Aktivität **[!UICONTROL JavaScript-Code]** und starten Sie den Workflow.

   ![Benutzeroberfläche für die Konfiguration der Aktivität „JavaScript-Code“](assets/options-sample-javascript.png)

1. Führen Sie den Workflow aus, um den aktualisierten Wert in den Workflow-Protokollen anzuzeigen.

   ![Workflow-Protokolle mit dem aktualisierten Wert der benutzerdefinierten Option](assets/options-sample-logs.png)

1. Der aktualisierte Wert ist jetzt im Menü **[!UICONTROL Optionen]** sichtbar.

   ![Menü „Optionen“ mit dem aktualisierten Wert der benutzerdefinierten Option](assets/options-sample-updated.png)
