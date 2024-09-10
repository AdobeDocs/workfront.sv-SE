---
title: Återställ en användares inställningar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du återställa eller ta bort användarinställningarna för alla användare i Workfront-systemet. Enskilda användare kan även återställa sina egna användarinställningar.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Återställ en användares inställningar

<!-- Audited: 12/2023 -->

Som Adobe Workfront-administratör kan du återställa eller ta bort användarinställningarna för alla användare i Workfront-systemet.

Enskilda användare kan även återställa sina egna användarinställningar.

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
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Om påverkade inställningar

När du återställer användarinställningarna återställs vissa inställningar till systemets standardinställningar och andra tas bort:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Inställningar</strong> </th> 
   <th><strong>Status efter återställningen</strong> </th> 
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
   <td> <p>Återställd till systemstandard</p> <p>E-postmeddelanden återställs till systemets standardinställningar. Standardmeddelandena visas i <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Händelsemeddelanden i Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Användardefinierade anpassade flikar</td> 
   <td>Borttagen</td> 
  </tr> 
  <tr> 
   <td>Användardefinierade alternativ för global navigering</td> 
   <td>Återgå till layoutmallsdefinition eller till systemstandard om ingen layoutmall har tilldelats.</td> 
  </tr> 
 </tbody> 
</table>

## Återställ användarinställningar

{{step-1-to-setup}}

1. Välj **Logga in som**.
1. Börja skriva namnet på den användare vars inställningar du vill återställa och klicka sedan på namnet när det visas i listrutan.
1. Välj **Logga in**.
1. Om din organisation inte har anslutit sig till Adobe enhetliga upplevelse följer du följande steg:

   * Lägg till `/resetUser` efter `workfront.com` i URL-fältet högst upp i webbläsaren.

     >[!NOTE]
     >
     >Det här är skiftlägeskänsligt. U måste ha inledande versal och de återstående tecknen måste ha gemener. Exempel:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Om din organisation har anslutit sig till Adobe enhetliga upplevelse följer du detta steg:

   * Lägg till `/resetUser` efter `workfront` i URL-fältet högst upp i webbläsaren.

     >[!NOTE]
     >
     >Det här är skiftlägeskänsligt. U måste ha inledande versal och de återstående tecknen måste ha gemener. Exempel:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Tryck på **Retur**.
1. Om du vill återställa alla användarinställningar väljer du **Återställ**.

   eller

   Om du bara vill återställa anpassade flikar väljer du **Återställ flikar**.
