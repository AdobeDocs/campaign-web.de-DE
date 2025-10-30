---
title: Verwalten eines externen Kontos
description: Informationen zum Konfigurieren externer Konten
exl-id: 8f41312e-422f-4be1-b874-1b143c500912
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: tm+mt
source-wordcount: '3892'
ht-degree: 100%

---

# Externe Datenbankkonten {#external-accounts}

Verwenden Sie ein externes Konto vom Typ „Externe Datenbank“, um Adobe Campaign mit einer Drittanbieterdatenbank zu verbinden.

Die Konfigurationseinstellungen für das externe Konto variieren je nach der Datenbank-Engine, mit der Sie eine Verbindung herstellen. Detaillierte Anweisungen zu den einzelnen unterstützten Datenbanken finden Sie in den folgenden Abschnitten.

## Amazon Redshift

Über das externe Konto „Amazon Redshift“ können Sie Ihre Campaign-Instanz mit Ihrer externen Amazon Redshift-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Amazon Redshift“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Amazon Redshift“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Amazon Redshift]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Amazon Redshift

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Redshift-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den RedShift-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign ausgeführt werden soll.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Amazon Redshift“.](assets/ext-account-amazon.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Redshift-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

1. Verknüpfen Sie Ihr **[!UICONTROL Speicherkonto]**, um die Leistung zu optimieren und schnellere Datenladevorgänge zwischen Adobe Campaign und Amazon Redshift zu ermöglichen.

1. Geben Sie Ihre **[!UICONTROL Kontorolle]** ein, die die Berechtigungen bestimmt, die Adobe Campaign bei der Interaktion mit Ihrer Redshift-Umgebung verwenden wird.

## Amazon Redshift (veraltet)

Über das externe Konto „Amazon Redshift (veraltet)“ können Sie Ihre Campaign-Instanz mit Ihrer externen Amazon Redshift-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Amazon Redshift (veraltet)“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Amazon Redshift (veraltet)“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Amazon Redshift (veraltet)]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Amazon Redshift (veraltet)

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Redshift-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den RedShift-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign ausgeführt werden soll.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Amazon Redshift (veraltet)“.](assets/ext-account-amazon-legacy.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Redshift-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## Azure Synapse Analytics

Über das externe Konto „Azure Synapse Analytics“ können Sie Ihre Campaign-Instanz mit Ihrer externen Azure Synapse-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Azure Synapse Analytics“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Amazon Redshift“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Azure Synapse Analytics]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Azure Synapse Analytics

   * **[!UICONTROL Server]**: Geben Sie die URL des Azure Synapse-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Benutzernamen an, der für die Authentifizierung bei der Synapse-Datenbank verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Konto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie die Zieldatenbank an, mit der Adobe Campaign eine Verbindung herstellen soll.

   * **[!UICONTROL Präfix für Tabellen und Funktionen]**: Standardmäßig ist dies auf den Kontonamen festgelegt. Sie können diese Option anpassen, wenn Sie ein anderes Präfix zum Identifizieren von Campaign-bezogenen Objekten verwenden möchten.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Azure Synapse Analytics“.](assets/ext-account-azure.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Azure Synapse Analytics“.](assets/ext-account-azure-2.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Azure Synapse Analytics-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## Databricks

Über das externe Konto „Databricks“ können Sie Ihre Campaign-Instanz mit Ihrer externen Databricks-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Databricks“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Databricks“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Databricks]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Databricks

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Databricks-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Databricks-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Katalog]**: Geben Sie den Katalog an, den Sie verwenden möchten.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign seine Arbeitsobjekte erstellen und verwalten soll.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Databricks“.](assets/ext-account-databricks.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Databricks-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

1. Verknüpfen Sie Ihr **[!UICONTROL Speicherkonto]**, um die Leistung zu optimieren und schnellere Datenladevorgänge zwischen Adobe Campaign und Databricks zu ermöglichen.

## Google BigQuery

Über das externe Konto „Google BigQuery“ können Sie Ihre Campaign-Instanz mit Ihrer externen Google BigQuery-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Google BigQuery“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Google BigQuery“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Google BigQuery]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Google BigQuery

   * **[!UICONTROL Konto]**: Geben Sie den Benutzernamen oder das Service-Konto ein, den bzw. das Adobe Campaign für die Verbindung mit BigQuery verwenden soll.

   * **[!UICONTROL Upload-Methode für Anmeldedatei]**: Wählen Sie aus, wie der Schlüssel für das Service-Konto bereitgestellt werden soll. Geben Sie entweder den Pfad der Schlüsseldatei manuell ein oder laden Sie die Schlüsseldatei direkt auf den Server hoch.

   * **[!UICONTROL Server]**: Wenn Sie die Option für die manuelle Eingabe auswählen, geben Sie die Server-URL an.

   * **[!UICONTROL Projekt]**: Geben Sie die Google Cloud-Projekt-ID an, die mit Ihrer BigQuery-Instanz verknüpft ist.

   * **[!UICONTROL Datensatz]**: Geben Sie den Namen des Datensatzes ein, in dem Adobe Campaign Daten speichert und abfragt.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Google BigQuery“.](assets/ext-account-google.png)

1. Fügen Sie unter **[!UICONTROL Parameter]** den Inhalt der JSON-Schlüsseldatei für das Service-Konto ein, um Adobe Campaign bei Google BigQuery zu authentifizieren.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Google BigQuery-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

1. Wenn Ihre Umgebung Proxy-Zugriff zum Herstellen einer Verbindung zum BigQuery-Server benötigt, konfigurieren Sie die Proxy-Einstellungen.

   Wählen Sie zunächst Ihren Proxy-Typ aus: „http“, „http_no_tunnel“, „socks4“ oder „socks5“.

1. Füllen Sie die folgenden Felder zur Proxy-Konfiguration aus, um einen sicheren Zugriff zu ermöglichen:

   * **[!UICONTROL Proxy-Host]**: Die Adresse des Proxy-Servers.
   * **[!UICONTROL Proxy-Port]**: Der vom Proxy-Server verwendete Port.
   * **[!UICONTROL Proxy-UID]**: Die Benutzer-ID für die Authentifizierung beim Proxy-Server, falls erforderlich.
   * **[!UICONTROL Proxy-Host]**: Das Passwort, das der Proxy-UID entspricht (falls zutreffend).

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Google BigQuery“.](assets/ext-account-google-2.png)

## Microsoft SQL Server

Über das externe Konto „Microsoft SQL Server“ können Sie Ihre Campaign-Instanz mit Ihrer externen Microsoft SQL Server-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Microsoft SQL Server“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Microsoft SQL Server“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Microsoft SQL Server]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Microsoft SQL Server

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Microsoft SQL-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Microsoft SQL Server-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Präfix für Tabellen und Funktionen]**: Standardmäßig ist dies auf den Kontonamen festgelegt. Sie können diese Option anpassen, wenn Sie ein anderes Präfix zum Identifizieren von Campaign-bezogenen Objekten verwenden möchten.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Microsoft SQL Server“.](assets/ext-account-microsoft-sql.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Microsoft SQL Server-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## MySQL

Über das externe Konto „MySQL“ können Sie Ihre Campaign-Instanz mit Ihrer externen MySQL-Datenbank verbinden.
Konfigurieren Sie Ihr externes Konto „MySQL“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „MySQL“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL MySQL]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: MySQL

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres MySQL-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den MySQL-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „MySQL“.](assets/ext-account-mysql.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer MySQL-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## Netezza

Über das externe Konto „Netezza“ können Sie Ihre Campaign-Instanz mit Ihrer externen Netezza-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Netezza“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Netezza“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Netezza]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Netezza

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Netezza-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Netezza-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Netezza“.](assets/ext-account-netezza.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Netezza-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## ODBC (Sybase ASE, Sybase IQ)

Über das externe Konto „ODBC (Sybase ASE, Sybase IQ)“ können Sie Ihre Campaign-Instanz mit Ihrer externen Datenbank des Typs „ODBC (Sybase ASE, Sybase IQ)“ verbinden.
Konfigurieren Sie Ihr externes Konto „ODBC (Sybase ASE, Sybase IQ)“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „ODBC (Sybase ASE, Sybase IQ)“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL ODBC (Sybase ASE, Sybase IQ)]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: ODBC (Sybase ASE, Sybase IQ)

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Servers für ODBC (Sybase ASE, Sybase IQ) ein.

   * **[!UICONTROL Konto]**: Geben Sie den Namen des Servers für ODBC (Sybase ASE, Sybase IQ) an, der für die Authentifizierung verwendet wird.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Sammel-Einfügewerkzeug]**: Geben Sie den vollständigen Pfad zum ausführbaren Sammel-Einfügewerkzeug an.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „ODBC“.](assets/ext-account-odbc.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer ODBC-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## HTTP-Weiterleitung auf Remote-Datenbank

Über das externe Konto „HTTP-Weiterleitung auf Remote-Datenbank“ können Sie Ihre Campaign-Instanz mit Ihrer externen Datenbank des Typs „HTTP-Weiterleitung auf Remote-Datenbank“ verbinden.

Konfigurieren Sie Ihr externes Konto „HTTP-Weiterleitung auf Remote-Datenbank“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Amazon Redshift“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL HTTP-Weiterleitung auf Remote-Datenbank]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: HTTP-Weiterleitung auf Remote-Datenbank

   * **[!UICONTROL Server]**: Geben Sie die vollständige URL des HTTP-Weiterleitungs-Servers ein, der eine Verbindung zu Ihrer Remote-Datenbank herstellt.

   * **[!UICONTROL Konto]**: Geben Sie den Benutzernamen an, der für die Authentifizierung beim HTTP-Weiterleitungs-Server verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit diesem Konto verknüpfte Passwort ein.

   * **[!UICONTROL Datenquelle]**: Geben Sie die Zieldatenbank an, mit der sich Adobe Campaign über das Relais verbinden soll.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „HTTP-Weiterleitung auf Remote-Datenbank“.](assets/ext-account-azure.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Remote-Datenbank des Typs „HTTP-Weiterleitung auf Remote-Datenbank“. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## Oracle

Über das externe Konto „Oracle“ können Sie Ihre Campaign-Instanz mit Ihrer externen Oracle-Datenbank verbinden.
Konfigurieren Sie Ihr externes Konto „Oracle“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Oracle“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Oracle]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Oracle

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Oracle-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Oracle-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Oracle“.](assets/ext-account-oracle.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Oracle-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## PostgreSQL

Über das externe Konto „PostgreSQL“ können Sie Ihre Campaign-Instanz mit Ihrer externen PostgreSQL-Datenbank verbinden.
Konfigurieren Sie Ihr externes Konto „PostgreSQL“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „PostgreSQL“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL PostgreSQL]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: PostgreSQL

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres PostgreSQL-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den PostgreSQL-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign seine Arbeitsobjekte erstellen und verwalten soll.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „PostgreSQL“.](assets/ext-account-postgresql.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer PostgreSQL-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## SAP HANA

Über das externe Konto „SAP HANA“ können Sie Ihre Campaign-Instanz mit Ihrer externen SAP HANA-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „SAP HANA“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „SAP HANA“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL SAP HANA]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: SAP HANA

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres SAP HANA-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den SAP HANA-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign seine Arbeitsobjekte erstellen und verwalten soll.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „SAP HANA“.](assets/ext-account-saphana.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer SAP HANA-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## Snowflake

Über das externe Konto „Snowflake“ können Sie Ihre Campaign-Instanz mit Ihrer externen Snowflake-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Snowflake“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Snowflake“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Snowflake]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Snowflake

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Snowflake-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Snowflake-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign seine Arbeitsobjekte erstellen und verwalten soll.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Snowflake“.](assets/ext-account-snowflake.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Snowflake-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

1. Wenn Sie die Authentifizierung über ein Schlüsselpaar verwenden, geben Sie im Menü **[!UICONTROL Schlüsselpaar-Authentifizierung]** die erforderlichen Werte für Folgendes ein:

   * **[!UICONTROL Passwort]**: Die Passphrase zum Schutz des privaten Schlüssels, falls zutreffend.

   * **[!UICONTROL Privater Schlüssel]**: Der zur Authentifizierung des Snowflake-Kontos verwendete private Schlüssel.

## Teradata

Über das externe Konto „Teradata“ können Sie Ihre Campaign-Instanz mit Ihrer externen Teradata-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Teradata“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Teradata“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Teradata]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Teradata

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Teradata-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Teradata-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Teradata“.](assets/ext-account-teradata.png)

1. Sie können die Option **[!UICONTROL Arbeits-Tablespace für Tabellen verwenden]** aktivieren und dann den **[!UICONTROL Tabellen-Tablespace]** angeben, in dem Ihre Arbeitstabellen gespeichert werden.

1. Aktivieren Sie bei Bedarf die Option **[!UICONTROL Arbeits-Tablespace für Indizes verwenden]** und geben Sie dann den **[!UICONTROL Index-Tablespace]** an.

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Teradata-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

1. Geben Sie bei Bedarf Ihr **[!UICONTROL PostConnect-Skript]** ein, wenn Sie möchten, dass nach jedem Herstellen einer Verbindung automatisch ein Skript ausgeführt wird. Wenn das Skript jedes Mal ausgeführt werden soll, aktivieren Sie die Option **[!UICONTROL Jedes Mal ausführen]**.

## Vertica Analytics

Konfigurieren Sie Ihr externes Konto „Vertica Analytics“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Vertica Analytics“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Vertica Analytics]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Vertica Analytics

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Vertica Analytics-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Vertica Analytics-Benutzernamen an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Benutzerkonto verknüpfte Passwort ein.

   * **[!UICONTROL Datenbank]**: Geben Sie den Datenbanknamen an, sofern er nicht bereits im DSN definiert ist. Lassen Sie dieses Feld leer, wenn das DSN die Datenbank enthält.

   * **[!UICONTROL Arbeitsschema]**: Geben Sie den Namen des Schemas ein, in dem Adobe Campaign seine Arbeitsobjekte erstellen und verwalten soll.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   * **[!UICONTROL Zeitzone]**: Wählen Sie die Zeitzone des Servers aus oder geben Sie sie ein, um genaue zeitbasierte Vorgänge sicherzustellen.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Vertica Analytics“.](assets/ext-account-vertica.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Vertica Analytics-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

## Microsoft Fabric {#fabric}

Über das externe Konto „Microsoft Fabric“ können Sie Ihre Campaign-Instanz mit Ihrer externen Microsoft Fabric-Datenbank verbinden.

Konfigurieren Sie Ihr externes Konto „Microsoft Fabric“ in der Adobe Campaign Web-Benutzeroberfläche.

1. [Erstellen Sie Ihr externes Konto](external-account.md) und wählen Sie **[!UICONTROL Externe Datenbank]** als **[!UICONTROL Typ]** Ihres externen Kontos und „Microsoft Fabric“ als **[!UICONTROL Anbietertyp]** aus.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

1. Um das externe Konto **[!UICONTROL Microsoft Fabric]** zu konfigurieren, füllen Sie folgende Felder aus:

   * **[!UICONTROL Typ]**: Microsoft Fabric

   * **[!UICONTROL Server]**: Geben Sie den DNS-Namen Ihres Microsoft Fabric-Servers ein.

   * **[!UICONTROL Konto]**: Geben Sie den Microsoft Fabric-Benutzernamen (oder Service-Prinzipal) an, der für die Authentifizierung verwendet werden soll.

   * **[!UICONTROL Passwort]**: Geben Sie das mit dem Konto verknüpfte Passwort oder Geheimnis ein.

   * **[!UICONTROL Optionen]**: Fügen Sie alle erweiterten Konfigurationsoptionen hinzu, die für Ihre Umgebung erforderlich sein können.

   ![Screenshot mit den Feldern zur Konfiguration des externen Kontos „Microsoft Fabric“.](assets/ext-account-fabric.png)

1. Erstellen Sie nach dem Einrichten der Verbindung die Adobe Campaign SQL-Funktionen in Ihrer Redshift-Remote-Datenbank. Sobald diese Funktionen verfügbar sind, klicken Sie auf **[!UICONTROL Funktionen bereitstellen]**, um sie zu aktivieren.

1. Verknüpfen Sie Ihr **[!UICONTROL Speicherkonto]**, um die Leistung zu optimieren und schnellere Datenladevorgänge zwischen Adobe Campaign und Microsoft Fabric zu ermöglichen.

1. Geben Sie Ihre **[!UICONTROL Kontorolle]** ein, die die Berechtigungen bestimmt, die Adobe Campaign bei der Interaktion mit Ihrer Redshift-Umgebung verwendet.
