---
title: Skapa posttyper
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsuppgifter som behövs i organisationens livscykel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 0%

---


<!--this is linked to the UI in an empty workspace screen-->

# Skapa posttyper

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsrelaterade objekt som behövs i organisationens livscykel.

Mer information om posttyper finns i [Översikt över posttyper](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

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
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Hantera behörigheter till en arbetsyta </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Att tänka på när du skapar posttyper

* Du kan skapa posttyper på en arbetsyta på följande sätt:

   * Automatiskt:
      * När du skapar en arbetsyta med hjälp av en mall.

        Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

      * När du importerar dem med en CSV- eller Excel-fil.

        Mer information finns i [Skapa posttyper genom att importera information från en CSV- eller Excel-fil](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

     >[!TIP]
     >
     >När du importerar en posttyp från en CSV- eller Excel-fil kan du även importera poster och fält.

   * Manuellt:

      * Från scratch.

        I den här artikeln beskrivs hur du skapar posttyper från grunden.

     <!--
        * <span class="preview">By importing them from another workspace or adding cross-workspace record types</span>
            <span class="preview">For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md). </span>-->


* Du kan flytta posttyper inom ett avsnitt och från ett avsnitt på en arbetsyta till ett annat. Du kan inte flytta posttyper från en arbetsyta till en annan.

## Skapa posttyper med hjälp av en arbetsytemall

Du kan skapa posttyper automatiskt när du skapar en arbetsyta med en Workfront Planning-mall. Varje mall innehåller exempelposttyper.

När du skapar en arbetsyta från en mall grupperas posttyperna i följande avsnitt:

* Operativa posttyper
* Taxonomier

Du kan lägga till posttyper manuellt i avsnitten Driftposttyper och Taxonomier.

Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).

Mer information om vilka posttyper som ingår i varje mall finns i [Lista över arbetsytemallar](/help/quicksilver/planning/architecture/workspace-templates.md).

## Skapa en posttyp från grunden

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill skapa en posttyp,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.
1. (Valfritt) Klicka på **Lägg till avsnitt** om du vill lägga till ett nytt avsnitt på arbetsytan.
1. Klicka på **Lägg till posttyp** och sedan **Lägg till manuellt**.

   Rutan Lägg till posttyp öppnas.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![Lägg till posttypsruta med utseendealternativ](assets/add-record-type-box-with-appearance-options.png)

1. Uppdatera följande information på fliken **Utseende**:

   * Ersätt&quot;Namnlös posttyp&quot; med namnet på din framtida posttyp. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beskrivning**: Lägg till mer information om posttypen.
   * Välj en färg och form för den ikon som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar den nya posttypen. Det här är färgen på ikonen för posttyp. Grått är markerat som standard.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.


   <!--old setting:
    1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Connectivity scope** section: 
        * Enable the **Connect from other workspace** setting. When enabled, the record type is accessible and can be connected from other workspaces. 
        * Choose from which workspaces the record type can be accessed. Choose from the following options:
            * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions. 
            * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type. 
    -->

1. (Valfritt och villkorligt) Om du är systemadministratör klickar du på **Avancerade inställningar** och uppdaterar följande information i avsnittet **Arbetsytans funktioner**: <!--the info here is duplicated in the Edit record types article-->
   * Aktivera inställningen **Tillåt anslutning till den här posttypen i andra arbetsytor**: Detta gör att arbetsytehanterare kan ansluta till den här posttypen från andra arbetsytor.\
     Du kan ange vilka arbetsytor som den här posttypen kan anslutas från. Du kan göra den tillgänglig för alla arbetsytor eller ange specifika arbetsytor där du kan importera den.
Mer information finns i [Konfigurera funktioner för arbetsytan över flera arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


   ![Skapa en ruta för posttyp på fliken Avancerade inställningar](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release dynamic record types; the preview tags might need to be edited, too:
        <div class="preview">
        1. (Optional and conditional) If you are a system administrator, click **Advanced settings** and update the following information in the **Cross-workspace capability** section: **** the info here is duplicated in the Edit record types article ***
            * Enable the **Allow adding this record type to other workspaces** setting: This allows workspace managers to add this record type to other workspaces. 
                You can designate specific users who can add this record type to other workspaces. 
            * Enable the **Allow connecting to this record type in other workspaces** setting: This allows workspace managers to connect to this record type from other workspaces.  
                You can designate which workspaces this record type can be connected from. You can make it available for all workspaces or designate specific ones where you can import it.
            For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).  </div>
            ******** replace screen shot below **********
            ![Create record type box on advanced settings tab](assets/create-record-type-box-advanced-settings-tab.png) 
        -->

1. Klicka på **Spara**.

   Posttypkortet läggs till i avsnittet och på den arbetsyta som du har valt.
Beskrivning av posttypen visas på kortet.

   ![Posttypkort med beskrivning](assets/record-type-card-with-description.png)

   Om du valde att ansluta den här posten från andra arbetsytor visas ikonen **Anslut från andra arbetsytor** ![Anslut från andra arbetsytor](assets/connect-from-other-workspaces-icon.png) på postkortet.

   <!--<span class="preview">If you configured the cross-workspace capabilities for the record, the **connect from other spaces** icon ![Connect record type from other spaces icon](assets/connect-from-other-workspaces-icon.png) and the **add to other workspaces** icon ![Add record type to other workspaces](assets/global-icon.png) also display on the card. </span>-->

1. (Valfritt) Håll markören över posttypskortet, klicka på ikonen **Mer** ![Mer meny](assets/more-menu.png) i det övre högra hörnet och klicka sedan på **Redigera** för att ändra information om posttypen.
1. (Valfritt) Klicka på posttypskortet för att öppna posttypssidan.

   ![Posttypen för operativt ](assets/operational-record-type-blank.png) är tom

   Posttypssidan visas som standard i tabellvyn. Kolumnerna i tabellen är fält som är kopplade till den nya posttypen. Varje rad är en unik post som du måste lägga till.

   Som standard visas följande fält i tabellvykolumnerna för en operativ posttyp:

   * Namn
   * Beskrivning
   * Startdatum
   * Slutdatum
   * Status

1. (Valfritt) Uppdatera posttypens namn i sidhuvudet

   eller

   Klicka på ikonen **Mer** ![Mer meny](assets/more-menu.png) till höger om posttypens namn och klicka på **Redigera** för att byta namn på den eller ändra informationen om den. Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Valfritt) Klicka på **+ Ny post** om du vill lägga till poster av den valda posttypen. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
1. (Valfritt) Klicka på ikonen **+** i tabellens övre högra hörn för att lägga till fler fält i posttypen.

   Mer information om hur du skapar fält finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).

1. (Valfritt) Klicka på vänsterpilen till vänster om posttypens namn i sidhuvudet för att gå tillbaka till den valda arbetsytan.

1. (Valfritt) Klicka på och håll ned ett posttypskort på arbetsytan om du vill dra och släppa posttypen på en önskad plats, eller om du vill flytta den till ett annat avsnitt.

   Ändringarna sparas automatiskt.

   Mer information om hur du lägger till poster, tar bort eller redigerar posttyper eller uppdaterar vyn på posttypsidan finns i följande artiklar:

   * [Skapa poster](/help/quicksilver/planning/records/create-records.md)
   * [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Hantera postvyer](/help/quicksilver/planning/views/manage-record-views.md)

## Skapa posttyper genom att importera information från en CSV- eller Excel-fil

Du kan importera följande när du importerar information från en CSV- eller Excel-fil:

* Posttyper
* Poster
* Postfält

Mer information finns i [Skapa posttyper genom att importera information från en CSV- eller Excel-fil](/help/quicksilver/planning/architecture/import-file-to-create-record-types.md).

<!--

<div class="preview">

## Create record types by importing them from another workspace 

You can add record types to a workspace by importing them from another workspace. You can only add record types that have been configured as centralized record types. 

For information, see [Add existing record types](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

</div>

-->