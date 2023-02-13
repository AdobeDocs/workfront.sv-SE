---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Hantera företagsmedlemskap
description: I [!UICONTROL Companies] under Konfigurera kan du lägga till och ta bort ett företags medlemmar. Du kan även redigera användarprofilerna och påminna dem om att registrera dig i [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] system.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 1%

---

# Hantera företagsmedlemskap

I [!UICONTROL Companies] område i [!UICONTROL Setup]kan du lägga till och ta bort företagets medlemmar. Du kan även redigera användarprofilerna och påminna dem om att registrera dig i [!DNL Workfront], inaktivera dem i [!DNL Workfront]och ta bort dem från [!DNL Workfront] system.

Mer information om hur du skapar ett nytt företag finns i [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

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
        <li> <p>På din åtkomstnivå [!UICONTROL Edit] måste väljas för [!UICONTROL Users] inställning. För [!UICONTROL Users] inställning, under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> , [!UICONTROL Create] och minst ett av de två [!UICONTROL User Admin] måste vara aktiverade. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Om du använder [!UICONTROL User Admin (Group Users)] måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
       </ul> <p>Mer information om inställningen Användare på en åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har kontaktar du [!DNL Workfront] administratör.

## Hantera företagsmedlemskap

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Companies]**.
1. Klicka på företagets namn.
1. Med **[!UICONTROL Company Members]** gör något av följande om du markerar ett avsnitt i den vänstra panelen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Lägg till en medlem</td> 
      <td> <p>Klicka <b>[!UICONTROL Add member]</b>väljer du sedan något av följande alternativ på den nedrullningsbara menyn som visas:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b>: Lägg till en användare som ännu inte har lagts till i [!DNL Workfront].</p> <p>Mer information om hur du lägger till användare i [!DNL Workfront], se <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Lägg till användare</a> och <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Lägg till en användare som redan finns i systemet och som du kan redigera.</p> <p><b>VIKTIGT</b>: Om användaren redan är medlem i ett annat företag åsidosätter det nya uppdraget det gamla. Användaren förlorar åtkomsten till objekt som delats med det tidigare företaget och får åtkomst till objekt som delas med det här företaget.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: Importera en användare genom att överföra en kalkylbladsimportfil. Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importera användare</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redigera medlemmar</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Markera minst en användare och klicka sedan på [!UICONTROL Edit] icon <img src="assets/edit-icon.png"> i verktygsfältet.</p> </li> 
        <li value="2"> <p>Konfigurera alternativen i <b>[!UICONTROL Edit User]</b> som visas.</p> <p>Mer information om de här alternativen finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiera medlem</td> 
      <td> <p>Du kan skapa en företagsmedlem genom att kopiera en befintlig. </p> <p><b>ANMÄRKNING</b>:  <p>När du skapar en användare på det här sättet kopieras all information från den ursprungliga användaren till den nyskapade användaren förutom följande:</p> 
        <ul> 
         <li>Informationen i [!UICONTROL Personal Info] -avsnitt.</li> 
         <li>[!UICONTROL When I log in, show]: Standardfliken för landning för åtkomstnivån är markerad i den här rutan.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Markera användaren och klicka sedan på [!UICONTROL Copy] icon <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>I <b>[!UICONTROL New User]</b> som visas redigerar du fälten som är tillgängliga för den nya användaren.</p> <p>Information om alla fält som är associerade med en användare finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
        <li value="3"> <p>Klicka på <strong>[!UICONTROL Add This User]</strong>.</p> <p>eller</p> <p>Klicka <strong>[!UICONTROL Add Person User & Start Another]</strong> för att spara den nya användaren och lägga till en till.</p> </li> 
       </ol> <p>Detta skapar ett nytt konto i [!DNL Workfront] för användaren.</p> <p>Om du har valt att skicka en inbjudan till användaren bör han/hon få ett e-postmeddelande där han/hon kan följa en länk för att skapa sin inbjudan [!DNL Workfront] lösenord.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort användare</td> 
      <td> 
       <div> 
        <p>Välj minst en användare, klicka på <b>[!UICONTROL Remove users]</b>väljer du sedan något av följande alternativ i listrutan som visas:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b>: Tar bort användaren eller användarna från företaget.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: Tar bort användaren eller användarna från [!DNL Workfront] system.</p> <p><b>VIKTIGT</b>: Om du tar bort en användare från systemet tas även information som är kopplad till användaren bort. Vi rekommenderar att du inaktiverar användare i stället för att ta bort dem. Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skicka en kommentar till användare och till deras [!UICONTROL Updates] områden</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Markera minst en användare och klicka sedan på [!UICONTROL Comment] icon <img src="assets/comment-icon.png"> i verktygsfältet.</p> </li> 
        <li value="2"> <p>Skriv den kommentar du vill skicka till användarna och till [!UICONTROL Updates] i användarprofilerna.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera listan över företagsmedlemmar</td> 
      <td> <p>Klicka på [!UICONTROL Export] icon <img src="assets/export.png"> i verktygsfältet väljer du det format du vill använda för den exporterade filen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inaktivera medlemmar i systemet</td> 
      <td> <p>Välj minst en användare och klicka på [!UICONTROL More] icon <img src="assets/more-icon.png"> i verktygsfältet väljer du <b>[!UICONTROL Deactivate]</b>.</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Påminn en användare om att registrera sig i systemet</td> 
      <td> <p> I <b>[!UICONTROL Name]</b> kolumn, <b>[!UICONTROL Unregistered]</b> visas bredvid namnet på varje oregistrerad användare. Om du vill påminna användarna om att registrera sig i systemet väljer du användarna och klickar på [!UICONTROL More] icon <img src="assets/more-icon.png"> i verktygsfältet väljer du <b>[!UICONTROL Remind user to register]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
