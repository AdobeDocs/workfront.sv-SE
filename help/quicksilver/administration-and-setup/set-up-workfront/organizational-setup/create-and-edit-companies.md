---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Skapa och redigera företag
description: Du kan lägga till företag i  [!DNL Adobe Workfront] och använda dem för ekonomisk planering, rapportering, för att definiera behörigheter runt objekt och för att hålla information konfidentiell.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: b89715649473ba13e1b6b7a250dfed7a468bb4b4
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 0%

---

# Skapa och redigera företag

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Ett företag är en organisationsenhet i [!DNL Adobe Workfront] som kan representera din organisation, en avdelning inom organisationen eller en klient som du arbetar med. Du kan lägga till företag i [!DNL Workfront] och använda dem för ekonomisk planering, rapportering, för att definiera behörigheter runt objekt och för att hålla information konfidentiell.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>eller</p>
   <p>Nytt: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån [!UICONTROL System Administrator], som gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
     <li> <p>Administrativ åtkomst för att hantera företag, vilket gör att du kan redigera vilket företag som helst i systemet.</p> </li> 
    </ul> <p><b>OBS</b>:  
     <ul> 
      <li> <p>Du kan också hantera företag som är kopplade till en grupp där du har tilldelats som gruppadministratör.</p> </li> 
      <li> <p>Om du vill lägga till och ta bort användare från systemet [!DNL Workfront] måste du ha något av följande:</p> 
       <ul> 
        <li> <p>Åtkomstnivån [!UICONTROL System Administrator]. </p> </li> 
        <li> <p>I din åtkomstnivå måste [!UICONTROL Edit] väljas för inställningen [!UICONTROL Users]. Dessutom måste alternativet [!UICONTROL Create] och minst ett av de två alternativen [!UICONTROL User Admin] aktiveras under [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> för inställningen [!UICONTROL Users]. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Om du använder alternativet [!UICONTROL User Admin (Group Users)] måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fördelar med att lägga till användare i ett företag {#benefits-of-adding-users-to-a-company}

* Du kan skapa ett företags organisationsschema genom att associera användare med direkta rapporter. Endast användare från samma företag kan läggas till som direkta rapporter för en annan användare från det företaget.
* Som projektledare kan du identifiera tillgängliga resurser inom samma företag.
* Du kan hålla information privat mellan företag genom att välja en eller alla av följande inställningar:

   * Användare från samma företag kan se varandras förfrågningar.

     Mer information om hur en [!DNL Workfront]-administratör kan ge liknande åtkomst till begäranden baserade på användarens företag finns i avsnittet [Konfigurera aktivitets- och probleminställningar för alla i [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) i artikeln [Konfigurera systemomfattande aktivitets- och probleminställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Mer information om hur en gruppadministratör kan ge liknande åtkomst till begäranden baserade på användarens företag finns i [Konfigurera uppgifter och utgåvinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * Användare kan bara se begärandeköer som är kopplade till deras företag. Mer information om att begränsa synligheten för en begärandekö finns i [Ge åtkomst till begärandeköer](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * Du kan begränsa användare så att de bara kan se användare i sitt företag eller i sitt företag och i det primära företaget. Mer information om de primära företagsfunktionerna för användarsekretess finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Användare kan begränsa de uppdateringar de gör av objekt så att de bara visas av deras företagsanvändare. Mer information om hur du gör en uppdatering privat för ett företag finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Skapa eller redigera ett företag i [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Det finns ingen gräns för hur många företag du kan lägga till. Vi rekommenderar dock att du begränsar antalet företag som du använder på grund av problem som kan uppstå med objektbehörigheter. För mycket fragmentering kan störa användarnas synlighet för arbetsobjekten.

Som standard har det företag som är associerat med din instans av [!DNL Workfront] redan skapats i ditt [!DNL Workfront]-system och är det primära företaget för din organisation. Det har samma namn som ditt kundnamn. Mer information om din kundinformation i [!DNL Workfront] finns i [Konfigurera grundläggande information för ditt system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Så här lägger du till eller redigerar ett företag:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Companies]**.

   En lista över företag visas.

1. Om du lägger till ett företag klickar du på **[!UICONTROL New Company]**.

   eller

   Om du redigerar ett befintligt företag markerar du företaget och klickar sedan på ikonen **[!UICONTROL Edit]** ![Redigera](assets/edit-icon.png) överst i företagslistan.

1. Uppdatera följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Ange ett namn för företaget.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: När det här alternativet är aktiverat kan användarna hitta företaget och bifoga det till projekt som de skapar och redigerar. Ett inaktivt företag kan inte bifogas till projekt. Det här alternativet är aktiverat som standard.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Tilldelar företaget som din organisations primära företag. Det primära företaget representerar vanligtvis ditt [!DNL Workfront]-konto där de flesta av dina användare arbetar.</p> <p>Du kan ha ett företag eller inget företag angivet som primärt företag, men du kan inte ha flera företag angivna som primärföretag. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> <p><b>OBS!</b>: Genom att ändra åtkomstnivåerna kan du begränsa användarnas möjligheter att se andra användare: endast i deras primära företag eller i deras associerade företag och det primära företaget. Mer information om hur det primära företaget arbetar med användarnas åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Om det finns en grupp som gör affärer med företaget kan du lägga till namnet på gruppen här. Detta är användbart för gruppadministratörer som behöver rapportera om och hantera alla företag som deras grupper gör affärer med.</p> <p><b>VIKTIGT</b>: Om du inte associerar gruppen som ska arbeta med det här företaget kan inte administratörer för gruppen få åtkomst till företaget såvida de inte har administrativ åtkomst till företag på åtkomstnivå. Mer information om hur den här åtkomsten beviljas finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Börja skriva namnet på gruppen och tryck sedan på <strong>[!UICONTROL Enter]</strong> när den visas.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">När du tilldelar en grupp till ett företag får gruppadministratörerna för gruppen [!UICONTROL Manage] åtkomst till företaget. Mer information finns i <a href="#group-administrators-and-companies" class="MCXref xref">Gruppadministratörer och företag</a> i den här artikeln.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Lägg till befintliga användare i företaget. Genom att göra detta associerar du de här användarna med det här företaget.</p> <p>Det finns ingen gräns för hur många användare du associerar med ett företag, men en användare kan inte associeras med mer än ett företag.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>Om det finns fält som du vill lägga till i ditt företag som inte är tillgängliga i [!DNL Workfront] kan du skapa ett anpassat formulär och associera det med ditt företag. </p> <p>Du kan bifoga det här formuläret till ditt företag genom att välja det i listrutan. Endast aktiva anpassade formulär visas på menyn.</p> <p><strong>Obs!</strong> Avancerade anpassade formulärfunktioner som externa sökningsfält och inbyggda Workfront-fält är bara tillgängliga när du öppnar företagsposten på informationssidan, inte i dialogrutan Redigera företag. (I listan över företag klickar du på företagsnamnet för att öppna informationen.)</p> <p> Mer information om hur du skapar anpassade formulär finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Skapa ett anpassat formulär</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du skapar ett företag klickar du på **[!UICONTROL Create Company]**.

   eller

   Om du redigerar ett befintligt företag klickar du på **[!UICONTROL Save Changes]**.

## Hantera företagsmedlemskap

Mer information om hur du hanterar medlemskap för ett befintligt företag finns i [Hantera företagsmedlemskap](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Hantera faktureringstariffer

Mer information om att åsidosätta faktureringstariffer på företagsnivå finns i [Åsidosätt faktureringstaxor för jobbroller på företagsnivå](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Översikt över att dela objekt med företag

Vissa behörigheter är tillgängliga för användare som är associerade med ett företag, vilket förklaras i avsnittet [Fördelar med att lägga till användare i ett företag](#benefits-of-adding-users-to-a-company). Förutom dessa behörigheter kan du ge användare behörighet att visa, bidra och redigera objekt i [!DNL Workfront] genom att dela objektet med företaget.

I stället för att dela ett objekt med en enskild användare åt gången kan du dela det med hela företaget. Alla användare i företaget har samma behörigheter för det objektet.

Mer information om att dela objekt finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Gruppadministratörer och företag {#group-administrators-and-companies}

När en [!DNL Workfront]-administratör tilldelar en grupp till ett företag får gruppadministratörerna för gruppen [!UICONTROL Manage] åtkomst till företaget i [!UICONTROL Setup]. Detta inkluderar åtkomst till sidan [!UICONTROL Companies] i [!UICONTROL Setup], där de kan se och hantera det företag som är associerat med deras grupp.

Med den här åtkomsten till sidan [!UICONTROL Companies] kan en gruppadministratör tilldela en grupp till ett företag, men det måste vara ett företag som gruppadministratören har skapat. Om gruppadministratörens åtkomstnivå inte är konfigurerad med administrativ åtkomst till företag, krävs fältet [!UICONTROL Group] när gruppadministratören skapar företaget. Den feta titeln anger följande:

![Redigera företag](assets/group-admin-add-company.png)

Mer information om hur användare får administrativ åtkomst till företag på åtkomstnivå finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Mer information om hur du hanterar ett företag i området [!UICONTROL Setup] finns i [Skapa eller redigera ett företag i  [!DNL Workfront]](#create-or-edit-a-company-in-workfront) i den här artikeln.
