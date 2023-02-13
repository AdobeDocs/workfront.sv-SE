---
product-area: templates
navigation-topic: templates-navigation-topic
title: Dela projektmallar
description: Du kan dela en mall med användare eller definiera hur projekt som skapas från en mall ska delas med användarna med hjälp av följande delningsalternativ på mallnivå.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 0%

---

# Dela projektmallar

Du kan dela en mall med användare eller definiera hur projekt som skapas från en mall ska delas med användarna med hjälp av följande delningsalternativ på mallnivå.

När du delar ett objekt i Adobe Workfront kan andra användare visa, bidra till eller redigera det objektet.

Mer information om Workfront behörigheter finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Mer information om vilka behörigheter du kan ge användare när du delar en mall finns i [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mallar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en mall</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Dela en mall {#share-a-template}

Du kan dela dina mallar med andra användare genom att använda malldelning. Den här åtgärden definierar vem som har behörighet till mallen.

>[!NOTE]
>
>När du anger en aktiv användare som mallägare får den användaren automatiskt behörigheten Hantera för mallen. Mer information om hur du anger någon som mallägare finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Så här delar du en mall:

1. Från **Huvudmeny** icon ![](assets/main-menu-icon.png), klicka **Mallar**.

1. Gör något av följande:\
   Klicka på namnet på en mall för att öppna den och klicka sedan på **Mer** meny ![](assets/qs-more-icon-on-an-object.png)sedan **Malldelning**.

   eller

   Välj en mall från listan och klicka på ikonen Dela ![](assets/share-icon.png)och sedan klicka **Mall.**

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. I **Mallåtkomst** markerar du de personer, team, roller, grupper eller företag som du vill dela mallen med.

   Du kan också klicka på **Alternativ** -ikonen för att göra mallen tillgänglig för hela systemet:

1. Välj något av följande i listrutan för varje enhet som du delar med:

   * **Visa**: Användare med dessa behörigheter kan visa mallen och skapa ett projekt med hjälp av den eller bifoga den till ett befintligt projekt.

      >[!TIP]
      >
      >Din Workfront-administratör måste ge dig redigeringsåtkomst till projekt för att kunna skapa projekt.

   * **Hantera**: Användare med dessa behörigheter kan redigera eller ta bort mallen.

      Mer information om de avancerade inställningarna ![](assets/gear-icon-in-access-levels.png) finns här, se avsnittet [Avancerade inställningar för malldelning](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) i artikeln [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Klicka **Spara**.

## Dela ett projekt från en mall {#share-a-project-from-a-template}

Med Projektdelning för mallar kan du definiera vem som har behörighet för de projekt som skapas från mallen på mallnivå.

Så här delar du framtida projekt som skapats från en mall med användare:

1. Gör något av följande:\
   Klicka på namnet på en mall för att öppna den och klicka sedan på **Mer** meny ![](assets/qs-more-icon-on-an-object.png)sedan **Malldelning**.

   ![Dela projekt från mall](assets/project-sharing-on-template-nwe-2022-350x172.png)

   eller

   Välj en mall från listan och klicka på **Dela** och sedan klicka **Projekt.**

1. I **Projektåtkomst** markerar du de personer, team, roller, grupper eller företag som mallen delas med.

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. Välj något av följande i listrutan för varje enhet:

   * **Ingen åtkomst**: Du kan ange vilka användare som inte har tillgång till mallen.\
      Det här alternativet är endast tillgängligt när du delar projekt gruppvis från mallar. 
   * **Visa**: Användare med dessa behörigheter kan visa projekt som skapats från mallen.
   * **Contribute**: Användare med den här behörigheten kan bidra till projekt som skapas från mallen 
   * **Hantera**: Användare med dessa behörigheter kan hantera eller ta bort projekt som skapats från den här mallen.

1. (Valfritt) Klicka på **Alternativ** om du vill göra projekten tillgängliga i hela systemet.
1. Klicka **Spara**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## Dela mallar och projekt från mallar i grupp

Du kan dela flera mallar samt projekt från flera mallar samtidigt.

>[!NOTE]
>
>När du väljer flera mallar kan du inte visa vem som redan har behörighet till de enskilda mallarna.

1. Gå till en lista med mallar.
1. Markera flera mallar och klicka sedan på ![Dela](assets/share-icon.png).

   ![Dela mallar och projekt i grupp](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. Klicka **Mall** för att dela de valda mallarna.

   eller

   Klicka **Projekt** för att dela projekt som ska skapas från de valda mallarna.

1. Fortsätt att dela mallarna eller projekten enligt beskrivningen i följande avsnitt i den här artikeln:

   * [Dela en mall](#share-a-template)
   * [Dela ett projekt från en mall](#share-a-project-from-a-template)
