---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: '''Workfront Fusion-lanseringsaktivitet: Vecka 11 januari 2021"'
description: Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 11 januari 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 0%

---

# Versionsaktivitet för Workfront Fusion: 11 januari 2021

Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 11 januari 2021.

En lista med alla senaste ändringar finns på [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

En lista med de senaste felkorrigeringarna i Workfront Fusion finns i [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) och sök efter uppdateringar som heter Workfront Fusion Maintenance Update.

## Widen Connector och moduler är nu tillgängliga

Nu kan du använda Workfront Fusion för att ansluta till ditt Widen-konto. Med Widen-modulerna kan du

* Lägga till resurser i eller ta bort resurser från en samling
* Hämta eller överföra filer
* Läs eller uppdatera metadata för resurser
* Sök efter resurser baserat på villkor som du anger
* Hämta en lista med resurser i en samling
* Utför ett anpassat API-anrop.

Mer information finns i [Bredda moduler](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Datadogganslutning och moduler är nu tillgängliga

Nu kan du använda Workfront Fusion för att ansluta till ditt Datadog-konto.

Med datadoggmodulerna kan du

* Bokför tidsuppgiftspunkter
* Utför ett anpassat API-anrop

Mer information om datadoggmoduler finns i [Datadogmoduler](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Nu finns händelseanslutning och moduler

Nu kan du använda Workfront Fusion 2.0 för att ansluta till ditt Cvent-konto.

Med händelsemodlingarna kan du:

* Skapa en mötesförfrågan
* Läs poster som kontakter, händelser eller inbjudningar
* Visa poster baserat på villkor som du anger
* Registrera eller lägga till inbjudningar till specifika evenemang
* Uppdatera eller ta bort kontakter
* Göra ett anpassat API-anrop

Mer information om tillgängliga händelsemoduler finns i [Kundmoduler](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Koppling och moduler för Microsoft Dynamics 365 är nu tillgängliga

Nu kan du använda Workfront Fusion 2.0 för att ansluta till ditt Microsoft Dynamics 365-konto. Med modulerna i Microsoft Dynamics 365 kan du

* Utlösa ett scenario när poster läggs till eller uppdateras i Microsoft Dynamics 365
* Skapa, läsa, uppdatera eller ta bort en Microsoft Dynamics 365-post
* Utför ett anpassat API-anrop

Mer information om tillgängliga Microsoft Dynamics 365-moduler finns i [Microsoft Dynamics 365-moduler](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## DocuSign-anslutning och moduler är nu tillgängliga

Nu kan du använda Workfront Fusion 2.0 för att ansluta till ditt Docusign-konto. Med Documentum-modulerna kan du:

* Utlösa ett scenario när ett kuvert ändrar sin status
* Skapa ett omslag
* Läsa, skicka eller lägga till en mottagare i ett befintligt kuvert
* Lägga till eller ändra anpassade fält i dokument
* Hämta ett dokument som ett arkiv
* Överföra en fil till ett kuvert
* Utför ett anpassat API-anrop

Mer information finns i [DocuSign-moduler](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Sök i körningshistoriken för ditt scenario

Vi har gjort det enklare för dig att hitta specifik information från tidigare körningar av scenarier. Fusions nya textsökning gör det möjligt att söka i exekveringshistorik efter alla data i ett paket. Om du till exempel vill identifiera vilken körning som har skapat en viss uppgift kan du använda fullständig textsökning för att söka efter detta uppgifts-ID.

Tidigare var det nödvändigt att hitta specifik körningsinformation för att se varje körning separat.

Mer information finns i [Visa ett scenarios körningshistorik i Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Uppdateringar i Fusion 2.0 Data Store

För att göra det enklare för dig att anpassa dina datalager har vi lagt till en del nya funktioner. Nu när du visar ett datalager kan du:

* Dra och släpp för att ändra ordning på kolumner
* Redigera en enskild cell
* Lägga till flera rader

Mer information om datalager finns i [Datalagermoduler](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Gör en API-nyckelauktoriseringsbegäran via HTTP-anslutningen

För att öka flexibiliteten i hur du kan komma åt API:er har vi lagt till en ny modul i HTTP-anslutningen. Nu kan du använda HTTP-anslutningen för att göra en begäran när webbtjänsten som du använder kräver att en API-nyckel används.

Mer information finns i [HTTP-moduler](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Nya funktioner på mappningspanelen

Vi har lagt till några nya funktioner för att hjälpa dig att anpassa och förenkla formler i dina moduler.

* The

   ```
   omit
   ```

   -funktionen är en allmän funktion som utelämnar de angivna tangenterna för objektet och returnerar resten.
* The

   ```
   pick
   ```

   är en allmän funktion som bara väljer de angivna tangenterna från objektet.
* The

   ```
   escapeMarkdown
   ```

   -funktionen är en strängfunktion som undgår alla Markdown-taggar i en text.

Mer information om funktionerna Uteslut och Plockning finns i [Allmänna funktioner i Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Mer information om funktionen escapeMarkdown finns i [Strängfunktioner i Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
