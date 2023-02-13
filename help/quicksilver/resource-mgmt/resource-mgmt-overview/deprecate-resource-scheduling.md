---
content-type: reference
product-area: resource-management
keywords: arbetsbelastning,utjämnare
navigation-topic: resource-management-overview
title: Borttagning av verktygen för resursplanering i Adobe Workfront
description: Vi håller för närvarande på att ta bort alla schemaläggningsverktyg från Adobe Workfront och ersätta dem med arbetsbelastningsutjämnaren.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Borttagning av verktygen för resursplanering i Adobe Workfront

>[!IMPORTANT]
>  
><span class="preview">Funktionen för schemaläggning som beskrivs i den här artikeln har tagits bort och ersatts från Adobe Workfront från och med version 23.1 i januari 2023.   </span>
>  
> <span class="preview"> Den här artikeln kommer också att tas bort kort efter version 23.1, i början av 2023. Nu rekommenderar vi att du uppdaterar bokmärkena i enlighet med detta. </span>
> 
><span class="preview"> Du kan nu använda belastningsutjämnaren för att schemalägga arbete för dina resurser. </span>
>  
> <span class="preview">Mer information om att schemalägga resurser med hjälp av belastningsutjämnaren finns i avsnittet [Utjämning av arbetsbelastning](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## Hur du ska förbereda dig

Mer information om hur du förbereder övergången mellan schemaläggning och arbetsbelastningsutjämnaren finns i [Migrera från resursschemaläggning till arbetsbelastningsutjämnaren](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

Om du använder schemaläggningsverktygen rekommenderar vi att du avbryter dem och börjar använda belastningsutjämnaren.

![Det globala området för resursplanering](assets/resource-scheduler-global-350x127.png)

Nästan alla funktioner som tidigare fanns tillgängliga i schemaläggningsområdena finns nu tillgängliga i arbetsbelastningsutjämnaren. Mer information finns i avsnittet [Tillgänglighet](#feature-availability) i den här artikeln. Du kan fortsätta att schemalägga dina resurser för arbete exklusivt i Utjämning av arbetsbelastning.

![Det globala området Utjämning av arbetsbelastning](assets/workload-balancer-pti-350x111.png)

## Information som inte överförs till arbetsbelastningsutjämnaren

Följande information överförs inte från schemaläggningsverktygen till arbetsbelastningsutjämnaren:

* **Dagliga allokeringar för användare**: Du bör inte använda både Schemaläggning och Utjämning av arbetsbelastning samtidigt för att justera samma användarallokeringar. Om du har hanterat användarallokeringar i schemaläggningsverktygen överförs inte de justerade dagliga allokeringarna till arbetsbelastningsutjämnaren. Om du har justerat användartilldelningar i Utjämning av arbetsbelastning överförs de inte till planeringsverktygen. Vi rekommenderar starkt att du ser till att de dagliga tilldelningarna är korrekta i arbetsbelastningsutjämnaren för att förbereda övergången. Mer information finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **Filter**: Om du har sparat filter i områden för schemaläggning överförs de inte till Utjämning av arbetsbelastning. Du måste återskapa filtren i Utjämning av arbetsbelastning. Mer information finns i [Filtrera information i Utjämning av arbetsbelastning](../workload-balancer/filter-information-workload-balancer.md).

## Högdagrar i tidslinjen för borttagning

>[!IMPORTANT]
>
>Läs den här artikeln om du vill veta mer om den senaste tidslinjen för borttagning av schemaläggningsverktygen. Alla uppdateringar av tidslinjen meddelas i den här artikeln och i meddelanden från meddelandecentret.

Här följer en tidslinje för borttagningsprocessen för verktygen för resursplanering:

* [2020.4-utgåvan (november 2020)](#2020-4-release-november-2020)
* [2021.4-utgåvan (oktober 2021)](#2021-4-release-october-2021)
* [2022.4-2023.1-utgåvor (oktober 2022-januari 2023)](#2022-4-2023-1-releases)

### 2020.4-utgåvan (november 2020) {#2020-4-release-november-2020}

* Ny funktionalitet är inte längre implementerad för schemaläggningslösningen
* Endast allvarliga fel med hög och kritisk allvarlighetsgrad prioriteras för en korrigering
* Nya funktioner för belastningsutjämnare för arbetsbelastning har lagts till i Workfront

### 2021.4-utgåvan (oktober 2021) {#2021-4-release-october-2021}

* Utjämning av arbetsbelastning är inställt som standard för alla förstagångsanvändare av Workfront
* Förbättrade filter som kan delas och innehålla ytterligare fält

### 2022.4-2023.1-utgåvor (oktober 2022-januari 2023) {#2022-4-2023-1-releases}

* Inga fel prioriteras för en korrigering under och efter 2022.4- eller 2023.1-utgåvan
* Alla schemaläggningsområden tas bort från förhandsvisningsmiljön (**20 oktober 2022**)
* Alla schemaläggningsområden tas bort från produktionsmiljön (**Januari 2023**)
* Arbetsbelastningsutjämnaren är det enda resursplaneringsverktyget som är tillgängligt i Workfront (efter **Januari 2023**)

## Tillgänglighet {#feature-availability}

Om inget annat anges har alla funktioner för resursplanering varit eller kommer att vara tillgängliga i arbetsbelastningsutjämnaren. Mer information om belastningsutjämnaren finns i [Översikt över belastningsutjämnaren](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Förutom befintliga funktioner har eller kommer belastningsutjämnaren att ha nya funktioner som inte fanns i verktygen för resursplanering, vilket visas i följande tabell:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>Funktioner</b></span> </td> 
   <td rowspan="2"> <b>Tillgänglighet för verktyg för resursplanering</b></td> 
   <td colspan="3"><b>Tillgänglighet för funktion för belastningsutjämnare</b></td> 
  </tr> 
  <tr> 
   <td><b>Ute nu</b></td> 
   <td><b>Finns snart</b></td> 
   <td><b>Inte planerat</b></td> 
  </tr> 
  <tr> 
   <td> <p>Åtkomstverktyg från resursområdet</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Separata områden för ej tilldelat och tilldelat arbete</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tillämpa och skapa filter för ej tilldelat och tilldelat arbete</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Få åtkomst till objekt direkt från verktyget</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Tilldela eller ta bort tilldelning av uppgifter och ärenden manuellt</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Justera enskilda allokeringar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Inkludera utgivningstid</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa planerade datum </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa slutfört arbete</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa användartid, helger och schemaläggningsundantag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Tilldela snabbt användare baserat på roller*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Ersätt användare snabbt*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Ta snabbt bort användartilldelning*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Åtkomstverktyg från ett team</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Åtkomstverktyg från ett projekt</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>Användare med arbetslicens kan justera användartilldelningar när de får åtkomst till arbetsbelastningsutjämnaren från ett projekt </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>Visa problem i området Ej tilldelat arbete</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>Tilldela och ta bort tilldelning av uppgifter och ärenden genom att dra och släppa*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Synligt för alla plananvändare, utan att ha utsetts till resurshanterare för projektet.</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppinformation per projekt</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dela arbetsbelastningsutjämnaren med användare utan åtkomst till resursområdet</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa och justera tilldelningar per vecka</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Få åtkomst till användare direkt från verktyget</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Med hjälp av panelen Sammanfattning får du tillgång till mer information om arbetsobjekt utan att behöva navigera bort*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa och justera allokering som ett procentvärde </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa skillnaden mellan tillgänglig och allokerad tid</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visa användartillgänglighet i ett diagram</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Färgkoda arbetsobjekt och projekt efter projektstatus</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uppdatera automatiskt planerade timmar när du justerar användartilldelning (för uppgifter med en enkel varaktighetstyp)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Föreslå tilldelningar baserat på användarens tilldelningsmönster, befintliga roll- eller teamtilldelningar</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Förbättrade filter som kan delas och innehålla ytterligare fält</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Gör avancerade uppdrag</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>Färgkoda arbetsobjekt efter projekt och projektstatus</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>Lägg till användare i projektteamet (omlokaliserat till <b>Folk</b> projektflik) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>Tilldela uppgifter och ärenden automatiskt</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*Dessa funktioner är endast tillgängliga i den nya Adobe Workfront-upplevelsen.
