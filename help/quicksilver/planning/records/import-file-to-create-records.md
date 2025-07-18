---
title: Skapa poster genom att importera information från en CSV- eller Excel-fil
description: Poster är enskilda instanser av posttyper, som är objekttyperna i Adobe Workfront Planning. I Workfront Planning kan du skapa poster genom att importera information från en CSV- eller Excel-fil.
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

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är endast tillgänglig i förhandsversionsmiljön för alla kunder. Efter de månatliga versionerna till produktion är samma funktioner också tillgängliga i produktionsmiljön för kunder som har aktiverat snabba versioner. </span>

<span class="preview">Information om snabba versioner finns i [Aktivera eller inaktivera snabba versioner för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Poster är enskilda instanser av posttyper, som är objekttyperna i Adobe Workfront Planning. I Workfront Planning kan du skapa poster genom att importera information från en CSV- eller Excel-fil.

Mer information om hur du skapar poster finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

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
   <td> Standard
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p> 
   <p>Redigeringsåtkomst i Workfront för de objekttyper som du vill skapa (projekt, program och portföljer) när du kopplar dem från nya poster  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td> <p>Bidra eller högre behörigheter till arbetsytan och posttypen där du vill lägga till poster. </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat</p>
   <p>Hantera behörigheter till Workfront-objekt (portföljer) för att lägga till underordnade objekt (projekt).</p>
   </td> 
  </tr> 
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Att tänka på när du importerar poster med hjälp av en Excel- eller CSV-fil

* Kolumnrubrikerna i varje blad blir de fält som är associerade med posterna.
* Varje rad i varje blad blir en unik post som är associerad.
* Om Excel-filen innehåller mer än ett blad importeras endast den information från ett blad som du väljer under importen.
* Filen får inte vara längre än följande:
   * 25 000 rader
   * 500 kolumner
* Filen får inte vara större än 5 MB.
* Tomma ark stöds inte.
* Fält av följande typer stöds inte och kan inte mappas till fält på importbladet:

   * Anslutningsfält till objekttyperna Workfront och AEM Assets. Du kan endast mappa anslutningsfält till posttyper för planering.
   * Uppslagsfält från anslutna planeringsposter eller Workfront- och AEM Assets-objekt
   * Fält för formler
   * Skapad den, Skapad av
   * Datum för senaste ändring, Senast ändrad av
   * <span class="preview">Godkänt datum, Godkänt av</span>
   * Folk
   * Om ett flervalsfält eller ett flervalsfält importeras och det har fler val än ett liknande fält i Planering, skapas de ytterligare alternativen under importen. Endast användare med behörigheten Hantera till arbetsytan kan importera nya val.

## Skapa poster genom att importera en CSV- eller Excel-fil

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill skapa poster,

   Eller

   Från en arbetsyta expanderar du den nedåtpekande pilen till höger om ett befintligt arbetsytenamn, söker efter en arbetsyta och väljer den sedan när den visas i listan.
1. Klicka på kortet för den posttyp som du vill importera posterna till.
1. Klicka på **Ny post** i det övre högra hörnet av skärmen.

   ![Välj sätt att lägga till poster med tre knappar](assets/choose-way-to-add-records-three-button-box.png)
1. Klicka på **Ladda upp från fil** och sedan **på Fortsätt**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Dra och släpp en Excel- eller CSV-fil som tidigare sparats på datorn, eller klicka på **Välj en CSV- eller Excel-fil** för att bläddra efter en.
1. Klicka på **Förhandsgranska och redigera**.
1. (Villkorligt) Om den importerade filen innehåller mer än ett blad markerar du alternativknappen för det blad som du vill importera i **rutan Välj ett blad att importera** och klickar sedan på **Nästa**. Annars fortsätter du till nästa steg.

   ![Välj ett blad för att importera poster](assets/select-a-sheet-to-import-box.png)
1. I Mappa planeringsfälten **till kolumnrubrikerna** väljer du det **planeringsfält** som bäst matchar informationen i varje kolumn i bladet.

   ![Mappa planeringsfält till kolumner vid import av poster](assets/map-planning-fields-to-columns-when-importing-records.png)

   Varje rad representerar en ny post. Endast de första 10 posterna visas i rutan Förhandsgranska och redigera.

   >[!TIP]
   >
   >Alla fälttyper stöds inte. Mer information finns i avsnittet [Att tänka på när du importerar poster med hjälp av en Excel- eller CSV-fil](#considerations-about-importing-records-using-an-excel-or-csv-file) i den här artikeln.


1. (Valfritt och villkorligt) Om du har behörighet att hantera arbetsytan väljer du **alternativen Skapa saknade i** det nedre vänstra hörnet på skärmen. När det här alternativet är aktiverat läggs de saknade valen för enkel- och flervalsfält till.

   >[!NOTE]
   >
   >Om den valda posttypen till exempel har ett statusfält med ett val med alternativen Nytt, Pågår och Stängt, och ett statusfält som importerats från en fil också har ett alternativ för Spärrstatus, läggs även statusvalet Spärrad till.
   >
   >Om du inte har behörigheten Hantera till arbetsytan kan du importera poster, men de ytterligare valen kommer inte att skapas. I stället får du följande meddelande i det övre högra hörnet av rutan Mappa planeringsfälten till kolumnrubrikerna: **De alternativ som inte finns i anslutnings-, enkel- eller flervalsfält kommer inte att läggas till**.

1. Klicka på **Importera**.

   Följande information importeras till Workfront Planning:

   * Nya poster som visas längst ned i tabellvyn för den valda posttypen.
   * Nya fältvärden för befintliga fält som är associerade med varje post.
   * Nya val av ett flervals- eller enkelvalsfält som inte fanns i Planering.  <!--when we add connected records - add those here too-->

   Du kan börja hantera fält och poster på sidan för posttyper.

   Alla som har tillgång till Workfront Planning och arbetsytan kan nu visa och redigera de importerade posterna och deras information.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
