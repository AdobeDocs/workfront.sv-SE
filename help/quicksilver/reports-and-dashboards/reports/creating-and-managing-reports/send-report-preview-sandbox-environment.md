---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Skicka en rapport i förhandsgranskningssandlådemiljön
description: Informationen på den här sidan hänvisar till funktioner som bara är tillgängliga i sandlådemiljöerna Förhandsvisa och Anpassad uppdatering. Den här funktionen är inte tillgänglig i produktionsmiljön.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Skicka en rapport i förhandsgranskningssandlådemiljön

<!-- Audited: 11/2024 -->

Informationen på den här sidan hänvisar till funktioner som bara är tillgängliga i sandlådemiljöerna Förhandsvisa och Anpassad uppdatering. Den här funktionen är inte tillgänglig i produktionsmiljön.

Du kan ställa in alternativ för rapportleverans i vilken testmiljö som helst i Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Testmiljöerna ska fungera så nära produktionsmiljön som möjligt, men vissa funktioner skiljer sig från produktionsmiljön.

Du kan schemalägga rapporter i testmiljöerna, men hur de levereras skiljer sig från hur de levereras från produktionsmiljön.

Mer information om schemaläggning av leveransrapporter i produktionsmiljön finns i [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Beroende på var du schemalägger rapporterna skiljer sig leveransfunktionen mellan sandlådorna Förhandsgranska och Anpassad uppdatering.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
   <p>Redigera åtkomst till filter, vyer, grupperingar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
     <td> <p>Hantera behörigheter i en rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Schemalägg rapporter i förhandsgranskningsmiljön

* [Schemalägg rapporter i förhandsgranskningsmiljön](#schedule-reports-in-the-preview-environment)

### Schemalägg rapporter i förhandsgranskningsmiljön

Huruvida en levererad rapport skapas eller inte i förhandsvisningsmiljön beror på om **Ta emot e-post från den här testmiljön** är aktiverat eller inte.

Mer information om hur du aktiverar e-postmeddelanden från sandlådemiljön finns i [Aktivera leverans av e-postmeddelanden från sandlådemiljön för förhandsgranskning](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![Ta emot e-post från sandlådealternativet](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Schemaläggningsrapporter för leverans i förhandsvisningsmiljön är identiska med schemaläggningsrapporter i produktionsmiljön. Mer information om att schemalägga en leveransrapport finns i [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

När du schemalägger en rapport för leverans i förhandsgranskningsmiljön finns följande scenarier:

* När **Ta emot e-post från den här testmiljön** är inaktiverat för den användare som tar emot rapporten skapas ingen fil när rapporten schemaläggs för leverans.
* När **Ta emot e-post från den här testmiljön** är aktiverat för den användare som tar emot rapporten, läggs den fil som skapas när rapporten schemaläggs för leverans till på fliken Dokument för användaren.

## Schemalägg rapporter i sandlådemiljön för anpassad uppdatering

Huruvida en levererad rapport skapas eller inte i sandlådan för anpassad uppdatering beror på om inställningen Ta emot e-post från den här testmiljön är aktiverad eller inte.

Information om hur du aktiverar e-postmeddelanden från förhandsvisningsmiljön finns i avsnittet [Visa och ändra inställningarna för e-postmeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) i artikeln [Ändra dina egna e-postmeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![Ta emot e-post från sandlådealternativet](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Schemaläggningsrapporter för leverans i sandlådemiljön för anpassad uppdatering är identiska med schemaläggningsrapporter i produktionsmiljön. Mer information om att schemalägga en leveransrapport finns i [Översikt över rapportleverans](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

När du schemalägger en rapport för leverans i sandlådemiljön för anpassad uppdatering finns följande scenarier:

* När Ta emot e-post från den här testmiljön är inaktiverat för den användare som tar emot rapporten skapas ingen fil när rapporten schemaläggs för leverans.
* När Ta emot e-post från den här testmiljön är aktiverat för den användare som tar emot rapporten, skickas rapporten via e-post som en bilaga till den e-postadress som är kopplad till användaren.

## Hur externa användare meddelas

Externa användare får inte rapporter som skickas från Workfront testmiljöer och de får inte heller något e-postmeddelande.

Externa användare får endast e-postrapporter om de levereras från en produktionsmiljö.
