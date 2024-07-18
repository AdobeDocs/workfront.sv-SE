---
navigation-topic: notifications
title: Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan
description: Om du vill få e-postmeddelanden från förhandsgranskningssandlådemiljön måste du aktivera den här funktionen i dina användarinställningar när du är inloggad på Förhandsgranska.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan

[!UICONTROL Adobe Workfront] inaktiverar all e-postkommunikation både från förhandsvisningen och från anpassade sandlådemiljöer för uppdatering. Mer information om sandlådemiljön för förhandsgranskning finns i [Sandlådemiljön för Adobe Workfront Preview](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Mer information om anpassad sandlådemiljö för uppdatering finns i [Anpassad sandlådemiljö för Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Om du vill få följande e-postmeddelanden från förhandsgranskningssandlådan måste du aktivera den här funktionen i dina användarinställningar när du är inloggad på Förhandsgranska:

* E-postmeddelanden som utlöses av händelsemeddelanden
* Påminnelsemeddelanden
* Automatiska påminnelsemeddelanden för sent eller tidigt
* E-postinbjudningar

Du kan göra detta för dig själv eller för alla användare som du har behörighet att redigera. Mer information om den åtkomst som krävs för att redigera användare finns i [Bevilja åtkomst till användare](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Rapportleverans och push-meddelanden på mobilappen är alltid inaktiverade för förhandsvisningssandlådemiljön. Varken du eller administratören för [!DNL Workfront] kan aktivera rapportleverans eller push-meddelanden för mobilappen när du använder sandlådemiljön för förhandsgranskning.
>
>Mer information om rapportleveranser finns i [Översikt över rapportleverans](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre för att ändra din egen inställning</p> <p>[!UICONTROL Plan] för att redigera inställningen för andra användare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån [!UICONTROL System Administrator].</p> <p> Mer information om åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p>I din åtkomstnivå måste [!UICONTROL Edit] väljas för inställningen [!UICONTROL Users]. Och för inställningen [!UICONTROL Users] måste alternativet [!UICONTROL Create] och minst ett av de två alternativen [!UICONTROL User Admin] aktiveras under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> . </p> <p>Om du använder alternativet [!UICONTROL User Admin (Group Users)] måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Mer information om inställningen [!UICONTROL Users] på en åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan

1. Logga in i din förhandsvisningssandlådemiljö.
1. Klicka på din profilbild i det övre högra hörnet av [!DNL Adobe Workfront]. Klicka sedan på menyn **[!UICONTROL More]** och välj **[!UICONTROL Edit]**.

   eller

   Sök efter en användare i [!DNL Workfront] och klicka på deras namn. Klicka sedan på menyn **[!UICONTROL More]** och välj **[!UICONTROL Edit]**.

   eller

   För flera användare: Klicka på ikonen **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **[!UICONTROL Users]** ![](assets/users-icon-in-main-menu.png).  Markera sedan flera användare och klicka på **[!UICONTROL Edit]**.

1. Klicka på **[!UICONTROL Preferences]**.
1. Välj **[!UICONTROL Receive emails from this test environment]**.

   >[!NOTE]
   >
   >Det här alternativet är inte tillgängligt om du arbetar i en produktionsmiljö.

1. Klicka på **[!UICONTROL Save Changes]**.
