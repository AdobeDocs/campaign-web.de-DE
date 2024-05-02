---
audience: end-user
title: Nutzung der Aktivität An-/Abmeldedienst
description: Erfahren Sie, wie Sie die Workflow-Aktivität "An-/Abmeldedienst"verwenden
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 23%

---

# Abonnementdienste {#subscriptipon-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Aktivität &quot;Anmeldedienste&quot;"
>abstract="Mit der Aktivität An-/Abmeldedienst können mehrere Profile in einer einzigen Aktion für einen Dienst angemeldet oder von einem Dienst abgemeldet werden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Allgemeine Parameter des Anmeldedienstes"
>abstract="Wählen Sie den gewünschten Dienst aus und wählen Sie die auszuführende Aktion aus (An- oder Abmeldung). Ein-/Ausschalten der **Bestätigungsnachricht senden** -Option, um die Population darüber zu informieren, dass sie den ausgewählten Dienst abonniert oder abbestellt hat."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Ausgehende Transition erzeugen"
>abstract="Schalten Sie die Option **Ausgehende Transition erzeugen** ein, um eine Transition nach der Aktivität hinzuzufügen."

Die **Abonnementdienste** -Aktivität **Data Management** -Aktivität. Damit können Sie ein Abonnement für einen Informationsdienst für die in der Transition angegebene Population erstellen oder löschen.

## Konfigurieren der Aktivität An-/Abmeldedienst {#subscription-services-configuration}

Führen Sie die folgenden Schritte aus, um die **Abonnementdienste** Aktivität:

1. Hinzufügen einer **Abonnementdienste** in Ihren Workflow ein. Sie können diese Aktivität verwenden, nachdem Sie Profile ausgewählt oder eine Datei mit identifizierten Daten importiert haben.

1. Wählen Sie mit einer der folgenden Optionen den Dienst aus, für den Sie die Abonnements verwalten möchten:

   * **[!UICONTROL Auswählen eines bestimmten Dienstes]**: Wählen Sie einen Dienst manuell mithilfe der **[!UICONTROL Dienst]** -Feld.

   * **[!UICONTROL Aus der eingehenden Transition]**: Verwenden Sie den in der eingehenden Transition angegebenen Dienst. Beispielsweise können Sie eine Datei importieren, in der der zu verwaltende Dienst für jede Zeile spezifiziert wird. Der Dienst, für den der Vorgang ausgeführt werden soll, wird dann für jedes Profil dynamisch ausgewählt.

   ![](../assets/workflow-subscription-service.png)

1. Wählen Sie den auszuführenden Vorgang aus: **Abonnieren** oder **Abmelden**.

   Wenn der Dienst in der eingehenden Transition definiert ist, können Sie auswählen, wie dieser Vorgang abgerufen werden soll:

   * **Auswählen eines bestimmten Vorgangstyps**: Wählen Sie den auszuführenden Vorgang manuell aus (**Abonnieren** oder **Abmelden**)

   * **Einen Vorgangstyp aus einem Pfad der eingehenden Transition auswählen**: Wählen Sie die Spalte der eingehenden Daten aus, die den für jeden Datensatz auszuführenden Vorgang angibt. Beispielsweise können Sie eine Datei importieren, die den Vorgang angibt, der für jede Zeile in einer Spalte &quot;Vorgang&quot;ausgeführt werden soll.

     >[!NOTE]
     >
     >Hier können nur boolesche oder ganzzahlige Felder ausgewählt werden. Stellen Sie sicher, dass die Daten, die den auszuführenden Vorgang enthalten, diesem Format entsprechen. Wenn Sie beispielsweise Daten aus einer Datei laden -Aktivität laden, überprüfen Sie, ob Sie das Format der Spalte, die den Vorgang enthält, im **[!UICONTROL Datei laden]** -Aktivität. Ein Beispiel finden Sie unter [diesem Abschnitt](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Um Empfänger darüber zu informieren, dass sie den ausgewählten Dienst abonniert haben oder sich von ihm abgemeldet haben, aktivieren Sie die Option **[!UICONTROL Bestätigungsnachricht senden]** aktiviert. Der Inhalt dieser Benachrichtigung wird in einer Versandvorlage definiert, die dem Informationsdienst zugeordnet ist.

1. Wenn Sie Daten aus einer eingehenden Transition verwenden, wird eine **[!UICONTROL Zusätzliche Informationen]** -Bereich angezeigt, in dem Sie die Daten und den Ursprung des Abonnements für jeden Datensatz angeben können. Sie können diesen Abschnitt leer lassen. In diesem Fall wird bei Ausführung des Workflows kein Datum oder keine Herkunft festgelegt.

   * Wenn die eingehenden Daten eine Spalte enthalten, die das Abonnementdatum des Profils für den Dienst angibt, können Sie diese im **[!UICONTROL Datum]** -Feld.

   * Im **[!UICONTROL Ausgangspfad]** -Feld den Ursprung des Abonnements angeben. Sie können ihn auf eines der Felder der eingehenden Daten oder auf einen konstanten Wert Ihrer Wahl setzen, indem Sie die Option **[!UICONTROL Konstante als Ursprung festlegen]** -Option.

   ![](../assets/workflow-subscription-service-additional.png)

1. Um eine ausgehende Transition nach der Aktivität hinzuzufügen, können Sie die **[!UICONTROL Ausgehende Transition erzeugen]** aktiviert.

## Beispiele {#example}

### Abonnieren einer Audience für einen bestimmten Dienst {#uc1}

Dieser Workflow unten zeigt, wie Sie eine Audience für einen vorhandenen Dienst abonnieren können.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL Audience erstellen]** -Aktivität auf eine bestehende Zielgruppe ausgerichtet ist.

* A **[!UICONTROL An-/Abmeldedienst]** -Aktivität können Sie den Dienst auswählen, für den die Profile angemeldet sein müssen.

### Mehrere Abonnementstatus über eine Datei aktualisieren {#uc2}

Der folgende Workflow zeigt, wie eine Datei mit Profilen importiert und ihr Abonnement für mehrere in der Datei angegebene Dienste aktualisiert wird.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Datei laden]** -Aktivität lädt eine CSV-Datei mit den Daten und definiert die Struktur der importierten Spalten. In den Spalten &quot;Dienst&quot;und &quot;Vorgang&quot;werden der zu aktualisierende Dienst und der auszuführende Vorgang (An- oder Abmeldung) angegeben.

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Der Vorgang wird in der Datei als &quot;sub&quot; oder &quot;unsub&quot; spezifiziert. Vom System wird ein **boolescher** Wert oder eine **Integer** erwartet, der/die angibt, welcher Vorgang ausgeführt werden soll: Mit &quot;0&quot; wird eine Abmeldung vorgenommen und mit &quot;1&quot; eine Anmeldung. Um dieser Anforderung zu entsprechen, muss eine Neukodifizierung der Werte im Detail der Spalte &quot;Vorgang&quot; im Konfigurationsbildschirm der Beispieldatei durchgeführt werden.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Wenn in Ihrer Datei der Vorgang bereits mit &quot;0&quot; und &quot;1&quot; spezifiziert ist, müssen Sie diese Werte nicht erneut kodifizieren. Vergewissern Sie sich nur, dass die Spalte als **Boolesch** oder **Ganzzahl** in den Beispieldateispalten.

* Mit der Aktivität **[!UICONTROL Abstimmung]** werden die Daten der Datei als der Profildimension der Adobe Campaign-Datenbank zugehörig identifiziert. Die **email** -Feld der Datei mit dem **email** -Feld der Profilressource.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* Ein **[!UICONTROL Anreicherung]** -Aktivität erstellt eine Verknüpfung zur Tabelle &quot;Dienste (nms)&quot;und erstellt eine einfache Verknüpfung zwischen der Spalte &quot;Dienst&quot;der hochgeladenen Datei und dem Feld &quot;Interner Name&quot;der Dienste in der Datenbank.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Deduplizierung]** basierend auf der **email** -Feld gibt Dubletten an. Die Eliminierung von Dubletten ist wichtig, da andernfalls die Anmeldung für einen Dienst für alle Daten fehlschlägt.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)

* Mit der Aktivität **[!UICONTROL An-/Abmeldedienst]** werden die zu aktualisierenden, von der Transition stammenden Dienste über die in der Aktivität **[!UICONTROL Abstimmung]** erstellte Verknüpfung identifiziert.

  Der **[!UICONTROL Kampagnentyp]** wird über das **operation**-Feld der Datei identifiziert. Hier können nur die Felder „Boolesch“ oder „Integer“ ausgewählt werden. Wenn die Spalte Ihrer Datei, die den auszuführenden Vorgang enthält, nicht in der Liste erscheint, vergewissern Sie sich, dass Sie Ihr Spaltenformat in der Aktivität **[!UICONTROL Datei laden]** richtig eingerichtet haben, wie zuvor in diesem Beispiel erläutert.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
