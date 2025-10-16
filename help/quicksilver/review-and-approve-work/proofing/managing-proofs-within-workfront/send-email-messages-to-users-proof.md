---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Skicka e-postmeddelanden till granskare vid korrektur
description: Under gransknings- och godkännandeprocessen kan du skicka ett meddelande till en eller alla granskare om ett korrektur. Meddelanden är ett enkelt sätt att påminna granskarna om att slutföra granskningen av ett korrektur eller att lämna annan information om korrekturet.
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Skicka e-postmeddelanden till granskare vid korrektur

Under gransknings- och godkännandeprocessen kan du skicka ett meddelande till en eller alla granskare om ett korrektur. Meddelanden är ett enkelt sätt att påminna granskarna om att slutföra granskningen av ett korrektur eller att lämna annan information om korrekturet.

Du kan välja mellan att skicka ett generiskt påminnelsemeddelande eller att skicka ett anpassat meddelande till en eller alla användare som är kopplade till en viss fas.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Arbete eller plan</p>
   </td> 
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
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skicka e-postmeddelanden till användare vid korrektur

1. Sök efter dokumentet för det korrektur som innehåller de användare som du vill skicka ett meddelande till.
1. Håll muspekaren över dokumentet och klicka sedan på **Korrektur**.

   ![Språkarbetsflöde](assets/proof-workflow-doc-list-350x92.png)

1. Om du vill skicka ett meddelande till alla användare på scenen klickar du på menyn **Mer** på scenen och väljer **Meddelande alla**.

   ![Meddelande på scen](assets/message-stage-350x122.png)

1. Om du vill skicka ett meddelande till en enskild användare klickar du på menyn **Mer** bredvid användaren och väljer **Meddelande**.

   ![Meddelandeanvändare](assets/message-user-350x121.png)

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
