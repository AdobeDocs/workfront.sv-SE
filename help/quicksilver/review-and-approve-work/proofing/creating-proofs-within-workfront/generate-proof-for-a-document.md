---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett korrektur för ett dokument
description: Du kan generera ett korrektur för ett dokument när du överför det till Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Skapa ett korrektur för ett dokument

Du kan generera ett korrektur för ett dokument när du överför det till Workfront.

Du kan också generera ett korrektur för ett dokument som redan har överförts till Adobe Workfront eller för en ny version av ett korrektur som redan har överförts till Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

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
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan, roll eller behörighetsprofil du har kontaktar du Workfront- eller Workfront-administratören.

## Överföra ett dokument och skapa ett korrektur

1. Gå till projektet, uppgiften eller utgåvan där du vill skapa ett nytt korrektur.
1. Klicka på **Dokument** -fliken.
1. Klicka på Dokument ![](assets/document-icon.png) i den vänstra panelen.
1. Klicka **Lägg till ny** och sedan klicka **Korrektur** på menyn som visas.

   >[!TIP]
   >
   >Du kan aktivera **Generera korrektur automatiskt när dokument överförs** ange i din användarprofil för att automatisera den här processen. Mer information finns i [Konfigurera mina inställningar](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. I **Nytt korrektur** sida som visas kan du

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Överföra ett dokument och skapa en ny version av ett korrektur

1. Gå till projektet, uppgiften eller utgåvan där du vill skapa en ny version av ett befintligt korrektur.
1. Klicka på **Dokument** -fliken.
1. Markera dokumentet där du vill lägga till en ny version.
1. Klicka **Lägg till ny** > **Version** > **Korrektur**.
1. I **Ny korrekturversion** sida som visas kan du

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Använd dra-och-släpp för att generera ett enkelt korrektur för en ny version

Du kan dra och släppa ett dokument från filsystemet (till exempel skrivbordet) för att skapa ett nytt korrektur eller en ny version av ett befintligt korrektur. Korrekturläret innehåller följande inställningar, beroende på om du skapar ett nytt korrektur eller en ny version:

* **Nytt korrektur:** Skapar ett enkelt korrektur som bara delas med dig. Du kan ändra delningsinställningarna när korrekturet har skapats enligt beskrivningen i [Redigera korrekturinställningar](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Ny version av befintligt korrektur:** Skapar en ny version med samma korrekturinställningar som i den tidigare versionen.

Så här använder du dra och släpp för att generera ett nytt korrektur eller en ny korrekturversion:

1. Kontrollera att korrektur har konfigurerats för att genereras automatiskt, enligt beskrivningen i .
1. Fortsätt med  [Lägga till dokument i Adobe Workfront från filsystemet](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), som förklarar hur du lägger till dokument genom att dra och släppa. 

## Skapa ett korrektur för ett befintligt dokument

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på **Dokument** -avsnitt.
1. Håll muspekaren över dokumentet och klicka sedan på **Skapa korrektur** som visas under dokumentnamnet.

   >[!NOTE]
   >
   >Om du har **Generera korrektur automatiskt när dokument överförs** som är aktiverat i din användarprofil skapar systemet automatiskt ett enkelt korrektur.

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
