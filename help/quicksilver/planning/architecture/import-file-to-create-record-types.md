---
title: Skapa posttyper genom att importera information från en CSV- eller Excel-fil
description: Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar vilka arbetsobjekt som behövs i organisationens livscykel genom att importera information från en CSV- eller Excel-fil.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Skapa posttyper genom att importera information från en CSV- eller Excel-fil

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Posttyperna är objekttyperna för Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar vilka arbetsobjekt som behövs i organisationens livscykel genom att importera information från en CSV- eller Excel-fil.

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
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
<p>eller</p>
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
 
</tbody> 
</table>-->


## Att tänka på när du importerar posttyper med hjälp av en Excel- eller CSV-fil

* Varje blad i Excel-filen blir en posttyp. Kalkylbladets namn blir posttypens namn.
* Om det bara finns ett blad, eller om du importerar en CSV-fil, får filen namnet som posttyp.
* Kolumnrubrikerna i varje blad blir de fält som är kopplade till varje posttyp.
* Fält är unika för respektive posttyp.
* Varje rad i varje blad blir en unik post som är kopplad till respektive posttyp.
* Varje blad i Excel-filen får inte överskrida följande:
   * 25 000 rader
   * 500 kolumner
* Filen får inte vara större än 5 MB.
* Tomma blad stöds inte.
* Fält av följande typer stöds inte och kan inte mappas till fält på importbladet:

   * Anslutningsfält till objekttyperna Workfront och AEM Assets.
   * Sök efter fält från anslutna Planning-poster eller Workfront- och AEM Assets-objekt
   * Formelfält
   * Skapad den, skapad av
   * Senast ändrat den
   * Godkänt den
   * Folk

Så här importerar du posttyper med en Excel- eller CSV-fil:

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill skapa posttyper,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.
1. Klicka på **Lägg till posttyp**.
1. Klicka på **Överför från fil**.
1. Dra och släpp en Excel- eller CSV-fil som du tidigare har sparat på datorn eller klicka på **Välj en CSV- eller Excel-fil** om du vill bläddra efter en fil och markera den.
1. Klicka på **Förhandsgranska och redigera**.

   Rutan **Förhandsgranska och redigera** visas med följande information:

   * Namnen på arken eller de framtida posttyperna visas på den vänstra panelen. I Workfront Planning väljs en ikon och en färg för varje ny posttyp som standard.
   * Den första arks- eller posttypen markeras och namnen på de fält som är kopplade till den visas som kolumnrubriker. Som standard väljs typen för varje fält.
   * Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

   ![Rutan Förhandsgranska och redigera](assets/preview-and-edit-box.png)

1. (Valfritt) Klicka på namnet på varje blad i den vänstra panelen för att granska informationen som det innehåller.

   >[!NOTE]
   >
   >Blad som är tomma stöds inte och är nedtonade.

1. (Valfritt) Avmarkera de blad som du inte vill importera från den vänstra panelen.

   ![Markera ark som ska importeras i den nedrullningsbara listan med omarkerade ark](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blad som du avmarkerat visas med grå bakgrund.

1. (Valfritt) Klicka på den nedåtriktade pilen till höger om en kolumnrubrik om du vill göra något av följande på fliken **Fält**:

   ![Fliken Fält i importrutan för posttypsmappning](assets/field-tab-on-record-type-import-mapping-box.png)

   * Byt namn på ett av fälten
   * Ändra **fälttypen**
   * Uppdatera fältet **Beskrivning**

1. (Valfritt) Klicka på fliken **Anslutning** för att mappa informationen i kolumnen till ett anslutet fält från andra posttyper.

   ![Fliken Anslutning i importmappningsrutan för posttyp](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >Du kan bara mappa till fält från Workfront Planning-anslutna poster. Du kan inte mappa till fält från Workfront- eller AEM Assets-anslutningar. Mer information finns i avsnittet [Att tänka på när du importerar posttyper med hjälp av en Excel- eller CSV-fil](#considerations-about-importing-record-types-using-an-excel-or-csv-file) i den här artikeln.

1. (Villkorligt) När du har uppdaterat informationen om fältet klickar du på **Spara**.

1. Klicka på **Importera** när du är klar att importera filen.

   Följande information importeras till Workfront Planning:

   * Nya posttyper
   * Nya fält som är associerade med varje posttyp
   * Nya poster associerade med varje posttyp

   Du kan börja hantera fält och poster på posttypssidorna.

   Alla som har tillgång till Workfront Planning och arbetsytan kan nu visa och redigera de importerade posttyperna och deras information.
