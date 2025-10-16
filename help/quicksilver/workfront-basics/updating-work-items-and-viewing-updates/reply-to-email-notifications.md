---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Svara på e-postmeddelanden
description: Du kan besvara e-postmeddelanden från Workfront som genererats från kommentarer som gjorts i projekt, uppgifter, utgåvor och andra objekt för att lägga till svar på de ursprungliga kommentarerna som gjorts i Adobe Workfront-programmet.
author: Nolan and Alina
feature: Get Started with Workfront
exl-id: fea88410-8f37-49d0-9f5d-9fbac4ab5de6
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Svara på e-postmeddelanden

<!-- Audited: April 2024-->

Beroende på hur dina e-postmeddelanden är konfigurerade kan du få ett e-postmeddelande när en uppdatering görs för vissa objekt som du har åtkomst till.

Du kan svara på en uppdatering från ett e-postmeddelande på följande sätt:

* Använd knappen Kommentar i e-postmeddelandet för att gå tillbaka till Workfront och svara på uppdateringen i uppdateringsområdet.
* Svara på det e-postmeddelande du får. Ditt e-postmeddelande läggs till som ett svar från Workfront på den ursprungliga kommentaren.

<!--
>[!NOTE]
>
>Replying to updates by email is not available for environments on Cluster 6.
-->

Du kan svara på e-post från Workfront som genereras från kommentarer som gjorts på följande objekt:

* Projekt
* Uppgift
* Problem
* Dokument
* Mall- och malluppgift
* Portfolio
* Program
* Upprepning
* Tidrapport

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront package</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td> <p>För ärenden och dokument:</p>

<ul><li><p>Medarbetare eller högre</p></li>
   <li><p>Begäran eller senare</p></li></ul>

<p>För alla andra objekt:</p>
   <ul><li><p>Ljus eller högre</p></li>
   <li><p>Granska eller högre</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa eller ge senare åtkomst till de objekt där du vill skicka svaret</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörighet</strong></td> 
   <td> <p>Visa eller högre behörigheter för de objekt där du vill skicka svaret</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p>
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or higher access to the objects where you want to post the reply</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permission</strong></td> 
   <td> <p>View or higher permissions to the objects where you want to post the reply</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Svara på en uppdatering från ett e-postmeddelande

När du får ett e-postmeddelande kan du snabbt öppna det associerade Workfront-objektet från e-postmeddelandet och lägga till ett svar direkt i kommunikationstråden.

1. Öppna e-postmeddelandet som genererats av en uppdatering i Workfront.

   ![email.png](assets/email-350x202.png)
1. Klicka på **Kommentar** i e-postmeddelandet.

   Sidan Information om objektet öppnas i Workfront.

1. Gå till uppdateringen som du vill lägga till ett svar på.

   Förutom att se vilka användare som aktivt deltar i konversationen kan du se vilka som taggats i varje svar högst upp i uppdateringstråden. Dessa användare, tillsammans med alla användare som prenumererar på objektet, får meddelanden när en uppdatering eller ett svar görs för objektet. Mer information om hur du taggar fler användare finns i [Tagga andra för uppdateringar](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Klicka på **Svara,** ange ditt svar och klicka sedan på **Svara**.

   Svaret läggs till som en ny kommentar i kommentarstråden.

## Lägga till en uppdatering av ett objekt genom att svara på ett e-postmeddelande

När du får ett e-postmeddelande från Workfront kan du snabbt lägga till en uppdatering i kommunikationstråden utan att logga in på Workfront.

>[!IMPORTANT]
>
>* Du måste ha behörighet att åtminstone visa objektet som utlöste uppdateringen innan du kan svara på e-postmeddelandet.
>
>* För att undvika inskickningsfel bör Outlook-användare ta bort det befintliga e-postinnehållet innan de skriver in ditt svar.

Så här lägger du till en uppdatering i ett e-postmeddelande från Workfront:

1. Öppna Workfront-mejlet som du vill svara på i ditt e-postprogram och öppna sedan ett svarsfönster från det ursprungliga e-postmeddelandet.

   >[!NOTE]
   >
   >    Du kan inte svara på ett e-postmeddelande som har vidarebefordrats till dig från någon annan.


1. Skriv din uppdatering i e-postsvaret.

   Bifogade filer tillåts inte och eventuell RTF-formatering som används på en uppdatering i ett e-postmeddelande visas inte på uppdateringen när den visas på fliken Uppdateringar.
1. Klicka på **Skicka**.

   Din uppdatering läggs till som ett svar på kommunikationstråden för objektet.
