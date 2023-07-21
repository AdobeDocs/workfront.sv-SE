---
content-type: overview
product-area: projects
navigation-topic: manage-projects
title: Hantera information i projektöversiktsområdet
description: Hantera information i projektöversiktsområdet
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6113bc62-18f2-4558-bc2f-986b1e7d1a83
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 0%

---

# Hantera information i projektöversiktsområdet

<!--
<p>(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Du kan visa eller redigera information om ett projekt genom att gå till området Översikt i avsnittet Projektinformation. Det finns ett begränsat antal fält som du kan visa eller redigera i det här området. Mer information om hur du redigerar all information för ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront-licens*</p> </td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst till projekt eller högre</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till projektet eller högre</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Öppna avsnittet Översikt

1. Gå till det projekt vars översiktsavsnitt du vill visa.
1. Klicka **Projektinformation** i den vänstra panelen.
1. The **Översikt** -avsnittet ska visas först som en del av projektinformationen och ska expanderas som standard

   eller

   Klicka på **Redigera** icon ![](assets/edit-icon.png) i det övre högra hörnet av detaljavsnittet och klicka sedan på **Översikt**. Då öppnas området Översikt för redigering.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör har konfigurerat layoutmallen kanske inte översiktsavsnittet visas först, och då komprimeras det. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Villkorligt) Om det finns ett specifikt fält som behöver uppdateras i ett projekt men inte visas i det här avsnittet, klickar du på **Menyn Mer** ![](assets/more-icon.png) bredvid projektnamnet, och **Redigera** om du vill visa fler projektfält.

   Mer information om hur du redigerar projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Redigera eller granska fälten i tabellen nedan som visas i **Översikt** -avsnitt.\
   Om du vill redigera ett fält som är tillgängligt för redigering klickar du på fältet eller klickar **+Lägg till** om du vill lägga till information i ett tomt fält.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör har konfigurerat din layoutmall kanske inte alla fält visas. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader"><b>Fält</b></td> 
      <td><b>Beskrivning</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Beskriv syftet med det här projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>Infoga en URL i det här fältet. Det kan vara en Workfront-URL eller någon annan. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioritet</td> 
      <td>Fungerar som angiven prioritet eller prioritet för projektet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Projektstatus. </p> <p>Tips: Du kan inte slutföra ett projekt om inte alla aktiviteter och ärenden också har slutförts. Om du har valt Automatiskt för Projektets slutföringsläge går det inte att slutföra ett projekt manuellt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Villkorstyp</td> 
      <td>Avgör om projektledaren ställer in villkoret för projektet eller om Workfront gör det. Mer information om projektvillkor finns i artikeln <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Översikt över projektvillkor och villkorstyp</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schemaläge</td> 
      <td>Anger hur projektet schemaläggs. Om projektet till exempel är schemalagt från Startdatum eller från Slutförandedatum. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerat startdatum och starttid</td> 
      <td> När projektet planeras att starta. Detta anges manuellt av projektledaren när projektet är schemalagt från startdatum. Workfront anger automatiskt detta datum när projektet schemaläggs från Slutförandedatum, baserat på varaktigheten för aktiviteterna i projektet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerat slutförandedatum och tid</td> 
      <td> När projektet är planerat att slutföras. Detta anges manuellt av projektledaren när projektet schemaläggs från slutförandedatum. Workfront anger automatiskt detta datum när projektet schemaläggs från startdatum, baserat på varaktigheten för aktiviteterna i projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Portfolio</td> 
      <td>Den portfölj som är associerad med projektet. Du måste skapa portföljen innan du kan lägga till den i ett projekt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Program</td> 
      <td>Det program som är associerat med projektets portfölj. Du måste skapa programmet innan du kan lägga till det i ett projekt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupp</td> 
      <td> <p>Gruppen som är associerad med projektet.</p> <p>Du kan kontrollera att du markerar rätt grupp genom att hålla markören över den och klicka på informationsikonen <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
      Som standard kopplas en av följande grupper automatiskt till ett projekt när det skapas, såvida du inte anger en annan grupp:
        <ul> 
         <li> <p><span>När projektet skapas från projektområdet kopplas den som skapat projektet till hemgruppen.</span> </p> </li> 
         <li> <p><span>När projektet skapas från en grupps huvudsida i inställningsområdet kopplas gruppen automatiskt till projektet.</span> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Företag</td> 
      <td>Det företag som är associerat med projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projektägare </td> 
      <td>Detta är ägaren till projektet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projektsponsorer</td> 
      <td> <p>Detta är den främsta intressenten för projektet. Detta är vanligtvis en verkställande direktör som övervakar och leder projektet, eller det är den person som har budgetansvar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resurshanteraren</td> 
      <td> <p>Det här är den person som kan hantera användarresurser i projektet. </p> <p>Mer information om Resurshanterare finns i artikeln <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">Ange resurshanterare för ett projekt eller en mall </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >När du uppdaterar fälten Projektägare, Projektsponsor och Resurshanterare ska du lägga märke till avataren, användarens primära roll eller deras e-postadress för att skilja mellan användare med identiska namn.
   >
   >Användarna måste vara associerade med minst en jobbroll för att kunna visa den när du lägger till dem.
   > 
   >Du måste ha inställningen Visa kontaktinformation aktiverad på din åtkomstnivå för att användare ska kunna visa användarnas e-postmeddelanden. Mer information finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. Granska följande fält i avsnittet Översikt. Du kan inte redigera följande fält:

   | Fält | Beskrivning |
   |---|---|
   | Referensnummer | Det här är ett automatiskt genererat fält och har alltid ett unikt värde för varje projekt. |
   | Planerat startdatum | Detta är ett&quot;realtidsdatum&quot; som anger när arbetet ska börja baserat på slutfört arbete och återstående arbete. |
   | Planerat slutförandedatum | Detta är ett&quot;realtidsdatum&quot; för när projektet ska slutföras baserat på förloppet för slutförda uppgifter och baserat på förloppsuppdateringarna för de uppgifter som är antingen Ny eller Pågår. |
   | Planerade timmar | Planerade timmar för projektet. De här timmarna är det totala antalet planerade timmar för varje uppgift. |
   | Faktiska timmar | Timmar som är inloggade på projektet. De här timmarna är det totala antalet loggade timmar i projektet, aktiviteterna eller problemen i projektet. |
   | Planerad varaktighet | Den tid som projektet kommer att spänna över, baserat på tidsramen mellan det tidigaste planerade startdatumet för en aktivitet och det senaste planerade slutdatumet för en aktivitet i projektet. |
   | Faktisk varaktighet | Den tid som projektet i själva verket sträcker sig över, baserat på tidsramen mellan det tidigaste faktiska startdatumet för en aktivitet och det senaste faktiska slutförandedatumet för en aktivitet i projektet. |
   | Anmälningsdatum | Datum och tid då projektet skapades. |
   | Anges av | Namnet på den användare som skapade projektet. |
   | Senaste uppdateringsdatum | Datum och tid då projektet senast uppdaterades. |
   | Senast uppdaterad av | Namnet på den användare som senast uppdaterade projektet. |
   | Mall |   |


1. Om ditt företag har köpt ytterligare en licens för Adobe Workfront Scenario Planner och projektet innehåller information som publicerats från ett länkat initiativ kan du läsa följande information i Scenarioplaneringsområdet:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>Fält</b></td> 
      <td><b>Beskrivning</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader"><span>Initiativvaraktighet</span> </td> 
      <td><span>varaktigheten för motsvarande initiativ när projektet är kopplat till ett initiativ. Det här fältet kan inte redigeras.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Senast publicerat den</span> </td> 
      <td><span>Det datum då projektet senast offentliggjordes från ett motsvarande initiativ.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Startdatum för projekt</span> </td> 
      <td><span>Den första dagen i startmånaden för initiativet, när projektet är kopplat till ett initiativ.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Startdatum för projektet</span> </td> 
      <td><span>Den sista dagen i programmets slutmånad, när projektet är kopplat till ett initiativ. </span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Initiera befattningsroller inom heltidsanställda och timmar</span> </td> 
      <td> <p>Information om associerade jobbroller och deras tidsfördelningar för initiativet. Detta omfattar följande:</p> 
       <ul> 
        <li>Jobbrollsnamn</li> 
        <li>Antal heltidsanställda</li> 
        <li> <p>Antal timmar för alla heltidsanställda</p> <p>Du kan beräkna antalet jobbroller som behövs för din plan eller ditt initiativ med hjälp av timmar eller heltidsanställda. </p> <p>Mer information finns i <a href="../../../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplaneraren</a>. </p> </li> 
       </ul> <p>Tips: <span>Om antalet befattningar är olika för varje månad i initiativet visas det maximala antalet roller som krävs för initiativet i det här fältet. Om du till exempel behöver en konsult för januari och 2 för februari, visar kolumnen 2 heltidsanställda och motsvarande antal timmar för 2 heltidsanställda för alla månader.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Mer information om hur du länkar projekt till initiativ finns i [Uppdatera eller skapa projekt genom att publicera initiativ i Scenarioplanen](../../../scenario-planner/publish-scenarios-update-projects.md).

1. Klicka **Spara ändringar**.
