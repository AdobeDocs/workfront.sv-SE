---
product-area: resource-management
navigation-topic: resource-pools
title: Associera resurspooler med projekt och mallar
description: Resurspooler är användarsamlingar som hjälper dig att hantera resurser i Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Associera resurspooler med projekt och mallar


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningsmiljön.</span>


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
</div>
-->

Resurspooler är användarsamlingar som hjälper dig att hantera resurser i Adobe Workfront.

När du har skapat resurspooler kan du associera dem med projekt eller mallar så att du senare kan budgetera dina resurser för projekten.

Vi rekommenderar att du skapar resurspooler i förväg, associerar dem med projekt och budgeterar dina resurser innan projektet startar.

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

## Associera resurspooler med ett projekt eller en mall

Du kan associera resurspooler med en mall på samma sätt som du associerar resurspooler med ett projekt. I den här artikeln beskrivs hur du kan associera resurspooler med projekt.

1. Gå till ett projekt och klicka på **Mer** icon ![](assets/more-icon.png)bredvid projektnamnet och klicka sedan på **Redigera**.

1. Klicka **Projektinställningar**.

1. Börja skriva namnet på en resurspool i **Resurspooler** markerar du det i listan när det visas.\
   Du kan associera flera resurspooler med ett projekt eller en mall.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Klicka **Spara**.

Mer information om hur du redigerar ett projekt och associerar det med resurspooler finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Mer information om hur du redigerar en mall och associerar den med resurspooler finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associera resurspooler med flera projekt eller mallar i grupp

Du kan redigera flera projekt eller mallar samtidigt och associera samma resurspooler med alla samtidigt.

Du kan associera resurspooler med mallar på samma sätt som du associerar resurspooler med projekt.

Så här associerar du resurspooler med flera projekt samtidigt:

1. Gå till en lista med projekt.
1. Markera flera projekt och klicka sedan på **Redigera** icon ![](assets/edit-icon.png) högst upp i listan.

1. Klicka **Inställningar**.
1. Börja skriva namnet på en resurspool i **Resurspooler** markerar du det i listan när det visas.\
   Du kan koppla flera resurspooler till projekt eller mallar.

   >[!NOTE]
   >
   >* När du redigerar flera projekt eller mallar samtidigt i produktionsmiljön visas endast de resurspooler som är gemensamma för alla projekt eller mallar som är markerade i det här fältet. Om de valda projekten inte har några delade resurspooler kommer det här fältet att vara tomt. Resurspoolerna som du anger här skriver över de enskilda resurspoolerna för projekten eller mallarna.
   >
   >* <span class="preview">När du redigerar flera projekt samtidigt i förhandsgranskningsmiljön visas en indikator för flera värden om de valda projekten har olika resurspooler. Om du lägger till flera resurspooler samtidigt läggs alla pooler till i det valda projektet och de ursprungliga resurspoolerna skrivs över.</span>


   <span class="preview">![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)</span>

1. Klicka **Spara ändringar**.\
   När resurspoolerna är kopplade till dina projekt eller dina mallar kan du budgetera användarallokeringar för dina projekt i resursplaneraren.\
   Mer information om resursplaneraren finns i [Översikt över resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Mer information om hur du redigerar flera projekt samtidigt finns i avsnittet Redigera flera projekt i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Mer information om hur du redigerar flera mallar samtidigt finns i avsnittet Redigera mallar samtidigt i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
