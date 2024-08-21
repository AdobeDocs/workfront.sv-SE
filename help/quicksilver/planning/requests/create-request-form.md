---
title: Skapa ett begärandeformulär i Adobe Workfront Planning
description: När du har valt en posttyp i Adobe Workfront Planning kan du skapa ett begärandeformulär som är kopplat till den posttypen och dela en länk till den med andra interna eller externa användare.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Skapa ett begärandeformulär i Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

När du har valt en posttyp i Adobe Workfront Planning kan du skapa ett begärandeformulär och associera det med den posttypen. Du kan sedan dela en länk till den med andra interna eller externa användare. <!--double-check on the external part of it-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna komma åt Workfront Planning:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkter</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td>
   <td>
<p>Något av följande Workfront-planer:</p>
<ul><li>Välj</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td>
   <td>
<p>Alla </p>   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <ul>
   <li><p>Hantera behörigheter till en arbetsyta</p></li>
    <li><p>Systemadministratörer kan hantera arbetsytor som de inte skapade. </p></li>
    </ul>
   <p>Information om delningsbehörigheter för Workfront Planning-objekt finns i  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett begärandeformulär för en posttyp

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.

1. Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn i sidhuvudet och klicka sedan på **Skapa begärandeformulär**.
1. Uppdatera namnet på förfrågningsformuläret. Som standard är formulärets namn **Namnlöst begärandeformulär**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Valfritt) Lägg till en **beskrivning** för begärandeformuläret.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klicka på **Skapa**. Formuläret för förfrågan för den valda posttypen öppnas.

   Formuläret innehåller som standard följande information:

   * **Standardavsnitt**: Det här är standardavsnittsbrytningen som Workfront tillämpar på begärandeformuläret. Det går inte att byta namn på eller ta bort standardavsnittet.
   * Fältet **Ämne**: Fältet som identifierar begäran i Workfront. Den här funktionen är inte tillgänglig än.
   * Alla fält som är associerade med posttypen.

   Fälten i begärandeformuläret är synliga för alla som skickar en begäran till den här posttypen.

1. (Valfritt) Ta bort fältet **Ämne** eftersom det inte visas i Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Håll muspekaren över de fält i formuläret som du vill ta bort. De läggs till på fliken **Fält** till vänster i formuläret.
1. Klicka på ett fält och använd sedan kontrollerna till höger i formuläret för att definiera någon av följande information om fälten:

   * **Etikett**: Det här är namnet på fältet som det kommer att visas i begärandeformuläret. Detta ändrar inte postfältets namn.
   * **Instruktioner**: Lägg till mer information om fältet.
   * **Gör ett obligatoriskt fält**: När du väljer det här alternativet måste fältet ha ett värde. Annars kan formuläret inte skickas.
   * **Lägg till logik**: Definiera vilka villkor som måste uppfyllas för att fältet ska kunna visas eller döljas.

1. Klicka på fliken Innehållselement till höger i formuläret och lägg till något av följande element:

   * Beskrivning
   * Avsnittsbrytning

   Mer information om hur du skapar ett anpassat formulär finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).





