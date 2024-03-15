---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Lägga till ett anpassat fält i ett anpassat formulär med det äldre formulärverktyget
description: När du arbetar med ett anpassat formulär kan du skapa ett nytt anpassat fält och lägga till det i ett anpassat formulär. Du kan också lägga till ett anpassat fält som redan har lagts till i ett annat anpassat formulär.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '2327'
ht-degree: 0%

---

# Lägga till ett anpassat fält i ett anpassat formulär med det äldre formulärverktyget

<!-- Audited: 02/2024 -->

När du arbetar med ett anpassat formulär kan du skapa ett nytt anpassat fält och lägga till det i ett anpassat formulär.

Du kan också lägga till ett anpassat fält som redan har lagts till i ett annat anpassat formulär. Instruktioner finns i [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Mer information om hur du lägger till en resurswidget i ett anpassat formulär, vilket är en process som liknar hur du lägger till ett anpassat fält, finns i [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>I ett anpassat formulär som innehåller många anpassade fält eller många alternativ för att markera flera i anpassade fält, kan användare uppleva sämre prestanda när de lägger till eller ändrar värden i dessa fält. Ett formulär som innehåller till exempel 100 anpassade fält, eller anpassade fält som innehåller flera markeringar med fler än 200 alternativ, kan ta längre tid när användarna interagerar med det.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Administrativ åtkomst till anpassade formulär </td> 
  </tr>  
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Lägga till ett anpassat fält i ett anpassat formulär {#add-custom-field-to-custom-form}

1. Börja skapa eller redigera ett anpassat formulär, enligt beskrivningen i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Välj **Lägg till ett fält** -fliken.

   ![Lägg till en fältflik](assets/add-a-field.jpg)

1. Med **Nytt fält** ![Ikonen Nytt fält](assets/new-field.jpg) väljer du någon av följande fälttyper:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Textfält med en rad</td> 
      <td>Tillåter användare att skriva en enda textrad i fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Textfält för stycke</td> 
      <td>Tillåter användare att skriva flera textrader i fältet.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Textfält med formatering</td> 
      <td>Används för att skriva flera textrader i fältet och formatera texten med fet, kursiv stil, understrykning, punkter, numrering, hyperlänkar och blockcitattecken. Det här är tillgängligt i Hem, uppdateringsområdet, listorna och detaljområdet för Workfront-objekt. En teckengräns på 15 000 tillåter mycket text och formatering.</p> <p>Den här anpassade fälttypen stöds inte i filter för listor och rapporter.</p> <p>Mer information om hur du kommer åt det här fältet via API:t finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">RTF-fältslagring i API</a>.</p> <p><b>ANMÄRKNING</b>: Textfält med formatering är inte tillgängliga för Workfront mobilappar. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Listruta</td> 
      <td>Innehåller en lista med alternativ i listrutan.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typeahead </td> 
      <td>Tillåter användare att skriva namnet på ett objekt som finns i Workfront. En lista med förslag visas när användaren börjar skriva.
      Den här fälttypen har stöd för följande objekt:
      <ul><li>Användare</li>
      <li>Grupp</li>
      <li>Jobbroll</li>
      <li>Portfolio</li>
      <li>Program</li>
      <li>Projekt</li>
      <li>Team</li>
      <li>Mall</li>
      <li>Företag</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beräknat</td> 
      <td>Gör att du kan definiera ett uttryck och visa resultatet i det anpassade formuläret. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Lägga till beräknade data i ett anpassat formulär</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datum</td> 
      <td>Visar en kalender där användare kan välja datum och tid.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kryssrutor</td> 
      <td>Tillåter användare att välja flera alternativ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alternativknappar</td> 
      <td>Kräver att användare bara väljer ett alternativ.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Gör att du kan inkludera instruktioner och länka till sidor utanför Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Avsnittsbrytning</td> 
      <td>En avsnittsbrytning är egentligen inte ett fält. Du kan använda en avsnittsbrytning för att ordna anpassade fält och widgetar i avsnitt och, om det behövs, konfigurera olika visnings- och redigeringsbehörigheter för varje avsnitt. Mer information om hur du lägger till och konfigurerar avsnittsbrytningar finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Lägga till en avsnittsbrytning i ett anpassat formulär</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Fält som tillåter flera val, som kryssrutor och listrutor, är svåra att schemalägga och gruppera i rapporter. Om du vill att det ska vara enklare att rita och gruppera i rapporter kan du skapa separata fält för varje val (till exempel ett textfält med en rad).

1. På **Fältinställningar** konfigurerar du de alternativ som är tillgängliga för den typ av anpassat fält som du lägger till:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar det anpassade fältet när du lägger till det i olika områden i Workfront, till exempel rapporter, Hem- och API-interaktioner.</p> <p>När du konfigurerar det anpassade fältet för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> 
      <p><b>VIKTIGT</b>:   
      <ul> 
      <li>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront. <p>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.</p> </li>
      <li> <p>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.</p> </li>
      <li><p>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.</p></li>
      </ul> <p>Varje anpassat fältnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. Mer information finns i <a href="#add-a-custom-field-to-a-custom-form">Lägga till ett anpassat fält i ett anpassat formulär</a> i den här artikeln.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Ange eventuell ytterligare information om det anpassade fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Välj den typ av data som ska hämtas i det anpassade fältet. Du kan ändra formatvalet när du har sparat formuläret, men det nya formatet måste ha stöd för det angivna värdet.</p>

   <p><strong>Exempel:</strong> Om du sparar ett numeriskt värde för ett fält med textformat för minst ett objekt och senare ändrar formatet till Nummer eller Valuta, kommer du inte att stöta på något fel. </p>
      <p>Om du sparar ett alfanumeriskt värde i ett fält med textformat för minst ett objekt och sedan försöker ändra formatet till Nummer eller Valuta, kommer du att stöta på ett fel eftersom det sparade alfanumeriska värdet inte är kompatibelt med formatet Nummer eller Valuta. </p>

   <p><strong>Obs!</strong> Teckengränsen för nummerfält är 16. Du kan också använda ett textfält för att ange tal och undvika gränsen.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visningstyp</td> 
      <td>(Endast listrutor, kryssrutor och alternativknappar) Växla den typ av alternativ som du vill använda för fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Storlek</td> 
      <td>(Endast textfält) Välj en bredd för fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa tid på dagen</td> 
      <td>(Endast datumfält) Välj det här alternativet om du vill visa tiden på dagen tillsammans med datumet i fältet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Refererad objekttyp</td> 
      <td> <p>(Endast typsnittsfält) Markera den objekttyp som du vill associera med fältet.</p> <p>När du har klickat på Använd eller Spara+Stäng kan du inte ändra fälttypen.</p> <p><b>ANMÄRKNING</b>:   
        <ul> 
         <li>Om Workfront-administratören har anpassat namnet på Portfolio, Program eller Projekt i Workfront användargränssnitt, visas Workfront-standardnamnet för objektet i den här listrutan, inte det anpassade namnet. Kontakta Workfront-administratören om du behöver hjälp med detta.<br></li> 
         <li>Följande objekttyper stöds i iOS och Android Workfront mobilappar: User, Company, Group, Job Role, Portfolio, Program, Project och Template.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Lägg till filter</td> 
      <td> <p>(Endast typsnittsfält) Lägg till ett filter för en objekttyp för att begränsa vilka objekt som användarna kan välja när de använder fältet. </p> <p>Du kan till exempel begränsa ett fält så att användarnamn bara kan väljas om de uppfyller följande villkor:</p> 
       <ul> 
        <li>De tillhör en grupp eller grupper som du anger</li> 
        <li>De är kopplade till en roll eller jobbtitel som du anger</li> 
        <li>De tillhör samma grupp som den person som använder fältet</li> 
       </ul> <p>Du måste definiera filtret för den objekttyp som du har valt med syntaxen för textläge. Mer information om hur du skapar ett filter i textläge finns i <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Redigera ett filter i textläge</a>.</p>
       <p><b>ANMÄRKNING</b>:   
        <ul> 
         <li>Om du redigerar ett befintligt anpassat formulär och lägger till ett filter i ett texthuvudfält, tas inga objekt bort (utanför filteromfånget) som användare redan har lagt till med fältet.</li> 
         <li>Filtret är inte tillgängligt på mobila enheter. Om du använder filtret för ett Typeahead-fält visas fältet på användarens mobila enheter som inte påverkas av filtret.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>(Endast beskrivande textfält) Skriv den text som du vill visa för att ange instruktioner eller en länk i det anpassade formuläret. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hyperlänk</td> 
      <td>(Endast beskrivande textfält) Om du vill använda en hyperlänk i den beskrivande texten lägger du till den här.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gör ett obligatoriskt fält</td> 
      <td>Välj det här alternativet om du vill att fältet ska vara obligatoriskt för att användaren ska kunna fylla i det anpassade formuläret. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spåra fältändringar i uppdateringsflöden</td> 
      <td><p>Klicka på listrutan och välj sedan de objekttyper där du automatiskt vill spåra fältets värdeändringar.</p> 
      <p><b>ANMÄRKNING</b>: Det här alternativet är inte tillgängligt för följande:</p> 
      <ul> 
      <li>Anpassade formulär som är associerade med följande objekttyper: Utgift, Företag, Iteration, Faktureringspost, Dokument och Grupp.</li> 
      <li>Följande fälttyper: Beräknat, Beskrivande text och Avsnittsbrytning</li> 
      </ul>
      <p><b>VIKTIGT</b>: Om du markerar eller avmarkerar en objekttyp här påverkas alla anpassade formulär som är kopplade till den valda objekttypen och som innehåller det här fältet. Om du till exempel avmarkerar en objekttyp här och sparar det anpassade formuläret spåras inte längre fältets värdeändringar för den objekttypen i något anpassat formulär som innehåller fältet.</p>
       <p>När du har valt en objekttyp här för ett fält och sparat det anpassade formuläret, visas fältet på fliken Anpassade fält i området Uppdatera feeds i inställningarna.</p> 
       <p>Om det här fältet däremot tas bort i området Uppdatera feeds i Inställningar, avmarkeras objekttypen för den här inställningen för alla anpassade formulär som är associerade med objekttypen och som innehåller det här fältet.</p> 
       <p>Mer information finns i avsnittet <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Lägg till fält som Workfront ska spåra</a> i artikeln <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">Konfigurera systemuppdateringar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lägg till logik</td>
      <td>Ange vilka fält som ska visas i formuläret, baserat på de val som användarna gör i befintliga fält. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Lägga till visningslogik och hoppa över logik i ett anpassat formulär</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Val </td> 
      <td> <p>(Endast listrutor, kryssrutor eller alternativknappar; valfritt)</p> 
       <ol> 
        <li> <p>Klicka <b>Alternativ</b>aktiverar du sedan något av följande:</p> 
           <ul> 
            <li><strong>Visa värden</strong>: Visar värdena för varje val i fältet. Etiketten för varje val visas som standard.</li> 
            <li><strong>Sorteringsalternativ A-Z</strong>: Sorterar de alternativ du lägger till i bokstavsordning i fältet.</li> 
           </ul> 
        </li> 
        <li> <p>Klicka på kugghjulsikonen för varje val som du lägger till för användaren <img src="assets/gear-icon-settings.png">väljer du sedan något av följande alternativ:</p> 
           <ul> 
            <li><strong>Markera som standard</strong>: Välj alternativet som standard i fältet.</li> 
            <li> <p><strong>Dölj alternativ</strong>: Dölj alternativet i fältet. Dolda alternativ är fortfarande tillgängliga i rapporter.</p> </li> 
            <li> <p><strong>Ta bort alternativ</strong>: Ta bort alternativet från fältet.</p> <p><b>VARNING</b>: Om du har aktuella objekt med det här alternativet ska du inte ta bort det från fältet. Om du tar bort den går historikdata förlorade. Välj i stället alternativet att dölja det, vilket förhindrar att användarna väljer det i framtiden.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om du vill ändra visningstypen för ett fält i det anpassade formuläret klickar du på **Visningstyp** och klicka sedan på önskad typ.

   Du kan växla mellan följande fälttyper:

   * **Markeringstypfält**: Kryssrutor, listrutor, alternativknappar.
   * **Textfält**: Textfält med en rad, Textfält med stycke. (Du kan inte växla ett textfält med formatering till en annan visningstyp. Du kan dock ta bort den och lägga till en annan typ av fält.)

   Om du t.ex. har skapat ett kryssrutefält kan du ändra det till ett nedrullningsbart fält eller ett alternativknappsfält. Om du har skapat ett textfält med en rad kan du ändra det till ett textfält med en rad.

   >[!NOTE]
   >
   >Tänk på följande när du vill ändra ett fälts visningstyp från ett kryssrutefält eller ett flervalsfält (en listruta där mer än ett alternativ kan väljas) till en fälttyp:
   >
   >* Om du ändrar till Alternativknappar behåller Workfront alla flervalsvärden som en användare kan ha angett i fältet tills användaren ändrar och sparar data i någon del av formuläret. I det här läget ersätts alla värden som har markerats med flervalsfältet av det valda alternativknappsvärdet.
   >* Om du ändrar till en listruta med endast ett val, behåller Workfront alla flervalsvärden som en användare kan ha angett i fältet tills användaren ändrar och sparar värdena i fältet. I det här läget ersätts alla värden som har markerats med fältet för flervalstyp med det valda nedrullningslistvärdet.

1. (Valfritt) Upprepa steg 3-5 om du vill lägga till fler anpassade fält.

   eller

   Lägg till fält som redan har skapats för din organisation, vilket förklaras i [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   >[!NOTE]
   >
   >Du kan lägga till upp till 500 fält och widgetar i ett anpassat formulär. Prestandaförsämringen kan dock inträffa när det finns mer än 100 blanketter, beroende på hur komplex den är. Exempel på komplexa formulär är formulär med överlappande parametrar, beräknade anpassade datafält och flera värdealternativ i ett enda fält.

1. Klicka **Använd**.
1. Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Lägga till en avsnittsbrytning i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fylla i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
