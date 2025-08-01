---
product-area: user-management
navigation-topic: manage-your-workfront-account
title: Återställ en användares lösenord med Förbättrad autentisering
description: När Förbättrad autentisering (eAuth) är aktiverat för din [!DNL Workfront] miljö kan en [!DNL Workfront] administratör inte återställa inloggningsuppgifter för en annan användare. Detta skiljer sig från  [!DNL Workfront] miljöer utan eAuth eller miljöer där enkel inloggning (SSO) är aktiverat.
author: Courtney
feature: Get Started with Workfront
hide: true
hidefromtoc: true
exl-id: 72f955e9-75ff-4ff7-b434-7a2b2d5ee0e8
source-git-commit: 1d7d094a682a02b09651023f94e81ee0b330163c
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Återställ en användares lösenord med Förbättrad autentisering

<!--This article has been hidden by request-->

När Förbättrad autentisering (eAuth) är aktiverat för din [!DNL Workfront]-miljö kan en [!DNL Workfront]-administratör inte återställa inloggningsuppgifter för en annan användare. Detta skiljer sig från [!DNL Workfront]-miljöer utan eAuth eller de miljöer där enkel inloggning (SSO) är aktiverat.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Systemadministratör </p> </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Återställ en användares lösenord i en eAuth-aktiverad miljö

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront] och klicka sedan på **[!UICONTROL Users]** ![ikonen Användare](assets/users-icon-in-main-menu.png) .



1. Markera **[!UICONTROL User]** som kräver en lösenordsåterställning.
   ![Markera användaren](assets/100520classicnweselectuser-350x105.png)

1. Klicka på knappen **[!UICONTROL More]** som visas när du har valt önskat **[!UICONTROL User]** och välj alternativet **[!UICONTROL Send Forgot Password Email]** i listrutan.

   ![Skicka e-post om glömt lösenord](assets/100520classicnwesendemail-350x134.png)

När du har valt alternativet **[!UICONTROL Send Forgot Password Email]** skickas ett e-postmeddelande till den valda användaren med instruktioner om att ändra sitt eget lösenord.

![Återställ e-post](assets/pwresetemail-resized-350x461.png)
