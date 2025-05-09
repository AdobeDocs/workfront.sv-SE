---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Skapa och ändra en koncerns företag
description: När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med företag som är kopplade till gruppen och någon av dess undergrupper.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Skapa och ändra en grupps företag

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med företag som är kopplade till gruppen och någon av dess undergrupper.

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa, arbeta med och skapa företag för din grupp från gruppområdet

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen som du vill skapa eller ändra företag för.
1. Klicka på **Företag** i den vänstra panelen för att visa en lista över de företag som är associerade med gruppen och eventuella undergrupper som den har.
1. (Valfritt) Om du vill lägga till ett företag klickar du på **Lägg till företag** och konfigurerar sedan företaget med alternativen nedan. När du är klar klickar du på **Skapa företag**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Avsnittet Grundläggande information</td> 
      <td> 
       <ul> 
        <li> <p><b>Företagsnamn</b>: Ange ett namn för företaget.</p> </li> 
        <li> <p><b>Är aktiv</b>: När det här alternativet är aktiverat kan användare hitta företaget och bifoga det till projekt som de skapar och redigerar. Ett inaktivt företag kan inte bifogas till projekt. Det här alternativet är aktiverat som standard.</p> </li> 
        <li> <p><b>Det här är det primära företaget</b>: Tilldelar företaget som din organisations primära företag. Det primära företaget representerar vanligtvis ditt Workfront-konto där de flesta av dina användare arbetar.</p> <p>Genom att ändra åtkomstnivåerna kan du begränsa användarnas möjligheter att se andra användare:</p> 
         <ul> 
          <li>Endast i deras primära företag</li> 
          <li> <p>I sitt intressebolag och det primära företaget</p> <p>Mer information om de primära företagsfunktionerna i användarnas åtkomstnivåer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> <p>Du kan bara ha ett eller inget företag angivet som primärt företag, men du kan inte ha flera företag angivna som primärföretag. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Grupp</b>: Om det finns en grupp som gör affärer med företaget kan du lägga till namnet på gruppen här. Detta är användbart för gruppadministratörer som behöver rapportera om och hantera alla företag som deras grupper gör affärer med.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Systemet fyller i fältet <strong>Grupp</strong> för det nya företaget med gruppen som du visar.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Om du har administrativ åtkomst till företag på din åtkomstnivå kan du ta bort gruppen från företaget och tilldela en annan, eller lämna företaget utan någon grupp.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Om du inte har administrativ åtkomst till företag är fältet <strong>Grupp</strong> obligatoriskt och du kan bara välja de grupper som du hanterar eller undergrupper under dessa grupper.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Mer information om administrativ åtkomst till företag finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> </li> 
        <li> <p><b>Företagsmedlemmar</b>: Lägg till befintliga användare i företaget. Genom att göra detta associerar du de här användarna med det här företaget.</p> <p>Det finns ingen gräns för hur många användare du associerar med ett företag, men en användare kan inte associeras med mer än ett företag.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Anpassat Forms-avsnitt</td> 
      <td> <p>Om det finns fält som du vill lägga till i ditt företag som inte är tillgängliga i Workfront kan du skapa ett anpassat formulär och associera det med ditt företag. Du kan bifoga det här formuläret till ditt företag genom att välja det i listrutan. Endast aktiva företag visas i listrutan. Mer information om hur du skapar anpassade formulär finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Skapa ett anpassat formulär</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Om du har administrativ åtkomst till företag på din åtkomstnivå kan du även klicka på Lägg till fler företag längst ned i listan. Då läggs en rad till där du snabbt kan konfigurera det nya företaget.

1. (Valfritt) Om du vill redigera eller ta bort företag markerar du minst ett företag och använder sedan verktygsfältsknapparna för att redigera ![redigeringsikonen](assets/edit-icon.png) eller tar bort ![ikonen Ta bort](assets/delete.png) den.

   Mer information om hur du redigerar ett företag finns i avsnittet [Skapa eller redigera ett företag i Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) i artikeln [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Valfritt) Om du vill exportera listan med företag klickar du på ikonen Exportera ![ikonen Exportera](assets/export.png) och väljer sedan det filformat som du vill använda för den exporterade listan.
