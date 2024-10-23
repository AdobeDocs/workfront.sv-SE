---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Lägg till användare
description: Som Workfront-administratör eller en användare med fullständig administrativ åtkomst kan du lägga till användare i Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# Lägg till användare

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>Om din organisation har anslutit sig till Adobe Admin Console måste du skapa systemadministratörer via Adobe Admin Console.
>
>Instruktioner om hur du skapar systemadministratörer i Adobe Admin Console finns i [Hantera systemadministratörer i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Gruppadministratörer i organisationer som har anslutit sig till Adobe Admin Console kan använda den här proceduren för att skapa användare och skicka in användaren för administratörsgodkännande.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade skillnader i administration (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Du kan lägga till användare i Adobe Workfront genom att skapa enskilda användare från grunden eller genom att kopiera befintliga användare.

Mer information om hur du importerar flera användare samtidigt finns i [Importera användare](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td><p>Nytt: Standard</p><p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
* Vilket hemteam ska den här användaren vara i? Ska personen vara i mer än ett team? Mer information om team finns i [Teams overview](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* Vilken anpassad information behöver du associera med den här användaren?

  Om information om användare hämtas i anpassade fält som du har skapat måste du ha ett anpassat formulär när du skapar en användare. Mer information om anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Skapa en helt ny användare

{{step-1-to-users}}

1. Klicka på **Ny användare > Ny användare** om du vill lägga till en användare som ännu inte har lagts till i Workfront.

   eller

   Klicka på **Ny användare > Importera användare** om du vill lägga till användare genom att överföra en kalkylbladsimportfil.

   Om du importerar användare behöver du inte fortsätta med de här stegen. Mer information finns i [Importera användare](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. I rutan **Ny användare** som visas klickar du på **Visa avancerade alternativ** och konfigurerar sedan de tillgängliga alternativen för att ange personens information.

   Mer information om de här alternativen finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Gör något av följande:

   * Lämna **Skicka en inbjudan via e-post till den här personen** aktiverad. Om du gör det får användaren ett e-postmeddelande där han/hon kan följa en länk för att skapa ett eget lösenord för Workfront. Användare som inte accepterar e-postinbjudan och skapar ett Workfront-lösenord listas som Oregistrerade i Workfront.
   * Inaktivera **Skicka en inbjudan via e-post till den här personen**, skriv ett **lösenord** för personen och bekräfta det i rutan **Bekräfta lösenord**. Du måste dela det här lösenordet med användaren utanför Workfront.

   >[!NOTE]
   >
   >* Om Workfront-administratören har aktiverat en SSO-integrering med Workfront är fältet Tillåt endast &lt;SSO-konfiguration>-autentisering dolt om du inaktiverar e-postinbjudan. Fältet Federations-ID eller &lt;SSO-konfiguration>-användarnamn är fortfarande synligt.
   >
   * Om din organisation har anslutit sig till Admin Console och du lägger till en användare via Workfront har du inte möjlighet att skicka en e-postinbjudan.
   >
   För användare som redan har Adobe kan användaren få ett e-postmeddelande om att Workfront är tillgängligt eller inte. Detta är en inställning som styrs av Adobe-administratören för produkten.

1. Klicka på **Lägg till den här personen**.

   eller

   Klicka på **Lägg till person och starta en annan** för att spara den nya användaren och lägga till en ny.

   >[!NOTE]
   >
   Om du är gruppadministratör och lägger till en användare i en organisation som har anslutit till Adobe Admin Console är alternativen för det här steget **Skicka användare för administratörsgodkännande** och **Skicka för godkännande och starta ett annat**. Användaren skapas i en inaktiverad och väntande godkännandestatus. En Workfront-administratör måste godkänna användaren, som aktiverar användaren i Workfront och lägger till dem i Adobe Admin Console.

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

{{step-1-to-users}}

1. Markera användaren som du vill kopiera och klicka sedan på ikonen Kopiera ![](assets/copy-icon.png).
1. I rutan **Kopiera användare** som visas redigerar du de fält som är tillgängliga för den nya användaren.

   Mer information om alla fält som är associerade med en användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Klicka på **Lägg till den här personen**.

   eller

   Klicka på **Lägg till person och starta en annan** för att spara den nya användaren och lägga till en ny.

Detta skapar ett nytt konto i Workfront för användaren.

Om du har valt att skicka en inbjudan till användaren bör användaren få ett e-postmeddelande där han/hon kan följa en länk för att skapa sitt Workfront-lösenord.

>[!NOTE]
>
Om din organisation har anslutit sig till Admin Console och du lägger till en användare via Workfront har du inte möjlighet att skicka en e-postinbjudan.
>
För användare som redan har Adobe kan användaren få ett e-postmeddelande om att Workfront är tillgängligt eller inte. Detta är en inställning som styrs av Adobe-administratören för produkten.
