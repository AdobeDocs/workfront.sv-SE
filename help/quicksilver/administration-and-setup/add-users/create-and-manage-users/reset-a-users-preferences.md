---
title: Återställ en användares inställningar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du återställa eller ta bort användarinställningarna för alla användare i Workfront-systemet. Enskilda användare kan även återställa sina egna användarinställningar.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Återställ en användares inställningar

Som Adobe Workfront-administratör kan du återställa eller ta bort användarinställningarna för alla användare i Workfront-systemet.

Enskilda användare kan även återställa sina egna användarinställningar.

## Åtkomstkrav

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Om påverkade inställningar

När du återställer användarinställningarna återställs vissa inställningar till systemets standardinställningar och andra tas bort:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Inställningar</strong> </th> 
   <th><strong>Status efter återställning</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Vyer</td> 
   <td> <p> Återställd till systemstandard</p> <p>Befintliga vyer tas inte bort. Du kan markera dem igen.</p> </td> 
  </tr> 
  <tr> 
   <td>Filter</td> 
   <td> <p>Återställd till systemstandard</p> <p>Befintliga filter tas inte bort. Du kan markera dem igen.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupperingar</td> 
   <td> <p>Återställd till systemstandard</p> <p>Befintliga grupperingar tas inte bort. Du kan markera dem igen.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista med senaste objekt</td> 
   <td>Rensad</td> 
  </tr> 
  <tr> 
   <td>Favoritlista</td> 
   <td>Opåverkad</td> 
  </tr> 
  <tr> 
   <td>Användarinställningar</td> 
   <td> <p>Återställd till systemstandard</p> <p>E-postmeddelanden återställs till systemets standardinställningar</p> </td> 
  </tr> 
  <tr> 
   <td>Användardefinierade anpassade flikar</td> 
   <td>Borttagen</td> 
  </tr> 
  <tr> 
   <td>Användardefinierade alternativ för global navigering</td> 
   <td>Återgå till layoutmallsdefinition eller systemstandard om ingen layoutmall har tilldelats.</td> 
  </tr> 
 </tbody> 
</table>

## Återställ användarinställningar

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Välj **Logga in som**.
1. Börja skriva namnet på den användare vars inställningar du vill återställa och klicka sedan på namnet när det visas i listrutan.
1. Välj  **Logga in**.
1. Lägg till `/resetUser` efter `workfront.com`.

   >[!NOTE]
   >
   >Det här är skiftlägeskänsligt. U måste ha inledande versal och de återstående tecknen måste ha gemener. Exempel:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Tryck **Retur**.
1. Om du vill återställa alla användarinställningar väljer du **Återställ**.

   eller

   Om du bara vill återställa anpassade flikar väljer du **Återställ flikar**.
