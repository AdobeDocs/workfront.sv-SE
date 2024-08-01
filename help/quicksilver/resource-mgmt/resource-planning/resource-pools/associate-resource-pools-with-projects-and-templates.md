---
product-area: resource-management
navigation-topic: resource-pools
title: Associera resurspooler med projekt och mallar
description: Resurspooler är användarsamlingar som hjälper dig att hantera resurser i Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Associera resurspooler med projekt och mallar


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
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
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Hantera resurspooler</p> <p>Redigera åtkomst till projekt, mallar och användare</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
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

1. Gå till ett projekt och klicka på ikonen **Mer** ![](assets/more-icon.png)bredvid projektnamnet och klicka sedan på **Redigera**.

1. Klicka på **Projektinställningar**.

1. Börja skriva namnet på en resurspool i fältet **Resurspooler** och markera den i listan när den visas.\
   Du kan associera flera resurspooler med ett projekt eller en mall.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Klicka på **Spara**.

Mer information om hur du redigerar ett projekt och associerar det med resurspooler finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Mer information om hur du redigerar en mall och associerar den med resurspooler finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Associera resurspooler med flera projekt eller mallar i grupp

Du kan redigera flera projekt eller mallar samtidigt och associera samma resurspooler med alla samtidigt.

Du kan associera resurspooler med mallar på samma sätt som du associerar resurspooler med projekt.

Så här associerar du resurspooler med flera projekt samtidigt:

1. Gå till en lista med projekt.
1. Markera flera projekt och klicka sedan på ikonen **Redigera** ![](assets/edit-icon.png) längst upp i listan.

1. Klicka på **Inställningar**.
1. Börja skriva namnet på en resurspool i fältet **Resurspooler** och markera den i listan när den visas.\
   Du kan koppla flera resurspooler till projekt eller mallar.

   >[!NOTE]
   >
   >* När du redigerar flera mallar samtidigt visas endast de resurspooler som är gemensamma för alla valda mallar i det här fältet. Om de valda mallarna inte har några delade resurspooler är det här fältet tomt. Resurspoolerna som du anger här skriver över de enskilda resurspoolerna för projekten eller mallarna.
   >
   >* När du redigerar flera projekt samtidigt visas en indikator för flera värden om de markerade projekten har olika resurspooler. Om du lägger till resurspooler gruppvis för projekt läggs alla pooler till i det valda projektet och de ursprungliga resurspoolerna skrivs över.

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Klicka på **Spara ändringar**.\
   När resurspoolerna är kopplade till dina projekt eller dina mallar kan du budgetera användarallokeringar för dina projekt i resursplaneraren.\
   Mer information om resursplaneraren finns i [Översikt över resursplaneraren](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Mer information om hur du redigerar flera projekt samtidigt finns i avsnittet Redigera projekt i grupp i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

Mer information om hur du redigerar flera mallar samtidigt finns i avsnittet Redigera mallar i grupp i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
