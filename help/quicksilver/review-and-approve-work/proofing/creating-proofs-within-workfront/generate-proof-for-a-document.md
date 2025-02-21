---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett korrektur för ett dokument
description: Du kan generera ett korrektur för ett dokument när du överför det till Workfront. Du kan också generera ett korrektur för ett dokument som redan har överförts till Adobe Workfront eller för en ny version av ett korrektur som redan har överförts till Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Skapa ett korrektur för ett dokument

<!-- Audited: 1/2024 -->

Du kan generera ett korrektur för ett dokument när du överför det till Workfront.

Du kan också generera ett korrektur för ett dokument som redan har överförts till Adobe Workfront eller för en ny version av ett korrektur som redan har överförts till Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> 
   <p>Nytt: Alla </p>
   <p>Aktuell: Pro eller högre</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Nytt: Standard</p>
   <p>Aktuell: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överföra ett dokument och skapa ett korrektur

1. Gå till projektet, uppgiften eller utgåvan där du vill skapa ett nytt korrektur.
1. Klicka på fliken **Dokument**.
1. Klicka på ikonen ![Dokument](assets/document-icon.png) i den vänstra panelen.
1. Klicka på **Lägg till ny** och sedan på **Korrektur** på den meny som visas.

   >[!TIP]
   >
   >Du kan aktivera inställningen **Generera korrektur automatiskt när du överför dokument** i din användarprofil för att automatisera den här processen. Mer information finns i [Konfigurera mina inställningar](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. På sidan **Nytt korrektur** som visas kan du

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Överföra ett dokument och skapa en ny version av ett korrektur

1. Gå till projektet, uppgiften eller utgåvan där du vill skapa en ny version av ett befintligt korrektur.
1. Klicka på fliken **Dokument**.
1. Markera dokumentet där du vill lägga till en ny version.
1. Klicka på **Lägg till ny** > **Version** > **Korrektur**.
1. På sidan **Nytt korrekturversion** som visas kan du

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Använd dra-och-släpp för att generera ett enkelt korrektur för en ny version

Du kan dra och släppa ett dokument från filsystemet (till exempel skrivbordet) för att skapa ett nytt korrektur eller en ny version av ett befintligt korrektur. Korrekturläret innehåller följande inställningar, beroende på om du skapar ett nytt korrektur eller en ny version:

* **Nytt korrektur:** Skapar ett enkelt korrektur som bara delas med dig. Du kan ändra delningsinställningarna efter att korrekturet har skapats enligt beskrivningen i [Redigera korrekturinställningar](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Ny version av befintligt korrektur:** Skapar en ny version med samma korrekturinställningar som i den tidigare versionen.

Så här använder du dra och släpp för att generera ett nytt korrektur eller en ny korrekturversion:

1. Kontrollera att korrektur har konfigurerats för att genereras automatiskt, enligt beskrivningen i .
1. Fortsätt med  [Lägg till dokument i Adobe Workfront från filsystemet](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), som förklarar metoden att dra och släppa när du lägger till dokument. 

## Skapa ett korrektur för ett befintligt dokument

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
