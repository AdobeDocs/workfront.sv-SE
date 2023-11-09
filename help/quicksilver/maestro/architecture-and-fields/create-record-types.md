---
title: Skapa driftsposttyper
description: Posttyperna är objekttyperna för Adobe Maestro. I Maestro kan du skapa anpassade posttyper som illustrerar de arbetsuppgifter som behövs i organisationens livscykel.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Skapa driftsposttyper

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Posttyperna är objekttyperna för Adobe Maestro. I Maestro kan du skapa anpassade posttyper som illustrerar de arbetsrelaterade objekt som behövs i organisationens livscykel.

Posttyper kan vara något av följande:

* **Operativa posttyper**
* **Taxonomier**

Mer information om posttyper i Maestro finns i [Översikt över posttyper och taxonomier](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

Att skapa driftsposttyper liknar att skapa taxonomiposttyper. I den här artikeln beskrivs hur du skapar driftsposttyper.

Mer information om att skapa taxonomier finns i [Skapa taxonomiposttyper](../architecture-and-fields/create-a-taxonomy.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när du skapar posttyper

* Du kan skapa posttyper på en arbetsyta genom att göra något av följande:

   * Automatiskt:
      * När du skapar en arbetsyta med hjälp av en mall.

        Mer information finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).
      * När du importerar dem med en Excel- eller CSV-fil. Detta är inte tillgängligt för taxonomiposttyper.
      * När du skapar en anslutning till objekttyper från ett annat program, när du lägger till fält till en posttyp. Detta skapar en skrivskyddad posttyp i Maestro som är kopplad till objekttyper från det ursprungliga programmet.

     Mer information om hur du kopplar objekttyper till Maestro-poster finns i [Koppla poster](../records/connect-records.md).
   * Manuellt:

      * Från scratch.

## Skapa posttyper med hjälp av en arbetsytemall

Du kan skapa posttyper automatiskt när du skapar en arbetsyta med hjälp av en mall. Varje Maestro-mall innehåller exempel på användnings- och taxonomiposttyper.

Mer information om hur du skapar arbetsytor finns i [Skapa arbetsytor](../architecture-and-fields/create-workspaces.md).

Mer information om vilka posttyper som ingår i respektive mall finns i [Lista över arbetsytemallar](../architecture-and-fields/workspace-templates.md).

## Skapa en posttyp från grunden

I den här artikeln beskrivs hur du skapar driftsposttyper från grunden. Att skapa operativa posttyper från grunden liknar att skapa taxonomier.

Mer information om taxonomier finns i [Skapa en taxonomi](../architecture-and-fields/create-a-taxonomy.md).

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i det övre högra hörnet av Workfront eller **Huvudmeny** icon ![](assets/main-menu-shell.png)  i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill skapa posttyper för.
1. Klicka **Lägg till posttyp**.
1. (Villkorligt) Om du skapar en operativ posttyp klickar du på **Från början**. Det här alternativet är inte tillgängligt när du skapar taxonomier.

   Rutan Lägg till posttyp öppnas.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Välj följande information:

   * **Postnamn**: Ersätt&quot;Namnlös operativ posttyp&quot; med namnet på din framtida posttyp. <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **Utseende**: Definiera färg och form för ikonen som är associerad med posttypen. Gör följande:
      * Välj en färg som identifierar den nya posttypen. Det här är färgen på ikonen för posttyp. Grått är markerat som standard.
      * Välj en ikon i listan eller börja skriva namnet på en ikon för att beskriva vad den representerar och markera den sedan när den visas. Det här är ikonen för posttypen. Som standard är en filikon markerad.

1. Klicka utanför **Lägg till posttyp** för att spara posten.

   Posttypkortet läggs till på den arbetsyta som du har valt.
Antalet fält som posttypen innehåller visas på kortet.
1. (Valfritt) Klicka på posttypskortet för att öppna posttypssidan.

   ![](assets/operational-record-type-blank.png)

   Posttypssidan visas som standard i tabellvyn. Kolumnerna i tabellen är fält som är kopplade till den nya posttypen. Varje rad är en unik post som du måste lägga till.

   Som standard visas följande fält i tabellvykolumnerna för en operativ posttyp:

   * Namn

     Fältet Namn är det enda fält som skapas automatiskt för taxonomier.
   * Beskrivning
   * Startdatum
   * Slutdatum
   * Status

1. (Valfritt) Uppdatera posttypens namn i sidhuvudet

   eller

   Klicka på **Mer** icon ![](assets/more-menu.png) till höger om posttypens namn och klicka på **Byt namn** för att byta namn på den.

1. (Valfritt) Klicka på **+ Ny &lt; posttypsnamn >** om du vill lägga till poster av den valda posttypen. Mer information finns i [Skapa poster](../records/create-records.md).
1. (Valfritt) Klicka på **+** i tabellens övre högra hörn om du vill lägga till fler fält i posttypen. Mer information finns i [Skapa fält](../architecture-and-fields/create-fields.md).
1. (Valfritt) Klicka på vänsterpilen till vänster om posttypens namn för att gå tillbaka till den valda arbetsytan.

   Posttypkortet visar antalet fält och anslutningar som posttypen innehåller.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Mer information om hur du lägger till poster, tar bort eller redigerar posttyper eller uppdaterar vyn på posttypsidan finns i följande artiklar:

   * [Skapa poster](../records/create-records.md)
   * [Ta bort posttyper](../architecture-and-fields/delete-record-types.md)
   * [Redigera posttyper](../architecture-and-fields/edit-record-types.md)
   * [Hantera postvyer i Adobe Maestro](../views/manage-record-views.md) <!--add information here about the sorting and grouping when available-->

## Skapa posttyper genom att importera en Excel- eller CSV-fil

Tänk på följande när du importerar posttyper med en Excel- eller CSV-fil:

* Varje blad i Excel-filen blir en posttyp i Maestro.
* Kolumnerna i varje blad blir de fält som är kopplade till varje posttyp.
* Fält är unika för respektive posttyp.
* Varje rad i varje blad blir en unik post som är kopplad till respektive posttyp.
* Varje blad i Excel-filen får inte överskrida följande:
   * 10 000 rader
   * 500 kolumner
* Excel-filen får inte vara större än 5 MB.
* Tomma blad stöds inte.

Så här importerar du posttyper med en Excel-fil:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i Workfront övre högra hörn, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klicka sedan på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta och markera den arbetsyta som du vill skapa posttyper för.
1. Klicka **Lägg till posttyp**.
1. (Villkorligt) Om du skapar en operativ posttyp klickar du på **Excel/CSV**.

   >[!NOTE]
   >
   >    Det här alternativet är inte tillgängligt när du skapar taxonomiposttyper.

1. Dra och släpp en Excel- eller CSV-fil som tidigare sparats på datorn eller klicka på **Välj en CSV- eller Excel-fil** för att hitta en.
1. Klicka **Granska dina data**.

   Rutan Förhandsgranska och redigera visas med följande information:

   * Namnen på arken eller de framtida posttyperna visas på den vänstra panelen. Som standard väljs en ikon och en färg för varje ny posttyp.
   * Den första arks- eller posttypen markeras och namnen på de fält som är kopplade till den visas som kolumnrubriker. Som standard väljs typen för varje fält.
   * Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

   ![](assets/preview-and-edit-box.png)

1. (Valfritt) Klicka på namnet på varje blad i den vänstra panelen för att granska informationen som det innehåller.

   >[!NOTE]
   >
   >    Blad som är tomma stöds inte och är nedtonade.


1. (Valfritt) Klicka på **Välj ark att importera** och avmarkera de blad som du inte vill importera.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blad som du avmarkerat visas med grå bakgrund.

1. Klicka **Importera** när du är redo att importera filen.

   Följande information importeras till Maestro:

   * Nya posttyper
   * Nya fält som är associerade med varje posttyp
   * Nya poster associerade med varje posttyp

   Du kan börja hantera fält och poster på posttypssidorna.

   Alla som har tillgång till Maestro kan nu visa och redigera de importerade posttyperna och deras information. <!--this will change with permissions-->

## Koppla posttyper med objekttyper från andra program

Du kan importera posttyper när du skapar en anslutning mellan en Maestro-posttyp och en objekttyp från ett annat program. Detta skapar en skrivskyddad posttyp i Maestro som motsvarar objekttypen i tredjepartsprogrammet.

Du kan till exempel skapa posttyper genom att koppla Maestro-posttyper till Workfront-projekt. Därför importeras Workfront projektobjekttyp till Maestro som en skrivskyddad posttyp. Som standard heter posttypen&quot;Workfront Project&quot;. <!--has this name changed? Lusine wanted to change it at some point-->

Du kan importera följande objekt från följande program:

* Från Workfront:

   * Projekt
   * Portfolio
   * Program
   * Företag
   * Grupp

Mer information finns i [Koppla posttyper](../architecture-and-fields/connect-record-types.md).
