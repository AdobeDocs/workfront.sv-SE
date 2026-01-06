---
product-area: templates
navigation-topic: templates-navigation-topic
title: Dela projektmallar
description: Du kan dela en mall med användare eller definiera hur projekt som skapas från en mall ska delas med användarna med hjälp av följande delningsalternativ på mallnivå.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Dela projektmallar

Du kan dela en mall med användare eller definiera hur projekt som skapas från en mall ska delas med användarna med hjälp av följande delningsalternativ på mallnivå.

När du delar ett objekt i Adobe Workfront kan andra användare visa, bidra till eller redigera det objektet.

Mer information om Workfront-behörigheter finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Mer information om vilka behörigheter du kan ge användare när du delar en mall finns i [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till mallar</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en mall</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Dela en mall {#share-a-template}

Du kan dela dina mallar med andra användare genom att använda malldelning. Den här åtgärden definierar vem som har behörighet till mallen.

>[!NOTE]
>
>När du anger en aktiv användare som mallägare får den användaren automatiskt behörigheten Hantera för mallen. Mer information om hur du anger någon som mallägare finns i [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Så här delar du en mall:

{{step1-to-templates}}

1. Gör något av följande:\
   Klicka på namnet på en mall för att öppna den, klicka sedan på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) och sedan på **Malldelning**.

   eller

   Välj en mall från listan, klicka på delningsikonen ![Dela mall](assets/share-icon.png) och klicka sedan på **Mall.**

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. I rutan **Mallåtkomst** markerar du de personer, team, roller, grupper eller företag som du vill dela mallen med.

   Du kan också klicka på ikonen **Alternativ** för att göra mallen tillgänglig i hela systemet:

1. Välj något av följande i listrutan för varje enhet som du delar med:

   * **Visa**: Användare med de här behörigheterna kan visa mallen och skapa ett projekt med hjälp av den, eller bifoga den till ett befintligt projekt.

     >[!TIP]
     >
     >Din Workfront-administratör måste ge dig redigeringsåtkomst till projekt för att kunna skapa projekt.

   * **Hantera**: Användare med de här behörigheterna kan redigera eller ta bort mallen.

     Mer information om de avancerade inställningarna ![Kugghjulsikonen](assets/gear-icon-in-access-levels.png) som finns här finns i avsnittet [Avancerade inställningar för malldelning](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) i artikeln [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Klicka på **Spara**.

## Dela ett projekt från en mall {#share-a-project-from-a-template}

Med Projektdelning för mallar kan du definiera vem som har behörighet för de projekt som skapas från mallen på mallnivå.

Så här delar du framtida projekt som skapats från en mall med användare:

1. Gör något av följande:\
   Klicka på namnet på en mall för att öppna den, klicka sedan på **Mer**-menyn ![Mer-ikonen](assets/more-icon.png) och sedan på **Malldelning**.

   ![Dela projekt från mall](assets/project-sharing-on-template-nwe-2022-350x172.png)

   eller

   Välj en mall från listan, klicka på **Dela** och sedan på **Projekt.**

1. I rutan **Projektåtkomst** markerar du de personer, team, roller, grupper eller företag som mallen delas med.

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. Välj något av följande i listrutan för varje enhet:

   * **Ingen åtkomst**: Du kan ange vilka användare som inte har åtkomst till mallen.\
     Det här alternativet är endast tillgängligt när du delar projekt gruppvis från mallar.
   * **Visa**: Användare med den här behörigheten kan visa projekt som skapats från mallen.
   * **Contribute**: Användare med dessa behörigheter kan bidra till projekt som skapas från mallen
   * **Hantera**: Användare med de här behörigheterna kan hantera eller ta bort projekt som skapats från den här mallen.

1. (Valfritt) Klicka på ikonen **Alternativ** för att göra projekten tillgängliga i hela systemet.
1. Klicka på **Spara**.

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

## Dela mallar och projekt från mallar

Du kan dela flera mallar samt projekt från flera mallar samtidigt.

>[!NOTE]
>
>När du väljer flera mallar kan du inte visa vem som redan har behörighet till de enskilda mallarna.

1. Gå till en lista med mallar.
1. Markera flera mallar och klicka sedan på ![Dela](assets/share-icon.png).

   ![Dela mallar eller projekt i grupp](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Du kan bara dela ett objekt med aktiva användare, team, roller eller företag.

1. Klicka på **Mall** om du vill dela de valda mallarna.

   eller

   Klicka på **Projekt** om du vill dela de projekt som ska skapas från de valda mallarna.

1. Fortsätt att dela mallarna eller projekten enligt beskrivningen i följande avsnitt i den här artikeln:

   * [Dela en mall](#share-a-template)
   * [Dela ett projekt från en mall](#share-a-project-from-a-template)
