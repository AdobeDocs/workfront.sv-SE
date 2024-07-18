---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtrera: Rapport om godkännande av korrektur för att utesluta tidigare korrekturversioner'
description: I en korrekturgranskningsrapport kan du använda filtret Är aktuell dokumentversion för att endast inkludera de aktuella versionerna av korrektur som väntar på ditt godkännande.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Filter: Rapport för korrekturgodkännande om du vill utesluta tidigare korrekturversioner

På en korrekturgodkännanderapport kan du använda filtret **Är aktuell dokumentversion** för att endast inkludera de aktuella versionerna av korrektur som väntar på ditt godkännande.

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
   <td> <p>Begäran om att ändra ett filter </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Filtrera korrekturgodkännanderapport för att utelämna tidigare korrekturversioner

1. Om du redan har en rapport för korrektur av godkännande öppnar du den.

   eller

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Om du vill skapa en egen korrekturgranskningsrapport klickar du på huvudmenyn ![](assets/main-menu-icon.png) och sedan på **Rapporter** ![](assets/reports-in-main-menu.png). Klicka på **Ny rapport**. Bläddra till och klicka på **Korrektur för godkännande** i listan som visas. Klicka på **Spara + stäng**, skriv ett **rapportnamn** (valfritt) och klicka sedan på **Spara rapport**.

1. Klicka på **Rapportera åtgärder > Redigera**.
1. Klicka på **Filter** och sedan på **Lägg till en filterregel**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klicka på **Korrektur för godkännande**.
1. Klicka på **Är aktuell dokumentversion** i listan som visas.
1. Klicka på **Spara + stäng** i det nedre vänstra hörnet av Adobe Workfront och klicka sedan på **Spara rapport** i den ruta som visas.
