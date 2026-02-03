---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Dela en dokumentmapp
description: Du kan dela en mapp och dess innehåll från området Dokument.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Dela en dokumentmapp

Du kan dela en mapp och dess innehåll från området Dokument.

>[!NOTE]
>
>* Mappen måste finnas på de fem översta nivåerna i en mapphierarki på ett objekt. Varje mapp på sjätte nivån eller tidigare ärver sina delningskonfigurationer från mappen direkt ovanför den.
>
>  Mer information om hur du lägger till undermappar för att skapa en mapphierarki finns i avsnittet [Skapa mappar och undermappar](../../documents/organizing-documents/create-documents-folder.md#creating-folders) i artikeln [Skapa dokumentmappar](../../documents/organizing-documents/create-documents-folder.md).
>
>* Smarta mappar kan inte delas.
>* Om du konfigurerar delningsalternativ för en dokumentmapp i en mall, och någon sedan skapar ett projekt från den mallen, överförs inte dina delningskonfigurationer till dokumentmappen i det nya projektet.
>* Om du konfigurerar delningsalternativ för en dokumentmapp i ett arbetsobjekt och sedan kopierar arbetsobjektet, överförs inte dina delningskonfigurationer till dokumentmappen i det nya arbetsobjektet.
>

## Åtkomstkrav

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td> <p>Ljus eller högre</p> 
   <p>Granska eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst till dokument</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till ett objekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dela en mapp

{{step1-to-documents}}

eller

Klicka på **Dokument** i den vänstra panelen när ett Workfront-objekt är öppet.

1. Markera mappen och klicka sedan på delningsikonen ![Dela-ikonen](assets/share-icon.png) i verktygsfältet.

   Mappen måste finnas på de fem översta nivåerna i en mapphierarki på ett objekt och kan inte vara en smart mapp.

1. I rutan som visas, under **Ge mappåtkomst till**, börjar du skriva namnet på den användare, det team, den jobbroll, den grupp eller det företag som du vill dela mappen med och trycker sedan på **Retur** när namnet visas.
1. Om du vill justera åtkomsten för användaren, teamet, jobbrollen, gruppen eller företaget som du just lade till klickar du på listrutan till höger om namnet och konfigurerar sedan något av följande tillgängliga alternativ och någon av de avancerade inställningarna:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Se det</td> 
      <td> <p>Möjlighet att visa mappen och dess innehåll.</p> <p>Klicka på <strong>Avancerade inställningar</strong> för att ange om du vill tillåta följande:</p> 
       <ul> 
        <li><strong>Hämta</strong>: Möjlighet att hämta mappen och dess innehåll som en ZIP-fil</li> 
        <li> <p><strong>Dela</strong>: Möjlighet att dela mappen med andra i systemet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hantera det</td> 
      <td> <p>Möjlighet att visa och redigera mappen och dess innehåll</p> <p>Klicka på <strong>Avancerade inställningar</strong> för att ange om du vill tillåta användare att göra följande:</p> 
       <ul> 
        <li><strong>Ta bort</strong>: Ta bort mappen och dess innehåll från systemet</li> 
        <li><b>Hämta</b>: Hämta mappen och dess innehåll som en ZIP-fil</li> 
        <li><strong>Dela</strong>: Dela mappen och dess innehåll med andra användare i systemet</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa steg 3-4 om du vill lägga till andra namn i listan och konfigurera deras alternativ.
1. (Valfritt) Om du vill att alla i systemet ska kunna visa mappen och dess innehåll klickar du på kugghjulsikoninställningarna ![Kugghjulsikoner med nedpilen](assets/gear-icon-settings-with-dn-arrow.jpg) i det övre högra hörnet av delningsrutan och klickar sedan på **Gör den här synliga systemomfattande.**

   Om du ändrar dig kan du klicka på **Ta bort systemomfattande åtkomst** (standardalternativet).

## Hur användare får åtkomst till innehållet i en mapp som delas med dem

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story   <a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

När du delar en mapp kan mottagarna för närvarande inte se mappen i området Dokument. De kan dock komma åt sina dokument genom att köra en dokumentrapport.

Mer information om hur du kör en rapport finns i avsnittet [Rapport om objekt](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) i artikeln [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Se även [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Ärvda behörigheter när du delar ett objekt som innehåller en mapp

När du delar ett objekt som har en dokumentmapp får mottagarna även åtkomst till mappen:

* Om du ger mottagarna åtkomst till det överordnade objektet Visa har de åtkomst till mappen.
* Om du ger mottagarna Contribute eller Hantera åtkomst till det överordnade objektet har de Hantera-åtkomst till mappen.
* Om du ger en typ av åtkomst (Visa, Contribute eller Hantera) till det överordnade objektet, och en annan typ till mappen, har mottagarna den högsta av dessa två typer av åtkomst till dokument i mappen

  Om du till exempel delar det överordnade objektet med behörigheten Visa och mappen med behörigheten Hantera, har mottagarna behörigheten Hantera för dokumenten i mappen.

  >[!NOTE]
  >
  >Ett bifogat dokument ärver endast behörigheter från det objekt som det bifogades till. Om du skapar en mapp på objektet och flyttar dokumentet till mappen, ärver den mappens behörigheter. Men om du skapar en mapp i ett överordnat eller indirekt överordnat objekt och flyttar dokumentet till den mappen, ärver den inte mappens behörigheter.

* Om alternativet&quot;Ärv aldrig dokumentåtkomst från projekt, uppgifter, problem osv.&quot; är aktiverat på mottagarens åtkomstnivå ärver de inte behörigheter till dokument i en mapp som du delar med dem. Om du vill ge dem åtkomst till ett dokument i mappen måste du dela dokumentet.

  Mer information om alternativet Ärv aldrig finns i [Konfigurera åtkomst till Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Mer information om hur du delar ett dokument finns i [Dela ett dokument](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
