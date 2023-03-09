---
title: Lägga till beräknade data i ett anpassat formulär med äldre formulärverktyg
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: I ett anpassat formulär kan du skapa ett beräknat anpassat fält som genererar beräkningar. För att göra detta skapar du en programsats som använder datauttryck och namnen på befintliga fält, som kan vara anpassade fält, beräknade anpassade datafält och inbyggda Workfront-fält. Den här satsen beräknar de data du anger och visar resultatet i det nya beräknade anpassade fältet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2573'
ht-degree: 0%

---

# Lägga till beräknade data i ett anpassat formulär med äldre formulärverktyg

I ett anpassat formulär kan du lägga till ett beräknat anpassat fält som använder befintliga data för att generera nya data när det anpassade formuläret kopplas till ett objekt.

Ett beräknat anpassat fält kan innehålla:

* En enkel referens till ett enda inbyggt fält.

   >[!INFO]
   >
   > **Exempel:** Om du vill beräkna intäkten som genereras av projekt och uppgifter kan du skapa ett beräknat anpassat fält som innehåller det inbyggda fältet Faktisk intäkt. När någon kopplar det anpassade formuläret till ett projekt eller en uppgift visas intäkterna för projektet eller uppgiften i fältet.

* Ett uttryck som refererar till ett eller flera fält. Dessa kan vara anpassade fält, andra beräknade anpassade fält och inbyggda fält.

   >[!INFO]
   >
   >**Exempel:** Om du vill beräkna vinsten som genereras av projekt och uppgifter kan du skapa ett beräknat anpassat fält som heter Vinst som innehåller ett matematiskt uttryck som subtraherar kostnaden från intäkterna.
   >
   >För att göra detta kan du använda det matematiska uttrycket SUB (subtrahera) med de inbyggda Workfront-fälten Faktisk kostnad och Faktisk intäkt.
   >
   >I stegen nedan ser du hur det här exemplet kan utföras.

Mer information om hur du skapar anpassade formulär för din organisation och förstår vilken typ av fält du kan associera med dem finns i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Lägga till ett beräknat fält i ett anpassat formulär {#add-a-calculated-field-to-a-custom-form}

Du kan använda både inbyggda Workfront-fält och anpassade fält som du redan har skapat.

>[!IMPORTANT]
>
>Innan du skapar ett nytt beräknat anpassat fält identifierar du de befintliga fält som du vill inkludera, så att du är säker på att de data som behövs för beräkningen finns i Workfront.

1. Börja skapa eller redigera ett anpassat formulär, enligt beskrivningen i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. På **Lägg till ett fält** flik, klicka **Beräknat**.

   I visningsområdet till höger visas fältet *12345*. Detta är bara en indikator som påminner dig om att fältet är ett beräknat anpassat fält när du skapar eller redigerar det anpassade formuläret. När formuläret är kopplat till ett objekt och användarna fyller i det, ser de resultatet av beräkningen i fältet, aldrig resultatet *12345* indikator.

1. Ange följande information för beräkningsfältet:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td>Ange en etikett för fältet. Detta är vad användarna kommer att se när de använder det anpassade formuläret. Fältet <b>Namn</b>, som fylls i automatiskt, refereras av Workfront i rapporter.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instruktioner</td> 
      <td> Som standard lagras formeln som du skapar för fältet här. Du kan lägga till text om du vill ha mer information om fältet och formeln i det. Detta kan vara användbart på två sätt: 
       <ul> 
        <li> <p>Som en påminnelse om vad formeln är och hur den fungerar. Detta är särskilt användbart om du tänker använda det här beräknade anpassade fältet på flera formulär.</p> </li> 
        <li> <p>Som ett verktygstips kan användarna se när de hovrar över fältet. Du lägger till text här som du vill att de ska se i verktygstipset.</p> <p>Om du inte vill att de ska se formeln i verktygstipset, vilket kan vara förvirrande för dem, kan du dölja den. Instruktioner finns i tabellraden "Visa formel i instruktioner" i avsnittet <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">Bygg beräkningen för ditt beräknade anpassade fält</a> i den här artikeln.</p> </li> 
       </ul> <p>Mer information om hur du använder samma beräknade anpassade fält i ett nytt formulär finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Det format som du vill att fältets resultat ska sparas och visas i.</p> <p>Om fältet ska användas i matematiska beräkningar ska du alltid använda en <strong>Nummer</strong> eller en <strong>Valuta</strong> format. När du väljer Nummer eller Valuta trunkeras nummer som börjar med 0 automatiskt.</p> 
      <p><b>VIKTIGT</b>: Innan du väljer ett format bör du tänka på rätt format för det nya fältet. Det går inte att redigera formatfältet efter att det anpassade formuläret har sparats. Om du väljer fel format kan framtida beräkningar och aggregerade värden i rapport- och listgrupperingar påverkas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt till [Bygg beräkningen för ditt beräknade anpassade fält](#build-the-calculation-for-your-calculated-custom-field) i den här artikeln.

## Bygg beräkningen för ditt beräknade anpassade fält {#build-the-calculation-for-your-calculated-custom-field}

1. Börja skapa det beräknade anpassade fältet enligt anvisningarna i avsnittet [Lägga till ett beräknat fält i ett anpassat formulär](#add-a-calculated-field-to-a-custom-form) i den här artikeln.

1. Klicka **Maximera** för att öppna **Beräkningsredigerare** och bygga upp dina beräkningar.

   >[!INFO]
   >
   >**Exempel:** Med hjälp av exemplet i inledningen till den här artikeln kan du skapa ett beräknat anpassat fält med namnet Vinstdrivande i ett anpassat formulär för projekt och uppgifter. Det här fältet kan innehålla en beräkning som visar skillnaden mellan Faktisk intäkt och Faktisk kostnad:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >I det här exemplet `SUB` är uttrycket och de refererade fälten är `actualRevenue` och `actualCost`.

   En beräkning börjar oftast med ett uttryck följt av parenteser som innehåller de fält som du vill referera till när det anpassade formuläret är kopplat till ett objekt. Mer information om tillgängliga uttryck finns i [Beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Varje fält måste omges av klammerparenteser, vilket förklaras i avsnittet [Syntax krävs i beräknade anpassade fält](#syntax-required-in-calculated-custom-fields) i den här artikeln. När du börjar skriva namnet på ett fält ger systemet förslag och du kan välja ett som infogar det i beräkningen.

   Du kan referera till alla typer av anpassade fält i en beräkning förutom två: Textfält med formateringstyp och Beskrivande text. Mer information om de anpassade fälttyperna finns i [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. Klicka i den stora textrutan och klicka sedan på **Uttryck** och **Fält** som är tillgängliga för att lägga till dem i beräkningen.

   Du kan också börja skriva ett uttryck eller fält i den stora textrutan och sedan markera det när det visas. Varje objekt visas med &quot;F&quot; för fält eller &quot;E&quot; för uttryck.

   Om du skriver en inledande parentes läggs den avslutande parentesen till automatiskt.

   >[!TIP]
   >
   >Du kan göra något av följande för att få hjälp med beräkningen:
   > 
   >* Håll muspekaren över ett uttryck i beräkningen för att se en beskrivning, ett exempel som visar hur det kan användas och en Lär dig mer-länk för mer information i artikeln [Beräknade datauttryck](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
   >* Använd färgkodningen för att identifiera de komponenter du har lagt till. Uttryck visas i blått och fält visas i grönt.
      >  ![](assets/colors-fields-expressions.jpg)
   >* Hitta beräkningsfel, markerade i rosa allt eftersom. Du kan hovra över ett markerat fel om du vill visa en kort beskrivning av orsaken.
      >  ![](assets/error-help.png)
   >* Förhandsgranska resultatet för ett befintligt Workfront-objekt i området under beräkningen.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

      >  ![](assets/preview-calc.jpg)
   >* Referensuttryck i en lång beräkning med radnumren som visas till vänster.


1. Klicka **Minimera** när du är klar med att skapa beräkningen för det beräknade anpassade fältet.

   >[!NOTE]
   >
   >I visningsområdet till höger visas fältet *12345.* Detta är bara en indikator som påminner dig om att fältet är ett beräknat anpassat fält när du skapar eller redigerar det anpassade formuläret. När formuläret är kopplat till ett objekt och användarna fyller i det, ser de resultatet av beräkningen i fältet, aldrig resultatet *12345* indikator.

1. (Valfritt) Använd något av följande alternativ för att ytterligare konfigurera det beräknade anpassade fältet:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lägg till logik</td> 
      <td>Du kan lägga till Display Logic för att avgöra om beräkningsfältet ska visas, baserat på minst ett val som en användare gör i ett föregående flervalsfält (listrutor, kryssrutor eller alternativknappar) när formuläret fylls i. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Lägga till visningslogik och hoppa över logik i ett anpassat formulär</a>. <p>Detta är endast tillgängligt när minst en kryssruta, alternativknapp eller ett nedrullningsbart fält föregår det beräknade anpassade fältet i formuläret. </p> <p>Hopplogik är inte tillgängligt för beräknade anpassade fält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdatera tidigare beräkningar</td> 
      <td>När du redigerar ett befintligt beräknat anpassat fält kan du välja det här alternativet om du vill aktivera en uppdatering i beräkningen när du sparar det anpassade formuläret. Detta händer bara en gång när du sparar det anpassade formuläret. Alternativet återgår till inaktiverat läge när du har gjort det.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa formel i instruktioner</td> 
      <td>Låt det här alternativet vara aktiverat om du vill att de användare som fyller i det anpassade formuläret ska se fältets formel när de hovrar över fältet. Mer information finns i informationen om <a href="#instructions" class="MCXref xref">Instruktioner</a> tidigare i denna tabell.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Klar** när alla ändringar har slutförts i det beräknade anpassade fältet.

   Eller klicka **Använd** om du vill lägga till egna fält i formuläret ska du tillämpa ändringarna i formuläret så länge du vill.

   Eller klicka **Spara + Stäng** när alla ändringar har gjorts i det anpassade formuläret.
1. För att verifiera att det beräknade anpassade fältet fungerar som det ska, bifogar du det anpassade formuläret till ett objekt och granskar sedan resultatet i det beräknade anpassade fältet.

   Instruktioner om hur du bifogar ett anpassat formulär finns i [Lägga till ett anpassat formulär i ett objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till eller redigera en resurswidget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fylla i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Syntax krävs i beräknade anpassade fält

Varje fält måste ha den syntax som beskrivs nedan, med klammerparenteser runt varje fältnamn. När du börjar skriva namnet på ett fält ger systemet förslag och du kan välja ett som infogar det i beräkningen. Om du anger data i en beräkning felaktigt visas ett varningsmeddelande. Du kan inte spara formuläret om du inte redigerar beräkningen så att den innehåller giltiga fält och ett giltigt beräknat uttryck.

>[!NOTE]
>
>Systemet ger för närvarande endast förslag när du börjar skriva namnet på ett fält som du vill referera till på ett objekt som det anpassade formuläret ska kopplas till, inte på objektets överordnade.

### Omgivande fältnamn med klammerparenteser

* Om du vill att beräkningen ska referera till ett inbyggt fält måste fältnamnet omges av klammerparenteser.

Exempel: `{actualRevenue}`

Fältnamn är skiftlägeskänsliga och måste visas exakt som de visas i Workfront.

* Om du vill att beräkningen ska referera till ett anpassat fält måste fältnamnet omges av klammerparenteser och föregås av `DE:` inom parentes.

Exempel: `{DE:Profit}`

Alla anpassade fält som du kan välja mellan när du skriver visas. `DE:`.

* Om du vill att beräkningen ska referera till ett fält som hämtar data från *parent* när det anpassade formuläret är kopplat till ett objekt, måste du före fältnamnet skriva objekttypen för det överordnade objektet, även inom klammerparenteser.

   Om det anpassade formuläret till exempel är konfigurerat att fungera med uppgifter och du vill att fältet ska beräkna den faktiska intäkten för det överordnade objektet när formuläret kopplas till en uppgift, måste du ange `Project` som fälttyp:

   `{project}.{actualRevenue}`

   Eller, om det är ett anpassat fält:

   `{project}.{DE:profit}`

   Om du är osäker på vilken objekttyp det överordnade objektet kommer att vara eftersom den anpassade för har konfigurerats för flera objekttyper kan du använda filtret för jokertecken `$$OBJCODE` så att beräkningen kan fungera för alla möjliga typer. Mer information finns i [Beräknade anpassade fält i anpassade formulär med flera objekt](#calculated-custom-fields-in-multi-object-custom-forms) i den här artikeln.

### Separera artiklar med punkter

När du refererar till ett relaterat objekt i ett beräknat anpassat fält måste du separera objektnamn och attribut med punkter.

Om du till exempel vill visa namnet på Portfolio-ägaren i ett beräknat anpassat fält i ett anpassat formulär av uppgiftstyp skriver du följande:

`{project}.{porfolio}.{owner}`

Detta skulle avgöra följande: Från objektet i det anpassade formuläret (en uppgift) kan du komma åt nästa objekt som är relaterat till uppgiften (ett projekt). Därifrån kan du komma åt nästa relaterade objekt till projektet (en portfölj) och sedan nästa relaterade objekt till portföljen (ägaren).

### Namnsyntax för att referera till ett anpassat fält

När du refererar till ett annat anpassat fält i ett beräknat anpassat fält måste du ange fältets namn så som det visas i Workfront användargränssnitt.

Om du till exempel vill referera till det valda alternativet i ett anpassat fält med namnet Executive sponsor skriver du följande:

`{DE:Executive sponsor}`

>[!NOTE]
>
>Syntaxen för ett texthuvudfält skiljer sig lite från den för andra typer av fält eftersom du måste lägga till `:name` i slutet.
>
>Om du till exempel vill referera till det valda alternativet i ett anpassat typsnittsfält med namnet&quot;Executive sponsor&quot; skriver du:
>
>`{DE:Executive sponsor:name}`


## Beräknade anpassade fält i anpassade formulär med flera objekt {#calculated-custom-fields-in-multi-object-custom-forms}

I ett anpassat formulär med flera objekt måste de valda objekttyperna vara kompatibla med alla fält som refereras i formulärets beräknade anpassade fält. Om det finns inkompatibilitet visas ett meddelande som varnar dig om att göra ändringar.

>[!INFO]
>
>**Exempel:**
>
>I ett anpassat formulär som är konfigurerat att fungera med aktivitetsobjekttypen skapar du ett beräknat anpassat fält med namnet In Charge. Du konfigurerar det så att det refererar till det inbyggda fältet så att det kan visa namnet på den primära tilldelade personen när formuläret är kopplat till en uppgift:
>
>`{assignedTo}.{name}`
>
>Senare lägger du till objekttypen i det anpassade formuläret. Ett varningsmeddelande anger att projektobjekttypen inte är kompatibel med det beräknade anpassade fältet.

När detta inträffar kan du göra något av följande:

* Ta bort ett av de två inkompatibla objekten från det anpassade formuläret, antingen objekttypen eller det refererade beräknade anpassade fältet.
* Behåll båda objekten och använd filtret för jokertecken `$$OBJCODE` som ett villkor i ett IF-uttryck för att skapa två olika versioner av fältet I Charge. Detta gör att fältet kan fungera utan problem, oavsett vilken typ av objekt formuläret är kopplat till.

>[!INFO]
>
>**Exempel:** Även om det inte finns något tilldelat till: Namnfält i projekt innehåller ett inbyggt ägarfält (som automatiskt fyller i med namnet på den person som skapade projektet, såvida inte någon ändrar detta manuellt).
>
>Så i ditt anpassade avgiftsfält kan du använda `$$OBJCODE` så som visas nedan för att hänvisa till fältet Ägare när det anpassade formuläret bifogas till ett projekt och fältet Tilldelad till: Namnfält när formuläret är kopplat till en uppgift:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Mer information om variabler som `$$OBJCODE,` se [Variabler för jokertecken](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Automatiska uppdateringar av beräknade anpassade fält

Beräknade anpassade fält i ett objekt beräknas om automatiskt när följande inträffar:

* Något på objektet ändras, till exempel en daglig tidslinjeberäkning.
* Någon redigerar ett annat fält som refereras av ett beräknat anpassat fält i objektet.
* Det beräknade uttrycket är tomt och fältet innehåller ett värde. Värdet ställs in på null.

   >[!NOTE]
   >
   ><div>I ett anpassat formulär som bifogas till ett objekt beräknas och sparas datum- och tidssatser i beräknade anpassade fält med UTC (Coordinated Universal Time), inte med de tidszonskonfigurationer som angetts för organisationens instans och din användarprofil. Beräkningar i ett anpassat formulär genereras baserat på varje användares enskilda tidszoner.</div>

