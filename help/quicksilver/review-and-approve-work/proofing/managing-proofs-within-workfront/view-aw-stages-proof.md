---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Visa automatiska arbetsflödesfaser i ett korrektur
description: Du kan enkelt spåra förloppet för ett korrektur som konfigurerats med ett automatiserat arbetsflöde. Du kan visa, ändra, lägga till, starta och låsa det arbete som redan har gjorts i steg i korrekturet.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Visa automatiska arbetsflödesfaser i ett korrektur

Du kan enkelt spåra förloppet för ett korrektur som konfigurerats med ett automatiserat arbetsflöde. Du kan visa, ändra, lägga till, starta och låsa det arbete som redan har gjorts i steg i korrekturet.

Mer information om hur du lägger till faser och användare i ett korrektur med ett automatiserat arbetsflöde finns i [Lägga till faser och användare i ett automatiserat arbetsflöde på ett korrektur](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>
   <p>Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p >
   <p>Arbete eller plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Visa det automatiserade arbetsflödesdiagrammet

1. I en dokumentlista som innehåller dokumentet för du muspekaren över raden som innehåller dokumentet och klickar sedan på **Korrekturarbetsflöde**.

   Diagrammet för det automatiserade arbetsflödet visas precis under arbetsflödets rubrik.

   Stegen i diagrammet markeras enligt följande:

   ![dot.png](assets/dot.png) Aktiv scen

   ![gray_dot.png](assets/grey-dot.png) Inaktiv scen\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Privat fas

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Låst scen

   Raderna mellan faserna visar beroendena mellan faserna. Linjerna som leder till inaktiva stadier prickas tills scenen aktiveras.

   Du kan hålla markören över en scen i diagrammet för att visa dess förlopp. Om scenen inte är aktiv och du har redigeringsbehörighet på scenen, kan du klicka på knappen Aktivera fas ![Aktivera fas](assets/activate-stage-btn.png) för att starta scenen. Om scenen är aktiv och du har redigeringsbehörighet på scenen kan du låsa den. ![Lås scen](assets/lock-stage-btn.png) Mer information om förloppsindikatorn (S, O, C, D) finns i  [Visa förlopp och status för ett korrektur i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Visa en scen

1. I en dokumentlista som innehåller dokumentet för du muspekaren över raden som innehåller dokumentet och klickar sedan på **Korrekturarbetsflöde**.
1. Klicka på den scen du vill visa i diagrammet.

   ![Visa scendiagram](assets/view-stage-diagram-350x204.png)

1. Om du vill expandera informationen för en scen klickar du på pilen under dess namn.

   ![Sceninformation](assets/stage-details-caret-350x167.png)

## Visa alla faser

Så här visar du alla faser i ett automatiserat arbetsflöde:

1. Klicka på knappen Ändra vy längst upp på sidan ![Ändra vy](assets/change-view-btn.png) och klicka sedan på **Visa alla faser**.

   Alla steg i det automatiserade arbetsflödet visas i avsnittet, men informationen är dold.

1. Om du vill expandera informationen för en scen klickar du på sidpilen under namnet.

## Visa alla faser i detalj

Så här visar du alla faser i ditt automatiserade arbetsflöde med utökad information:

1. Klicka på knappen Ändra vy längst upp på sidan ![Ändra vy](assets/change-view-btn.png) och klicka sedan på **Visa alla faser i detalj**.
1. Om du vill visa information om en scen klickar du på nedpilen under namnet.
