---
title: Skapa poster genom att importera information från en CSV- eller Excel-fil
description: Poster är enskilda instanser av posttyper, som är objekttyper i Adobe Workfront Planning. I Workfront Planning kan du skapa poster genom att importera information från en CSV- eller Excel-fil.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---


# Skapa poster genom att importera information från en CSV- eller Excel-fil

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Poster är enskilda instanser av posttyper, som är objekttyper i Adobe Workfront Planning. I Workfront Planning kan du skapa poster genom att importera information från en CSV- eller Excel-fil.

Mer information om hur du skapar poster finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

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
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p> 
   <p>Redigera åtkomst i Workfront för de objekttyper som du vill skapa (projekt, program och portföljer) när du kopplar dem från nya poster  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Contribute eller högre behörigheter på arbetsytan och den posttyp där du vill lägga till poster. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Att tänka på när du importerar poster med hjälp av en Excel- eller CSV-fil

* Kolumnrubrikerna i varje blad blir de fält som är kopplade till poster.
* Varje rad i varje blad blir en unik post som kopplas till.
* Om Excel-filen innehåller mer än ett blad importeras endast den information från ett blad som du väljer under importen.
* Filen får inte överskrida följande:
   * 25 000 rader
   * 500 kolumner
* Filen får inte vara större än 5 MB.
* Tomma blad stöds inte.
* Fält av följande typer stöds inte och kan inte mappas till fält på importbladet:

   * Anslutningsfält till objekttyperna Workfront och AEM Assets. Du kan bara mappa anslutningsfält till posttyperna Planering.
   * Sök efter fält från anslutna Planning-poster eller Workfront- och AEM Assets-objekt
   * Formelfält
   * Skapad den, skapad av
   * Senast ändrat den
   * <span class="preview">Godkänt den </span>
   * Folk
   * Om ett fält med flera eller enstaka val importeras och det har fler alternativ än ett liknande fält i Planering, skapas de ytterligare alternativen under importen. Endast användare med behörigheten Hantera på arbetsytan kan importera nya alternativ.

## Skapa poster genom att importera en CSV- eller Excel-fil

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill skapa poster,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.
1. Klicka på kortet för den posttyp där du vill importera posterna.
1. Klicka på **Ny post** i skärmens övre högra hörn.

   ![Välj sätt att lägga till poster med tre knappar](assets/choose-way-to-add-records-three-button-box.png)
1. Klicka på **Överför från fil** och sedan på **Fortsätt**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Dra och släpp en Excel- eller CSV-fil som tidigare sparats på datorn eller klicka på **Välj en CSV- eller Excel-fil** om du vill bläddra efter en.
1. Klicka på **Förhandsgranska och redigera**.
1. (Villkorligt) Om den importerade filen har fler än ett ark markerar du alternativknappen för det blad du vill importera i rutan **Markera ett ark som ska importeras** och klickar sedan på **Nästa**. I annat fall fortsätter du till nästa steg.

   ![Välj ett kalkylblad för att importera poster](assets/select-a-sheet-to-import-box.png)
1. I **Mappa planeringsfälten till kolumnrubrikerna** väljer du det **planeringsfält** som bäst matchar informationen i varje blads kolumner.

   ![Mappa planeringsfält till kolumner vid import av poster](assets/map-planning-fields-to-columns-when-importing-records.png)

   Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

   >[!TIP]
   >
   >Alla fälttyper stöds inte. Mer information finns i avsnittet [Att tänka på när du importerar poster med hjälp av en Excel- eller CSV-fil](#considerations-about-importing-records-using-an-excel-or-csv-file) i den här artikeln.


1. (Valfritt och villkorligt) Om du har behörigheten Hantera på arbetsytan väljer du **Skapa saknade alternativ** i skärmens nedre vänstra hörn. När det här alternativet är aktiverat läggs de saknade alternativen för ett- och flervalsfält till.

   >[!NOTE]
   >
   >Om den valda posttypen till exempel har ett statusfält med en enda markering där alternativen Nytt, Pågår och Stängt och ett statusfält som importeras från en fil också har ett alternativ för Håll kvar-status, läggs statusalternativet Vid parkering också till.
   >
   >Om du inte har behörigheten Hantera på arbetsytan kan du importera poster, men de ytterligare alternativen skapas inte. Du får i stället följande meddelande i det övre högra hörnet av karta över planeringsfälten till kolumnrubrikrutan: **De alternativ som inte finns i anslutning, envalsfält eller flervalsfält läggs inte till**.

1. Klicka på **Importera**.

   Följande information importeras till Workfront Planning:

   * Nya poster som visas längst ned i tabellvyn för den valda posttypen.
   * Nya fältvärden för befintliga fält som är associerade med varje post.
   * Nya alternativ för ett flervalsfält eller envalsfält som inte fanns i Planning.  <!--when we add connected records - add those here too-->

   Du kan börja hantera fält och poster på posttypssidan.

   Alla som har tillgång till Workfront Planning och arbetsytan kan nu visa och redigera importerade poster och deras information.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
