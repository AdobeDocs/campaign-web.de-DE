---
title: Steuern von Aktionen für Daten
description: Erfahren Sie, wie Sie die Aktionen zum Erstellen, Bearbeiten und Löschen von benutzerdefinierten Schemaeinträgen einschränken können.
source-git-commit: 75aeccc9878bb0aab7bdaf62113303dbd14f985b
workflow-type: ht
source-wordcount: '386'
ht-degree: 100%

---

# Steuern von Aktionen für Daten {#action-data}

>[!CONTEXTUALHELP]
>id="acw_schema_action_data"
>title="Aktionsdaten"
>abstract="Konfigurieren Sie die Aktionen, die für die Detail- und Listenbildschirme des Schemas verfügbar sind. Aktivieren Sie die Option **[!UICONTROL Schreibgeschützt]**, um den Detailbildschirm als schreibgeschützt festzulegen und Aktionen aus der Liste zu entfernen. Aktivieren Sie die Option **[!UICONTROL Löschen nicht zulassen]** um die Löschaktion aus den Detail- und Listenbildschirmen zu entfernen."

Im Abschnitt **[!UICONTROL Aktionsdaten]** können Sie die Aktionen einschränken, die für die Einträge eines benutzerdefinierten Schemas verfügbar sind, unabhängig von den [Sicherheitsregeln](../get-started/work-with-folders.md), die für einzelne Ordner konfiguriert wurden. Diese Einschränkung gilt auf Schemaebene, in jedem Ordner, für jede Benutzerin bzw. jeden Benutzer, einschließlich Admins.

>[!NOTE]
>
>Dieser Abschnitt ist nur für benutzerdefinierte Schemata verfügbar.

Weitere Informationen zum Bildschirm „Bildschirmdefinition“ und zum Zugriff darauf finden Sie im Abschnitt [Zugreifen auf die Bildschirmdefinition](schemas-browse-access.md#screen-def).

Um die Aktionsdaten zu konfigurieren, gehen Sie wie folgt vor:

1. Navigieren Sie zum Menü **[!UICONTROL Schemata]** und suchen Sie mithilfe der Filter nach bearbeitbaren Schemata.

1. Wählen Sie den Schemanamen in der Liste aus, um das Schema zu öffnen, und klicken Sie in der Ansicht der Schemadetails auf die Schaltfläche **[!UICONTROL Bildschirmbearbeitung]**, um die Bildschirmdefinition aufzurufen.

1. Scrollen Sie nach unten zum Abschnitt **[!UICONTROL Aktionsdaten]** am Ende der Bildschirmdefinition.

   ![Abschnitt „Aktionsdaten“ in der Bildschirmdefinition](assets/schemas-action-data1.png)

1. Wählen Sie eine der verfügbaren Optionen oder beide aus:

   * **[!UICONTROL Schreibgeschützt]**: Der Detailbildschirm wird für alle Benutzenden schreibgeschützt. In der Liste ist keine Aktion zum Erstellen, Duplizieren, Aktualisieren oder Löschen verfügbar, und die Aktionen zum Löschen und Duplizieren sind im Detailbildschirm ausgeblendet. Die Auswahl dieser Option ähnelt der Konfiguration einer Ansicht: Benutzende können weiterhin Einträge öffnen und wiederverwenden, z. B. bei der Zielgruppenbestimmung für einen Versand, aber sie können diese nicht ändern.

   * **[!UICONTROL Löschen nicht zulassen]**: Die Löschaktion wird in jedem Ordner aus dem Detailbildschirm und aus der Liste entfernt. Andere Aktionen wie Erstellen, Duplizieren und Aktualisieren bleiben verfügbar.

     >[!NOTE]
     >
     >Bei Aktivierung der Option **[!UICONTROL Schreibgeschützt]** wird das Löschen auch automatisch abgedeckt, sodass die Option **[!UICONTROL Löschen nicht zulassen]** deaktiviert ist, während **[!UICONTROL Schreibgeschützt]** aktiviert ist.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

1. Navigieren Sie zur Liste der Einträge für dieses Schema, um das Ergebnis zu überprüfen.

   In diesem Beispiel ist **[!UICONTROL Schreibgeschützt]** aktiviert: Die Aktionen zum Löschen und Duplizieren werden in der Liste nicht mehr angezeigt.

   ![Schreibgeschütztes Rendern im Listenbildschirm](assets/schemas-action-data2.png)

1. Öffnen Sie einen Eintrag, um den Detailbildschirm zu überprüfen. Die zugehörigen Felder werden angezeigt, ohne dass eine Bearbeitung möglich ist.

   ![Schreibgeschütztes Rendern im Detailbildschirm](assets/schemas-action-data3.png)
