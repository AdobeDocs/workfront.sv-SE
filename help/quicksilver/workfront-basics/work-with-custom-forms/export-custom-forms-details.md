---
title: Exportera anpassad Forms och objektinformation
description: Du kan exportera översikten och den anpassade formulärinformationen från avsnittet Detaljer för ett objekt till en PDF-fil. Du kan sedan skriva ut eller dela PDF med andra användare.
author: Alina
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Exportera anpassade formulär och objektinformation

<!--Audited: 10/2025-->

Du kan exportera översikten och den anpassade formulärinformationen från avsnittet Detaljer för ett objekt till en PDF-fil. Du kan sedan skriva ut eller dela PDF med andra användare.

Den här funktionen stöds för följande objekt:

* Projekt
* Uppgifter
* Problem
* Portfolio
* Program

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Fälten i detaljavsnittet som din Workfront- eller gruppadministratör har tagit bort med en layoutmall visas inte.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront package</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licens</p> </td> 
   <td><p>För problem:</p>
   <ul><li><p>Medarbetare eller högre</p></li>
   <li><p>Begärande eller högre</p> </li></ul>
   <p>För projekt och uppgifter:</p>
   <ul><li><p>Ljus eller högre</p></li>
   <li><p>Granskare eller högre</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller högre för projekt, uppgifter och ärenden</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Objektbehörigheter</p> </td> 
   <td> <p>Visa eller högre behörigheter för det projekt, den uppgift eller det problem vars formulär du vill exportera</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Innan du börjar måste du ha följande:

1. Skapa ett anpassat formulär för ett specifikt objekt som du vill exportera det från.
1. Låt det anpassade formuläret vara kopplat till objektet

   eller

   Ha rätt åtkomst för att bifoga ett anpassat formulär och redigera informationen i formuläret.

Mer information om hur du skapar anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Mer information om hur du bifogar formulär till objekt finns i [Lägga till ett anpassat formulär till ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportera information i detaljavsnittet

Att exportera information från detaljavsnittet för ett objekt är identiskt för alla objekt där det stöds.

1. Gå till ett projekt, en uppgift, en portfölj, ett program eller ett problem som du har minst behörigheten Visa.
1. Klicka på **&quot;Detaljer&quot;** på den vänstra panelen, till exempel **Uppgiftsinformation**.
1. (Valfritt) Om det inte finns något anpassat formulär kopplat till objektet börjar du skriva namnet på ett anpassat formulär i fältet **Lägg till anpassat formulär** och klickar sedan på det när det visas i listan.

   Du kan lägga till upp till 10 formulär.

1. (Valfritt) Uppdatera informationen i detaljavsnittet och klicka sedan på **Spara ändringar**.
1. Klicka på listrutan **Exportera** i det övre högra hörnet, välj **Översikt** eller de formulär som du vill exportera och klicka sedan på **Exportera**.

   Du kan också välja **Markera alla** om du vill exportera översiktsområdet och alla anpassade formulär.

   ![Knappen Exportera anpassat formulär](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Följande scenarier kan finnas:
   >
   >   * När gruppadministratören eller Workfront-administratören avmarkerar alla fält i översiktsområdet och objektet har anpassade formulär bifogade, visas inte översiktsavsnittet.
   >   * När en gruppadministratör eller Workfront-administratör avmarkerar alla fält i området Översikt och objektet inte har några anpassade formulär bifogade visas inte listrutan Exportera.
   >   * När objektet inte har några anpassade formulär kan du bara exportera området Översikt.
   >   * Anpassade fält som ligger bakom logik och inte är synliga i formuläret exporteras inte. Mer information om hur du lägger till logik i ett anpassat formulär finns i [Lägga till logiska regler i anpassade formulär och fält](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

   En PDF-fil skapas och hämtas till din dator. PDF-filen innehåller följande information:

   * Namnet på objektet som formuläret är kopplat till
   * Namnet på den användare som exporterade PDF
   * Datum och tid då PDF skapades
   * Namnet på de formulär som du exporterade
   * Information från de fält som fyllts i i formuläret
