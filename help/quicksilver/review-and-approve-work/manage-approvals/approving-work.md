---
product-area: projects
navigation-topic: approvals
title: Godkänna arbete
description: Godkänna arbete
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# Godkänna arbete

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Om du har utsetts till godkännare bör du regelbundet se över vilket arbete som väntar på ditt godkännande.

Mer information om hur du skapar godkännandeprocesser finns i [Skapa en godkännandeprocess för arbetsobjekt](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Mer information om hur du associerar godkännanden med arbete i Workfront finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till objekt som är kopplade till godkännanden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för objekt som är associerade med godkännanden</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Hitta godkännanden i Adobe Workfront

Du kan visa och hantera godkännanden inom olika områden av Workfront.

Mer information om hur du visar objekt som väntar på godkännanden eller objekt som du har skickat in för godkännande själv finns i [Visa godkännanden](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Godkänn arbete från startsidan

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Klicka på **Anpassa** för att lägga till widgeten **Mina godkännanden**.
1. (Villkorligt) Klicka på listrutan **Filter** och välj sedan **Alla** för att visa godkännanden som tilldelats och delegerats till dig.

   >[!NOTE]
   >
   >Godkännanden som tilldelats till jobbroller eller grupper visas inte i Hem. Godkännanden som tilldelats team visas i widgeten Mina godkännanden för varje teammedlem.


1. Markera objektet där du vill fatta ett beslut om godkännande.

   ![Widgeten Mina godkännanden](assets/my-approvals-widget.png)

1. Klicka på ett av de tillgängliga alternativen när du ska fatta ett beslut om godkännande på den högra panelen. Följande alternativ visas i det övre högra hörnet av sidan, beroende på vilken typ av objekt du godkänner:

   <table>
   <tr>
      <td>
      <p><strong>Åtkomst</strong></p>
      </td>
      <td>
      <p><strong>Arbetsobjekt</strong></p>
      </td>
      <td>
      <p><strong>Dokument</strong></p>
      </td>
      <td>
      <p><strong>Korrektur</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Bidrag</li>
      <li>Ignorera</li>
      </ul>
      Du kan justera åtkomstnivån i listrutan <b>Ändra åtkomst</b> om du vill.
      </td>
      <td>
         <ul>
         <li>Godkänn</li>
         <li>Avvisa</li>
         </ul>
      Du kan lämna en kommentar med ditt beslut genom att klicka på listrutan i beslutsknappen.
      </td>
      <td>
   Tilldelad som godkännare
         <ul>
         <li>Godkänn</li>
         <li>Godkänn med ändringar</li>
         <li>Behöver göras</li>
         </ul>
   Tilldelad som granskare
         <ul>
         <li>Slutför min granskning</li>
         </ul>
      Alternativen i den här kolumnen gäller endast för godkännanden av nya dokument. Godkännanden av äldre dokument visas på samma sätt som godkännanden av arbetsobjekt. 
      </td>
      <td>
         <ul>
         <li>Gå till korrektur</li>
         </ul>
         Du fattar ditt beslut i korrekturläsaren. Mer information om hur du granskar korrektur finns i <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Granska korrektur i Adobe Workfront</a>.
      </td>
   </tr>
   </table>

När du har fattat ett beslut tas godkännandet bort från widgeten Mitt godkännande.


## Godkänn arbete direkt från ett projekt, en uppgift eller ett ärende

När ett projekt, en uppgift eller en utgåva väntar på godkännande kan du godkänna eller avvisa godkännandet direkt från projektet, uppgiften eller utgåvan. Du kan även visa information om godkännandeprocessen.

Så här godkänner du arbete direkt från ett projekt, en uppgift eller en utgåva:

1. Gå till det projekt, den uppgift eller det problem som kräver ditt godkännande.

   Godkännandeinformation om den aktuella godkännandeprocessen för ett projekt, en uppgift eller ett problem visas i artikelhuvudet.

   ![Aktuell godkännandeprocess i projekthuvudet](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Följande godkännandeinformation finns:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>Aktuell status för projektet, aktiviteten eller utgåvan. Detta är den aktuella statusen för artikeln som väntar på godkännande. Statusen godkänns när varje steg i godkännandeprocessen har godkänts.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännandefaser</td> 
      <td>Stegen i godkännandeprocessen. <br>Den aktuella fasen som väntar på godkännande visas som Väntande. Steg som redan har godkänts visas som Godkända. Steg som ännu inte har godkänts visas som Inte startat.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Godkänn** eller **Avvisa**, beroende på om du vill godkänna eller avvisa godkännandeprocessen.\
   Godkännandefasen som väntar på godkännande har nu godkänts och godkännandeprocessen går vidare till nästa steg. Statusen godkänns när alla faser har godkänts.

## Godkänn ett dokument direkt från ett dokument

1. Gå till dokumentområdet som innehåller dokumentet som kräver ditt godkännande.
1. Markera dokumentet och klicka sedan på **Godkänn**, **Ändringar** eller **Avvisa**.\
   ![Godkänn dokument](assets/approval-approve-document-350x215.png)\
   ![Godkännande av dokument](assets/document-approval-350x199.png)

1. (Valfritt) Om ett korrektur har skapats för dokumentet kan du godkänna dokumentet i korrekturgränssnittet, vilket beskrivs i [Godkänn ett dokument från ett korrektur](#approve-a-document-from-a-proof).

## Godkänn ett dokument från ett e-postmeddelande om godkännande

Beroende på dina meddelandeinställningar kan du få e-postmeddelanden som meddelar dig om dokument som andra användare behöver att du ska fatta ett beslut om godkännande av. När du får ett e-postmeddelande som innehåller knappen **Make Approval Decision** kan du starta godkännandeprocessen direkt från e-postmeddelandet:

1. I e-postmeddelandet klickar du på **Make Approval Decision** för att öppna sidan Document Details (Dokumentinformation) för korrekturet.
1. Gör något av följande för att granska dokumentet:

   * Visa metadata om dokumentet.
   * Om ett korrektur har skapats för granskning av dokumentet med markeringar och kommentarer klickar du på **Öppna korrektur** ![Öppna korrektur](assets/open-proof-icon-qs.png) i det övre högra hörnet och granskar korrekturet.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Mer information om granskning av korrektur finns i [Granska korrektur i Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klicka på ett **beslutsalternativ** i det övre högra hörnet om du vill godkänna, godkänna med ändringar eller avvisa dokumentet.

## Godkänn ett dokument från ett korrektur {#approve-a-document-from-a-proof}

Du kan godkänna ett dokument i korrekturläsaren. Mer information finns i [Ta ett beslut om ett korrektur i korrekturläsaren](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) i artikeln [Ta ett beslut om ett korrektur i korrekturläsaren](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
