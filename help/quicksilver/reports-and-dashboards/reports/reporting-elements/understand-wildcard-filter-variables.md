---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variabler för jokertecken
description: Genom att använda jokertecken i filter kan du referera till en allmän användare eller ett allmänt datum i stället för en specifik användare eller ett specifikt datum. På så sätt är elementen som du skapar dynamiska och resultatet ändras beroende på i vilket sammanhang de används.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Översikt över filtervariabler för jokertecken

<!-- Audited: 11/2024 -->

<!--(NOTE: This article is linked to the training self-serve promoted articles for user-based and date-based wildcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.)
(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.
This was included but it is not supported???:
The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.
For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:
AssignedToID Equals $$USER.roleIDs.)-->

Med jokertecken kan du referera till en allmän användare eller ett allmänt datum i stället för en specifik användare eller ett specifikt datum. På så sätt är elementen som du skapar dynamiska. Resultatet ändras beroende på i vilket sammanhang de används.

Om du till exempel filtrerar $$USER.homeGroupID i en projektrapport hämtas endast projekt som är kopplade till hemgruppen för den användare som är inloggad.

Du kan använda filtervariabler, som också kallas jokertecken, när du skapar följande element:

<table>
    <tr>
        <td>Filter i listor, rapporter och Resursplanering</td>
        <td>Mer information om Workfront-filter finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Översikt över filter</a>.
</td>
    </tr>
    <tr>
        <td>Avancerade sökningar</td>
        <td>Mer information om avancerade sökningar finns i avsnittet <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Använd avancerad sökning</a> i artikeln <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Sök i Adobe Workfront</a>.
    </tr>
    <tr>
        <td>Beräknade kolumner i vyer</td>
        <td></td>
    </tr>
    <tr>
        <td>Villkorsstyrd formatering i vyer</td>
        <td>Mer information om villkorsstyrd formatering finns i artikeln <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Använd villkorsstyrd formatering i vyer</a>.
    </tr>
    <tr>
        <td>Beräknade anpassade fält</td>
        <td>Jokerteckensfiltervariabler stöds inte när kapslade samlingar i en beräknad kolumn refereras.

Mer information om beräknade anpassade fält och kolumner finns i artikeln <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Beräknade anpassade fält kontra beräknade kolumner</a>.
</td>
    </tr>
</table>

## Datumbaserade jokerteckensfiltervariabler

Alternativen för datumbaserade jokertecken kan användas i kombination med alla datumfilterattribut. Mer information om hur du lägger till ett datumbaserat jokertecken i en rapport finns i artikeln [Använd datumbaserade jokertecken för att generera rapporter](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Om du skapar en datum- och tidsberäkning som inte innehåller någon tidsdel, eller som använder datumjokertecknen $$TODAY eller $$NOW, används datumet enligt UTC-zonen (Coordinated Universal Time), inte enligt din lokala tidszon. Detta kan orsaka ett oväntat datumresultat.

Du kan välja mellan följande datumbaserade jokertecken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$IDAG</strong> </p> </td> 
   <td> <p>Vi rekommenderar att du skapar datumkänsliga filter med detta jokertecken så att du slipper skapa filtret igen i morgon, nästa vecka eller nästa månad.</p> <p>Om du till exempel vill visa alla aktiviteter som förfaller idag kan du använda följande regel i ett aktivitetsfilter: <em>Planerat startdatum mindre än $$TODAY</em>.</p> <p>$$TODAY är alltid lika med midnatt för den aktuella dagen.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NU</strong> </p> </td> 
   <td> <p>Detta liknar jokertecknet $$TODAY, men innehåller aktuellt datum och aktuell tid. $$NOW är lika med aktuellt datum och aktuell tid.</p> <p>Om du till exempel vill visa alla timposter som har tillhandahållits fram till den aktuella tiden kan du göra detta genom att använda följande regel i ett timfilter: <em>Planerat startdatum mindre än $$NOW</em>.</p> <p>Obs! Detta jokertecken stöds inte i resursplaneraren.</p> </td> 
  </tr> 
 </tbody> 
</table>

Om du vill ange olika tidsperioder och olika tidpunkter (framtida eller tidigare) kan du kombinera jokertecknen ovan med följande:

| Attribut |   |
|---|---|
| **q** | kalenderkvartal |
| **h** | timme |
| **d** | dag |
| **w** | vecka |
| **m** | månad |
| **y** | år |

{style="table-layout:auto"}

| **Kvalificerare** | |
|---|---|
| **b** | början av perioden (utan ett angivet attribut blir veckans början som standard: söndag) |
| **e** | slutet av perioden (utan ett angivet attribut är standardvärdet till slutet av veckan: lördag) |

{style="table-layout:auto"}

| **Operatorer** | |
|---|---|
| **+** | lägg till värde i jokerteckenvärde |
| **-** | subtrahera värde från jokertecken |

{style="table-layout:auto"}

Jokertecknet `$$TODAYb+2w` refererar till exempel till&quot;2 veckor från början av den här veckan&quot;. Jokertecknet *`$$NOW+2h` refererar till&quot;2 timmar från och med nu&quot;.

## Användarbaserade variabler för jokertecken

>[!IMPORTANT]
>
>Om ett filter eller en rapport innehåller en användarbaserad jokerteckensfiltervariabel visar resultaten alltid information som filtrerats av den användare som är inloggad. När du delar ett sådant filter eller en sådan rapport med en annan användare, hämtar jokertecknet information för användaren som tittar på rapporten. De två användarna ser olika resultat.
>
>Mer information om hur du lägger till ett användarbaserat jokertecken i en rapport finns i artikeln [Använda användarbaserade jokertecken för att generera rapporter](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Du kan välja mellan följande användarbaserade variabler:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>Den vanligaste användarbaserade variabeln är $$USER.ID. Detta returnerar alltid den inloggade användarens ID. Detta är det ID som används för att identifiera vilken användare som har skapat varje objekt och deras arbetstilldelningar.</p> <p>När jokertecknet används i rapporter minskar det antalet rapporter som du behöver skapa i systemet. Du kan skapa en rapport och dela den med flera användare, och resultatet ändras baserat på den användare som är inloggad och tittar på rapporten.</p> <p>Om du till exempel vill skapa en rapport för alla utgåvor som tilldelats den användare som är inloggad, kan du använda följande regel i ett utgivningsfilter: <em>Tilldelad till ID är lika med $$USER.ID</em>.</p> <p>Workfront använder den här variabeln i följande inbyggda filter:</p> 
    <ul> 
     <li>Mina rapporter</li> 
     <li>Mina projekt</li> 
     <li>Mina uppgifter</li> 
     <li>Mina problem</li> 
     <li>Mina timmar</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.categoryID refererar till ett specifikt anpassat formulär som är associerat med den inloggade användaren.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.accessLevelID refererar till ID:t för åtkomstnivån som är associerad med den inloggade användaren.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>Variabeln $$USER.accessLevelRank refererar till den åtkomstnivårangordning som är associerad med den inloggade användaren.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.companyID refererar till det företag som är associerat med den inloggade användaren.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.customerID refererar till ID:t för kundkontot som är kopplat till din miljö. För din miljö finns det bara ett möjligt värde för den här variabeln och den används vanligtvis bara när du skapar integreringar via API:t.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>Variabeln $$USER.firstName refererar till den inloggade användarens förnamn.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>Variabeln $$USER.lastName refererar till den inloggade användarens efternamn.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>Variabeln $$USER.name refererar till det fullständiga namnet för den inloggade användaren.</p> <p>Obs!   <p>Denna jokervariabel fungerar bara när du ändrar ett filter i textläge. Du kan inte använda det här jokertecknet i filter som inte har stöd för textläge. Du kan till exempel inte använda jokertecknet i filtren i följande områden:</p> 
     <ul> 
      <li> <p>Resursplanering</p> </li> 
      <li> <p>Utjämning av arbetsbelastning</p> </li> 
      <li> <p>Analyser</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.homeGroupID refererar till ID:t för hemgruppen för den inloggade användaren. Som gruppadministratör kan du använda den här variabeln för att filtrera endast objekt som tillhör användarna i din hemgrupp.</p> <p>Om du till exempel vill se alla ofullständiga uppgifter i projekt i den ekonomiska gruppen använder du följande filterregler i ett aktivitetsfilter:<br><em>Projekt: Grupp-ID motsvarar $$USER.homeGroupID </em><br><em>Procent färdigt mindre än 100</em></p> <p>Om du vill visa alla ofullständiga uppgifter som tilldelats enskilda personer i en viss grupp som är hemgruppen för den inloggade användaren använder du följande filterregler i ett uppgiftsfilter:</p> <p><em>Tilldelad: Grupp-ID motsvarar $$USER.homeGroupID<br>Procent färdigt mindre än 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>Variabeln $$USER.otherGroupIDs refererar till alla grupper (inklusive hemgruppen) som är kopplade till den inloggade användarens profil.</p> <p>Funktionen för den här variabeln liknar funktionen för variabeln $$USER.homeGroupID, förutom att resultaten visar information om de användare som tillhör någon av de grupper som är associerade med den inloggade användaren.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.homeTeamID refererar till ID:t för hemteamet för den inloggade användaren. Som gruppansvarig kan du använda den här variabeln för att filtrera endast objekt som tillhör användarna i ditt hemteam.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamID:n</strong> </p> </td> 
   <td> <p>Variabeln $$USER.teamIDs returnerar en lista över alla team som är associerade med den inloggade användaren.</p> <p>Funktionen för den här variabeln liknar funktionen för variabeln $$USER.homeTeamID, förutom att resultaten visar information om användaren som tillhör någon av de team som identifieras i filtret.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>Variabeln $$USER.roleID refererar till den inloggade användarens primära roll. Med hjälp av den här variabeln kan du rapportera uppgifter eller ärenden som tilldelats en specifik jobbroll.</p> <p>Om du till exempel vill se alla uppgifter som tilldelats den inloggade användarens primära roll kan du använda följande filterregel i ett uppgiftsfilter:</p> <p><em>Aktivitet: Roll-ID är lika med $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>Variabeln $$USER.roleIDs refererar till alla jobbroller som är associerade med den inloggade användaren. Med den här variabeln kan du rapportera uppgifter eller ärenden som tilldelats någon av de jobbroller som är kopplade till den inloggade användaren. </p> <p>Om du till exempel vill se alla uppgifter som tilldelats någon av de roller som är associerade med den inloggade användaren, kan du använda följande filterregel i ett uppgiftsfilter:</p> <p><i>Aktivitet: Roll-ID är lika med $$USERID.roleID<br></i> </p> <p>Tips! <i>Aktiviteten: Roll-ID är lika med $$USERID.roleIDs</i> filterregeln finns i de inbyggda filtren Ej tilldelade uppgifter i Min roll och Ej tilldelade ärenden i min roll. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Objektbaserade jokerteckensfiltervariabler

Du kan välja mellan följande objektbaserade jokertecken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>Variabeln $$OBJCODE refererar till objekttypen. </p> 
     <p>Om formulärets valda objekttyper i ett anpassat formulär inte är kompatibla med ett fält som refereras i ett beräknat anpassat fält, kan du använda jokertecknet för att undvika problemet med att skapa dubbletter för de objekttyperna.</p> 
     <p>I det beräknade anpassade fältet gör du detta genom att ta med jokertecknet i ett IF-uttryck, så att beräkningen kan generera olika värden för vart och ett av formulärets objekttyper. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
