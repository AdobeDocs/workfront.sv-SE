---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Visa automatiska arbetsflödesfaser i ett korrektur
description: Du kan enkelt spåra förloppet för ett korrektur som konfigurerats med ett automatiserat arbetsflöde. Du kan visa, ändra, lägga till, starta och låsa det arbete som redan har gjorts i steg i korrekturet.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Visa automatiska arbetsflödesfaser i ett korrektur

Du kan enkelt spåra förloppet för ett korrektur som konfigurerats med ett automatiserat arbetsflöde. Du kan visa, ändra, lägga till, starta och låsa det arbete som redan har gjorts i steg i korrekturet.

Mer information om hur du lägger till faser och användare i ett korrektur med ett automatiserat arbetsflöde finns i [Lägga till faser och användare i ett automatiserat arbetsflöde vid ett korrektur](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Valfritt (Du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för korrektur </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan, roll eller behörighetsprofil du har kontaktar du Workfront- eller Workfront-administratören.

## Visa det automatiserade arbetsflödesdiagrammet

1. Håll markören över raden som innehåller dokumentet i en dokumentlista som innehåller dokumentet och klicka sedan på **Korrektur**.

   Diagrammet för det automatiserade arbetsflödet visas precis under arbetsflödets rubrik.

   Stegen i diagrammet markeras enligt följande:

   ![dot.png](assets/dot.png) Aktiv fas

   ![gray_dot.png](assets/grey-dot.png) Inaktiv fas\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Privat fas

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Låst scen

   Raderna mellan faserna visar beroendena mellan faserna. Linjerna som leder till inaktiva stadier prickas tills scenen aktiveras.

   Du kan hålla markören över en scen i diagrammet för att visa dess förlopp. Om scenen inte är aktiv och du har redigeringsbehörighet på scenen kan du klicka på knappen Aktivera scen ![](assets/activate-stage-btn.png) för att starta scenen. Om scenen är aktiv och du har redigeringsbehörighet på scenen kan du låsa den. ![](assets/lock-stage-btn.png) Mer information om förloppsindikatorn (S, O, C, D) finns i  [Visa status och förlopp för ett korrektur i Workfront](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Visa en scen

1. Håll markören över raden som innehåller dokumentet i en dokumentlista som innehåller dokumentet och klicka sedan på **Korrektur**.
1. Klicka på den scen du vill visa i diagrammet.

   ![](assets/view-stage-diagram-350x204.png)

1. Om du vill expandera informationen för en scen klickar du på pilen under dess namn.

   ![](assets/stage-details-caret-350x167.png)

## Visa alla faser

Så här visar du alla faser i ett automatiserat arbetsflöde:

1. Klicka på knappen Ändra vy längst upp på sidan ![](assets/change-view-btn.png)och sedan klicka **Visa alla faser**.

   Alla steg i det automatiserade arbetsflödet visas i avsnittet, men informationen är dold.

1. Om du vill expandera informationen för en scen klickar du på sidpilen under namnet.

## Visa alla faser i detalj

Så här visar du alla faser i ditt automatiserade arbetsflöde med utökad information:

1. Klicka på knappen Ändra vy längst upp på sidan ![](assets/change-view-btn.png)och sedan klicka **Visa alla faser i detalj**.
1. Om du vill visa information om en scen klickar du på nedpilen under namnet.
