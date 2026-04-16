---
title: Bevilja åtkomst till jobbroller
description: Som Adobe Workfront-administratör kan du definiera en användares åtkomst till jobbroller i Workfront via åtkomstnivån.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a5ba79da-37f3-43f8-a7e2-4ccd75b56fef
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Bevilja åtkomst till jobbroller

Som Adobe Workfront-administratör kan du definiera en användares åtkomst till jobbroller via användarens åtkomstnivå, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Mer information om jobbroller finns i [Skapa och hantera jobbroller](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera användares åtkomst för att redigera jobbroller med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen **Visa** eller **Redigera** till höger om jobbroller och välj sedan de funktioner som du vill ge under **Finjustera inställningarna**.

   >[!NOTE]
   >
   >**Vyn** är standardåtkomst för jobbroller.

   ![Finjustera tillgången till jobbrollen](assets/job-role-access-view-fine-tune.png)

   Användare med **Visa**-åtkomst kan visa befintliga jobbroller och kan göra följande om du vill:

   * Visa faktureringstariffer för jobbroller
   * Visa kostnadstariffer för jobbroller
   * Visa allmänna finansfält (som inte är relaterade till fakturering eller kostnadstariffer) för jobbroller

   Användare med **Redigera**-åtkomst kan visa och redigera befintliga jobbroller och kan göra följande om du vill:

   * Skapa nya jobbroller
   * Ta bort jobbroller
   * Redigera faktureringstariffer för jobbroller
   * Redigera kostnadstariffer för jobbroller
   * Redigera allmänna finansfält (som inte är relaterade till fakturering eller kostnadstariffer) på jobbroller
   * Visa faktureringstariffer, kostnadstariffer och allmänna finansområden för jobbroller

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Åtkomst till jobbroller efter licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med jobbroller finns i avsnittet [Jobbroller](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#job-roles) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
