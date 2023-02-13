---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Inaktivera eller återaktivera ett företag
description: Du kan inaktivera ett företag som du inte längre använder samtidigt som alla tillhörande historiska data bevaras. Om du inaktiverar ett företag som redan används någonstans i systemet fortsätter det att fungera precis som vanligt. Den har inte tagits bort eller blockerats.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Inaktivera eller återaktivera ett företag

Du kan inaktivera ett företag som du inte längre använder samtidigt som alla tillhörande historiska data bevaras. Om du inaktiverar ett företag som redan används någonstans i systemet fortsätter det att fungera precis som vanligt. Den har inte tagits bort eller blockerats.

## Åtkomstkrav

Du måste ha följande för att kunna hantera företag i [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licens*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>Något av följande:</p> 
    <ul> 
     <li> <p>The [!UICONTROL System Administrator] åtkomstnivå som gör att du kan redigera vilket företag som helst i systemet. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p>Administrativ åtkomst för att hantera företag, vilket gör att du kan redigera vilket företag som helst i systemet. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </li> 
    </ul> <p><b>ANMÄRKNING</b>:  
     <ul> 
      <li> <p>Du kan också hantera företag som är kopplade till en grupp där du har tilldelats som gruppadministratör.</p> </li> 
      <li> <p>För att lägga till och ta bort användare från [!DNL Workfront] måste du ha något av följande:</p> 
       <ul> 
        <li> <p>The [!UICONTROL System Administrator] åtkomstnivå. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
        <li> <p>På din åtkomstnivå [!UICONTROL Edit] måste väljas för [!UICONTROL Users] inställning. För [!UICONTROL Users] inställning, under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> , [!UICONTROL Create] och minst ett av de två [!UICONTROL User Admin] måste vara aktiverade. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Om du använder [!UICONTROL User Admin (Group Users)] måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
       </ul> <p>Mer information om inställningen Användare på en åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har kontaktar du [!DNL Workfront] administratör.

## Inaktivera eller återaktivera ett företag

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **[!UICONTROL Companies]** ![](assets/companies-icon-left-panel.png).

1. Välj ett eller flera företag att inaktivera eller återaktivera.
1. Klicka på **[!UICONTROL Edit]**.
1. För ett enskilt företag inaktiverar du **[!UICONTROL Is Active]** om du vill inaktivera det eller aktivera alternativet för att aktivera det.

   eller

   För flera företag väljer du **[!UICONTROL No]** från **[!UICONTROL Is Active]** nedrullningsbar meny för att inaktivera dem, eller **[!UICONTROL Yes]** för att aktivera dem.

1. Klicka på **[!UICONTROL Save Changes]**.
