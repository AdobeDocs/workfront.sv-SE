---
title: Importera fält från Adobe Workfront
description: I Adobe Workfront Planning kan du skapa anpassade fält för varje typ av posttyp. Du kan sedan associera fältet med Workfront Planning-poster.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 994594f2-a888-423a-bf66-0d14baf57c55
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

<!--add to TOC-->

# Importera fält från Adobe Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Du kan importera kopior av befintliga Workfront-fält. När du importerar fält från Workfront skapas en kopia av varje fält för en posttyp av Workfront Planning.


## Åtkomstkrav

+++ Expandera för att visa åtkomstkrav..

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
   <td><p> Standard </p>
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
   <td>   <p>Hantera behörigheter till en arbetsyta <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Systemadministratörer har behörighet för alla arbetsytor, inklusive de som de inte skapade.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du importerar fält från Workfront

* Du kan importera inbyggda eller anpassade Workfront-fält till en posttyp i Workfront Planning.
* När du importerar Workfront-fält skapas kopior av samma fält och fältnamnet bevaras i Workfront Planning. När de har kopierats till Workfront Planning är fälten oberoende av de ursprungliga Workfront-fälten och de delar ingen information.
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* Du kan lägga till inbyggda eller anpassade fält från följande Workfront-objekt:
   * Portfolio
   * Program
   * Projekt
   * Uppgift
   * Problem
   * Dokument
   * Företag
   * Grupp
   * Användare
   * Jobbroll
   * Tilldelning
   * Timme
   * Faktureringspost
     <!--Available only to Preview, but might not come to Prod:* Rate card - visible in Production but asking PM if it should be hidden-->
   * Utgift
   * Upprepning
     <!--* Non-labor resource - - visible in Production but asking PM if it should be hidden-->
     <!--* Non-labour resource category - - visible in Production but asking PM if it should be hidden-->
* Fälten i Workfront kanske inte behåller sin fälttyp när de har importerats till Workfront Planning.

  Tabellen nedan visar Workfront-fälttyper och deras motsvarande Workfront Planning-fälttyp.

  | Workfront fälttyp | Workfront Planning, fälttyp |
  |------------------------------------------|-------------------------------|
  | Textformaterad enkelradig text | Enkelradig text |
  | Nummerformaterad enkelradstext | Nummer |
  | Valutaformaterad enkelradstext | Valuta |
  | Stycke | Stycke |
  | Text med formatering | Stycke |
  | Listruta med ett val | Enkelval |
  | Listruta för flera val | Flera val |
  | Användartypsnittsfilter stöds inte | Folk |
  | Beräknat* | Formel |
  | Datum | Datum |
  | Kryssrutegrupp | Flera val |
  | Alternativknapp | Flera val |

  *Beräknade fält kommer att vara tillgängliga vid ett senare datum.
Alla andra Workfront-fälttyper stöds inte i Workfront Planning.


## Importera fält från Workfront

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill skapa fält för.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på kortet för en posttyp.

   Alla befintliga poster som är associerade med posttypen visas i tabellvyns rader.

   >[!TIP]
   >
   >    Vissa fält kan vara dolda. Klicka på **Fält** och aktivera växlingen för de fält som du vill visa som kolumner i tabellvyn.

1. Klicka på ikonen **+** i tabellvyns övre högra hörn

   eller

   Håll markören över en kolumnrubrik, klicka på den nedåtriktade pilen efter fältnamnet och klicka sedan på **Infoga vänster** eller **Infoga höger** för att lägga till det nya fältet.
1. Klicka på **Lägg till befintlig** i det nedre högra hörnet på fliken **Nytt fält**. <!--check UI - did they change this??-->

   ![Lägg till befintliga fält från Workfront modal](assets/add-existing-fields-from-workfront-modal.png)

1. Börja skriva namnet på ett befintligt Workfront-fält i sökområdet och klicka sedan på **+** när det visas i listan.
1. (Valfritt) Skriv ett annat fält och klicka sedan på **+** när det visas i listan.
1. (Valfritt) Klicka på ikonen **Filter** ![Filter i importfältikonen](assets/filters-in-import-fields-icon.png) och uppdatera sedan ett eller båda av följande fält:

   * Objekttyp: Markera en Workfront-objekttyp vars fält du vill importera.
   * Anpassat formulär: Välj ett eller flera anpassade formulär från Workfront. Du kan välja ett anpassat formulär utan att först markera en objekttyp.
1. Klicka på **+** och sedan på **Lägg till fält**.
Fälten läggs till i tabellvyn och på posternas informationssidor.

   >[!IMPORTANT]
   >
   >    Det finns en gräns på 500 fält för valfri posttyp. De befintliga fälten tillsammans med de importerade fälten bidrar till den här gränsen.

   De tillagda fälten är kopior av Workfront-fälten och är inte längre kopplade till originalfälten i Workfront.