---
title: 'Konfigurieren von Optionen in [!DNL Campaign] '
description: Erfahren Sie, wie Sie Campaign-Optionen konfigurieren und Ihre eigenen benutzerdefinierten Optionen erstellen.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 49%

---

# Konfigurieren von Optionen in [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Options"
>abstract="Options"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Create option"
>abstract="Create option"

Adobe Campaign Web enthält technische Optionen, mit denen Sie die Anwendung spezifischer konfigurieren können. Einige dieser Optionen sind integriert, während andere bei Bedarf manuell hinzugefügt werden können.

>[!IMPORTANT]\
Die integrierten Optionen sind vorkonfiguriert und sollten nur von erfahrenen Benutzenden geändert werden. Wenden Sie sich bei Fragen oder Anfragen an Ihren Adobe-Support-Mitarbeiter.

## Zugriff auf Campaign-Optionen {#access}

Optionen sind im Menü **[!UICONTROL Administration]** > **[!UICONTROL Optionen]** verfügbar. Verwenden Sie den Filterbereich, um die Liste einzugrenzen und die benötigte Option schnell zu finden.

![](assets/options-list.png)\
[Optionsliste, die im Menü Administration / Optionen angezeigt wird]

>[!NOTE]\
Obwohl die Position des Menüs „Optionen“ in der Adobe Campaign-Konsole im Vergleich zur Web-Benutzeroberfläche abweicht, ist die Liste identisch und agiert wie ein Spiegel. Weitere Informationen zu den verfügbaren Optionen finden Sie in der Optionsliste in der [ zu Campaign v7](https://experienceleague.adobe.com/de/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}.

Über die Optionsliste haben Sie folgende Möglichkeiten:

* **Option duplizieren oder löschen**: Klicken Sie auf die Schaltfläche mit den Auslassungspunkten und wählen Sie die gewünschte Aktion aus.
* **Option ändern**: Klicken Sie auf den Namen der Option, um ihre Eigenschaften zu öffnen. Nehmen Sie Ihre Änderungen vor und speichern Sie sie.
* **Benutzerdefinierte Option erstellen**: Klicken Sie auf die Schaltfläche **[!UICONTROL Option erstellen]**.

## Erstellen einer Option {#create}

Mit der Web-Benutzeroberfläche von Adobe Campaign können Sie benutzerdefinierte Optionen erstellen, die Ihren Anforderungen entsprechen. Dies ist besonders nützlich, wenn Sie mit Workflow-Aktivitäten arbeiten, die **[!UICONTROL JavaScript-Code]** verwenden, um Zwischenergebnisse zu speichern.

So erstellen Sie eine Option:

1. Greifen Sie auf die Optionsliste zu und klicken Sie auf **[!UICONTROL Option erstellen]**.
1. Geben Sie einen Namen für die Option ein, wählen Sie ihren Typ aus und legen Sie den gewünschten Wert fest.
1. Klicken Sie auf **[!UICONTROL Erstellen]**, um die Option zu erstellen. 

![Erstellen Sie eine Optionsoberfläche, die Felder für Name, Typ und Wert enthält](assets/options-create.png)

Optionen können als temporärer Speicher für -Daten dienen und die folgenden Vorteile bieten:

* Eingegebene Werte: Optionen unterstützen bestimmte Datentypen wie Datumsangaben, Ganzzahlen, Zeichenfolgen usw.
* Flexibilität: Mit Optionen können die Benutzenden Daten effizient speichern und abrufen, ohne Datenbanktabellen aufwändig verwalten zu müssen.

Im folgenden Beispiel wird eine benutzerdefinierte Option mit dem Namen `sampleOption` mit dem Anfangswert „a“ erstellt. Eine Aktivität vom Typ **[!UICONTROL JavaScript]** Code&#39; in einem Workflow ändert den Wert dieser Option und speichert ihn in einer Variablen. Der aktualisierte Wert wird in den Workflow-Protokollen angezeigt und im Menü **[!UICONTROL Optionen]** angezeigt.

1. Erstellen Sie die Option.

   ![Benutzeroberfläche zur Erstellung benutzerdefinierter Optionen mit dem Namen `sampleOption` und dem Anfangswert „a“](assets/options-sample-create.png)

1. Konfigurieren Sie eine Aktivität **[!UICONTROL JavaScript-Code]** und starten Sie den Workflow.

   ![Konfigurationsschnittstelle für JavaScript-Code-Aktivitäten](assets/options-sample-javascript.png)

1. Führen Sie den Workflow aus, um den aktualisierten Wert in den Workflow-Protokollen anzuzeigen.

   ![Workflow-Protokolle, die den aktualisierten Wert der benutzerdefinierten Option anzeigen](assets/options-sample-logs.png)

1. Der aktualisierte Wert ist jetzt im Menü **[!UICONTROL Optionen]** sichtbar.

   ![Menü „Optionen“ mit dem aktualisierten Wert der benutzerdefinierten Option](assets/options-sample-updated.png)