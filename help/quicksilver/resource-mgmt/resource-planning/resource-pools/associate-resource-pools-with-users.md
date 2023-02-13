---
product-area: resource-management
navigation-topic: resource-pools
title: Associera resurspooler med användare
description: Associera resurspooler med användare
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '494'
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

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Hantera resurspooler</p> <p>Redigera åtkomst till projekt, mallar och användare</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för de projekt, mallar och användare som du associerar resurspoolerna med</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Associera resurspooler med en användare

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Användare**.
1. Markera rutan bredvid namnet på en användare i listan och klicka sedan på **Redigera**.
1. Klicka **Resursplanering**.
1. Börja skriva namnet på en resurspool som du vill associera med användaren i **Resurspooler** markerar du den i listan när den visas.\
   Du kan associera flera resurspooler med en användare.\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. Klicka **Spara ändringar**.

Mer information om hur du redigerar användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Mer information om hur du skapar nya användare finns i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Associera resurspooler med användare i grupp

Du kan redigera flera användare samtidigt och associera samma resurspooler med alla samtidigt.

Så här associerar du resurspooler med flera användare samtidigt:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka **Användare**.
1. Markera flera användare i listan och klicka på **Redigera**.
1. Klicka **Resursplanering**.
1. Börja skriva namnet på en resurspool som du vill associera med användarna i **Resurspooler** markerar du den i listan när den visas.\
   Du kan associera flera resurspooler med flera användare.

   >[!NOTE]
   >
   >Endast de resurspooler som är gemensamma för alla markerade användare visas i det här fältet. Om de valda användarna inte har några delade resurspooler är det här fältet tomt. Om det här fältet är tomt skrivs de resurspooler som du anger här över sina enskilda resurspooler.

1. Klicka **Spara ändringar**.

Mer information om hur du redigerar flera användare samtidigt finns i [Redigera användarprofiler gruppvis](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).
