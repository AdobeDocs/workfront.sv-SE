---
title: Återställ en användares inställningar
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Som Adobe Workfront-administratör kan du återställa eller ta bort användarinställningarna för alla användare i Workfront-systemet. Enskilda användare kan även återställa sina egna användarinställningar.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: f1fe1a2fe6e123d8a039e8d7e3547c0b0a8141df
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 1%

---

# Återställ en användares inställningar

<!-- Audited: 12/2023 -->

Som Adobe Workfront-administratör kan du återställa eller ta bort användarinställningarna för alla användare i Workfront-systemet.

Enskilda användare kan även återställa sina egna användarinställningar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Om påverkade inställningar

När du återställer användarinställningarna återställs vissa inställningar till systemets standardinställningar och andra tas bort:

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

| Inställningar | Status efter återställning |
| --- | --- |
| Vyer | Återställd till systemstandard <p>Befintliga vyer tas inte bort. Du kan markera dem igen.</p> |
| Filter | Återställd till systemstandard <p>Befintliga filter tas inte bort. Du kan markera dem igen.</p> |
| Grupperingar | Återställd till systemstandard <p>Befintliga grupperingar tas inte bort. Du kan markera dem igen.</p> |
| Lista med senaste objekt | Rensad |
| Favoritlista | Opåverkad |
| Användarinställningar | Återställd till systemstandard <p>E-postmeddelanden återställs till systemets standardinställningar. Standardmeddelandena visas i [Händelsemeddelanden i Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

## Återställ användarinställningar

{{step-1-to-setup}}

1. Välj **Logga in som**.
1. Börja skriva namnet på den användare vars inställningar du vill återställa och klicka sedan på namnet när det visas i listrutan.
1. Välj **Logga in**.
1. Om din organisation inte har anslutit sig till Adobe Unified Experience gör du så här:

   * Lägg till `/resetUser` efter `workfront.com` i URL-fältet högst upp i webbläsaren.

     >[!NOTE]
     >
     >Det här är skiftlägeskänsligt. U måste ha inledande versal och de återstående tecknen måste ha gemener. Exempel:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Om din organisation har anslutit sig till Adobe Unified Experience gör du så här:

   * Lägg till `/resetUser` efter `workfront` i URL-fältet högst upp i webbläsaren.

     >[!NOTE]
     >
     >Det här är skiftlägeskänsligt. U måste ha inledande versal och de återstående tecknen måste ha gemener. Exempel:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Tryck på **Retur**.

1. Om du vill återställa alla användarinställningar klickar du på **Återställ**.

   eller

   Om du vill återställa användarens vänstra navigering till den ursprungliga layoutmallskonfigurationen klickar du på **Återställ vänster navigering**.
