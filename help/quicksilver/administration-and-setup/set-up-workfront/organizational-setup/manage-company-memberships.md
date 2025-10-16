---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Hantera företagsmedlemskap
description: Under [!UICONTROL Companies] i Inställningar kan du lägga till och ta bort ett företags medlemmar. Du kan även redigera deras användarprofiler och påminna dem om att registrera dem i  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] system.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 1%

---

# Hantera företagsmedlemskap

I området [!UICONTROL Companies] i [!UICONTROL Setup] kan du lägga till och ta bort ett företags medlemmar. Du kan också redigera deras användarprofiler, påminna dem om att registrera sig i [!DNL Workfront], inaktivera dem i [!DNL Workfront] och ta bort dem från [!DNL Workfront]-systemet.

Mer information om hur du skapar ett nytt företag finns i [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>Alla</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
  <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån [!UICONTROL System Administrator], som gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
     <li> <p>Administrativ åtkomst för att hantera företag, vilket gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
    </ul> <p><b>OBS</b>:  
     <ul> 
      <li> <p>Du kan också hantera företag som är kopplade till en grupp där du har tilldelats som gruppadministratör.</p> </li> 
      <li> <p>Om du vill lägga till och ta bort användare från systemet [!DNL Workfront] måste du ha något av följande:</p> 
       <ul> 
        <li> <p>Åtkomstnivån [!UICONTROL System Administrator]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> inställningen i din åtkomstnivå konfigurerad till <b>[!UICONTROL Edit]</b> åtkomst, med <b>[!UICONTROL Create]</b> och minst ett av de två <b>[!UICONTROL User Admin]</b> alternativen aktiverade under <b>[!UICONTROL Fine-tune your settings]</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Om <b>[!UICONTROL User Admin (Group Users)]</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hantera företagsmedlemskap

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Companies]**.
1. Klicka på företagets namn.
1. Klicka på **[!UICONTROL Company Members]** i den vänstra panelen.
1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Lägg till en medlem</td> 
      <td> <p>Klicka på <b>[!UICONTROL Add member]</b> och välj sedan något av följande alternativ i listrutan som visas:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b>: Lägg till en användare som ännu inte har lagts till i [!DNL Workfront].</p> <p>Mer information om hur du lägger till användare i [!DNL Workfront] finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Lägg till användare</a> och <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Lägg till en användare som redan finns i systemet och som du kan redigera.</p> <p><b>VIKTIGT</b>: Om användaren redan är medlem i ett annat företag åsidosätter den nya tilldelningen den gamla. Användaren förlorar åtkomsten till objekt som delats med det tidigare företaget och får åtkomst till objekt som delas med det här företaget.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: Importera en användare genom att överföra en kalkylbladsimportfil. Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Importera användare</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redigera medlemmar</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Markera minst en användare och klicka sedan på ikonen [!UICONTROL Edit] <img src="assets/edit-icon.png"> i verktygsfältet.</p> </li> 
        <li value="2"> <p>Konfigurera alternativen i rutan <b>[!UICONTROL Edit User]</b> som visas.</p> <p>Mer information om de här alternativen finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiera medlem</td> 
      <td> <p>Du kan skapa en företagsmedlem genom att kopiera en befintlig. </p> <p><b>OBS</b>:  <p>När du skapar en användare på det här sättet kopieras all information från den ursprungliga användaren till den nyskapade användaren förutom följande:</p> 
        <ul> 
         <li>Informationen i avsnittet [!UICONTROL Personal Info].</li> 
         <li>[!UICONTROL When I log in, show]: Standardstartfliken för åtkomstnivån är markerad i den här rutan.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Markera användaren och klicka sedan på ikonen [!UICONTROL Copy] <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>I rutan <b>[!UICONTROL New User]</b> som visas redigerar du de fält som är tillgängliga för den nya användaren.</p> <p>Mer information om alla fält som är associerade med en användare finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Redigera en användares profil</a>.</p> </li> 
        <li value="3"> <p>Klicka på <strong>[!UICONTROL Add This User]</strong>.</p> <p>eller</p> <p>Klicka på <strong>[!UICONTROL Add Person User & Start Another]</strong> om du vill spara den nya användaren och lägga till en till.</p> </li> 
       </ol> <p>Detta skapar ett nytt konto i [!DNL Workfront] för användaren.</p> <p>Om du har valt att skicka en inbjudan till användaren bör användaren få ett e-postmeddelande där han/hon kan följa en länk för att skapa sitt [!DNL Workfront]-lösenord.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort användare</td> 
      <td> 
       <div> 
        <p>Välj minst en användare, klicka på <b>[!UICONTROL Remove users]</b> och välj sedan ett av följande alternativ i listrutan som visas:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b>: Tar bort användare från företaget.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: Tar bort användaren eller användarna från systemet [!DNL Workfront].</p> <p><b>VIKTIGT</b>: Om du tar bort en användare från systemet tas även information som är kopplad till användaren som du kanske vill behålla bort. Vi rekommenderar att du inaktiverar användare i stället för att ta bort dem. Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skicka en kommentar till användare och till deras [!UICONTROL Updates] områden</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Markera minst en användare och klicka sedan på <b>Skicka uppdatering till användare</b> i verktygsfältet.</p> </li> 
        <li value="2"> <p>Skriv den kommentar som du vill skicka till användarna och till [!UICONTROL Updates]-delen av deras användarprofiler.</p>
         <p>Mer information finns i <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">Skicka direktmeddelanden till andra användare</a>.</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera listan över företagsmedlemmar</td> 
      <td> <p>Klicka på ikonen [!UICONTROL Export] <img src="assets/export.png"> i verktygsfältet och välj sedan det format du vill använda för den exporterade filen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inaktivera medlemmar i systemet</td> 
      <td> <p>Markera minst en användare, klicka på ikonen [!UICONTROL More] <img src="assets/more-icon.png"> i verktygsfältet och välj sedan <b>[!UICONTROL Deactivate]</b>.</p> <p>Mer information finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Påminn en användare om att registrera sig i systemet</td> 
      <td> <p> I kolumnen <b>[!UICONTROL Name]</b> visas <b>[!UICONTROL Unregistered]</b> bredvid namnet på varje oregistrerad användare. Om du vill påminna användarna om att registrera sig i systemet markerar du användarna, klickar på ikonen [!UICONTROL More] <img src="assets/more-icon.png"> i verktygsfältet och väljer sedan <b>[!UICONTROL Remind user to register]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
