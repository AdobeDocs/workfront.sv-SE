---
title: Aktivera eller inaktivera AI Assistant
content-type: reference
description: Du kan styra vilka åtkomstnivåer i organisationen som har tillgång till AI Assistant.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: 0dcf12ed00c04e9d7acddfd034dbba6357bb1385
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Aktivera eller inaktivera AI Assistant

Som Workfront-administratör kan du styra vilka användare i organisationen som har AI Assistant aktiverat. Detta hanteras via åtkomstnivåer.

## Åtkomstkrav

Du måste ha följande åtkomst för att aktivera eller inaktivera AI-assistenten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Inte tillgänglig</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Inte tillgänglig</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Aktivera eller inaktivera AI-assistenten i Workfront

>[!NOTE]
>
>AI Assistant är inaktiverat som standard för icke-administratörer.

Så här aktiverar du AI-assistenten för en given åtkomstnivå:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Välj **Åtkomstnivåer** i den vänstra navigeringen.
1. Välj den åtkomstnivå som du vill aktivera AI-assistenten för.
1. I fönstret Redigera åtkomstnivå bläddrar du nedåt i fönstret och klickar på **Ange ytterligare begränsningar..**.
1. I området Ange ytterligare begränsningar inaktiverar du alternativet **Inaktivera AI-funktioner**.
1. Klicka på **Spara**.
1. Upprepa steg 3-6 för varje åtkomstnivå som du vill aktivera AI-assistenten för.

>[!NOTE]
>
>När AI-funktioner läggs till i Workfront kommer vissa AI-funktioner att bli grundläggande för hur Workfront fungerar. Möjligheten att inaktivera alla AI-funktioner kommer troligen att bli inaktuell inom den närmaste framtiden.
