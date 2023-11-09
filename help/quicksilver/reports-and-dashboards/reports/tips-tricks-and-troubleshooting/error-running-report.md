---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Felmeddelande när en rapport körs: "Du är inte inloggad."'
description: Läs mer om felmeddelandet"Du är inte inloggad".
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Felmeddelande när en rapport körs:&quot;Du är inte inloggad.&quot;

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera, arbeta</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Problem

När du kör en rapport, eller visar den på en kontrollpanel, returnerar följande fel:\
*Vi provar det igen. Du är inte inloggad.*

Inga resultat visas i rapporten.

## Orsak

Rapporten är inställd på att köras som en inaktiverad användare.

## Lösning

Du måste ha behörigheten Hantera för rapporten för att kunna ändra rapportinställningarna.\
Så här justerar du rapporten och ser resultaten:

1. Gå till rapporten.
1. Klicka **Rapportåtgärder** > **Redigera** > **Rapportinställningar**.

1. Ange namnet på en aktiv användare i **Kör den här rapporten med åtkomsträttigheterna för:** fält.\
   eller\
   Lämna **Kör den här rapporten med åtkomsträttigheterna för:** fältet är tomt.

1. Klicka **Klar**.
1. Klicka **Spara + Stäng**.\
   Felet bör inte visas igen när den här rapporten körs.
