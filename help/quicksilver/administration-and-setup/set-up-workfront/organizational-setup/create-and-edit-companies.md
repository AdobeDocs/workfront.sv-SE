---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Skapa och redigera företag
description: Du kan lägga till företag i [!DNL Workfront] och använda dem för ekonomisk planering, rapportering, för att definiera behörigheter kring objekt och för att hålla information konfidentiell.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1394'
ht-degree: 0%

---

# Skapa och redigera företag

{{highlighted-preview}}

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ett företag är en organisationsenhet i [!DNL Adobe Workfront] som kan representera din organisation, en avdelning inom organisationen eller en klient som du arbetar med. Du kan lägga till företag i [!DNL Workfront] och använda dem för ekonomisk planering, rapportering, för att definiera behörigheter kring objekt och för att hålla information konfidentiell.

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
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
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

## Fördelar med att lägga till användare i ett företag {#benefits-of-adding-users-to-a-company}

* Du kan skapa ett företags organisationsschema genom att associera användare med direkta rapporter. Endast användare från samma företag kan läggas till som direkta rapporter för en annan användare från det företaget.
* Som projektledare kan du identifiera tillgängliga resurser inom samma företag.
* Du kan hålla information privat mellan företag genom att välja en eller alla av följande inställningar:

   * Användare från samma företag kan se varandras förfrågningar.

     Mer information om hur [!DNL Workfront] kan administratören ge liknande åtkomst till förfrågningar som baseras på användarens företag, se avsnittet [Konfigurera inställningar för uppgifter och ärenden för alla i [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) i artikeln [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Mer information om hur en gruppadministratör kan ge liknande åtkomst till begäranden baserade på användarföretag finns i [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Användare kan bara se begärandeköer som är kopplade till deras företag. Mer information om hur du begränsar synligheten för en frågekö finns i [Ge åtkomst till begärandeköer](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Du kan begränsa användare så att de bara kan se användare i sitt företag eller i sitt företag och i det primära företaget. Mer information om det primära företagets funktioner för användarintegritet finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Användare kan begränsa de uppdateringar de gör av objekt så att de bara visas av deras företagsanvändare. Mer information om hur du gör en uppdatering privat för ett företag finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Skapa eller redigera ett företag i [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Det finns ingen gräns för hur många företag du kan lägga till. Vi rekommenderar dock att du begränsar antalet företag som du använder på grund av problem som kan uppstå med objektbehörigheter. För mycket fragmentering kan störa användarnas synlighet för arbetsobjekten.

Som standard är det företag som är associerat med din instans av [!DNL Workfront] har redan skapats i [!DNL Workfront] och är det primära företaget för din organisation. Det har samma namn som ditt kundnamn. Mer information om kundinformation finns i [!DNL Workfront], se [Konfigurera grundläggande information för ditt system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Så här lägger du till eller redigerar ett företag:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Companies]**.
1. Om du lägger till ett företag klickar du på **[!UICONTROL New Company]**.

   eller

   Om du redigerar ett befintligt företag väljer du företaget och klickar sedan på **[!UICONTROL Edit]**.

1. Använd alternativen som visas för att konfigurera följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Ange ett namn för företaget.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: När det här alternativet är aktiverat kan användare hitta företaget och bifoga det till projekt som de skapar och redigerar. Ett inaktivt företag kan inte bifogas till projekt. Det här alternativet är aktiverat som standard.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Tilldelar företaget som din organisations primära företag. Det primära företaget representerar vanligtvis din [!DNL Workfront] där de flesta av dina användare arbetar.</p> <p>Du kan ha ett företag eller inget företag angivet som primärt företag, men du kan inte ha flera företag angivna som primärföretag. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> <p><b>ANMÄRKNING</b>: Genom att ändra åtkomstnivåerna kan du begränsa användarnas möjligheter att se andra användare: endast i sitt huvudföretag, eller i sitt närstående företag och huvudföretaget. Mer information om hur huvudföretaget fungerar med användarnas åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Om det finns en grupp som gör affärer med företaget kan du lägga till namnet på gruppen här. Detta är användbart för gruppadministratörer som behöver rapportera om och hantera alla företag som deras grupper gör affärer med.</p> <p><b>VIKTIGT</b>: Om du inte associerar gruppen som ska arbeta med det här företaget, kan inte administratörer för gruppen komma åt såvida de inte har administrativ åtkomst till företag på åtkomstnivån. Mer information om hur den här åtkomsten beviljas finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Börja skriva namnet på gruppen och tryck sedan på <strong>[!UICONTROL Enter]</strong> när den visas.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">När du tilldelar en grupp till ett företag, ökar gruppadministratörerna för gruppen [!UICONTROL Manage] åtkomst till företaget. Mer information finns i <a href="#group-administrators-and-companies" class="MCXref xref">Gruppadministratörer och företag</a> i den här artikeln.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Lägg till befintliga användare i företaget. Genom att göra detta associerar du de här användarna med det här företaget.</p> <p>Det finns ingen gräns för hur många användare du associerar med ett företag, men en användare kan inte associeras med mer än ett företag.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rates] section</td> 
      <td> <p><span class="preview">Det här avsnittet har tagits bort i förhandsvisningsmiljön.</span></p><p>Du kan åsidosätta faktureringstariffer som är kopplade till dina jobbroller på företagsnivå. Mer information om hur du skapar jobbroller och associerar dem med faktureringstariffer finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Mer information om att åsidosätta faktureringssatser på företagsnivå finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref">Åsidosätt faktureringssatser för jobbroller på företagsnivå</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>Om det finns fält som du vill lägga till i företaget som inte är tillgängliga i [!DNL Workfront]kan du skapa ett eget formulär och associera det med ditt företag. Du kan bifoga det här formuläret till ditt företag genom att välja det i listrutan. Endast aktiva företag visas i listrutan. Mer information om hur du skapar anpassade Forms finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Skapa eller redigera ett anpassat formulär</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Om du skapar ett nytt företag klickar du på **[!UICONTROL Create Company]**.

   eller

   Om du redigerar ett befintligt företag klickar du på **[!UICONTROL Save Changes]**.

## Hantera företagsmedlemskap

Mer information om hur du hanterar medlemskap för ett befintligt företag finns i [Hantera företagsmedlemskap](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Hantera faktureringstariffer

Mer information om att åsidosätta faktureringssatser på företagsnivå finns i [Åsidosätt faktureringssatser för jobbroller på företagsnivå](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Om att dela objekt med företag

Vissa behörigheter är tillgängliga för användare som är kopplade till ett företag, vilket förklaras i avsnittet [Fördelar med att lägga till användare i ett företag](#benefits-of-adding-users-to-a-company). Förutom dessa behörigheter kan du ge användarna behörighet att visa, bidra till och redigera objekt i [!DNL Workfront] genom att dela objektet med företaget.

I stället för att dela ett objekt med en enskild användare åt gången kan du dela det med hela företaget. Alla användare i företaget har samma behörigheter för det objektet.

Mer information om att dela objekt finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Gruppadministratörer och företag {#group-administrators-and-companies}

När en [!DNL Workfront] administratör tilldelar en grupp till ett företag, gruppadministratörer för gruppökningen [!UICONTROL Manage] behörighet till företaget i [!UICONTROL Setup]. Detta inkluderar åtkomst till [!UICONTROL Companies] sida in [!UICONTROL Setup], där de kan se och hantera det företag som är associerat med deras grupp.

Med den här åtkomsten till [!UICONTROL Companies] kan en gruppadministratör tilldela en grupp till ett företag, men det måste vara ett företag som gruppadministratören har skapat. Om gruppadministratörens åtkomstnivå inte är konfigurerad med administrativ åtkomst till företag kan du [!UICONTROL Group] fältet är obligatoriskt när gruppadministratören skapar företaget. Det är en rubrik med fet stil som anger detta:

![](assets/manage-company-group-field-req.jpg)

Mer information om hur användare får administrativ åtkomst till företag på åtkomstnivå finns i [Ge användarna administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Mer information om hur du hanterar ett företag i [!UICONTROL Setup] område, se [Skapa eller redigera ett företag i [!DNL Workfront]](#create-or-edit-a-company-in-workfront) i den här artikeln.
