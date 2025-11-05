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
source-git-commit: 6fb64986260842c419c61fe386e9ccf1a0da8f14
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# Skapa och redigera företag

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningens sandlådemiljö och släpps i en fasad utrullning till produktion.</span>

Ett företag är en organisationsenhet i [!DNL Adobe Workfront] som kan representera din organisation, en avdelning inom organisationen eller en klient som du arbetar med. Du kan lägga till företag i [!DNL Workfront] och använda dem för ekonomisk planering, rapportering, för att definiera behörigheter runt objekt och för att hålla information konfidentiell.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Åtkomstnivåkonfiguration</td> 
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

1. Uppdatera följande information i avsnittet **Grundläggande information**:

   * **Företagsnamn** <span class="preview"> eller **Namn**</span>: Ange ett namn för företaget.
   * **Är aktiv**: När det här alternativet är aktiverat kan användare hitta företaget och bifoga det till projekt som de skapar och redigerar. Ett inaktivt företag kan inte bifogas till projekt. Det här alternativet är aktiverat som standard.
   * **Det här är det primära företaget** <span class="preview"> eller **Är primärt**</span>: Tilldelar företaget som din organisations primära företag. Det primära företaget representerar vanligtvis ditt Workfront-konto där de flesta av dina användare arbetar.

     Du kan ha ett företag eller inget företag angivet som primärt företag, men du kan inte ha flera företag angivna som primärföretag. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

     >[!NOTE]
     >
     >Genom att ändra deras åtkomstnivåer kan du begränsa användarna så att de kan se andra användare: endast i det primära företaget eller i det tillhörande företaget och det primära företaget. Mer information om hur det primära företaget fungerar med användarnas åtkomstnivåer finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   * **Grupp**: Om det finns en grupp som gör affärer med företaget kan du lägga till namnet på gruppen här. Detta är användbart för gruppadministratörer som behöver rapportera om och hantera alla företag som deras grupper gör affärer med.

     Om du inte associerar gruppen som ska arbeta med det här företaget, kan inte administratörer för gruppen få åtkomst till företaget såvida de inte har administrativ åtkomst till företagen på åtkomstnivån. Mer information om hur den här åtkomsten beviljas finns i [Bevilja användare administrativ åtkomst till vissa områden](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Börja skriva namnet på gruppen och markera den när den visas.

     När du tilldelar en grupp till ett företag får gruppadministratörerna för gruppen behörigheten Hantera till företaget. Mer information finns i [Gruppadministratörer och företag](#group-administrators-and-companies) i den här artikeln.

   * **Företagsmedlemmar**: Lägg till befintliga användare i företaget. Genom att göra detta associerar du de här användarna med det här företaget.

     Börja skriva namnet på en användare och markera den när den visas.

     Det finns ingen gräns för hur många användare du associerar med ett företag, men en användare kan inte associeras med mer än ett företag.

1. Lägg till eller uppdatera anpassade formulär i avsnittet **Anpassad Forms**.

   Om det finns fält som du vill lägga till i ditt företag som inte är tillgängliga i Workfront kan du skapa ett anpassat formulär och associera det med ditt företag.

   Du kan bifoga det här formuläret till ditt företag genom att välja det i listrutan. Endast aktiva anpassade formulär visas på menyn.

   >[!NOTE]
   >
   >Avancerade anpassade formulärfunktioner som externa sökningsfält och inbyggda Workfront-fält är bara tillgängliga när du öppnar företagsposten på informationssidan, inte i dialogrutan Redigera företag. (I listan över företag klickar du på företagsnamnet för att öppna informationen.)

   Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Villkorligt) Om du skapar ett företag klickar du på **[!UICONTROL Create Company]** <span class="preview">eller **Spara**.</span>

   eller

   Om du redigerar ett befintligt företag klickar du på **[!UICONTROL Save Changes]** <span class="preview">eller **Spara**.</span>

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

Med den här åtkomsten till sidan [!UICONTROL Companies] kan en gruppadministratör tilldela en grupp till ett företag, men det måste vara ett företag som gruppadministratören har skapat. Om gruppadministratörens åtkomstnivå inte är konfigurerad med administrativ åtkomst till företag, krävs fältet [!UICONTROL Group] när gruppadministratören skapar företaget - dess <span class="preview"> asterisk </span> eller rubrik med fetstil anger detta:

<span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
![Ny företagsdialog med grupp krävs](assets/group-admin-add-company-group-required.png)

Exempelbild i produktionsmiljön:
![Grupp krävs för företag](assets/group-admin-add-company.png)

Mer information om hur användare får administrativ åtkomst till företag på åtkomstnivå finns i [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Mer information om hur du hanterar ett företag i området [!UICONTROL Setup] finns i [Skapa eller redigera ett företag i  [!DNL Workfront]](#create-or-edit-a-company-in-workfront) i den här artikeln.

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
