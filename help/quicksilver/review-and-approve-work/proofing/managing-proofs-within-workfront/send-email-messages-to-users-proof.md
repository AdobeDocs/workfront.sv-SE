---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Skicka e-postmeddelanden till granskare vid korrektur
description: Under gransknings- och godkännandeprocessen kan du skicka ett meddelande till en eller alla granskare om ett korrektur. Meddelanden är ett enkelt sätt att påminna granskarna om att slutföra granskningen av ett korrektur eller att lämna annan information om korrekturet.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Skicka e-postmeddelanden till granskare vid korrektur

Under gransknings- och godkännandeprocessen kan du skicka ett meddelande till en eller alla granskare om ett korrektur. Meddelanden är ett enkelt sätt att påminna granskarna om att slutföra granskningen av ett korrektur eller att lämna annan information om korrekturet.

Du kan välja mellan att skicka ett generiskt påminnelsemeddelande eller att skicka ett anpassat meddelande till en eller alla användare som är kopplade till en viss fas.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturroll</td> 
   <td>Författare eller moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Skicka e-postmeddelanden till användare vid korrektur

1. Sök efter dokumentet för det korrektur som innehåller de användare som du vill skicka ett meddelande till.
1. Håll muspekaren över dokumentet och klicka sedan på **Korrektur**.

   ![](assets/proof-workflow-doc-list-350x92.png)

1. Om du vill skicka ett meddelande till alla användare på scenen klickar du på menyn **Mer** på scenen och väljer **Meddelande alla**.

   ![](assets/message-stage-350x122.png)

1. Om du vill skicka ett meddelande till en enskild användare klickar du på menyn **Mer** bredvid användaren och väljer **Meddelande**.

   ![](assets/message-user-350x121.png)

1. Ange följande information i avsnittet **Meddelandeinformation**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Meddela personer via e-post</td> 
      <td>Det här alternativet kan inte avmarkeras. Alla användare får meddelandet via e-post.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ignorera anpassat meddelande</td> 
      <td> <p>Klicka på <strong>Ignorera anpassat meddelande</strong> om du bara vill inkludera standardinnehållet för e-post.</p> <p>Standardpåminnelsemeddelandet innehåller följande information:</p> 
       <ul> 
        <li>Personlig länk till korrekturbilden<br>Miniatyrbild<br></li> 
        <li>Följande korrekturinformation: Korrekturnamn, versionsnummer, mappnamn (om tillämpligt) och en lista över granskarna och deras förlopp i korrekturet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ämne</td> 
      <td>Skriv ett ämne i meddelandet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meddelande</td> 
      <td>Skriv ditt meddelandeinnehåll.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skicka.**
