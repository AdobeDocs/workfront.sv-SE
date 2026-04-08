---
title: Bevilja åtkomst till jobbroller
description: xxxxxxxxxxxxxxxx
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 627d59c8c8296e5b6c8b6da53705a1c3d7633751
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# Bevilja åtkomst till jobbroller

{{highlighted-preview-article-level}}

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

   Användare med **Visa**-åtkomst kan visa befintliga jobbroller och eventuellt visa faktureringstariffer, kostnadstariffer och allmän ekonomi för jobbroller.

   Användare med **Redigera**-åtkomst kan visa och redigera befintliga jobbroller och kan göra följande om du vill:

   * Skapa nya jobbroller
   * Ta bort jobbroller
   * Visa faktureringstariffer, kostnadstariffer och allmänna finanser för jobbroller
   * Redigera faktureringstariffer, kostnadstariffer och allmänna finanser för jobbroller

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. När du är klar klickar du på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Åtkomst till jobbroller efter licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med jobbroller finns i avsnittet [Jobbroller](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#job-roles) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
