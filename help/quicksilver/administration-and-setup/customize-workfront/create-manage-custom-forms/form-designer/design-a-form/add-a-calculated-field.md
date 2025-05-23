---
title: Lägg till beräkningsfält i ett formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan lägga till ett beräknat anpassat fält som använder befintliga data för att generera nya data när det anpassade formuläret kopplas till ett objekt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: 0c2a54406ceb690e638cdc0376a3dc01a7c2df76
workflow-type: tm+mt
source-wordcount: '2434'
ht-degree: 0%

---

# Lägga till beräknade fält i ett formulär

<!-- Audited: 5/2025 -->

Du kan lägga till ett beräknat anpassat fält som använder befintliga data för att generera nya data när det anpassade formuläret kopplas till ett objekt.

Ett beräknat anpassat fält kan innehålla:

* En enkel referens till ett enda inbyggt fält.

  >[!INFO]
  >
  >**Exempel:** Om du vill beräkna intäkterna från projekt och aktiviteter kan du skapa ett beräknat anpassat fält som innehåller det inbyggda fältet Faktisk omsättning. När någon kopplar det anpassade formuläret till ett projekt eller en uppgift visas intäkterna för projektet eller uppgiften i fältet.

* Ett uttryck som refererar till ett eller flera fält. Dessa kan vara anpassade fält, andra beräknade anpassade fält och inbyggda fält.

  >[!INFO]
  >
  >**Exempel:** Om du vill beräkna vinsten som genereras av projekt och aktiviteter kan du skapa ett beräknat anpassat fält med namnet Vinst som innehåller ett matematiskt uttryck som subtraherar kostnaden från intäkterna.
  >
  >För att göra detta kan du använda det matematiska uttrycket SUB (subtrahera) med de inbyggda Workfront-fälten Faktisk kostnad och Faktisk omsättning.
  >
  >I stegen nedan kan du se hur du skapar ett uttryck som det här exemplet.

>[!NOTE]
>
>Ändringar i ett direktfält utlöser automatiskt en uppdatering av det beräknade fältets värde. (Direktfält är fält som är tillgängliga i Workfront API Explorer, eller anpassade fält i ett anpassat formulär som är kopplat till ett objekt.) Ändringar av en referens eller formel kräver en manuell omberäkning av fältvärdena.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <td> <p>Administrativ åtkomst till anpassade formulär</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär

Du kan använda samma beräknade anpassade fält i anpassade formulär som tillhör olika objekt. Du kan till exempel använda fältet Resultatberäkning som du skapade för det anpassade projektformuläret i ett anpassat aktivitetsformulär.

När du använder ett befintligt beräknat anpassat fält överförs inte beräkningen till det nya formuläret. Du måste lägga till beräkningen igen i samma fält i det nya anpassade formuläret.

Du kan också ha en annan beräkning för samma fält i det nya formuläret. Om du behåller samma namn för det beräknade anpassade fältet är namnkonventionen konsekvent och konsekvent.

>[!IMPORTANT]
>
>Ändringar i beräknade uttryck kan göra att fältvärdet för objekt blir inaktuellt. Gör något av följande om du alltid vill se den aktuella beräkningen i dessa fält:
>
>* När du har sparat ett objekt där du har redigerat data i ett kopplat anpassat formulär, klickar du på ikonen Mer ![Mer](assets/more-icon.png) på objektets huvudsida och beräknar om anpassade uttryck.
>* Markera alternativet Beräkna om anpassade uttryck när du redigerar flera objekt samtidigt.
>* Välj alternativet Uppdatera tidigare beräkningar när du redigerar ett beräknat anpassat fält i ett anpassat formulär.

Så här återanvänder du ett befintligt beräknat anpassat fält:

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms** och sedan på **Forms** i den vänstra panelen.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klicka på **Nytt anpassat formulär**.

1. I dialogrutan **Nytt anpassat formulär** väljer du vilka objekttyper du vill koppla det anpassade formuläret till och klickar sedan på **Fortsätt**.
1. Klicka på **Fältbibliotek** på skärmens övre vänstra sida.

   ![Fältbibliotek](assets/field-library.png)

1. Använd sökrutan eller utöka avsnittet **Beräknad** för att hitta det beräknade fält du behöver och dra sedan fältet där du vill att det ska visas i det anpassade formuläret.

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält.

   >[!NOTE]
   >
   >Du kan lägga till upp till 500 fält och widgetar i ett anpassat formulär. Prestandaförsämringen kan dock inträffa när det finns mer än 100 blanketter, beroende på hur komplex den är.
   >
   >
   >Exempel på komplexa formulär är formulär med överlappande parametrar, beräknade anpassade datafält och flera värdealternativ i ett enda fält.

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

## Lägg till ett nytt beräknat fält

>[!IMPORTANT]
>
>Innan du skapar ett nytt beräknat anpassat fält identifierar du de befintliga fält som du vill inkludera, så att du är säker på att de data som behövs för beräkningen finns i Workfront.

{{step-1-to-setup}}

1. Klicka på **Anpassad Forms** och sedan på **Forms** i den vänstra panelen.

1. Klicka på **Nytt anpassat formulär**.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. I dialogrutan **Nytt anpassat formulär** väljer du vilka objekttyper du vill koppla det anpassade formuläret till och klickar sedan på **Fortsätt**.

1. Leta upp **Beräknat** till vänster på skärmen och dra det till ett avsnitt på arbetsytan.

   ![Dra fält till avsnitt](assets/drag-field-to-section.png)

1. Till höger på skärmen konfigurerar du de alternativ som är tillgängliga för den typ av anpassat fält som du lägger till:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td>Ange en etikett för fältet. Detta är vad användarna kommer att se när de använder det anpassade formuläret. Workfront refererar till fältet <b>Namn</b>, som fylls i automatiskt, i rapporter.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instruktioner</td> 
      <td> Som standard lagras formeln som du skapar för fältet här. Du kan lägga till text om du vill ha mer information om fältet och formeln i det. Detta kan vara användbart på två sätt: 
       <ul> 
      <li><p>Som en påminnelse om vad formeln är och hur den fungerar. Detta är särskilt användbart om du tänker använda det här beräknade anpassade fältet på flera formulär.</p> </li> 
      <li> <p>Som ett verktygstips kan användarna se när de hovrar över fältet. Du lägger till text här som du vill att de ska se i verktygstipset.</p> <p>Om du inte vill att de ska se formeln i verktygstipset, vilket kan vara förvirrande för dem, kan du dölja den.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Det format i vilket du vill att fältets resultat ska lagras och visas.</p> <p>Om fältet ska användas i matematiska beräkningar ska du alltid använda formatet <strong>Number</strong> eller <strong>Currency</strong>. När du väljer <strong>Number</strong> eller <strong>Currency</strong> trunkeras nummer som börjar med 0 automatiskt.</p> 
      <p><b>VIKTIGT</b>: Innan du väljer ett format bör du överväga det nya fältets format. Det går inte att redigera formatfältet efter att det anpassade formuläret har sparats. Om du väljer fel format kan framtida beräkningar och aggregerade värden i rapport- och listgrupperingar påverkas.</p>
      <p><strong>Obs!</strong> Beräknade fält med formatet <strong>Valuta</strong> får inte innehålla citattecken. (Använd till exempel 800.00 och inte "800.00.") Användning av citattecken kan få oväntade konsekvenser på grund av nyanser med språkformatering för valutatyper.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Börja bygga beräkningen i rutan **Beräkning**:
   1. Klicka på **Maximera** för att öppna beräkningsredigeraren och skapa beräkningen.</p>
En beräkning börjar oftast med ett uttryck följt av parenteser som innehåller de fält som du vill referera till när det anpassade formuläret är kopplat till ett objekt.

      Varje fält måste omges av klammerparenteser. När du börjar skriva namnet på ett fält ger systemet förslag och du kan välja ett som infogar det i beräkningen.

+++ **Utöka för att se syntax som krävs i beräknade anpassade fält**

      Varje fält måste ha den syntax som beskrivs nedan, med klammerparenteser runt varje fältnamn. När du börjar skriva namnet på ett fält ger systemet förslag och du kan välja ett som infogar det i beräkningen. Om du anger data i en beräkning felaktigt visas ett varningsmeddelande. Du kan inte spara formuläret om du inte redigerar beräkningen så att den innehåller giltiga fält och ett giltigt beräknat uttryck.

      >[!NOTE]
      >
      >Systemet ger för närvarande endast förslag när du börjar skriva namnet på ett fält som du vill referera till på ett objekt som det anpassade formuläret ska kopplas till. Fält från det överordnade objektet föreslås inte.

      **Omgivande fältnamn med klammerparenteser**

      * Om du vill att beräkningen ska referera till ett inbyggt fält måste fältnamnet omges av klammerparenteser.

        Till exempel: `{actualRevenue}`

        Fältnamn är skiftlägeskänsliga och måste visas exakt som de visas i Workfront.

        Navigera till [Workfront API Explorer](https://developer.adobe.com/workfront/api-explorer/) för att identifiera fältnamnen som kan användas i beräkningar.

      * Om du vill att beräkningen ska referera till ett anpassat fält måste fältnamnet omges av klammerparenteser och föregås av `DE:` inom klammerparenteserna.

        Till exempel: `{DE:Profit}`

        Alla anpassade fält som du kan välja när du skriver `DE:` visas.

         * Om du vill att beräkningen ska referera till ett fält som hämtar data från objektet *parent* när det anpassade formuläret kopplas till ett objekt, måste du före fältnamnet skriva objekttypen för det överordnade objektet, även inom klammerparenteser.

        Om det anpassade formuläret till exempel är konfigurerat att fungera med uppgifter och du vill att fältet ska beräkna den faktiska intäkten för det överordnade objektet när formuläret kopplas till en uppgift, måste du ange `Project` som fälttyp:

        `{project}.{actualRevenue}`

        Eller, om det är ett anpassat fält:

        `{project}.{DE:profit}`

        **Separera objekt med punkter**

        När du refererar till ett relaterat objekt i ett beräknat anpassat fält måste du separera objektnamn och attribut med punkter.

        Om du till exempel vill visa namnet på Portfolio-ägaren i ett beräknat anpassat fält i ett anpassat formulär av uppgiftstyp skriver du följande:

        `{project}.{porfolio}.{owner}`

        Detta skulle bestämma följande: Från objektet i det anpassade formuläret (en uppgift) kan du komma åt nästa objekt som hör till uppgiften (ett projekt). Därifrån kan du komma åt nästa relaterade objekt till projektet (en portfölj) och sedan referera till fälten som definierats för portföljobjektet (ägaren)

        **Namnsyntax för att referera till ett anpassat fält**

        När du refererar till ett annat anpassat fält i ett beräknat anpassat fält måste du ange fältets namn så som det visas i Workfront användargränssnitt.

        Om du till exempel vill referera till det valda alternativet i ett anpassat fält med namnet Executive sponsor skriver du följande:

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >Syntaxen för ett typhuvudfält skiljer sig lite från den för andra typer av fält eftersom du måste lägga till `:name` i slutet.
        >
        >Om du till exempel vill referera till det valda alternativet i ett anpassat typsnittsfält med namnet&quot;Executive sponsor&quot; skriver du:
        >
        >`{DE:Executive sponsor:name}`


        **Beräknade anpassade fält i anpassade formulär med flera objekt**

        I ett anpassat formulär med flera objekt måste de valda objekttyperna vara kompatibla med minst ett fält som refereras i formulärets beräknade anpassade fält. Fält som inte är kompatibla med objektet kommer att visa N/A i formuläret.

        För att säkerställa att beräkningsfältet visar rätt resultat för alla objekttyper måste du använda `$$OBJCODE` för att definiera en beräkning för varje objekttyp.

        >[!INFO]
        >
        >**Exempel:**
        >
        >I ett anpassat formulär som är konfigurerat att fungera med projekt, uppgifter och ärenden kan du använda följande formel för att visa objekttypen:
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >I ett projekt kommer fältet att visa&quot;This is a project&quot;, i en uppgift kommer det att visa&quot;This is a task&quot;, och i en fråga kommer det att stå&quot;This is an issue&quot;.


        >[!INFO]
        >
        >**Exempel:** Även om det inte finns något tilldelat till: Namnfält i projekt finns det ett inbyggt ägarfält (som automatiskt fylls i med namnet på den person som skapade projektet, såvida inte någon ändrar detta manuellt).
        >
        >I ditt anpassade avgiftsfält kan du använda `$$OBJCODE` så som visas nedan för att referera till fältet Ägare när det anpassade formuläret är kopplat till ett projekt, och fältet Tilldelad: Namn när formuläret är kopplat till en uppgift:
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        Mer information om variabler som `$$OBJCODE,` finns i [Översikt över variabler för jokertecken](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **Automatiska uppdateringar av beräknade anpassade fält**

        Beräknade anpassade fält i ett objekt beräknas om automatiskt när följande inträffar:

         * Något på objektet ändras, till exempel en daglig tidslinjeberäkning.
         * Någon redigerar ett annat fält som refereras av ett beräknat anpassat fält i objektet.
         * Det beräknade uttrycket är tomt och fältet innehåller ett värde. Värdet ställs in på null.

           >[!NOTE]
           >
           ><div>I ett anpassat formulär som bifogas till ett objekt beräknas och sparas datum- och tidssatser i beräknade anpassade fält med UTC (Coordinated Universal Time), inte med de tidszonskonfigurationer som angetts för organisationens instans och din användarprofil. Beräkningar i ett anpassat formulär genereras baserat på varje användares enskilda tidszoner.</div>

+++

   1. Klicka i den stora textrutan och klicka sedan på **Uttryck** och **Fält** som är tillgängliga för att lägga till dem i beräkningen.

      Expandera ett objektnamn under **Fält** för att se alla fält som är tillgängliga för objektet. Listan är begränsad till 200 objekt. Om du känner till fältnamnet kan du söka efter det.

      Du kan också börja skriva ett uttryck eller fält i den stora textrutan och sedan markera det när det visas. Varje objekt visas med &quot;F&quot; för fält eller &quot;E&quot; för uttryck.

      Om du skriver en inledande parentes läggs den avslutande parentesen till automatiskt.

+++ **Expandera och se praktiska tips**

      >[!TIP]
      >
      >Du kan göra något av följande för att få hjälp med beräkningen:
      > 
      >* Hovra över ett uttryck i beräkningen för att se en beskrivning, ett exempel som visar hur det kan användas och en **Läs mer** -länk till mer information i artikeln [Översikt över beräknade datauttryck](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![Hjälptext för uttryck](assets/hover-expression-help-text.jpg)
      >* Använd färgkodningen för att identifiera de komponenter du har lagt till. Uttryck visas i blått och fält visas i grönt.
      >  ![Färger för fältuttryck](assets/colors-fields-expressions.jpg)
      >* Hitta beräkningsfel, markerade i rosa allt eftersom. Du kan hovra över ett markerat fel om du vill visa en kort beskrivning av orsaken.
      >  ![Felhjälp](assets/error-help.png)
      >* Förhandsgranska resultatet för ett befintligt Workfront-objekt i området under beräkningen.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![Förhandsgranska beräkning](assets/preview-calc.jpg)
      >* Referensuttryck i en lång beräkning med hjälp av radnumren som visas till vänster.

+++
   1. Klicka på **Minimera** när du är klar med att skapa beräkningen för det beräknade anpassade fältet.

   1. (Valfritt) Använd något av följande alternativ för att ytterligare konfigurera det beräknade anpassade fältet:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lägg till logik</td> 
      <td>Du kan lägga till Display Logic för att avgöra om beräkningsfältet ska visas, baserat på minst ett val som en användare gör i ett föregående flervalsfält (listrutor, kryssrutor eller alternativknappar) när formuläret fylls i. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Detta är endast tillgängligt när minst en kryssruta, alternativknapp eller ett listrutefält föregår det beräknade anpassade fältet i formuläret. </p> <p>Hopplogik är inte tillgängligt för beräknade anpassade fält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdatera tidigare beräkningar</td> 
      <td>När du redigerar ett befintligt beräknat anpassat fält kan du välja det här alternativet om du vill aktivera en uppdatering i beräkningen när du sparar det anpassade formuläret. Detta händer bara en gång när du sparar det anpassade formuläret. Alternativet återgår till inaktiverat läge när du har gjort det.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa formel i instruktioner</td> 
      <td>Låt det här alternativet vara aktiverat om du vill att de användare som fyller i det anpassade formuläret ska se fältets formel när de hovrar över fältet. Mer information finns i informationen om <a href="#instructions" class="MCXref xref">Instruktioner</a> tidigare i den här tabellen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.
