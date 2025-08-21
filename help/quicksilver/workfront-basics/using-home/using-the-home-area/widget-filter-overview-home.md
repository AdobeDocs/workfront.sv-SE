---
product-area: home
navigation-topic: new-home
title: Översikt över filter för hemwidget
description: Du kan välja bland ett antal widgetar för att anpassa innehållet som visas på hemsidan. Dessa widgetar kan storleksändras och ordnas på hemsidan.
author: Courtney
feature: Get Started with Workfront
exl-id: 58f79e81-df6b-456f-9e91-4e00a1c2a8a2
source-git-commit: 884ade1102e685ec01af2790b17acb50c2114ca7
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# Översikt över filter för hemwidget

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

Du kan använda filter på följande widgetar för att söka efter och ordna arbeten:

* [Mina projekt](#my-projects)
* [Mina uppgifter](#my-tasks)
* [Mina problem](#my-issues)
* [Mina förfrågningar](#my-requests)
* [Mitt arbete](#my-work)
* [Mina godkännanden](#my-approvals)

>[!IMPORTANT]
>
>* Om du vill visa uppgifter och problem i Home-widgetarna måste det överordnade projektet ha statusen Aktuell eller en status som motsvarar aktuell.
>* Projekt måste också ha statusen Aktuell eller en status som är lika med aktuell att visa.

## Mina projekt

Du kan använda följande filter i widgeten Mina projekt:

<table>
  <tr>
    <td>Aktiv</td>
    <td>Visar projekt i följande statusar: Aktuell, Planerad och Godkänd </td>
  </tr>
  <tr>
    <td>Risk</td>
    <td>Visar projekt i Riskstatus </td>
  </tr>
  <tr>
    <td>Efter schema</td>
    <td>Visar projekt i Bakom-status</td>
  </tr>
  <tr>
    <td>Aktuell</td>
    <td>Visar projekt med aktuell status </td>
  </tr>
  <tr>
    <td>Förfaller den här månaden</td>
    <td>Visar projekt med planerade slutförandedatum som ligger inom den aktuella kalendermånaden</td>
  </tr>
  <tr>
    <td>Sena</td>
    <td>Visar projekt med statusen Sent</td>
  </tr>
  <tr>
    <td>Mina projekt</td>
    <td>Visar projekt som är tilldelade mig eller mitt projektteam med statusen Aktuell</td>
  </tr>
  <tr>
    <td>I tid</td>
    <td>Visar projekt i statusen På tid</td>
  </tr>
  <tr>
    <td>Över kostnadsbudget</td>
    <td>Visar projekt där det faktiska kostnadsvärdet är större än det planerade kostnadsvärdet</td>
  </tr>
  <tr>
    <td>Över arbetsbudget</td>
    <td>Visar projekt där värdet Faktiskt arbete krävs är större än värdet Arbete krävs</td>
  </tr>
  <tr>
    <td>Endast köer</td>
    <td>Visar projekt som har angetts som begärandeköer</td>
  </tr>
  <tr>
    <td>Begärd</td>
    <td>Visar projekt i begärd status</td>
  </tr>
  <tr>
    <td>Scenarioplaneringsprojekt</td>
    <td>Visar projekt med ett ID för Initiative som angetts via Scenarioplanen</td>
  </tr>
</table>

## Mina uppgifter

Du kan använda följande filter i widgeten Mina uppgifter:

<table>
  <tr>
    <td>Aktiva aktiviteter</td>
    <td><p>Visar aktiviteter utan datum eller datum för leverans som är i dag eller tidigare och</p>
<ul>
  <li>En slutförandeprocent som är mindre än 100 %</li>
  <li>Värdet för Can Start är true</li>
</ul>
</td>
  </tr>
   <!-- <tr>
    <td>All Unassigned Tasks</td>
    <td></td>
  </tr> -->
  <tr>
    <td>Godkännandeuppgifter</td>
    <td>Visar uppgifter som väntar på godkännande</td>
  </tr>
  <tr>
    <td>Kan starta</td>
    <td><p>Visar uppgifter som tilldelats mig och som</p>
<ul>
  <li>Har inte samma status som fullständig</li>
  <li>Har ett Can Start-värde som är true</li>
</ul>
</td>
  </tr>
  <tr>
    <td>Kritisk sökväg</td>
    <td>Visar uppgifter som betecknas som Kritisk</td>
  </tr>
  <tr>
    <td>Ofullständiga uppgifter</td>
    <td>Visar uppgifter med statusvärden som är inställda på vad som helst förutom Fullständigt</td>
  </tr>
  <tr>
    <td>Milstolpeuppgifter</td>
    <td>Visar aktiviteter som är associerade med en milstolpe. Mer information finns i <a href="/help/quicksilver/manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Koppla milstolpar till aktiviteter</a>.
</td>
  </tr>
  <tr>
    <td>Mina projektuppgifter</td>
    <td>Visar aktiviteter med aktuell status där jag är medlem i projektteamet </td>
  </tr>
    <tr>
    <td>Mina uppgifter</td>
    <td>Visar uppgifter som tilldelats mig</td>
  </tr>
  <tr>
    <td>Inte tilldelad en iteration</td>
    <td>Visar uppgifter som inte har tilldelats en iteration</td>
  </tr>
  <tr>
    <td>Nyligen intressanta</td>
    <td><p>Visar aktiviteter där den senaste uppdateringen gjordes under de senaste två veckorna och</p>
<ul>
  <li>Bekräftelsedatumet är senare än det planerade slutförandedatumet</li>
  eller
  <li>Projektets längd är längre än den planerade varaktigheten</li>
  eller
  <li>Villkoret är jämnt eller vissa bekymmer</li>
  eller
  <li>Den primära tilldelade aktiviteten har börjat arbeta med uppgiften</li>
</ul>
</td>
  </tr>
  <tr>
    <td>Ej tilldelade uppgifter i Min roll</td>
    <td><p>Visar aktiviteter som</p>
<ul>
  <li>Tilldelad till min roll</li>
  <li>Ofullständig</li>
</ul>
</td>
  </tr>
  <tr>
    <td>Kommande uppgifter</td>
    <td><p>Visar uppgifter som</p>
<ul>
  <li>Är ofullständiga</li>
  <li>Tillhör ett projekt med aktuell status</li>
  <li>Har ett planerat startdatum inom två veckor från dagens datum</li>
</ul>
</td>
  </tr>
</table>

## Mina problem

Du kan använda följande filter i widgeten Mina problem:

<table>
<tr>
    <td>Alla ej tilldelade</td>
    <td>Visar alla problem som inte har tilldelats och som inte har ett matchande objekt bifogat </td>
  </tr>
  <tr>
    <td>Tilldelad mig</td>
    <td>Visar problem där jag är primär tilldelad</td>
  </tr>
  <tr>
    <td>Complete</td>
    <td>Visar problem med slutförandedatum </td>
  </tr>
  <tr>
    <td>Anges av mig</td>
    <td>Visar problem som har angetts</td>
  </tr>
  <tr>
    <td>Mina projektproblem</td>
    <td><p>Visar problem där</p>
<ul>
  <li>Jag är primär tilldelad</li>
  <li>Statusen är ofullständig</li>
  <li>Det finns inget matchande objekt bifogat</li>
</ul>
</td>
  </tr>
    <tr>
    <td>Mina senast skickade problem</td>
    <td><p>Visar problem som</p>
<ul>
  <li>Jag skickade</li>
  <li>Det finns inget matchande objekt bifogat</li>
  <li>Statusen är inte Klar och det finns inget Slutförandedatum</li>
  <li>Anges inom tre månader från dagens datum</li>
</ul>
</td>
  </tr>
    </tr>
    <tr>
    <td>Mina skickade problem</td>
    <td>Visar problem som jag äger</td>
  </tr>
  <tr>
    <td>Öppna</td>
    <td>Visar problem som inte har något slutförandedatum</td>
  </tr>
  <tr>
    <td>Lösbar</td>
    <td>Visar problem som åtgärdar bifogade objekt</td>
  </tr>
  <tr>
    <td>Ej tilldelad i min roll</td>
    <td>Visar alla problem som inte har tilldelats en primär användare men som har en tilldelad roll </td>
  </tr>
</table>

## Mina förfrågningar

I produktionsmiljön:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alla</td> 
      <td>Visar alla skickade begäranden, oavsett status eller vem som har skickat dem.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Öppna</td> 
      <td> <p>Visar alla skickade begäranden 
      <ul>
      <li>De är för närvarande öppna, oavsett vem som skickade dem. Det är bara begäranden om att du har minst behörighet att visa här om du inte har skickat in dem själv.</li>
      <li>Utan ett faktiskt slutförandedatum eller vars stängningsobjekt inte har något faktiskt slutförandedatum visas på underfliken Öppna.</li> 
      </ul>
      <p><b>OBS!</b> 
      Begäranden som har en status som inte är lika med Stängt betraktas som öppna.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mina förfrågningar</td> 
      <td>Visar begäranden som du har skickat, oavsett status. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mina öppna förfrågningar</td> 
      <td> <p>Visar begäranden 
      <ul>
      <li>Att du skickade in och fortfarande är öppen. </li> 
      <li>Utan ett faktiskt slutförandedatum eller vars matchande objekt inte har något faktiskt slutförandedatum visas på underfliken Mina öppna begäranden. </li> 
      </ul>
      <p><b>OBS!</b> 
      Begäranden som inte har en status som motsvarar stängda betraktas som öppna.</p> </td> 
     </tr> 
    </tbody> 
   </table>

<div class="preview">

I förhandsvisningsmiljön:

Widgeten Mina förfrågningar har ett anpassningsbart filter som gör att du kan styra vilka förfrågningar som visas i widgeten. Du kan konfigurera det här filtret för olika fält och värden, och du kan stapla villkor med AND och OR.

Instruktioner om hur du konfigurerar filtret i widgeten Mina förfrågningar finns i [Filterförfrågningar](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md#filter-requests) i artikeln Använda widgeten Mina förfrågningar.

</div>

## Mitt arbete

Du kan använda följande filter i widgeten Mitt arbete:

<table>
  <tbody>
    <tr>
      <td>Arbetar på</td>
      <td>Visar objekt som du arbetar med</td>
    </tr>
    <tr>
      <td>Klar att börja</td>
      <td>Visar objekt med 
      <ul>
      <li>Inga ofullständiga föregångare eller aktivitetsbegränsningar</li>
      <li>Det planerade startdatumet har passerat eller är upp till två veckor i framtiden</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>Inte klar</td>
      <td>Visar objekt som har
       <ul>
      <li>Ofullständiga föregående aktiviteter eller aktivitetsbegränsningar som förhindrar att objektet bearbetas</li>
      eller
      <li>Det planerade startdatumet är mer än två veckor i framtiden</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Begärd</td>
      <td>Visar problem som du inte har börjat arbeta med</td>
    </tr>
    <tr>
      <td>Delegerad av mig</td>
      <td>Visar objekt som du har delegerat till andra användare</td>
    </tr>
    <tr>
      <td>Delegerat till mig</td>
      <td>Visar objekt som användare har delegerat till dig</td>
    </tr>
    <tr>
      <td>Slutförd</td>
      <td>Visar det arbete som utförts de senaste två veckorna. Det här filteralternativet inkluderar inte godkännanden.</td>
    </tr>
  </tbody>
</table>

## Mina godkännanden

Du kan använda följande filter i widgeten Mina godkännanden:

<table>
  <tbody>
    <tr>
      <td>Delegerade godkännanden</td>
      <td>Visar godkännanden som har delegerats till dig</td>
    </tr>
    <tr>
      <td>Mina godkännanden</td>
      <td>Visar objekt som kräver ditt godkännande
      </td>
    </tr>
    <tr>
      <td>Godkännanden som jag har skickat</td>
      <td>Visar objekt som du har skickat in för godkännande
       </td>
    </tr>
  </tbody>
</table>
