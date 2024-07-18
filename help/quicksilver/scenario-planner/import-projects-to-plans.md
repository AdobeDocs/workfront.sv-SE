---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importera projekt till planer i scenarioplaneraren
description: Du kan importera befintliga projekt till en plan. De importerade projekten omvandlas till initiativ och du kan hantera dem i planen på samma sätt som du hanterar ett nytt projekt. Det ursprungliga projektet är fortfarande kopplat till det nya initiativet.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1625'
ht-degree: 0%

---

# Importera projekt till planer i [!DNL Scenario Planner]

Du kan importera befintliga projekt till en plan. De importerade projekten omvandlas till initiativ och du kan hantera dem i planen på samma sätt som du hanterar ett nytt projekt. Det ursprungliga projektet är fortfarande kopplat till det nya initiativet.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] eller högre</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licens*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till de funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du hämtar [!DNL Workfront Scenario Planner] finns i <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst som behövs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Åtkomstnivåkonfigurationer*</strong> </td> 
   <td> <p>[!UICONTROL Edit] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i scenarioplanen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du importerar projekt till planer som nya initiativ

* Du måste skapa projekt innan du kan importera dem till en plan som nya initiativ.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Du måste ha minst [!UICONTROL View] behörigheter för projekten för att kunna importera dem till en plan som ett nytt initiativ.
* Du kan importera samma projekt till flera planer.
* De projekt du vill importera måste ha datum i tidsplanen. Du kan inte importera projekt med en [!UICONTROL Planned Completion Date] tidigare än planens början eller en [!UICONTROL Planned Start Date] senare än planens slut.
* Du kan inte importera mer än 100 projekt åt gången.
* Viss projektinformation importeras också till planen och blir initiativinformation. Mer information om vilken projektinformation som importeras till planen och som blir initiativinformation finns i avsnittet [Projektinformation som importeras till planen](#project-information-imported-into-the-plan) i den här artikeln.
* Ändringar som görs i de länkade projekten påverkar inte initiativen i planen.
* De ändringar som görs i projekten påverkar inte automatiskt de länkade projekten Ändringar i Initiativfunktionen påverkar bara de länkade projekten när du publicerar initiativet från planen. Mer information om hur publiceringsinitiativen påverkar de länkade projekten finns i [Uppdatera eller skapa projekt genom att publicera initiativen i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* Om du tar bort ett projekt som har skapats genom att ett projekt importeras tas inte projektet bort.
* Initiativet tas inte bort om ett projekt som är kopplat till ett initiativ tas bort.

## Projektinformation som importerats till planen {#project-information-imported-into-the-plan}

När du importerar ett projekt till en plan importeras viss projektinformation också till planen och den blir initialinformation. Tabellen nedan visar vilken projektinformation som blir initiativinformation när du importerar ett projekt till en plan:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Projektinformation</td> 
   <td>Initiativinformation </td> 
  </tr> 
  <tr> 
   <td>Projektnamn</td> 
   <td>Initiativnamn</td> 
  </tr> 
  <tr> 
   <td>Planerade datum för projekt</td> 
   <td> <p>Start- och slutmånader för initiativet.</p> <p>Om ett projekt börjar eller slutar mitt i en månad förlängs de importerade datumen till att omfatta en hel månad i planen. Om Project Plananned Dates till exempel är 20 mars-5 maj 2020 är datumet för det importerade initiativet mars-maj 2020.</p> <p>Om det planerade start- eller slutförandedatumet ligger utanför planens varaktighet finns det en visuell indikation på att det importerade initiativet börjar före eller slutar efter planen. </p> </td> 
  </tr> 
  <tr> 
   <td>Jobbroller som tilldelats aktiviteter och ärenden</td> 
   <td> <p>Initiera befattningsroller. </p> <p>Obs!   <p>Om en användare ändrar roller under projektets livslängd beror de roller som importeras på uppdragets status när du importerar projektet. Följande scenarier finns:</p> 
     <ul> 
      <li> <p>Om en användare som har tilldelats en aktivitet eller ett problem har ändrat sin roll efter att de har markerat sin tilldelning som [!UICONTROL Done], importerar [!DNL Workfront] till initiativet som användaren fullgjorde innan han/hon markerade tilldelningen som [!UICONTROL Done].</p> </li> 
      <li> <p>Om en användare som har tilldelats en aktivitet eller en utgåva ändrade rollen under projektets livstid, men deras tilldelning för aktiviteten eller utgåvan inte är markerad som [!UICONTROL Done] när du importerar projektet, importerar [!DNL Workfront] bara den aktuella rollen för den tilldelade användaren. </p> </li> 
     </ul> <p>Mer information om status för ett uppdrag finns i Tilldelningsstatus i <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Ordlista i Adobe [!DNL Workfront] -terminologi</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt [!UICONTROL Planned Hours] som är associerat med jobbroller som har tilldelats aktiviteter eller ärenden</td> 
   <td> <p><span>Beroende på om planen är konfigurerad att använda FTE eller timmar blir [!UICONTROL Planned Hours] från aktiviteterna i projektet antingen </span> [!UICONTROL Required FTEs] <span> eller [!UICONTROL Required hours] i planen</span>. </p> <p>Mer information om hur du konfigurerar en plan för att använda FTE eller timmar finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i [!DNL Scenario Planner]</a>. </p> <p>Tänk på följande:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] använder de jobbroller som tilldelats uppgifter och ärenden eller de jobbroller som användarna tilldelade uppgifter eller ärenden är kopplade till i projektet och överför dem till det nya initiativet som obligatoriska jobbroller. </p> </li> 
     <li> <p>När planen är konfigurerad för att använda heltidsanställda konverteras de planerade timmarna som är kopplade till jobbrollerna för aktiviteterna och problemen i projektet först till heltidsanställda. Därefter tilldelas denna heltidsanställd en roll för initiativet. <span>Planerade timmar fördelas jämnt i [!DNL Workfront]. Om en aktivitet eller ett ärende sträcker sig över flera månader kommer antalet planerade timmar för varje månad under initieringens varaktighet att räknas om till månadsvis heltidsanställd och överföras till varje månad.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><span>Om en aktivitet till exempel tilldelas en jobbroll för 80 planerade timmar i september, visar den importerade jobbrollen 0,5 heltidsanställda för initiativet i september.</span> </p> </li> 
     <li> <p>[!DNL Workfront] beräknar heltidsanställd personal för de obligatoriska befattningsroller som är kopplade till initiativet med hjälp av följande formel:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Tips! [!DNL Scenario Planner] förutsätter att det finns 160 arbetstimmar per månad.</p> <p>Om ett projekt till exempel har en varaktighet på 1 200 minuter och en jobbroll för projektet är associerad med 600 minuters planerade timmar, är deras heltidsanställda 0,5. Vid import av projektet är den obligatoriska jobbrollen FTE för det nyskapade initiativet 0,5 för varje månad. </p> </li> 
     <li>När en jobbroll tilldelas till en aktivitet i projektet med noll planerade timmar är den begärda heltidsanställda för projektets jobbroll noll som standard. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>När en jobbroll tilldelas till en aktivitet i projektet med noll [!UICONTROL Duration] är den begärda FTE <span> eller timmar </span> för projektets jobbroll som standard noll, även om aktiviteten har Planerade timmar. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Importera projekt till en plan

>[!IMPORTANT]
>
>När du har importerat projekt till en plan blir de initiativ i planen. Även om de två objekten är länkade finns de som fristående enheter och påverkar inte automatiskt varandra när de uppdateras.
>
>Följande inträffar:
>
>* Ändringar i projektet påverkar aldrig initiativet efter att du har importerat projektet till planen. De här ändringarna inkluderar ändringar av rollallokeringarna för jobb.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Ändringar i initiativet påverkar bara informationen i projektområdet [!DNL Scenario Planner] när du publicerar initiativet till motsvarande projekt. Annars påverkar de inte [!UICONTROL Planned Hours]-informationen för aktiviteterna och problemen i projektet.
>
>  Mer information om hur publiceringsinitiativen påverkar de länkade projekten finns i [Uppdatera eller skapa projekt genom att publicera initiativen i scenarioplanen](../scenario-planner/publish-scenarios-update-projects.md).
>

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Workfront] och klicka sedan på [!DNL Scenarios] för att komma åt [!DNL Scenario Planner].

1. Klicka på namnet på en plan där du vill importera projekt.
1. Klicka på **[!UICONTROL New Initiative]** och sedan på **[!UICONTROL Import Projects]**.

   Rutan [!UICONTROL Import Projects] visas. Projekt som har datum inkluderade i tidsramen för din plan visas i en lista.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Projekt oavsett status visas i listan.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Valfritt) Klicka på **[!UICONTROL Filter icon]** ![](assets/filter-nwepng.png) och välj ett tillgängligt filter i listan för att minska antalet projekt i listan. Som standard filtreras projektlistan efter användarens aktuella projektfilter i en lista med projekt.

1. (Valfritt) Klicka på **[!UICONTROL Search icon]** ![](assets/search-icon.png) och lägg till ett nyckelord som visas i valfritt fält på skärmen. Objekten som innehåller sökordet visas automatiskt i listan och alla objekt döljs.

1. (Villkorligt) Klicka på **[!UICONTROL X icon]** för att ta bort sökningen och visa alla projekt.
1. Välj upp till 100 projekt och klicka på **[!UICONTROL Import]**.

   Projekten importeras som nya initiativ.

   Observera följande:

   * En projektikon ![](assets/project-icon-sp.png) visas till höger om företagsnamnet.
   * Om projekttidslinjen överskrider planens varaktighet, avslutas aktivitetsfältet med en spetsig marginal till vänster (när startdatumet är tidigare än planens datum) eller till höger (när slutdatumet är senare än planens datum).

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Antalet månader och jobbroller har uppdaterats för att matcha projektets.

   >[!TIP]
   >
   >Kostnaderna i samband med jobbrollerna uppdateras på initiativnivå och importeras inte från projektet.

1. Klicka på den stapel som representerar det nya initiativet för att öppna panelen med information om initiativ till höger.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Granska följande information i området **[!UICONTROL Initiative Duration]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Duration]</td> 
      <td>Detta är den tid som initiativet kommer att pågå i månader. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Initiativets start- och slutdatum. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Project]</td> 
      <td> <p>Det länkade projektets [!UICONTROL Planned Start] och [!UICONTROL Completion dates].</p> <p>Tips! Om [!UICONTROL Project]-informationen saknas har projektet tagits bort.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Redigera namnet på initiativet. Som standard matchar den namnet på projektet.
1. (Valfritt) Gör något av följande:

   * Uppdatera jobbroller i avsnittet **[!UICONTROL Required Job Roles]**
   * Uppdatera **[!UICONTROL Fixed Costs]** i avsnittet **[!UICONTROL Costs]**

   * Klicka på **[!UICONTROL Update available job roles]** eller **[!UICONTROL Update available budget]** för att lösa konflikter mellan det nya initiativet och andra initiativ i planen.

1. (Villkorligt) Klicka på **[!UICONTROL Apply]** om du vill spara ändringarna i ditt initiativ.
1. Klicka på **[!UICONTROL Save Plan]** om du vill spara ändringarna i din plan.
1. (Valfritt) Om du vill uppdatera ändringarna du gör i det projekt som det har importerats från tillbaka till publicerar du projektet från planen. Mer information om publiceringsplaner finns i [Uppdatera eller skapa projekt genom att publicera initiativen i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Valfritt) Klicka på projektikonen för att komma åt det länkade projektet.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
