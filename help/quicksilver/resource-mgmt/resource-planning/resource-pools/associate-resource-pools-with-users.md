---
product-area: resource-management
navigation-topic: resource-pools
title: Associera resurspooler med användare
description: Du måste skapa en resurspool innan du kan associera den med användare. Du kan associera användare med resurspooler när du skapar resurspooler.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Associera resurspooler med användare

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Resurspooler är användarsamlingar som hjälper dig att hantera resurser i Adobe Workfront.

Du måste skapa en resurspool innan du kan associera den med användare.

Du kan associera användare med resurspooler när du skapar resurspooler.

Om du skapar resurspooler utan att fylla dem med användare kan du senare koppla dem till användare när du redigerar eller skapar nya användare.

Mer information om resurspooler finns i [Översikt över resurspooler](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Mer information om hur du skapar resurspooler finns i [Skapa resurspooler](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Hantera resurspooler</p> <p>Redigera åtkomst till projekt, mallar och användare</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera behörigheter för de projekt, mallar och användare som du vill associera resurspoolerna med</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Associera resurspooler med en användare

{{step-1-to-users}}

1. Markera rutan bredvid namnet på en användare i listan och klicka sedan på **Redigera**.
1. Klicka på **Resursplanering**.
1. Börja skriva namnet på en resurspool som du vill associera med användaren i fältet **Resurspooler** och markera den sedan i listan när den visas.\
   Du kan associera flera resurspooler med en användare.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Klicka på **Spara ändringar**.

Mer information om hur du redigerar användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Mer information om hur du skapar nya användare finns i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associera resurspooler med användare i grupp

Du kan redigera flera användare samtidigt och associera samma resurspooler med alla samtidigt.

Så här associerar du resurspooler med flera användare samtidigt:

{{step-1-to-users}}

1. Markera flera användare i listan och klicka på **Redigera**.
1. Klicka på **Resursplanering**.
1. Börja skriva namnet på en resurspool som du vill associera med användarna i fältet **Resurspooler** och markera den sedan i listan när den visas.\
   Du kan associera flera resurspooler med flera användare.

   >[!NOTE]
   >
   >Endast de resurspooler som är gemensamma för alla markerade användare visas i det här fältet. Om de valda användarna inte har några delade resurspooler är det här fältet tomt. Om det här fältet är tomt skrivs de resurspooler som du anger här över sina enskilda resurspooler.

1. Klicka på **Spara ändringar**.

Mer information om hur du redigerar flera användare samtidigt finns i [Redigera flera användarprofiler](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
