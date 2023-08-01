---
product-area: projects
navigation-topic: manage-tasks
title: Redigera uppgifter
description: Du kan redigera information om åtgärder som du har skapat eller om du har behörighet att göra det i Contribute eller Hantera.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '3712'
ht-degree: 0%

---

# Redigera uppgifter

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


Du kan redigera information om åtgärder som du har skapat eller om du har behörighet att göra det i Contribute eller Hantera.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <ul> 
     <li> <p>Contribute-behörigheter för en uppgift om du vill redigera följande information i området Uppgiftsinformation: </p>
     <ul>
     <li>Beskrivning</li>
     <li>Status</li>
     </ul>  
      </li> 
     <li> <p>Hantera behörigheter för en uppgift för att redigera all information i området Detaljer och i rutan Redigera uppgift</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute eller högre behörighet för projektet</p> </li> 
    </ul> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Begränsningar för redigering av uppgifter

Det finns vissa begränsningar som kan hindra dig från att redigera uppgifter.

Tänk på följande när du redigerar uppgifter:

* När du uppdaterar uppgifter utlöses meddelanden för projekt som har statusen Aktuell. För att undvika förvirring för användare som är tilldelade till aktiviteterna bör du begränsa redigeringsuppgifterna så mycket som möjligt när projektet har statusen Aktuell.
* Du kan inte redigera uppgifter som ingår i en godkännandeprocess. Du kan bara logga tid eller uppdatera status för en aktivitet i en godkännandeprocess.

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* Du kan bara redigera och lägga till dokument i uppgifter i ett projekt som har statusen Fullständigt, Dölj eller Väntar på godkännande när Workfront-administratören eller en gruppadministratör har aktiverat den här funktionen i området Projektinställningar. Mer information om hur du anger projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Du kan alltid redigera följande information för en uppgift när projektet har markerats som Slutfört, Dölj eller pågår i en godkännandeprocess:

   * Loggtid
   * Redigera befintliga utgifter
   * Bifoga ett eget formulär

## Redigera en uppgift i en lista

Du kan redigera aktivitetsinformation i en lista med uppgifter genom att infoga redigeringsfält som visas i vyn för listan.

Mer information om hur du redigerar uppgifter i listor finns i [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## Redigera en uppgift i en lista med hjälp av Sammanfattning

Du kan redigera en uppgift i en lista med hjälp av panelen Sammanfattning. Mer information om hur du redigerar en uppgift i panelen Sammanfattning finns i avsnittet Redigera en uppgift i sammanfattningen i [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) artikel.

## Redigera en uppgift i rutan Redigera uppgift

Du kan redigera en uppgift i området Redigera uppgift eller Uppgiftsinformation. I följande steg beskrivs hur du redigerar en uppgift i rutan Redigera uppgift.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn.

1. Klicka **Projekt** klickar du sedan på namnet på ett projekt för att öppna det.
1. Klicka **Uppgifter** till vänster.
1. Klicka på den uppgift du vill redigera.
1. (Villkorligt) Om du vill redigera begränsad information om en uppgift klickar du på **Uppgiftsinformation** till vänster.

   ![](assets/nwe-task-details-expanded-350x273.png)

   Överväg att redigera information i följande områden i avsnittet Uppgiftsinformation:

   * **Ökning**

     Det här området utökas som standard.

   * **Anpassad Forms**

     Namnen på tullformulär visas bara om det finns anpassade formulär kopplade till objektet.

   * **Ekonomi**

   >[!NOTE]
   >
   >Beroende på hur Workfront-administratören eller gruppadministratören ändrade din layoutmall kan det hända att fälten i området Uppgiftsinformation ordnas om eller inte visas. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Om du vill ha information om de fält som visas i avsnittet Uppgiftsinformation kan du fortsätta redigera uppgiften i rutan Redigera uppgift enligt beskrivningen nedan.

   Så här redigerar du information i detaljavsnittet:

   1. (Valfritt) Klicka på **Komprimera alla** icon ![](assets/collapse-all-icon.png) i det övre högra hörnet om du vill komprimera alla områden.
   1. (Valfritt och villkorligt) När ett område är komprimerat klickar du på **högerriktad pil** ![](assets/right-pointing-arrow.png) bredvid varje område för att expandera området som du vill redigera.
   1. Mer information om hur du redigerar information på fliken Uppgiftsinformation finns i följande artiklar:

      * [Hantera aktivitetsinformation i området Översikt över aktivitetsinformation](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [Hantera aktivitetsfinanser i avsnittet Uppgiftsinformation](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. (Valfritt) Om det inte finns några anpassade formulär kopplade till uppgiften börjar du skriva namnet på ett formulär i **Lägg till anpassat formulär** och sedan markera den när den visas i listan och sedan klicka på **Spara ändringar**.
   1. (Valfritt) Klicka på **Exportera** icon ![](assets/export.png) om du vill exportera översikten och information om anpassade formulär till en PDF-fil, och sedan klicka på **Exportera**. Välj bland följande:

      * Markera alla (visas bara när det finns minst ett anpassat formulär bifogat)
      * Ökning
      * Namnet på ett eller flera anpassade formulär

      PDF-filen hämtas till datorn.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Mer information finns i [Exportera anpassade formulär och objektinformation](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. (Villkorligt) Om du vill redigera all information om uppgiften, som en användare med behörigheten Hantera, klickar du på **Mer** meny ![](assets/more-icon.png) bredvid namnet på uppgiften och klicka sedan på **Redigera**.

   eller

   Välj en uppgift i en lista och klicka sedan på **Redigera** icon ![](assets/edit-icon.png) högst upp i listan.

   Rutan Redigera uppgift öppnas.

   >[!IMPORTANT]
   >
   >Du måste ha behörighet att hantera uppgiften för att kunna se alternativet Redigera.

   Alla uppgiftsfält är tillgängliga i rutan Redigera uppgift och grupperas efter de områden som visas i den vänstra panelen.

   >[!NOTE]
   >
   >Beroende på hur Workfront-administratören eller gruppadministratören ändrade din layoutmall kan det hända att fälten i området Uppgiftsinformation ordnas om eller inte visas. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Det kan vara bra att ange information i följande avsnitt:

   * [Aktivitetsnamn](#task-name)
   * [Ökning](#overview)
   * [Uppdrag](#assignments)
   * [Anpassad Forms](#Custom%C2%A0F)
   * [Ekonomi](#finance)
   * [Inställningar](#settings)

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör eller gruppadministratör konfigurerar vår layoutmall kan det hända att fälten i rutan Redigera uppgift ordnas om eller inte visas. Mer information finns i [Anpassa detaljvyn med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Aktivitetsnamn {#task-name}

1. Börja redigera din uppgift enligt beskrivningen ovan.
1. Klicka **Aktivitetsnamn** till vänster.

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. Uppdatera aktivitetens namn.

1. Klicka **Spara** eller fortsätta med följande avsnitt.

### Ökning {#overview}

1. Börja redigera din uppgift enligt beskrivningen ovan.
1. Klicka **Ökning** till vänster.

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. Uppdatera följande information om uppgiften:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Lägg till ytterligare information om uppgiften. </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Avsnittet Grundinformation</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Välj status för uppgiften som anger vilket utvecklingsstadium aktiviteten befinner sig i.</p> <p><b>TIPS</b>

   Du kan uppdatera aktivitetsstatus i uppgiftshuvudet. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Prioritet</td> 
      <td> <p>Det här är en visuell flagga som gör att du kan prioritera dina uppgifter. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
      <li> <p> Ingen</p> </li> 
      <li> <p> Låg </p> </li> 
      <li> <p>Normal </p> </li> 
      <li> <p>Hög </p> </li> 
      <li> <p> Urgent </p> </li> 
       </ul> <p>Beroende på vilka projektinställningar du har valt av Workfront-administratören kan prioritetsnamnen vara olika för dig. Mer information om uppgiftsprioriteringar finns i <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">Uppdatera aktivitetsprioritet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">Avsnittet Datum och begränsningar för uppgift</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktivitetsbegränsning</td> 
      <td> <p>Bestäm när uppgiften ska slutföras genom att ange en aktivitetsbegränsning. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
      <li> <p><span>Fasta datum</span> </p> <p>Ange en <strong>Planerad start</strong> och <strong>Planerat slutförandedatum</strong>. </p> </li> 
      <li> <p><span>Måste börja på</span> </p> <p>Ange en <strong>Planerat startdatum</strong>. </p> </li> 
      <li> <p><span>Måste avslutas</span> </p> <p>Ange en <strong>Planerat slutförandedatum</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>Så snart som möjligt</span></p> </li> 
      <li> <p><span>Så sent som möjligt</span></p> </li> 
      <li> <p><span>Tidigaste tillgängliga tid</span></p> </li> 
      <li> <p> <span>Senaste tillgängliga tid</span></p> </li> 
      <li> <p><span>Starta senast</span> </p> </li> 
      <li> <p>Ange ett planerat startdatum</p> </li> 
      <li> <p><span>Starta tidigast</span> </p> <p>Ange en <strong>Planerat startdatum</strong>. </p> </li> 
      <li> <p> Slutför <span>Inte senare än</span></p> <p>Ange en <strong>Planerat slutförandedatum</strong>. </p> </li> 
      <li> <p> Slutför <span>Inte tidigare än</span></p> <p>Ange en <strong>Planerat slutförandedatum</strong></p> </li> 
       </ul> <p>Mer information om uppgiftsbegränsning finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bekräfta datum och tid</td> 
      <td> <p>Detta är det datum då användaren som tilldelats uppgiften åtar sig att slutföra den. Detta kan vara ett annat datum än det planerade slutförandedatumet. Endast tilldelningar kan redigera det här fältet. Mer information om implementeringsdatum i Workfront finns i <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Genomför datumöversikt</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerat startdatum och starttid</td> 
      <td> <p>När aktiviteten är planerad att starta. Det planerade startdatumet för en uppgift anges och påverkas av ett antal faktorer:</p> 
       <ul> 
      <li>Beroende på den systemomfattande inställningen för det planerade startdatumet för aktiviteten kan startdatumet för en ny aktivitet i ett projekt antingen vara idag eller startdatumet för projektet som standard. <span>Gruppadministratören för den grupp som är associerad med projektet kan också ange den här inställningen för gruppen.</span> Mer information om aktivitetsinställningar på systemnivå eller gruppnivå finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Konfigurera inställningar för uppgifter och problem i hela systemet</a>.</li> 
      <li>Beroende på vad som föregår uppgiften väljs det planerade startdatumet av Workfront som nästa tillgängliga datum efter att föregående aktiviteter har slutförts, eller startats, beroende på vilket förhållande som föregick aktiviteten. Mer information om föregående relationer finns i <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Översikt över föregående aktiviteter</a>.</li> 
      <li>Projektledaren eller aktivitetsägaren kan manuellt ange det planerade startdatumet när aktivitetsbegränsningen är antingen Fast datum eller Måste starta på. Mer information om uppgiftsbegränsningar finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planerat slutförandedatum och tid</td> 
      <td> <p>Det förväntade slutförandedatumet som visas när aktiviteten är planerad. Det planerade slutförandedatumet kan anges av flera faktorer:</p> 
       <ul> 
      <li>Det planerade slutförandedatumet beräknas från det planerade startdatumet genom att lägga till aktivitetens varaktighet till det planerade startdatumet. När projektledaren eller Workfront anger aktivitetens varaktighet utlöses en uppdatering av det planerade slutförandedatumet. Om det planerade datumet ändras beror det ofta på att tidslängden har uppdaterats.</li> 
      <li>Projektledaren eller aktivitetsägaren kan manuellt ange det planerade slutförandedatumet när aktivitetsbegränsningen är Fast datum eller Måste avslutas den. Mer information om uppgiftsbegränsningar finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a>.</li> 
      <li>Om aktivitetens varaktighetstyp ändras och antalet resurser på aktiviteterna ändras samtidigt, ändras även det planerade slutförandedatumet. Mer information om varaktighetstyper finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktiskt startdatum och -tid</td> 
      <td> <p>Ange ett faktiskt startdatum för aktiviteten. Standardvärdet fylls normalt i automatiskt när du ändrar aktivitetens status till Pågår. Det faktiska startdatumet kan även ändras manuellt av projektledaren eller aktivitetsägaren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Faktiskt slutförandedatum och -tid</td> 
      <td> <p>Ange det faktiska datumet och den faktiska tiden när uppgiften slutförs. Standarddatumet och standardtiden när en uppgift slutförs sammanfaller alltid med den faktiska tiden när statusen blir Slutförd. Det faktiska slutförandedatumet kan även ändras manuellt av projektledaren eller aktivitetsägaren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>Avsnittet Arbetstid</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbetsinsats </td> 
      <td>

   <p>Den mängd arbete som krävs för att slutföra uppgiften. Projektledaren kan välja att använda det här fältet i stället för Planerade timmar för att beräkna hur mycket arbete som krävs för att slutföra en uppgift. Det här fältet är bara synligt när följande villkor är uppfyllda:</p> 
      <ul> 
      <li> <p>Aktiviteten har en enkel varaktighetstyp. </p> <p><b>TIPS</b>

   Om du ändrar uppgiftens varaktighet, tonas det här fältet ned. </p> </li>
   <li>Projektledaren har aktiverat fältet Använd arbetsinsats för att automatiskt beräkna aktivitetsplanerade timmar i projektet. </li> 
      </ul> 
      <p>Välj bland följande alternativ:</p> 
      <ul> 
      <li>Liten</li> 
      <li>Medel <span style="font-weight: normal;">(det här är standardvärdet för en ny uppgift)</span></li> 
      <li>Stor</li> 
      </ul> 
      <p><b>ANMÄRKNING</b>

   Om du uppdaterar mängden arbetsinsats kan aktivitetens planerade timmar uppdateras. Uppdateringen görs omedelbart om projektets uppdateringstyp är Automatisk. När projektets uppdateringstyp är Manuell måste du beräkna om tidslinjen för att se de uppdaterade planerade timmarna. </p>

   <p>Mer information om hur du använder Arbetsinsats i stället för Planerade timmar för att beräkna aktivitetsinsats finns i <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Översikt över arbetsinsats</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara** eller fortsätta med följande avsnitt.

### Uppdrag {#assignments}

1. Börja redigera din uppgift enligt beskrivningen ovan.
1. Klicka **Uppdrag** till vänster.

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. Klicka **Sök efter personer, roller och team** och börja skriva namnet på en användare, roll eller team som du vill tilldela uppgiften och klicka sedan på den eller tryck på Retur när den visas i listan.

   >[!NOTE]
   >
   >Om användarens namn innehåller ett specialtecken måste du inkludera specialtecknet i sökfältet.

   >[!TIP]
   >
   >Du kan tilldela flera användare, jobbroller eller team. Du kan bara tilldela aktiva användare, jobbroller och team.
   >
   >Om en användare, jobbroll eller ett team tilldelades innan de inaktiverades, förblir de tilldelade till arbetsuppgiften. I det här fallet rekommenderar vi följande:
   >
   >* Tilldela om arbetsuppgiften till aktiva resurser.
   >* Associera användarna i ett inaktiverat team med ett aktivt team och omfördela arbetsposten till det aktiva teamet.

1. (Valfritt) Ange om en tilldelad är den primära tilldelaren för uppgiften genom att välja **Ägare** alternativknapp bredvid deras namn. Ett team kan inte vara den primära tilldelaren för en uppgift.
1. (Villkorligt och valfritt) Uppdatera följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Varaktighetstyp</td> 
      <td> <p>Detta identifierar relationen mellan följande: </p> 
       <ul> 
      <li> <p>Antalet resurser som tilldelats en aktivitet </p> </li> 
      <li> <p>Den totala arbetsinsats som krävs för att slutföra uppgiften </p> </li> 
      <li> <p> Aktivitetens totala varaktighet. </p> </li> 
       </ul> <p>Din Workfront-administratör <span> eller en gruppadministratör</span> väljer standardinställningen för varaktighetstyp för aktiviteterna i systemet eller gruppen. Mer information om hur du anger standardinställningar för projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>. </p> <p>Med varaktighetstyper kan du ange konsekventa resurstilldelningar baserat på uppgiftens behov. Mer information om varaktighetstypen för en uppgift finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
      <li> <p>Beräknad tilldelning </p> </li> 
      <li> <p> Beräknat arbete </p> </li> 
      <li> <p>Ansträngningsstyrd </p> </li> 
      <li> <p>Enkel</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">Varaktighet per förekomst</td> 
      <td> <p>Detta visas endast på den överordnade för återkommande uppgifter. Den visar varaktigheten för varje återkommande uppgift, enligt definition när uppgiften skapades. Mer information om hur du skapar återkommande uppgifter finns i <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Skapa återkommande uppgifter</a>. </p> <p> <b>ANMÄRKNING</b>

   Varaktigheter som ändras i enskilda återkommande aktiviteter visar inte det värde som anges i det här fältet. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Varaktighet</td> 
      <td> 
      <div> 
      <div> 
      <p>Det här är den tid som du tillåter att en uppgift förblir öppen innan den är slutförd. </p> 
      <p><b>VIKTIGT</b>

   Eftersom aktivitetens varaktighet vanligtvis är tiden mellan planerad start och planerad slutförandetid, påverkar det tidslinjen för projektet.</p>

   <p>Så här anger du aktivitetens varaktighet och tidsenhet:</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Skriv in tidslängden och välj en tidsenhet i listrutan.</p> <p><b>TIPS</b></p>
      När du uppdaterar varaktigheten för uppgifter i en uppgiftslista kan du använda förkortningen för tidsenheten. </p> </li> 
      </ul> 
      <p> Du kan välja mellan alternativen för normal tid eller förfluten tid i följande tabell: </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>Tidsenhet</td> 
      <td>Förkortning</td> 
      </tr> 
      <tr> 
      <td>Minuter</td> 
      <td>M</td> 
      </tr> 
      <tr> 
      <td>Timmar</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>Dagar. Det här är standardinställningen. </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>Veckor</td> 
      <td>B</td> 
      </tr> 
      <tr> 
      <td>Månader</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>Förflutna minuter</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>Förflutna timmar</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>Förflutna dagar</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>Förflutna veckor</td> 
      <td>FV</td> 
      </tr> 
      <tr> 
      <td>Förflutna månader</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>ANMÄRKNING</b>

   <p>Förfluten tid är en tidsenhet för en uppgifts varaktighet. Det är tiden mellan det planerade startdatumet och det planerade slutförandedatumet för en aktivitet som omfattar helger, helger och ledig tid. Med andra ord är förfluten tid en del av kalenderdagarna.

   Med normal tid räknas helger, helger och ledig tid som undantag från uppgiftens varaktighet. Mer information om aktivitetens varaktighet finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Planerade timmar</td> 
   <td> <p>Ange antalet planerade timmar för aktiviteten i timmar. Detta är den faktiska tid det skulle ta för uppgiftens tilldelare att slutföra den. Du kan bara ange antalet planerade timmar för en aktivitet när varaktighetstypen är inställd på Beräknad tilldelning. Mer information om varaktighetstyper finns i <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Översikt över aktivitetsvaraktighet och varaktighetstyp</a>.</p> 
   <b>ANMÄRKNING</b>
   <p>
   När du skapar återkommande uppgifter är de planerade timmarna för varje förekomst. De planerade timmarna för de överordnade uppgifterna är det totala antalet planerade timmar från alla förekomster. Mer information om hur du skapar återkommande uppgifter finns i <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Skapa återkommande uppgifter</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Allokering</td> 
   <td> <p>Om uppgiftsbegränsningen är Beräknad arbets- eller insatsstyrd anger du <strong>Allokering %</strong> (tilldelningsprocent) för varje tilldelad. Det här är den tid från schemat för den tilldelande personen som de kan lägga på den här aktiviteten. Om du ändrar allokeringsprocenten för en tilldelad ändrar du planerad tid för en uppgift. </p> <p>När aktivitetsbegränsningen är enkel kan du ange följande:</p> 
      <ul> 
      <li> <p>Allokeringstimmar för varje tilldelad.</p> </li> 
      <li> <p>Planerade timmar för uppgiften</p> </li> 
      <li> <p>Uppgiftens varaktighet</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">Uppdragarens roll</td> 
   <td> <p>Välj en roll från <strong>Uppdragarens roll</strong> när du har valt en person som tilldelad. Detta är den roll som den som tilldelas kan utföra den här uppgiften. </p> <p><b>TIPS</b>

   Endast de jobbroller som är kopplade till varje tilldelad i deras profil visas i listrutan.</p> </td>
   </tr> 
      </tbody> 
      </table>

1. Klicka **Spara** eller fortsätta med följande avsnitt.

### Anpassad Forms

Du kan definiera anpassade standardformulär som automatiskt ska kopplas till uppgifter när uppgifterna läggs till i ett projekt. Mer information om hur du ställer in projektet så att det innehåller anpassade formulär för standarduppgifter för alla nya uppgifter finns i avsnittet Åtgärder i artikeln [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Börja redigera uppgiften enligt beskrivningen ovan.
1. Klicka **Anpassad Forms** i den vänstra panelen eller klicka på namnet på ett anpassat formulär om det redan är kopplat.

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. Klicka **Lägg till anpassat formulär** och välj det eller de anpassade formulär som du vill associera med uppgiften. Du måste skapa anpassade formulär innan de kan väljas i det här fältet. Endast aktiva anpassade formulär visas i listan.

   Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)Du kan lägga till upp till tio anpassade formulär i en uppgift.

1. (Villkorligt) Om du har kopplat ett anpassat formulär till uppgiften kan du redigera alla fält i formuläret. Du måste ange alla obligatoriska fält innan du kan spara uppgiften.

   >[!NOTE]
   >
   >Beroende på hur din Workfront-administratör anger behörigheter för avsnitten i ditt anpassade formulär kan inte alla visa eller redigera samma fält i ett visst anpassat formulär. Behörigheterna att redigera fält i ett avsnitt i ett anpassat formulär beror på vilka behörigheter du har för själva uppgiften. Mer information om hur du anger aktivitetsbehörigheter finns i [Dela en uppgift](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. Klicka **Spara** eller fortsätta med följande avsnitt.

### Ekonomi {#finance}

1. Börja redigera din uppgift enligt beskrivningen i [Redigera uppgifter](#Edit2) i den här artikeln.
1. Klicka **Ekonomi** till vänster.

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. Uppdatera följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostnadstyp</td> 
      <td> <p>Ange uppgiftens kostnadstyp. Detta avgör hur kostnaden för uppgiften beräknas, baserat på antalet timmar för uppgifterna. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
        <li> <p>Ingen kostnad</p> </li> 
        <li> <p>Fast en timme </p> </li> 
        <li> <p> Användare per timme </p> </li> 
        <li> <p> Roll timvis</p> </li> 
       </ul> <p>Mer information om att hålla reda på kostnaderna finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a> . Workfront-administratören eller en gruppadministratör väljer standardinställningen för kostnadstyp för uppgifterna i ditt system eller din grupp. Mer information om hur du anger standardinställningar för projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intäktstyp</td> 
      <td> <p>Ange uppgiftens intäktstyp. Det här avgör hur Intäkten för uppgiften beräknas, baserat på antalet timmar för uppgifterna. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
      <li> <p> Ej fakturerbar </p> </li> 
      <li> <p>Användare per timme </p> </li> 
      <li> <p>Roll timvis </p> </li> 
      <li> <p>Fast en timme </p> </li> 
      <li> <p>Användartimme med versaler </p> </li> 
      <li> <p>Roll timvis med ändpunkt </p> </li> 
      <li> <p>Användarens timma plus fast </p> </li> 
      <li> <p>Roll timvis plus fast </p> </li> 
      <li> <p>Fast intäkt </p> </li> 
       </ul> <p>Mer information om att spåra intäkter finns i<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkt</a> . </p> <p>Din Workfront-administratör eller gruppadministratör väljer standardinställningen för Intäktstyp för uppgifterna i ditt system eller din grupp. Mer information om hur du anger standardinställningar för projekt finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurera systemomfattande projektinställningar</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara** eller fortsätta med följande avsnitt.

### Inställningar {#settings}

1. Börja redigera din uppgift enligt beskrivningen i [Redigera uppgifter](#Edit2) i den här artikeln.
1. Klicka **Inställningar** till vänster.

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. Uppdatera följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Spårningsläge</td> 
      <td> <p>Ange hur aktivitetens förloppsstatus ska spåras. </p> <p>Välj bland följande alternativ: </p> 
       <ul> 
      <li> <p> Användaren måste uppdatera </p> </li> 
      <li> <p>Anta i tid </p> </li> 
      <li> <p>Ignorera sena varningar</p> </li> 
      <li> <p> Komplettera automatiskt </p> </li> 
      <li> <p>Föregående </p> </li> 
       </ul> <p>Mer information om spårningsläget för uppgifter finns i <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Översikt över läget Uppgiftsspårning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resursutjämning</td> 
      <td> <p>Välj <strong>Exkludera från resursutjämning</strong> om du vill att de resurser som tilldelats aktiviteten ska uteslutas från utjämning.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Levelingfördröjning</td> 
      <td> <p>Ange nivåfördröjning i timmar. </p> <p> Mer information om fördröjning av utjämning finns i <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">Uppdatera nivåfördröjning för aktivitet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännandeprocess</td> 
      <td> <p>Välj en godkännandeprocess som du vill associera med uppgiften. Workfront-administratören måste definiera godkännandeprocesser på systemnivå innan du kan koppla dem till uppgifter. En användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser. </p> <p>Mer information om hur du skapar godkännandeprocesser finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">Skapa en godkännandeprocess för arbetsobjekt</a>. Tänk på följande när du lägger till godkännandeprocesser: </p> 
       <ul>

   <li> <p>Endast aktiva godkännandeprocesser visas i listan. </p> </li>

   <li> <p>Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. En godkännandeprocess som är associerad med en annan grupp än den som projektet har visas inte i listan. </p>

   <p><b>VIKTIGT</b>

   Om projektgruppen ändras blir den tidigare bifogade gruppspecifika godkännandeprocessen en godkännandeprocess för enstaka användning. Mer information om hur ändringar i projektgruppen eller i godkännandeprocessen påverkar godkännandeinställningarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Hur ändringar i gruppering och godkännandeprocess påverkar tilldelade godkännandeprocesser</a>. </p>

   </li>

   <li> <p>Du kan definiera standardgodkännandeprocesser som automatiskt kopplas till uppgifter när uppgifterna läggs till i ett projekt. Mer information om hur du ställer in projektet så att det omfattar standardprocesser för godkännande av uppgifter finns i avsnittet Åtgärder i artikeln <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Redigera projekt</a>. </p> </li>

   <li> <p>Följande scenarier finns när gruppredigeringsuppgifter utförs: </p> 
      <ul> 
      <li> <p>När du väljer flera uppgifter från samma grupp visas både godkännandeprocesser på systemnivå och på gruppnivå i det här fältet. </p> </li> 
      <li> <p>När du väljer flera uppgifter från olika grupper visas endast godkännandeprocesser på systemnivå i det här fältet. </p> </li> 
      <li> <p>När någon av uppgifterna har en enda godkännandeprocess, ersätts den av den process på system- eller gruppnivå som du väljer. </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. Klicka **Spara**.

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## Redigera en uppgift i uppgiftshuvudet (begränsat)

Du kan redigera en begränsad mängd information i uppgiftshuvudet.

Systemadministratören eller gruppadministratören kan anpassa fälten som visas i uppgiftshuvudet. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

Följande fält inkluderas som standard i projektrubriken:

* Uppgiftsnamn
* Procent färdigt
* Uppdrag
* Planerat slutförandedatum och tid

  >[!CAUTION]
  >
  >Vissa aktivitetsbegränsningar och andra beroenden kan hindra dig från att redigera det här fältet. Mer information om uppgiftsbegränsningar finns i [Översikt över uppgiftsbegränsning](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Status
* Fatta godkännandebeslut om du har angett som godkännare i en aktuell godkännandeprocess

## Redigera flera uppgifter samtidigt

Du kan redigera flera uppgifter samtidigt i en lista och uppdatera all information om dem samtidigt när du väljer att automatiskt spara de ändringar du gör i uppgifterna i listan.

Mer information om att spara flera uppgifter samtidigt finns i avsnittet Redigera uppgifter gruppvis i artikeln [Redigera uppgifter i en lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
