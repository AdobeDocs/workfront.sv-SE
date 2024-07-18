---
product-area: projects
navigation-topic: approvals
title: Godkänna arbete
description: Godkänna arbete
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1134'
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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Hitta godkännanden i Adobe Workfront

Du kan visa och hantera godkännanden inom olika områden av Workfront.

Mer information om hur du visar objekt som väntar på godkännanden eller objekt som du har skickat in för godkännande själv finns i [Visa godkännanden](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Godkänn arbete från startsidan

1. Klicka på ikonen **Hem** ![](assets/home-icon-30x29.png) i det övre vänstra hörnet av Adobe Workfront.

   >[!NOTE]
   >
   >Workfront-administratören kan göra följande ändringar av hemikonen i din miljö:
   >
   >   
   >* Ersätt den med en bild som är anpassad för att illustrera organisationen. I det här fallet ser ikonen annorlunda ut än i den här artikeln.
   >* Ersätt den länkade sidan med en annan sida. I det här fallet klickar du på **Huvudmenyn** ![](assets/main-menu-icon.png) i det övre högra hörnet på sidan och sedan på **Hem**.

1. Klicka på listrutan **Filter**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Välj **Godkännanden**.\
   Alla arbetsobjekt som kräver ditt godkännande visas. 

   >[!NOTE]
   >
   >Godkännanden som tilldelats till jobbroller eller grupper visas inte i Hem. Godkännanden som tilldelats team visas i grupperingen Teambegäran i arbetslistan.

1. (Valfritt) Ändra den ordning i vilken godkännanden visas, enligt beskrivningen i avsnittet Gruppera och sortera efter datum, projekt eller prioritet i artikeln [Visa objekt i arbetslistan i hemområdet](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Markera objektet där du vill fatta ett beslut om godkännande.

   ![](assets/task-approval-home-350x127.png)

1. Klicka på ett av de tillgängliga alternativen när du ska fatta ett beslut om godkännande på den högra panelen. Följande alternativ visas i det övre högra hörnet av sidan, beroende på vilken typ av objekt du godkänner:

   * **Projekt:** Klicka på **Godkänn** eller **Avvisa**.

   * **Uppgifter:** Klicka på **Godkänn** eller **Avvisa** .

   * **Problem:** Klicka på **Godkänn** eller **Avvisa** .

   * **Tidrapporter:** Klicka på **Godkänn** eller **Avvisa** .

   * **Dokument:** Klicka på **Godkänn**, **Avvisa** eller **Ändringar**.\
      Tänk på följande när du visar  godkännanden:

      * Bevisgodkännanden visas här när en användare delar ett korrektur med dig, vilket beskrivs i avsnittet Dela en korrekturlänk i artikeln [Dela ett korrektur i Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Språkgodkännanden visas bara i hemmet om din Workfront-miljö är integrerad med ett Workfront Proof Premium-konto. Om du inte kan använda korrektur som beskrivs här kontaktar du Workfront-administratören.
      * Du får ett meddelande i appen som meddelar dig om korrekturgodkännandet.\
        Mer information om meddelanden i appen finns i [Visa och hantera meddelanden i appen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * Namnet på den användare som begärde godkännandet visas bredvid miniatyrbilden i området Hem, med följande text:\
        &quot;*Användare A* vill ha ditt godkännande den..&quot;

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        Om användarnamnet inte är tillgängligt visas följande text:\
        &quot;En ny version av ett korrektur är klar att visas&quot;
      * Klicka på **Gå till korrektur**, **Slutför granskning** och sedan på ett av de tillgängliga alternativen om du vill fatta ett beslut om godkännande av korrekturet. De tillgängliga alternativen vid godkännande av korrektur är: **Godkänd**, **Godkänd med ändringar**, **Ändringar krävs** och **Inte relevant**.

      * När du har bestämt dig för korrekturet finns det kvar på fliken Mina godkännanden med texten &quot;Beslutsfattad&quot; tills du klickar på knappen **Uppdatera** eller tills du uppdaterar webbläsarsidan.

        Mer information om hur du granskar korrektur finns i [Granska korrektur i Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

   * **Åtkomst:** Välj åtkomstnivå i listrutan **Ändra åtkomst** och klicka sedan på **Bevilja åtkomst**. Du kan också klicka på **Ignorera**.

## Godkänn arbete direkt från ett projekt, en uppgift eller ett ärende

När ett projekt, en uppgift eller en utgåva väntar på godkännande kan du godkänna eller avvisa godkännandet direkt från projektet, uppgiften eller utgåvan. Du kan även visa information om godkännandeprocessen.

Så här godkänner du arbete direkt från ett projekt, en uppgift eller en utgåva:

1. Gå till det projekt, den uppgift eller det problem som kräver ditt godkännande.

   Godkännandeinformation om den aktuella godkännandeprocessen för ett projekt, en uppgift eller ett problem visas i artikelhuvudet.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

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
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Valfritt) Om ett korrektur har skapats för dokumentet kan du godkänna dokumentet i korrekturgränssnittet, vilket beskrivs i [Godkänn ett dokument från ett korrektur](#approve-a-document-from-a-proof).

## Godkänn ett dokument från ett e-postmeddelande om godkännande

Beroende på dina meddelandeinställningar kan du få e-postmeddelanden som meddelar dig om dokument som andra användare behöver att du ska fatta ett beslut om godkännande av. När du får ett e-postmeddelande som innehåller knappen **Make Approval Decision** kan du starta godkännandeprocessen direkt från e-postmeddelandet:

1. I e-postmeddelandet klickar du på **Make Approval Decision** för att öppna sidan Document Details (Dokumentinformation) för korrekturet.
1. Gör något av följande för att granska dokumentet:

   * Visa metadata om dokumentet.
   * Om du har skapat ett korrektur för granskning av dokumentet med markeringar och kommentarer klickar du på **Öppna korrektur** ![](assets/open-proof-icon-qs.png) i det övre högra hörnet och granskar korrekturet.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Mer information om granskning av korrektur finns i [Granska korrektur i Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klicka på ett **beslutsalternativ** i det övre högra hörnet om du vill godkänna, godkänna med ändringar eller avvisa dokumentet.

## Godkänn ett dokument från ett korrektur {#approve-a-document-from-a-proof}

Du kan godkänna ett dokument i korrekturläsaren. Mer information finns i [Ta ett beslut om ett korrektur i korrekturläsaren](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) i artikeln [Ta ett beslut om ett korrektur i korrekturläsaren](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
