---
audience: end-user
title: Verwalten von Kampagnenvorlagen mit Adobe Campaign Web
description: Erfahren Sie, wie Sie mit Adobe Campaign Web Kampagnenvorlagen verwalten
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 91%

---


# Kampagnenvorlagen verwalten{#manage-campaign-templates}

Alle Marketing-Kampagnen basieren auf einer Vorlage, in der die Hauptmerkmale und -funktionen gespeichert sind. Campaign verfügt über eine Reihe integrierter Vorlagen, die Ihnen bei den ersten Schritten helfen. Sie können Ihre Kampagnenvorlagen erstellen und konfigurieren und dann Kampagnen aus diesen Vorlagen erstellen.

## Erstellen einer Kampagnenvorlage

Gehen Sie wie folgt vor, um eine Kampagnenvorlage zu erstellen:

Öffnen Sie den Explorer von Campaign und gehen Sie zu Ressourcen > Vorlagen > Kampagnenvorlagen.
Klicken Sie in der Symbolleiste oberhalb der Vorlagenliste auf Neu.


Sie können die integrierte Vorlage auch duplizieren, um ihre Konfiguration wiederzuverwenden und anzupassen. Klicken Sie dazu mit der rechten Maustaste auf die Vorlage und wählen Sie Duplizieren.

Geben Sie den Titel der neuen Kampagnenvorlage ein.

Klicken Sie auf Speichern und öffnen Sie die Vorlage erneut.

Definieren Sie auf der Registerkarte Bearbeiten die Eigenschaften der Vorlage.

Wählen Sie den Link Erweiterte Kampagnenparameter.. aus, um Ihrer Kampagnenvorlage einen Workflow hinzuzufügen.



Ändern Sie den Wert für Zielgruppenbestimmungen und Workflows auf Ja und bestätigen Sie diesen. Wie Sie Funktionen hinzufügen können, erfahren Sie in diesem Abschnitt.

Die Registerkarte Zielgruppenbestimmungen und Workflows wird zur Vorlage hinzugefügt. Klicken Sie auf Workflow hinzufügen..., geben Sie einen Titel ein und klicken Sie auf OK.

Erstellen Sie Ihren Workflow entsprechend Ihren Anforderungen.



Klicken Sie auf Speichern. Ihre Vorlage kann jetzt zur Erstellung einer neuen Kampagne verwendet werden.

Die unterschiedlichen Registerkarten und Unterregisterkarten der Kampagnenvorlage ermöglichen den Zugriff auf die Einstellungen. Sie werden im Abschnitt Allgemeine Konfiguration beschrieben.

Module auswählen Der Link Erweiterte Kampagnenparameter.. ermöglicht die Aktivierung und Deaktivierung von Aufträgen für die auf dieser Vorlage basierenden Kampagnen. Wählen Sie die Funktionen aus, die Sie in den über diese Vorlage erstellten Kampagnen aktivieren möchten.



Wenn eine Funktion nicht ausgewählt ist, werden die den Prozess betreffenden Elemente (Menüs, Symbole, Optionen, Registerkarten, Unterregisterkarten usw.) nicht in der Benutzeroberfläche der Vorlage oder in den auf dieser Vorlage basierenden Kampagnen angezeigt. Die Registerkarten auf der linken Seite der Kampagnendetails und die verfügbaren Registerkarten entsprechen den in der Vorlage ausgewählten Funktionen. Wenn zum Beispiel die Funktion Ausgaben und Ziele nicht aktiviert ist, wird die entsprechende Registerkarte Budget in Kampagnen, die auf dieser Vorlage basieren, nicht angezeigt.

Im Dashboard der Kampagne werden zudem Verknüpfungen zu den Konfigurationsfenstern hinzugefügt: Wenn eine Funktionalität aktiviert ist, können Sie über einen Link im Dashboard direkt darauf zugreifen.

Konfigurationsbeispiele
Beispielsweise mit den folgenden Einstellungen:



Das Kampagnen-Dashboard zeigt Folgendes an:



Beachten Sie, dass die Registerkarte Zielgruppenbestimmungen und Workflows fehlt.

Folgende Funktionen stehen zur Verfügung:



Beachten Sie, dass die Registerkarte Budget fehlt.

Die erweiterten Einstellungen der Kampagne spiegeln diese Konfiguration ebenfalls wider.



Beachten Sie, dass die Registerkarte Genehmigungen nicht verfügbar ist.

Mit dieser Konfiguration:


Das Kampagnen-Dashboard zeigt Folgendes an:



Beachten Sie, dass die Registerkarte Zielgruppenbestimmungen und Workflows verfügbar ist, aber der Link Dokument hinzufügen fehlt.

Folgende Funktionen stehen zur Verfügung:



Beachten Sie, dass die Registerkarte Budget verfügbar ist.

Die erweiterten Einstellungen der Kampagne spiegeln diese Konfiguration ebenfalls wider.



Beachten Sie, dass die Registerkarte Genehmigungen verfügbar ist, aber die Registerkarten Kontrollpopulation und Testadressen nicht aktiviert sind.

Typologie der Module Kontrollgruppe

Wenn dieses Modul ausgewählt wird, wird ein zusätzlicher Tab in den erweiterten Parametern der Vorlage und der auf dieser Vorlage basierenden Kampagnen hinzugefügt. Die Konfiguration kann in der Vorlage oder direkt in den einzelnen Kampagnen erfolgen. Weitere Informationen zu Kontrollgruppen finden Sie in diesem Abschnitt.



Testadressen

Wenn dieses Modul ausgewählt wird, wird ein zusätzlicher Tab in den erweiterten Parametern der Vorlage und der auf dieser Vorlage basierenden Kampagnen hinzugefügt. Die Konfiguration kann in der Vorlage oder direkt in den einzelnen Kampagnen erfolgen.



Dokumente

Wenn dieses Modul ausgewählt wird, wird eine zusätzliche Registerkarte zur Registerkarte Bearbeiten der Vorlage und der auf dieser Vorlage basierenden Kampagnen hinzugefügt. Anhänge können für jede Kampagne in der Vorlage oder einzeln hinzugefügt werden. Weitere Informationen zu Dokumenten finden Sie in diesem Abschnitt.



Versandentwurf

Wenn dieses Modul ausgewählt wird, wird dem Tab Dokumente der Unter-Tab Versandentwürfe hinzugefügt, um für die Kampagne unterschiedliche Versandentwürfe zu erstellen. Weitere Informationen zu Versandentwürfen finden Sie in diesem Abschnitt.



Zielgruppenbestimmungen und Workflows

Wenn das Modul Zielgruppenbestimmungen und Workflows ausgewählt wird, wird ein Tab zum Erstellen eines oder mehrerer Workflows für Kampagnen hinzugefügt, die auf dieser Vorlage basieren. Workflows können auch auf Basis dieser Vorlage einzeln für jede Kampagne konfiguriert werden. Weitere Informationen zu Kampagnen-Workflows finden Sie in diesem Abschnitt.



Wenn dieses Modul aktiviert ist, wird die Registerkarte Vorgänge zu den erweiterten Einstellungen der Kampagne hinzugefügt, um die Reihenfolge der Prozessausführung zu definieren.

Validierungen

Wenn Sie die Validierungen aktivieren, können Sie die zu genehmigenden Prozesse und die für die Genehmigungen zuständigen Personen auswählen. Weitere Informationen zu Validierungen finden Sie in diesem Abschnitt.



Sie können wählen, ob Sie die Prozessvalidierung über die Registerkarte Genehmigungen im Abschnitt mit den erweiterten Einstellungen der Vorlagen aktivieren möchten oder nicht.

Ausgaben und Budget

Wenn dieses Modul ausgewählt wird, wird der Tab Budget den Details der Vorlage und der auf dieser Vorlage basierenden Kampagnen hinzugefügt, damit das zugehörige Budget ausgewählt werden kann.



Vorlageneigenschaften


Bei der Erstellung einer Kampagnenvorlage ist die Angabe folgender Informationen notwendig:

Geben Sie den Titel der Vorlage ein: Der Titel ist obligatorisch und wird als Standardbtitel für alle auf dieser Vorlage basierenden Kampagnen verwendet.
Kampagnenart: Die in der Dropdown-Liste angebotenen Werte entsprechen den in der Aufzählung natureOp gespeicherten Werten.
Auf dieser Seite erfahren Sie, wie Sie auf Ihre Auflistungen zugreifen und sie konfigurieren können.

Wählen Sie den Kampagnentyp: einmalig, wiederkehrend oder periodisch. Standardmäßig sind in Kampagnenvorlagen einmalige Kampagnen festgelegt. Wiederkehrende und periodische Kampagnen werden in diesem Abschnitt beschrieben.

Dauer der Kampagne an: Gemeint ist der Zeitraum, über den sich die Kampagne erstrecken wird. Bei Erstellung einer auf einer Vorlage basierenden Kampagne werden Beginn und Ende somit automatisch ausgefüllt.

Handelt es sich um eine wiederkehrende Kampagne, müssen Beginn und Ende direkt in der Vorlage angegeben werden.

Geben Sie das mit der Vorlage verknüpfte Programm an: Kampagnen, die auf dieser Vorlage basieren, sind mit dem ausgewählten Programm verknüpft.

