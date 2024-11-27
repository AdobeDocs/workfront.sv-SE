---
title: Skapa och hantera ett begärandeformulär i Adobe Workfront Planning
description: När du har valt en posttyp i Adobe Workfront Planning kan du skapa ett begärandeformulär och associera det med den posttypen. Du kan sedan dela en länk till den med andra interna eller externa användare. Användare som har en länk till formuläret kan fylla i fältvärdena på det och genom att skicka det kan de lägga till en ny post för den posttyp som är associerad med det.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# Skapa och hantera ett begärandeformulär i Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan skapa ett begärandeformulär och associera det med en posttyp i Adobe Workfront Planning. Du kan sedan dela en länk till den med andra interna eller externa användare.

Användare med en länk till formuläret kan uppdatera fältvärdena på det och lägga till nya poster genom att skicka det.

I den här artikeln beskrivs hur en arbetsytehanterare kan skapa ett begärandeformulär som är associerat med en posttyp.

Mer information om hur du skickar en begäran till en posttyp för att skapa en post finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td>
   <td>
<p>Alla </p>  
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </td>

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

   ![](assets/campaigns-request-form-edit-mode.png)

   Formuläret innehåller som standard följande information:

   * Postfält som är tillgängliga i tabellvyn för den valda posttypen. <!--they are working on removing the limitation below-->

   >[!IMPORTANT]
   >
   > Beroende på vilken miljö du använder för att skapa ett begärandeformulär finns följande scenarier:
   >
   >* Fält av följande typer visas inte i begärandeformuläret <span class="preview"> i förhandsgransknings- </span> eller produktionsmiljöerna:
   >
   >    * Skapad av och senast ändrad av
   >    * Formel
   >    * Skapad den och senast ändrad den
   >    * Workfront-objektens sökfält
   >    * Sökfält för Workfront Planning-anslutna poster
   >    * AEM Assets-anslutna fält
   >* Fält av följande typer visas inte i begärandeformuläret i produktionsmiljön. <span class="preview">De visas i förhandsvisningsmiljön:</span>
   >    * <span class="preview"> Workfront Planning records&#39; connected fields </span>
   >    * <span class="preview">Personer </span>
   >    * <span class="preview">Workfront-objektens anslutna fält</span>
   >    * <span class="preview">AEM Assets-anslutna fält </span>



   * **Standardavsnitt**: Det här är standardavsnittsbrytningen som Workfront tillämpar på begärandeformuläret. Det går inte att byta namn på eller ta bort standardavsnittet.
   * Fältet **Ämne**: Fältet som identifierar begäran i Workfront. Den här funktionen är inte tillgänglig än. Det går inte att redigera konfigurationen och värdet för ämnesfältet.
   * Alla fält som är associerade med posttypen.

     Fälten i begärandeformuläret är synliga för alla som skickar en begäran till den här posttypen.

1. (Valfritt) Håll markören över fält i formuläret som du vill ta bort och klicka sedan på ikonen **x** för att ta bort dem. De läggs till på fliken **Fält** till vänster om formuläret.

   Ta till exempel bort fältet **Ämne** eftersom det inte visas i Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Klicka på ett fält och använd sedan kontrollerna på den högra panelen i formuläret för att definiera deras storlek eller någon av följande information:

   * **Etikett**: Det här är namnet på fältet som det kommer att visas i begärandeformuläret. Detta ändrar inte postfältets namn.
   * **Instruktioner**: Lägg till mer information om fältet.
   * **Gör ett obligatoriskt fält**: När du väljer det här alternativet måste fältet ha ett värde. Annars kan formuläret inte skickas.
   * **Lägg till logik**: Definiera vilka villkor som måste uppfyllas för att fältet ska kunna visas eller döljas.

   >[!NOTE]
   >
   >   Fälttypen för varje fält visas längst upp på den högra panelen när du har valt fältet i formuläret.
   >   
   >
   >   Fälten Valuta, Nummer och Procenttal visas som ett textfält med en rad. Fältformatet bevaras dock och värdena i dessa fält visas som värden för Valuta, Nummer och Procent.

1. (Valfritt) Klicka på fliken **Innehållselement** till vänster i formuläret och lägg till något av följande element:

   * **Beskrivande text**
   * **Avsnittsbrytning**

   Mer information om hur du skapar ett anpassat formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Valfritt) Klicka på **Förhandsgranska** om du vill visa hur formuläret kommer att visas för andra användare när de kommer att använda det för att skicka en ny post.
1. (Valfritt) Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om formulärets namn i rubriken och klicka sedan på **Redigera** för att uppdatera formulärets namn.
1. Klicka på **Publish** för att publicera formuläret och få en unik länk till det.

   Följande saker händer:

   * Knappen **Publish** har tagits bort.
   * Knappen **Avpublicera** läggs till i formuläret. Om du klickar på den går det inte att komma åt formuläret.
   * En **Dela**-knapp läggs till i formuläret.

1. Klicka på **Dela** om du vill dela formuläret med andra.

   ![](assets/share-box-for-request-form.png)

1. Välj bland följande alternativ för att ange vilka typer av användare som har åtkomst till det här formuläret:

   * Alla som visar eller har högre åtkomst till arbetsytan
   * Alla som har Contribute eller senare åtkomst till arbetsytan
   * Alla med länken

   >[!WARNING]
   >
   >
   >* När du väljer **Vem som helst med länken** kan vem som helst få åtkomst till formuläret och skicka en ny post, även personer utanför organisationen som inte har något Workfront-konto.
   >
   > * <span class="preview">Ett formulär som innehåller följande fälttyper kan inte delas offentligt:</span>
   >
   >     * <span class="preview">Formel</span>
   >     * <span class="preview">Workfront- eller AEM Assets-anslutningar</span>
   >     * <span class="preview">Uppslagsfält</span>
   >     * <span class="preview">Personer</span>
   >

1. (Villkorligt) Om du valde **Vem som helst med länken** i föregående steg väljer du **länkens förfallodatum** i den tillgängliga kalendern. Användarna får ett felmeddelande när länken upphör att gälla och du måste uppdatera länkdatumet innan de kan komma åt formuläret igen.

   Du kan välja framtida datum inom 180 dagar från dagens datum.

1. Klicka på **Spara och kopiera länken** för att spara delningsinformationen för formuläret.

   Alternativen för formulärdelning sparas och länken kopieras till Urklipp. Nu kan du dela den med andra.

   Mer information om hur du skapar poster med hjälp av en länk till ett begärandeformulär finns i [Skicka Adobe Workfront Planning-begäranden](/help/quicksilver/planning/requests/submit-requests.md).

1. Klicka på **Spara** längst ned till höger på skärmen för att spara formuläret.
1. Klicka på vänsterpilen till vänster om formulärets namn i rubriken för att stänga formuläret.

   Posttypssidan öppnas.
1. (Valfritt) Klicka på menyn **Mer** ![](assets/more-menu.png) till höger om posttypens namn i rubriken och gör sedan något av följande:
   * Klicka på **Uppdatera begärandeformuläret** om du vill göra några ändringar i begärandeformuläret.
   * Klicka på **Kopiera länk till begärandeformuläret** om du vill dela länken till formuläret med andra.

   >[!TIP]
   >
   >Det finns en indikation på att länken delas offentligt när så är fallet.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
