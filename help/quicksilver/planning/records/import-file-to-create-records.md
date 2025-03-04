---
title: Skapa poster genom att importera information från en CSV- eller Excel-fil
description: Poster är enskilda instanser av posttyper, som är objekttyper i Adobe Workfront Planning. I Workfront Planning kan du skapa poster genom att importera information från en CSV- eller Excel-fil.
hide: true
hidefromtoc: true
source-git-commit: 9f17fcab210768923e866d2f1596f40ddf8a558e
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---


<!-- add the following in the metadata when live:

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog-->

# Skapa poster genom att importera information från en CSV- eller Excel-fil

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Poster är enskilda instanser av posttyper, som är objekttyper i Adobe Workfront Planning. I Workfront Planning kan du skapa poster genom att importera information från en CSV- eller Excel-fil.

Mer information om hur du skapar poster finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

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
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
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
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p> 
   <p>Redigera åtkomst i Workfront för de objekttyper som du vill skapa (projekt och portföljer) när du kopplar posterna till dem. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td> <p>Hantera behörigheter för den arbetsyta som du vill lägga till poster i. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>
   <p>Hantera behörigheter för Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du importerar posttyper med hjälp av en Excel- eller CSV-fil

* Kolumnrubrikerna i varje blad blir de fält som är kopplade till poster.
* Varje rad i varje blad blir en unik post som kopplas till.
* Om Excel-filen innehåller mer än ett blad importeras endast den information från ett blad som du väljer under importen.
* Filen får inte överskrida följande:
   * 10 000 rader
   * 500 kolumner
* Filen får inte vara större än 5 MB.
* Tomma blad stöds inte.
* Fält av följande typer stöds inte och kan inte mappas till fält på importbladet:
   * Sök efter fält för anslutna poster eller anslutna Workfront-objekt
   * Formelfält
   * Skapad den, skapad av
   * Senast ändrat den
   * Folk
* Om ett fält med flera eller enstaka val importeras och det har fler alternativ än ett liknande fält i Planering, skapas de ytterligare alternativen under importen.

## Skapa poster genom att importera en CSV- eller Excel-fil

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill skapa posttyper,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.
1. Klicka på kortet för den posttyp där du vill importera posterna.
1. Klicka på **Ny post** i skärmens övre högra hörn.
1. Klicka på **Överför från fil** och sedan på **Fortsätt**.
1. Dra och släpp en Excel- eller CSV-fil som tidigare sparats på datorn eller klicka på **Välj en CSV- eller Excel-fil** om du vill bläddra efter en.
1. Klicka på **Förhandsgranska och redigera**.
1. (Villkorligt) Om den importerade filen har fler än ett ark markerar du alternativknappen för det blad du vill importera i rutan **Markera ett ark som ska importeras** och klickar sedan på **Nästa**. I annat fall fortsätter du till nästa steg.

   ![Välj ett kalkylblad för att importera poster](assets/select-a-sheet-to-import-box.png)
1. I **Mappa planeringsfälten till kolumnrubrikerna** väljer du det **planeringsfält** som bäst matchar informationen i varje blads kolumner.

   ![Mappa planeringsfält till kolumner vid import av poster](assets/map-planning-fields-to-columns-when-importing-records.png)

   Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

1. (Valfritt) Välj **Skapa saknade alternativ** i skärmens nedre vänstra hörn. När det här alternativet är aktiverat läggs de saknade alternativen för ett- och flervalsfält till.

   Om den valda posttypen till exempel har ett statusfält med en enda markering med alternativen Nytt, Pågår och Stängt och ett statusfält som importerats från en fil också har alternativet Håll kvar, läggs statusalternativet till

   <!--when we add connected records and the info icon in the tool changes, also add those items to this step-->

1. Klicka på **Importera**.

   Följande information importeras till Workfront Planning:

   * Nya poster som visas längst ned i tabellvyn för den valda posttypen.
   * Nya fältvärden för befintliga fält som är associerade med varje post.
   * Nya alternativ för ett flervalsfält eller envalsfält som inte fanns i Planning.

   Du kan börja hantera fält och poster på posttypssidan.

   Alla som har tillgång till Workfront Planning och arbetsytan kan nu visa och redigera importerade poster och deras information.