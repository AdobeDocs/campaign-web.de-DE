---
title: Frühzeitige Versionshinweise zur Web-Benutzeroberfläche von Campaign v8
description: Entdecken Sie die neuen Funktionen der nächsten Version der Campaign Web-Benutzeroberfläche
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: d4f9f3562f7dc2550bf9fea01f27456fdfdad43e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 46%

---

# Frühzeitige Versionshinweise {#e-release}

Die Adobe Campaign Web-Benutzeroberfläche bietet kontinuierlich neue Funktionen, Verbesserungen vorhandener Funktionen und Fehlerbehebungen. Alle Änderungen werden am Ende jedes Monats in den [Versionshinweisen](release-notes.md) konsolidiert.

**Die nachfolgenden frühzeitigen Versionshinweise können ohne vorherige Ankündigung bis zum Verfügbarkeitsdatum der Version geändert werden**. Links, Bildschirme und die aktualisierte Dokumentation werden am Veröffentlichungsdatum in den [Versionshinweisen](release-notes.md) veröffentlicht.

## Versionshinweise Juli {#24-7-release}

**Veröffentlichungsdatum**: 30.-31. Juli 2024

Die folgenden Funktionen und Verbesserungen sind ab der Juli-Version verfügbar.

### Testlisten {#24-7-2}

Eine Testliste, auch bezeichnet als  **Trap-Gruppe**, ist eine Liste von Testadressen. Sie wird verwendet, um bestimmte Adressen in Ihre Sendungen einzubeziehen und dann Profile auszuwählen, die nicht den definierten Zielgruppenkriterien entsprechen. Auf diese Weise können Empfängerinnen und Empfänger, die außerhalb der Versandzielgruppe liegen, die Nachricht ebenso wie jede andere Person innerhalb der Zielgruppe erhalten.  Sie können Testadressen beim Versand von Testsendungen oder zum Schutz Ihrer Mailing-Liste verwenden.

### Vorlagen für Rich-Push-Benachrichtigungen {#24-7.3}

Sie können jetzt Rich-Push-Benachrichtigungen versenden. Eine Rich-Push-Benachrichtigung ist eine erweiterte Form der Mobile-Benachrichtigung, die über einfache Textnachrichten hinausgeht und Multimedia-Elemente wie Bilder, interaktive Schaltflächen oder andere Rich-Media-Inhalte enthält. Mit dieser Version sind jetzt eine Reihe von Vorlagen für Rich-Push-Benachrichtigungen für Ihre iOS- und Android-Apps verfügbar.

>[!AVAILABILITY]
>
>Diese Funktion erfordert eine Aktualisierung auf Campaign v8.6.3 oder v8.7.2. [Weitere Informationen finden Sie in den Versionshinweisen zur Campaign Client-Konsole](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes) .


### Verbesserungen {#improvements-24-7}

**Ordnerverwaltung** - Sie können jetzt Berechtigungen und Einschränkungen für Ordner verwalten.

### Neue Funktionen in eingeschränkter Verfügbarkeit {#acs-24-4}

>[!AVAILABILITY]
>
>Die folgenden Funktionen sind nur eingeschränkt verfügbar. Sie sind Kundinnen und Kunden vorbehalten, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und können nicht in anderen Umgebungen bereitgestellt werden.
>
>Weitere Informationen finden Sie auf den folgenden Seiten der Dokumentation: [Wechsel von Campaign Standard zu Campaign v8](../rn/acs-migration.md) und [Funktionen für Campaign Standard-Benutzende](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=de).

#### Inhaltsfragmente {#LA-24-7}

Sie können jetzt Inhaltsfragmente erstellen und verwenden. Ein Inhaltsfragment ist eine wiederverwendbare Komponente, die in einer oder mehreren Nachrichten referenziert werden kann. Beim Ändern eines Fragments wird jeder Inhalt, der dieses verwendet, aktualisiert. Mit dieser Funktion können Sie mehrere benutzerdefinierte Inhaltsbausteine vorab erstellen, die von Marketing-Benutzern verwendet werden können, um Nachrichteninhalte in einem verbesserten Designprozess schnell zusammenzustellen.

Es stehen zwei Fragmenttypen zur Verfügung:

* **Ausdrucksfragmente** sind vordefinierte Ausdrücke, die über einen dedizierten Eintrag im Ausdruckseditor verfügbar sind.
* **Visuelle Fragmente** sind vordefinierte visuelle Bausteine, die Sie in mehreren E-Mail-Sendungen oder in Inhaltsvorlagen wiederverwenden können. [Weitere Informationen](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >**Visuelle Fragmente** befinden sich in begrenzter Verfügbarkeit (LA). Diese Funktion ist auf Kunden beschränkt, die **von Adobe Campaign Standard zu Adobe Campaign v8** migrieren, und kann in keiner anderen Umgebung bereitgestellt werden.
