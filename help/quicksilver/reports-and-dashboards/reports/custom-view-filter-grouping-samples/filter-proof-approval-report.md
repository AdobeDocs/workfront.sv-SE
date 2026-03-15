---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Korrekturgodkännanderapport som utelämnar tidigare korrekturversioner'
description: I en korrekturgranskningsrapport kan du använda filtret Är aktuell dokumentversion för att endast inkludera de aktuella versionerna av korrektur som väntar på ditt godkännande.
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Filter: Rapport för korrekturgodkännande om du vill utesluta tidigare korrekturversioner

<!--Audited: 10/2024-->

På en korrekturgodkännanderapport kan du använda filtret **Är aktuell dokumentversion** för att endast inkludera de aktuella versionerna av korrektur som väntar på ditt godkännande.

Detta är användbart om du till exempel har ombetts att godkänna korrektur som har flera versioner. När du kör rapporten Korrektur på godkännande med filtret Är aktuell dokumentversion visas endast den aktuella versionen av varje korrektur som väntar på ditt godkännande, utan tidigare versioner som du inte längre behöver arbeta med.

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
   <p>Medarbetare eller begäran om att ändra ett filter </p>
   <p>Standard eller Plan för att ändra en rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrera korrekturgodkännanderapport för att utelämna tidigare korrekturversioner

Du kan skapa ett filter för en korrekturgodkännanderapport.

1. Om du redan har en rapport för korrektur av godkännande öppnar du den.

   eller

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Om du vill skapa en egen korrekturinställningsrapport klickar du på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet eller på ikonen **Huvudmeny** ![Huvudmenyrader](assets/lines-main-menu.png) i det övre vänstra hörnet, om en sådan finns, och klickar sedan på ikonen **Rapporter** ![Rapporter](assets/reports-in-main-menu.png) .

1. Klicka på **Ny rapport**. Listan med objekttyper visas.
1. Klicka på **Korrektur på godkännande** i listan.
Report builder öppnas.
1. Klicka på **Filter** och sedan på **Lägg till en filterregel**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klicka i rutan **Ange filterregler för rapporten** och välj sedan **Korrektur för godkännande** i listan.
1. Klicka på **Är aktuell dokumentversion** i listan under objektet **Korrekturgodkännande**.
1. Välj Lika med för filtermodifieraren och välj sedan Sant.
1. Klicka på **Spara + stäng** i det nedre vänstra hörnet av Adobe Workfront och klicka sedan på **Använd** i den ruta som visas.

   I rapporten Korrektur för godkännande visas endast korrektur som är kopplade till de aktuella versionerna av ett dokument, om några korrekturgodkännanden matchar det här filtreringsvillkoret.
