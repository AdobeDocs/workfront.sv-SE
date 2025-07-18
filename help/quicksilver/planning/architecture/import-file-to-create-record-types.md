---
title: Skapa posttyper genom att importera information från en CSV- eller Excel-fil
description: Posttyper är objekttyperna i Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsuppgifter som behövs i organisationens livscykel genom att importera information från en CSV- eller Excel-fil.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Skapa posttyper genom att importera information från en CSV- eller Excel-fil

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är endast tillgänglig i förhandsversionsmiljön för alla kunder. Efter de månatliga versionerna till produktion är samma funktioner också tillgängliga i produktionsmiljön för kunder som har aktiverat snabba versioner. </span>

<span class="preview">Information om snabba versioner finns i [Aktivera eller inaktivera snabba versioner för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Posttyper är objekttyperna i Adobe Workfront Planning. I Workfront Planning kan du skapa anpassade posttyper som illustrerar de arbetsuppgifter som behövs i organisationens livscykel genom att importera information från en CSV- eller Excel-fil.

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

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
   <li><p> Planering av Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p>  </td> 
  </tr>

</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Att tänka på när du importerar posttyper med hjälp av en Excel- eller CSV-fil

* Varje ark i Excel-filen blir en posttyp. Namnet på bladet blir namnet på posttypen.
* Om det bara finns ett blad, eller om du importerar en CSV-fil, blir namnet på filen namnet på posttypen.
* Kolumnrubrikerna i varje blad blir de fält som är associerade med varje posttyp.
* Fält är unika för sina respektive posttyper.
* Varje rad i varje blad blir en unik post som är kopplad till respektive posttyp.
* Varje ark i Excel-filen bör inte vara större än följande:
   * 25 000 rader
   * 500 kolumner
* Filen får inte vara större än 5 MB.
* Tomma ark stöds inte.
* Fält av följande typer stöds inte och kan inte mappas till fält på importbladet:

   * Anslutningsfält till objekttyperna Workfront och AEM Assets.
   * Uppslagsfält från anslutna planeringsposter eller Workfront- och AEM Assets-objekt
   * Fält för formler
   * Skapad den, Skapad av
   * Datum för senaste ändring, Senast ändrad av
   * <span class="preview">Godkänt datum, Godkänt av</span>
   * Folk

Så här importerar du posttyper med hjälp av en Excel- eller CSV-fil:

{{step1-to-planning}}

1. Klicka på den arbetsyta där du vill skapa posttyper,

   Eller

   Från en arbetsyta expanderar du den nedåtpekande pilen till höger om ett befintligt arbetsytenamn, söker efter en arbetsyta och väljer den sedan när den visas i listan.
1. Klicka på **Lägg till posttyp**.
1. Klicka på **Ladda upp från fil**.
1. Dra och släpp en Excel- eller CSV-fil som tidigare sparats på datorn, eller klicka på **Välj en CSV- eller Excel-fil** för att bläddra efter en och välj den sedan.
1. Klicka på **Förhandsgranska och redigera**.

   Rutan **Förhandsgranska och redigera** visas med följande information:

   * Namnen på bladen eller de framtida posttyperna visas i den vänstra panelen. Workfront Planning väljer som standard en ikon och en färg för varje ny posttyp.
   * Det första arket eller den första posttypen väljs och namnen på de fält som är associerade med det visas som kolumnrubriker. Typen för varje fält är markerad som standard.
   * Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

   ![Förhandsgranska och redigera ruta](assets/preview-and-edit-box.png)

1. (Valfritt) Klicka på namnet på varje blad i den vänstra panelen för att granska informationen som det innehåller.

   >[!NOTE]
   >
   >Blad som är tomma stöds inte och är nedtonade.

1. (Valfritt) Avmarkera de blad som du inte vill importera från den vänstra panelen.

   ![Välj ark att importera rullgardinsmenyn med avmarkerat](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blad som du har avmarkerat visas med en grå bakgrund.

1. (Valfritt) Klicka på den nedåtpekande pilen till höger om en kolumnrubrik om du vill göra något av följande på **fliken Fält** :

   ![Fliken Fält i importrutan för mappning av posttyp](assets/field-tab-on-record-type-import-mapping-box.png)

   * Byt namn på ett av fälten
   * **Ändra fälttyp**
   * Uppdatera fältet **Beskrivning**

1. (Valfritt) **Klicka på fliken Anslutning** om du vill mappa informationen i kolumnen till ett kopplat fält från andra posttyper.

   ![Fliken Anslutning i rutan för mappning av import av posttyp](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >Du kan bara mappa till fält från Workfront Planning-anslutna poster. Du kan inte mappa till fält från Workfront- eller AEM Assets-anslutningar. Mer information finns i avsnittet [Att tänka på när du importerar posttyper med hjälp av en Excel- eller CSV-fil](#considerations-about-importing-record-types-using-an-excel-or-csv-file) i den här artikeln.

1. (Villkorligt) När du har uppdaterat informationen om fältet klickar du på **Spara**.

1. Klicka på **Importera** när du är redo att importera filen.

   Följande information importeras till Workfront Planning:

   * Nya posttyper
   * Nya fält som är associerade med varje posttyp
   * Nya poster som är associerade med varje posttyp

   Du kan börja hantera fält och poster på sidorna för posttyper.

   Alla som har tillgång till Workfront Planning och arbetsytan kan nu visa och redigera de importerade posttyperna och deras information.
