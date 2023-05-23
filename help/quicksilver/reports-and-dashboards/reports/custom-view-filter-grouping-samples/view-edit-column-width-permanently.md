---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Visa: redigera bredden på en kolumn permanent'
description: Du kan tillfälligt ändra kolumnbredden genom att dra och släppa marginalerna så att de matchar den önskade bredden. Mer information finns i Ändra kolumnbredd och -ordning.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Visa: redigera bredden på en kolumn permanent

Du kan tillfälligt ändra kolumnbredden genom att dra och släppa marginalerna så att de matchar den önskade bredden. Mer information finns i [Ändra kolumnbredd och -ordning](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Du kan ändra bredden på valfri kolumn i vyn permanent genom att använda textläget i kolumnen när du redigerar vyn.

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
   <td> <p>Begäran om att ändra en vy </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra en vy</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Redigera bredden på en kolumn permanent

>[!IMPORTANT]
>
>Om du ändrar bredden på en kolumn manuellt enligt beskrivningen i avsnittet Ändra bredden och ordningen på kolumner tillfälligt i artikeln [Ändra kolumnbredd och -ordning](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) När du har ändrat bredden på kolumnen permanent bevaras kolumnens bredd enligt din manuella storleksändring och bredden på kolumnen som uppdateras enligt följande steg skrivs över. Du kan visa kolumnen enligt den bredd som definieras i följande steg när du har rensat cachen eller loggat in från en annan webbläsare.

1. Gå till en lista med objekt.
1. Från **Visa** nedrullningsbar meny, klicka **Ny vy**.

1. Klicka **Lägg till kolumn** om du vill lägga till en ny kolumn.

   eller

   Klicka på kolumnrubriken för en befintlig kolumn.

1. Klicka **Växla till textläge**.
1. Håll muspekaren över textlägesområdet och klicka **Klicka för att redigera text**.
1. Lägg till följande kod i textläget för kolumnen:

   ```
   width=200
   usewidths=true
   ```

   För **width** anger du ett tal (i pixlar) som anger hur bred du vill att kolumnen ska visas i vyn.

1. Klicka **Spara** sedan **Spara vy**.
