---
navigation-topic: notifications
title: Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan
description: Om du vill få e-postmeddelanden från förhandsgranskningssandlådemiljön måste du aktivera den här funktionen i dina användarinställningar när du är inloggad på Förhandsgranska.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '421'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td> 
   <p>Medarbetare eller senare för att ändra din egen inställning</p> <p>Standard för att redigera inställningen för andra användare</p> 
   eller
   <p> Begär eller högre för att ändra din egen inställning</p> <p>Planera att redigera inställningen för andra användare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån [!UICONTROL System Administrator].</p> </li> 
     <li> <p>I din åtkomstnivå måste [!UICONTROL Edit] väljas för inställningen [!UICONTROL Users]. Och för inställningen [!UICONTROL Users] måste alternativet [!UICONTROL Fine-tune your settings] och minst ett av de två alternativen <img src="assets/gear-icon-in-access-levels.png"> aktiveras under [!UICONTROL Create] [!UICONTROL User Admin] . </li> 
     <li>Om du använder alternativet [!UICONTROL User Admin (Group Users)] måste du vara gruppadministratör för en grupp där användaren är medlem.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådan

1. Logga in i din förhandsvisningssandlådemiljö.
1. Klicka på din profilbild i det övre högra hörnet av [!DNL Adobe Workfront]. Klicka sedan på menyn **[!UICONTROL More]** och välj **[!UICONTROL Edit]**.

   eller

   Sök efter en användare i [!DNL Workfront] och klicka på deras namn. Klicka sedan på menyn **[!UICONTROL More]** och välj **[!UICONTROL Edit]**.

   eller

   För flera användare: Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **[!UICONTROL Users]** ![användarikon](assets/users-icon-in-main-menu.png).  Markera sedan flera användare och klicka på **[!UICONTROL Edit]**.

1. Klicka på **[!UICONTROL Preferences]**.
1. Välj **[!UICONTROL Receive emails from this test environment]**.

   >[!NOTE]
   >
   >Det här alternativet är inte tillgängligt om du arbetar i en produktionsmiljö.

1. Klicka på **[!UICONTROL Save Changes]**.
