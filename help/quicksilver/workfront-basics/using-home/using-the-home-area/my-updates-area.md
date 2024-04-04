---
product-area: projects
navigation-topic: use-the-home-area
title: Använda området Mina uppdateringar
description: Du kan använda [!UICONTROL My Updates] för att snabbt granska godkännanden som väntar på ditt beslut eller de konversationer du har varit med om.
author: Lisa
feature: Get Started with Workfront
exl-id: 809605a0-8c24-4873-b98f-504a158be022
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Använd [!UICONTROL My Updates] area

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: there is a similar article like this in the "My Work" folder that is conditioned for Classic only)</p>
-->

Du kan använda [!UICONTROL My Updates] för att snabbt granska godkännanden som väntar på ditt beslut eller de konversationer du har varit med om.

Som en användare med [!UICONTROL Review] finns i [!UICONTROL My Updates] området i [!UICONTROL Main Menu] som standard och [!UICONTROL My Updates] area är standardlandningssida för dig.

Mer information om [!DNL Adobe Workfront] licenser, se [[!DNL Adobe Workfront] licensöversikt](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Om du har en annan licenstyp än Granska visas [!DNL Workfront] eller Gruppadministratören måste lägga till [!UICONTROL My Updates] till layoutmallen för att visa den på huvudmenyn. Mer information finns i [Anpassa [!UICONTROL Main Menu] använda en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>Nytt: Medarbetare eller högre</p>
   eller   
   <p>Aktuell: [!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Åtkomstnivåkonfiguration</strong></td> 
   <td> <p>Visa åtkomst eller högre till objekt som du har taggat i en konversation eller behöver lösa ett godkännande (Projekt, Åtgärder, Problem, Dokument)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View] behörigheter eller högre till projekt, uppgifter, problem, dokument där du är taggad i en konversation eller behöver lösa ett godkännande</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta din [!DNL Workfront] administratör. Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar

Du måste ha följande innan du börjar:

* Om du har en [!DNL Workfront] annan licens än [!UICONTROL Review], dina [!DNL Workfront] eller Gruppadministratören måste lägga till [!UICONTROL My Updates] området till [!UICONTROL Main Menu] använda en layoutmall och tilldela dig till den mallen.

* Granska licenser-användare kan visa [!UICONTROL My Updates] området i sina [!UICONTROL Main Menu] som standard.

## Öppna [!UICONTROL My Updates] area

1. Klicka **[!UICONTROL My Updates]** i **[!UICONTROL Main Menu]**.

   ![](assets/access-my-updates-from-main-menu-reviewer-user-nwe-350x294.png)

   The [!UICONTROL My Updates] -området öppnas.

   Godkännanden och förfrågningar om åtkomst som du har tilldelats visas i den första halvan av sidan, under **Mina uppdateringar**.

   ![](assets/my-updates-mentions-for-reviwers-nwe-350x418.png)

1. (Valfritt) Bläddra längst ned i [!UICONTROL My Updates] och klicka på högerpilen för att visa fler godkännanden som visas på ytterligare sidor.

   >[!TIP]
   >
   >De första fem godkännandena eller förfrågningarna om åtkomst visas som standard. Återstående godkännanden visas på ytterligare sidor. Du kan visa högst 2 000 godkännanden i dialogrutan [!UICONTROL My Updates] område.

   ![](assets/pagination-for-my-updates-page-highlighted-nwe-350x78.png)

1. (Valfritt) Expandera **[!UICONTROL Filter]** nedrullningsbar meny ![](assets/filter-nwepng.png) i det övre högra hörnet av **[!UICONTROL My Updates]** och välj något av följande:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>Godkännanden som har skickats till dig eller delegerats till dig av en annan användare. Mer information om hur du delegerar godkännanden finns i <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegera godkännandebegäran</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegated Approvals]</strong></td> 
      <td>Godkännanden som delegerats till dig av en annan användare. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Approvals]</strong></td> 
      <td> <p>Godkännanden har skickats till dig. </p> <p>Mer information om hur du godkänner objekt finns i <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Godkänna arbete </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Så här godkänner eller avvisar du ett objekt eller föreslår ändringar i ett dokument innan du godkänner:

   1. (Valfritt) Klicka på **nedrullningsbar** icon ![](assets/down-arrow-blue.png) bredvid ditt beslut om godkännande (**[!UICONTROL Approve]**, **[!UICONTROL Changes]**,**[!UICONTROL Reject]**) och lägga till en kommentar och sedan klicka på **[!UICONTROL Add]**.

      eller

      Klicka **[!UICONTROL Skip]** om du inte vill skriva en kommentar.

      ![](assets/approval-decision-buttons-in-my-updates-with-comment-box-nwe-350x183.png)

      >[!NOTE]
      >
      >The [!UICONTROL Changes] visas endast för dokumentgodkännanden.

      Beroende på vilken listruteikon du har valt godkänns, avvisas eller, om dokumentet godkänns, godkänns med en begäran om ytterligare ändringar.

      >[!TIP]
      >
      >Om du inte vill lägga till en kommentar i ditt beslut kan du klicka på **[!UICONTROL Approve]**, **[!UICONTROL Reject]**, eller **[!UICONTROL Changes]** och beslutet om godkännande beviljas omedelbart.
      >
      >
      >![](assets/approval-decision-buttons-in-my-updates-nwe-350x169.png)
      >
      >Mer information om hur du godkänner arbete finns i [Godkänna arbete](../../../review-and-approve-work/manage-approvals/approving-work.md).

1. Klicka **[!UICONTROL Grant access]** för att bevilja dig en begäran om åtkomst

   eller

   Expandera **[!UICONTROL Change access]** för att ändra den begärda åtkomsten innan du beviljar den.

   ![](assets/grant-access-button-in-my-updates-nwe-350x224.png)

1. (Valfritt) Klicka på **[!UICONTROL Ignore]** för att rensa åtkomstbegäran från din godkännandelista utan att bevilja den.
1. Klicka **[!UICONTROL Delegate my approvals]** att delegera godkännanden som skickas till dig om du inte kan fatta beslut om godkännande under en tid. Mer information om att delegera godkännanden finns i [Delegera godkännandebegäran](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).
1. Bläddra till **[!UICONTROL Mentions]** under ditt godkännande. Här kan du visa alla objekt där du har inkluderats i en konversation.

   ![](assets/mentions-area-for-reviewers-nwe-350x191.png)

   >[!TIP]
   >
   >De första 50 omnämnandena visas som standard.

1. (Valfritt) Klicka på **[!UICONTROL Show More Updates]** om du vill visa fler omnämnanden.
1. (Valfritt) Klicka på **[!UICONTROL Reply]** för att svara på en kommentar, ange ditt svar och klicka sedan på **[!UICONTROL Reply]** igen.

   Mer information om hur du uppdaterar objekt finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. (Valfritt) Klicka på **[!UICONTROL Pin current page]** för att fästa [!UICONTROL My Updates] till den översta navigeringen.
