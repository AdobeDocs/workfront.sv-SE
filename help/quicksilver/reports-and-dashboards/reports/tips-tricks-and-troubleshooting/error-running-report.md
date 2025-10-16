---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Felmeddelande när en rapport körs: ''Du är inte inloggad.'''
description: Läs mer om felmeddelandet"Du är inte inloggad".
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# Felmeddelande när en rapport körs:&quot;Du är inte inloggad.&quot;

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
     <p>Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problem

När du kör en rapport, eller visar den på en kontrollpanel, returnerar följande fel:\
*Vi försöker igen. Du är inte inloggad.*

Inga resultat visas i rapporten.

## Orsak

Rapporten är inställd på att köras som en inaktiverad användare.

## Lösning

Du måste ha behörigheten Hantera för rapporten för att kunna ändra rapportinställningarna.\
Så här justerar du rapporten och ser resultaten:

1. Gå till rapporten.
1. Klicka på **Rapportera åtgärder** > **Redigera** > **Rapportinställningar**.

1. Ange namnet på en aktiv användare i fältet **Kör den här rapporten med åtkomstbehörigheten**.\
   eller\
   Lämna fältet **Kör den här rapporten med åtkomstbehörigheten** tomt.

1. Klicka på **Klar**.
1. Klicka på **Spara + Stäng**.\
   Felet bör inte visas igen när den här rapporten körs.
