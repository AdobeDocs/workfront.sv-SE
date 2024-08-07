---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Korrektur för en länkad resurs med den utökade kopplingen
description: När du har länkat en resurs från Experience Manager Assets kan du skapa ett korrektur och tilldela användare behörighet att granska och lägga till kommentarer i resursen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Korrektur för en länkad resurs med den utökade kopplingen

När du har länkat en resurs från Experience Manager Assets kan du skapa ett korrektur och tilldela användare behörighet att granska och lägga till kommentarer i resursen. Korrektur som skapats från länkade resurser räknas in i din korrekturlagringskvot.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha Experience Manager Assets Essentials.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller högre</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du

* Installera den utökade Workfront för Experience Manager-anslutningen

## Skapa ett korrektur

Du kan skapa statiska eller interaktiva korrektur.

Skapa ett korrektur:

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på avsnittet **Dokument**.
1. Håll markören över dokumentet och klicka sedan på länken **Skapa korrektur** som visas under dokumentnamnet.

   >[!NOTE]
   >
   >Om du har **Generera korrektur automatiskt när dokument** överförs i din användarprofil skapas ett enkelt korrektur automatiskt.

1. Välj något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Enkelt korrektur</td> 
      <td>Med det här alternativet skapas ett korrektur utan ett kopplat arbetsflöde och standardinställningarna för korrektur används. Du kan uppdatera standardinställningarna för korrektur eller lägga till ett arbetsflöde när du har skapat korrekturet. Mer information om korrekturinställningar finns i <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Redigera korrekturinställningar</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avancerat korrektur</td> 
      <td> <p>Med det här alternativet kan du konfigurera ett grundläggande eller avancerat arbetsflöde och ändra korrekturinställningarna för det korrektur du skapar. Mer information finns i </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Skapa ett avancerat korrektur med ett grundläggande arbetsflöde</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Skapa ett avancerat korrektur med ett automatiserat arbetsflöde</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Hantera ett befintligt korrektur

När du har skapat ett bevis kan du göra saker som

* Visa aktuell scenaktivitet
* Uppdatera granskare och deadlines
* Redigera arbetsflödet

Mer information om hur du hanterar ett befintligt korrektur finns i [Hantera korrektur i Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Granska ett korrektur

Tilldelade granskare kan göra saker som

* Visa resursen och gör kommentarer
* Lägga till åtgärder i kommentarer
* Jämför versioner
* Godkänn eller avvisa korrekturet

Mer information om vad du kan göra med korrekturverktyget finns i [Granska korrektur i Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
