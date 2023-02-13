---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Rapport om godkännande av korrektur för att utesluta tidigare korrekturversioner'
description: I en korrekturgranskningsrapport kan du använda filtret Är aktuell dokumentversion för att endast inkludera de aktuella versionerna av korrektur som väntar på ditt godkännande.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Filter: Rapport för korrekturgodkännande om du vill utesluta tidigare korrekturversioner

På en korrekturgodkännanderapport kan du använda **Är aktuell dokumentversion** om du bara vill inkludera de aktuella versionerna av korrektur som väntar på ditt godkännande.

Detta är användbart om du till exempel har ombetts att godkänna korrektur som har flera versioner. När du kör rapporten Korrektur på godkännande med filtret Är aktuell dokumentversion visas endast den aktuella versionen av varje korrektur som väntar på ditt godkännande, utan tidigare versioner som du inte längre behöver arbeta med. 

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Filtrera korrekturgodkännanderapport för att utesluta tidigare korrekturversioner

1. Om du redan har en rapport för korrektur av godkännande öppnar du den.

   eller

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Om du vill skapa en egen korrekturgodkännanderapport klickar du på huvudmenyn ![](assets/main-menu-icon.png)och sedan klicka **Rapporter** ![](assets/reports-in-main-menu.png). Klicka **Ny rapport**. Bläddra till och klicka på listan som visas **Bevis godkännande**. Klicka **Spara + Stäng**, skriv en **Rapportnamn** (valfritt), klicka sedan på **Spara rapport**.

1. Klicka **Rapportåtgärder > Redigera**.
1. Klicka **Filter** och sedan klicka **Lägg till en filterregel**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klicka **Bevis godkännande**.
1. Klicka på i listan som visas **Är aktuell dokumentversion**.
1. Klicka **Spara + Stäng** i det nedre vänstra hörnet av Adobe Workfront och klicka sedan på **Spara rapport** i rutan som visas.
