---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Lägg till användare
description: Som Workfront-administratör eller en användare med fullständig administrativ åtkomst kan du lägga till användare i Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: b476c012f825afc4bc48b7172be26accc6bac0d1
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 0%

---

# Lägg till användare

>[!IMPORTANT]
>
>Om din organisation har anslutit sig till Adobe Admin Console måste du skapa systemadministratörer via Adobe Admin Console.
>
>Instruktioner om hur du skapar systemadministratörer i Adobe Admin Console finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Gruppadministratörer i organisationer som har anslutit sig till Adobe Admin Console kan använda den här proceduren för att skapa användare och skicka in användaren för administratörsgodkännande.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Du kan lägga till användare i Adobe Workfront genom att skapa enskilda användare från grunden eller genom att kopiera befintliga användare.

Mer information om hur du importerar flera användare samtidigt finns i [Importera användare](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> ange din åtkomstnivå som <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst en av de två <b>Användaradministratör</b> alternativ aktiverade under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>av dessa två alternativ, om användaren <b>Administratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om <b>Användare</b> ange en åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar

Innan du lägger till en användare ska du samla in informationen om användaren som anges nedan och ta reda på vilken information du vill associera med användaren:

* Vad är användarens personuppgifter? Du behöver minst följande:

   * Fullständigt namn
   * Ett användarnamn
   * Standardlösenord
   * E-postadress

  >[!NOTE]
  >
  >Du kan ange om användare ska kunna visa andra användares kontaktinformation genom att finjustera inställningen för användarvyn när du anger åtkomstnivåer för Workfront-objekt. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Vilken position har den nya användaren i företaget? Har den här personen några direkta rapporter? Vem rapporterar den här personen till?
* Vilken jobbroll fyller personen? Finns den här jobbrollen i Workfront? Finns det någon gräns för hur många personer som kan fylla den här jobbrollen? Mer information om hur du skapar jobbroller finns i [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* Vilken åtkomstnivå ska användaren ha? Finns den redan eller behöver du skapa en ny? Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* Vilken hemgrupp ska den här användaren vara i? Ska personen vara i mer än en grupp? Mer information om grupper finns i [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* Vilket hemteam ska den här användaren vara i? Ska personen vara i mer än ett team? Mer information om team finns i [Översikt över team](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Vilken anpassad information behöver du associera med den här användaren?

  Om information om användare hämtas i anpassade fält som du har skapat måste du ha ett anpassat formulär när du skapar en användare. Mer information om anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Skapa en helt ny användare

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).

1. Klicka **Ny användare > Ny användare** för att lägga till en användare som ännu inte har lagts till i Workfront.

   eller

   Klicka **Ny användare > Importera användare** om du vill lägga till användare genom att överföra en kalkylbladsimportfil.

   Om du importerar användare behöver du inte fortsätta med de här stegen. Mer information finns i [Importera användare](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. I **Ny användare** visas klickar du på **Visa avancerade alternativ** konfigurerar du sedan de tillgängliga alternativen för att ange personens information.

   Mer information om de här alternativen finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Gör något av följande:

   * Lämna **Skicka en inbjudan via e-post till den här personen** aktiverat. Om du gör det får användaren ett e-postmeddelande där han/hon kan följa en länk för att skapa ett eget lösenord för Workfront. Användare som inte accepterar e-postinbjudan och skapar ett Workfront-lösenord listas som Oregistrerade i Workfront.
   * Inaktivera **Skicka en inbjudan via e-post till den här personen** skriver du en **Lösenord** för personen och bekräfta det i dialogrutan **Bekräfta lösenord** box. Du måste dela det här lösenordet med användaren utanför Workfront.

   >[!NOTE]
   >
   >Om Workfront-administratören har aktiverat en SSO-integrering med Workfront är alternativet Tillåt endast &lt;sso configuration=&quot;&quot;> Autentiseringsfältet är dolt om du inaktiverar e-postinbjudan. Federations-ID eller &lt;sso configuration=&quot;&quot;> Fältet Användarnamn förblir synligt.

   >[!NOTE]
   >
   Om din organisation har anslutit sig till Admin Console och du lägger till en användare via Workfront har du inte möjlighet att skicka en e-postinbjudan.
   >
   Nya användare i Adobe läggs till i Admin Console, och Admin Console skickar ett e-postmeddelande som bjuder in dem att slutföra registreringsprocessen. Alla användare måste slutföra registreringsprocessen för att få tillgång till alla Adobe-system.
   >
   För användare som redan har Adobe kan användaren få ett e-postmeddelande om att Workfront är tillgängligt eller inte. Detta är en inställning som styrs av Adobe-administratören för produkten.

1. Klicka **Lägg till den här användaren**.

   eller

   Klicka **Lägg till person användare och starta en annan** för att spara den nya användaren och lägga till en till.

   >[!NOTE]
   >
   Om du är gruppadministratör och lägger till en användare i en organisation som har anslutit till Adobe Admin Console är alternativen för det här steget **Skicka användare för administratörsgodkännande** och **Skicka för godkännande och starta en annan**. Användaren skapas i en inaktiverad och väntande godkännandestatus. En Workfront-administratör måste godkänna användaren, som aktiverar användaren i Workfront och lägger till dem i Adobe Admin Console.

## Kopiera en användare för att skapa en ny

Du kan skapa en användare genom att kopiera en befintlig användare.

>[!NOTE]
>
När du skapar en användare på det här sättet kopieras all information från den ursprungliga användaren till den nyskapade användaren förutom följande:
>
* Informationen i avsnittet Personlig information.
* Visa när jag loggar in: Standardstartfliken för åtkomstnivån är markerad i den här rutan.
* Direktrapporter
>

Så här skapar du en ny användare genom att kopiera en befintlig:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Användare** ![](assets/users-icon-in-main-menu.png).
1. Markera den användare som du vill kopiera och klicka sedan på ikonen Kopiera ![](assets/copy-icon.png).
1. I **Ny användare** som visas redigerar du fälten som är tillgängliga för den nya användaren.

   Information om alla fält som är associerade med en användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Klicka **Lägg till den här användaren**.

   eller

   Klicka **Lägg till person användare och starta en annan** för att spara den nya användaren och lägga till en till.

Detta skapar ett nytt konto i Workfront för användaren.

Om du har valt att skicka en inbjudan till användaren bör användaren få ett e-postmeddelande där han/hon kan följa en länk för att skapa sitt Workfront-lösenord.

>[!NOTE]
>
Om din organisation har anslutit sig till Admin Console och du lägger till en användare via Workfront har du inte möjlighet att skicka en e-postinbjudan.
>
Nya användare i Adobe läggs till i Admin Console, och Admin Console skickar ett e-postmeddelande som bjuder in dem att slutföra registreringsprocessen. Alla användare måste slutföra registreringsprocessen för att få tillgång till alla Adobe-system.
>
För användare som redan har Adobe kan användaren få ett e-postmeddelande om att Workfront är tillgängligt eller inte. Detta är en inställning som styrs av Adobe-administratören för produkten.
