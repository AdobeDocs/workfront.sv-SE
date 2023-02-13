---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Korrektur för en länkad resurs för Experience Manager Assets eller Assets Essentials
description: När du har länkat en resurs från Experience Manager Assets Essentials kan du skapa ett korrektur och tilldela användare behörighet att granska och lägga till kommentarer i resursen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Korrektur för en länkad resurs för Experience Manager Assets eller Assets Essentials

När du har länkat en resurs från Experience Manager Assets Essentials kan du skapa ett korrektur och tilldela användare behörighet att granska och lägga till kommentarer i resursen.

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
   <td> <p>Arbeta eller högre</p>
   <p>Korrektur måste vara aktiverat för användaren.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha Experience Manager as a Cloud Service eller Assets Essentials, och du måste läggas till som användare i Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller högre</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera en integrering med Experience Manager. Mer information finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) eller [Konfigurera integreringen av Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Skapa ett korrektur

Du kan skapa statiska eller interaktiva korrektur.

Så här skapar du ett korrektur:

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
      <td role="rowheader"><strong>Enkelt korrektur</strong></td> 
      <td>Med det här alternativet skapas ett korrektur utan ett kopplat arbetsflöde och standardinställningarna för korrektur används. Du kan uppdatera standardinställningarna för korrektur eller lägga till ett arbetsflöde när du har skapat korrekturet. Mer information om korrekturinställningar finns i <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Redigera korrekturinställningar</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Avancerat korrektur</strong></td> 
      <td> <p>Med det här alternativet kan du konfigurera ett grundläggande eller avancerat arbetsflöde och ändra korrekturinställningarna för det korrektur du skapar. Mer information finns i </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Skapa ett avancerat korrektur med ett grundläggande arbetsflöde</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Skapa ett avancerat korrektur med ett automatiserat arbetsflöde</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Hantera ett befintligt korrektur

När du har skapat ett bevis kan du göra saker som

* Visa aktuell scenaktivitet
* Uppdatera granskare och deadlines
* Redigera arbetsflödet

Mer information om hur du hanterar ett befintligt korrektur finns i [Hantera korrektur i Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Granska ett korrektur

Tilldelade granskare kan göra saker som

* Visa resursen och gör kommentarer
* Lägga till åtgärder i kommentarer
* Jämför versioner
* Godkänn eller avvisa korrekturet

Mer information om vad du kan göra med korrekturverktyget finns i [Granska korrektur i Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
