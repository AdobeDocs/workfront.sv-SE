---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Granska begärda projekt
description: Projektbegäranden visas som projekt med statusen [!UICONTROL Requested] i Adobe Workfront. I den här artikeln beskrivs hur du granskar projektförfrågningar.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Granska begärda projekt

När flera projektförfrågningar skickas in för granskning kan projektledningskontoret eller portföljkommittén mötas för att granska inskickade förfrågningar och fastställa godkännanden av projektförfrågningar. Projektbegäranden visas som projekt med statusen [!UICONTROL Requested] i [!DNL Adobe Workfront].

Du kan skicka en projektförfrågan för granskning genom att göra något av följande:

* Ändra projektstatus till **[!UICONTROL Requested]**.
* Slutför [!UICONTROL Business Case] av projektet och skicka det för godkännande.\
   Mer information om hur du fyller i ett affärsärende för ett projekt finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Du kan granska begärda projekt i följande områden i [!DNL Adobe Workfront]:

* I en projektrapport
* Inom en portfölj

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Business] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL View] behörighet eller högre till Portfolio</p> <p>[!UICONTROL Edit] behörighet till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL View] behörigheter eller högre för portföljen</p> <p>[!UICONTROL Manage] behörigheter för projekten för att uppdatera deras status</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Granska begärda projekt i en projektrapport

Du kan skapa en rapport för projekt för att se vilka projekt som har statusen [!UICONTROL Requested].

Mer information om hur du godkänner projektbegäranden genom att skapa en projektrapport finns i avsnittet [[!UICONTROL Approving the Business Case by Building a Project Report]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) i [Godkänn ett affärsärende](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## Granska begärda projekt i en portfölj

1. Gå till portföljen vars begärda projekt du vill granska.
1. Klicka på &#x200B;**[!UICONTROL Projects]** i den vänstra panelen
1. Välj **[!UICONTROL Requested]** i listrutan **[!UICONTROL Filter]**.

   Endast projekt med statusen **[!UICONTROL Requested]** visas i listan.

   >[!TIP]
   >
   > Förutom statusen **[!UICONTROL Requested]** måste projekt associeras med det markerade Portfolio som ska visas i den här listan.

1. Klicka på namnet på ett projekt i listan för att öppna det.
1. Klicka på **[!UICONTROL Project Details]** i den vänstra panelen.
1. Gör något av följande:

   * Klicka på **[!UICONTROL Business Case]** och sedan på **[!UICONTROL Approve]** eller **[!UICONTROL Reject]** i området [!UICONTROL Business Case Summary] för att godkänna eller avvisa affärsärendet.

     ![approved_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     Projektstatusen ändras till **[!UICONTROL Approved]** om affärsärendet har godkänts.

     Projektstatusen ändras till **[!UICONTROL Rejected]** om affärsärendet avvisas.

     >[!NOTE]
     >
     >Det finns inga meddelanden som informerar användaren som skickade in godkännandet av affärsärendet om hans/hennes projektförfrågan godkändes eller avvisades. 

     eller

   * Ändra status för projektet till någon annan status i listrutan **[!UICONTROL Status]**.

     ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
