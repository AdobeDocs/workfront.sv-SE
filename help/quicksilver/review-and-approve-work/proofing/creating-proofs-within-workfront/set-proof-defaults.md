---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Konfigurera standardinställningar för personligt korrektur
description: Du kan definiera standardinställningar för personligt korrektur som gäller för korrektur som du skapar. Dessa standardvärden används varje gång du genererar ett första provtryck eller överför en ny provversion i Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Konfigurera standardinställningar för personligt korrektur

Du kan definiera standardinställningar för personligt korrektur som gäller för korrektur som du skapar. Dessa standardvärden används varje gång du genererar ett första provtryck eller överför en ny provversion i Workfront.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller högre</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Konfigurera standardinställningar för personligt korrektur

{{step1-to-proofing}}

1. Klicka på din avatar i det övre högra hörnet och välj **Personliga inställningar**.
1. Välj fliken **Korrekturinställningar** och ange sedan följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>Standardinställningar för e-postmeddelanden</strong> </td> 
     </tr> 
     <tr> 
      <td>Standardvarning för e-post</td> 
      <td>Ange hur ofta användaren får e-postuppdateringar. Välj Alla aktiviteter, Svar på mina kommentarer, beslut, Slutligt beslut, Sammanfattning varje timme, Sammanfattning varje dag eller Inaktiverad.</td> 
     </tr> 
     <tr> 
      <td>Standardvarning för nya gästgranskare</td> 
      <td>Ange hur ofta gästgranskare får e-postuppdateringar. Alternativen är desamma som för standardavisering via e-post.</td> 
     </tr> 
     <tr> 
      <td>Nytt korrekturmeddelande</td> 
      <td>Välj att få ett meddelande när du läggs till i ett korrektur.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Meddelandeinställningar</strong> </td> 
     </tr> 
     <tr> 
      <td>Ämnesmall för korrektur</td> 
      <td>Skriv vad du vill att användarna ska se i ämnet för ett e-postmeddelande när du delar ett korrektur med dem.</td> 
     </tr> 
     <tr> 
      <td>Mall för korrekturmeddelanden</td> 
      <td>Skriv vad du vill att användarna ska se i e-postmeddelandets text när du delar ett korrektur med dem.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Standardkorrekturinställningar</strong> </td> 
     </tr> 
     <tr> 
      <td>Lås korrektur när alla beslut fattas</td> 
      <td>Välj att automatiskt låsa korrekturet från ytterligare ändringar när alla beslut har fattats.</td> 
     </tr> 
     <tr> 
      <td>Endast ett beslut krävs</td> 
      <td>Välj om du bara vill ha ett beslut om ett bevis.</td> 
     </tr> 
     <tr> 
      <td>Inloggning krävs</td> 
      <td> <p>Välj om du bara vill att korrekturet ska vara tillgängligt för användare med inloggningsuppgifter för Workfront Proof.</p> <p>Obs! Workfront Proof-autentiseringsuppgifter kan skilja sig från dina Workfront-autentiseringsuppgifter, såvida inte företagets användare har enkel inloggning. Vi rekommenderar att du bara använder den här funktionen om din företagsanvändare har enkel inloggning.</p> </td> 
     </tr> 
     <tr> 
      <td>Prenumerationen är aktiverad</td> 
      <td>Tillåt granskare utanför organisationen att registrera sig för korrekturet via den offentliga URL:en eller inbäddningskoden. När det här alternativet är markerat måste prenumeranten klicka på en länk i ett e-postmeddelande för att få åtkomst till ett korrektur som också är tillgängligt. Välj det här alternativet om du vill att den externa granskaren ska klicka på en länk i e-postmeddelandet för att få åtkomst till korrekturet. Det här alternativet är aktiverat som standard om alternativet för offentlig delning är markerat och används på alla korrektur som skapas av den här användaren. </td> 
     </tr> 
     <tr> 
      <td>Standardroll för nya gästgranskare</td> 
      <td>Välj en korrekturroll som standard för gästgranskare. Alternativen är desamma som de i rollen Standardkorrektur.</td> 
     </tr> 
     <tr> 
      <td>Blockera hämtning av originalfilen</td> 
      <td>Välj att blockera användare från att hämta originalfilen. </td> 
     </tr> 
     <tr> 
      <td>Min standardkorrekturroll</td> 
      <td>Välj din standardkorrekturroll. </td> 
     </tr> 
     <tr> 
      <td>Min standardmarkeringsfärg</td> 
      <td>Välj standardmarkeringsfärg. </td> 
     </tr> 
    </tbody> 
   </table>
