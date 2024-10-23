---
title: Skapa ett eget formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan utforma ett anpassat formulär med formulärdesignern. Du kan koppla anpassade formulär till olika Workfront-objekt för att samla in data om dessa objekt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '5537'
ht-degree: 0%

---

# Skapa ett anpassat formulär

Du kan utforma ett anpassat formulär med formulärdesignern i Adobe Workfront. Du kan koppla anpassade formulär till olika Workfront-objekt för att samla in data om dessa objekt.

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

## Börja utforma ett anpassat formulär

{{step-1-to-setup}}

1. Klicka på **Egen Forms** i den vänstra panelen.

1. Klicka på **Nytt anpassat formulär.**
1. Välj vilka objekttyper du vill koppla det anpassade formuläret till och klicka sedan på **Fortsätt**.

   ![](assets/choose-object-type.jpg)

1. Skriv den anpassade formulärtiteln i området **Titel krävs**.
1. (Valfritt) Om du vill lägga till fler objekttyper i formuläret så att det kan kopplas till fler objekt klickar du på ikonen **Lägg till** ![](assets/add-objects-icon.png) efter **objekttyper** och väljer sedan önskad typ på menyn som visas. Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.

   Du kan också klicka på X för en objekttyp för att ta bort den från formuläret.

   >[!CAUTION]
   >
   >Om du tar bort ett anpassat formulär tas även alla anpassade data bort från objekten som är kopplade till formuläret. Det går inte att återställa borttagna data. Överväg att inaktivera ett anpassat formulär i stället. När du inaktiverar ett anpassat formulär som du inte längre använder behåller du alla tillhörande historiska data.
   >
   >Mer information finns i [Lägga till eller ta bort objekttyper från ett befintligt anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) och [Inaktivera eller återaktivera ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. Sedan kan du börja lägga till fält i det anpassade formuläret. Se följande avsnitt:
   * [Återanvända ett befintligt fält eller en befintlig widget som redan används i ett annat anpassat formulär](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Kommentarer till fältnamn och etiketter](#notes-on-field-names-and-labels)
   * [Lägg till textfält](#add-text-fields)
   * [Lägg till beräknade fält](#add-calculated-fields)
   * [Lägga till alternativknappar, kryssrutegrupper och listrutor](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Lägg till rubriker och datumfält](#add-typeahead-and-date-fields)
   * [Lägg till externa sökfält](#add-external-lookup-fields)
   * [Lägga till bilder, PDF och videoklipp](#add-images-pdfs-and-videos)
   * [Lägg till inbyggda Workfront-fält](#add-workfront-native-fields)
   * [Lägg till Adobe XD-filer](#add-adobe-xd-files)
     <!--* [Add Planning connection fields](#add-planning-connection-fields)-->

## Lägg till nya eller befintliga fält i det anpassade formuläret

Du kan använda nya eller befintliga fält när du utformar ditt anpassade formulär.

Anpassade formulär är begränsade till 500 fält. En räknare längst ned till vänster visar hur många fält som används i formuläret, och den visas alltid när du rullar i formulärdesignern.

### Återanvända ett befintligt fält eller en befintlig widget som redan används i ett annat anpassat formulär

1. Klicka på **Fältbibliotek** på skärmens övre vänstra sida.

1. Dra fältet eller widgeten hit du vill ha den i det anpassade formuläret.
1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   >[!NOTE]
   >
   >Du kan lägga till upp till 500 fält och widgetar i ett anpassat formulär. Prestandaförsämringen kan dock inträffa när det finns mer än 100 blanketter, beroende på hur komplex den är.
   >
   >
   >Exempel på komplexa formulär är formulär med överlappande parametrar, beräknade anpassade datafält och flera värdealternativ i ett enda fält.

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

### Kommentarer till fältnamn och etiketter {#notes-on-field-names-and-labels}

**label** är tillgänglig för de flesta fält. Det är en beskrivande etikett som visas ovanför fältet eller widgeten i det anpassade formuläret. Du kan när som helst ändra etiketten.

>[!NOTE]
>
>Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.

Ett **namn** krävs för varje fält. Det här namnet är det som identifierar det anpassade fältet när du lägger till det i olika områden i Workfront, till exempel rapporter, Hem och API-interaktioner. När du konfigurerar fältet eller widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.

Varje anpassat fältnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär.

>[!NOTE]
>
>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront.
>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.
>
>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.
>
>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.

Följande specialtecken stöds inte i anpassade fältetiketter och namn.

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### Lägg till textfält

Du kan lägga till flera olika textfält i ett anpassat formulär.

+++ **Utöka för att visa beskrivningar av tillgängliga textfält**

* **Textfält med en rad**: Tillåter användare att skriva en enda textrad i fältet.
* **Styckefält**: Tillåter användare att skriva flera rader med text i fältet.
* **Textfält med formatering**: Används för att skriva flera textrader i fältet och formatera texten med fet, kursiv, understrykning, punkter, numrering, hyperlänkar och blockcitattecken. En teckengräns på 15 000 tillåter mycket text och formatering.

  Den här anpassade fälttypen stöds inte i filter för listor och rapporter.

  Mer information om hur du får åtkomst till det här fältet via API finns i [RTF-fältslagring i API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >Textfält med formatering är inte tillgängliga för Workfront mobilappar (i kommande versioner).

* **Beskrivande text**: Gör att du kan inkludera instruktioner och länka till sidor utanför Workfront.

+++

Lägga till ett textfält:

1. Leta upp ett av följande textfält till vänster på skärmen och dra det till ett avsnitt på arbetsytan:

   * Enkelradig text
   * Stycke
   * Text med formatering
   * Beskrivning

   ![](assets/drag-field-to-section.png)

1. Till höger på skärmen konfigurerar du de alternativ som är tillgängliga för den typ av anpassat fält som du lägger till:

   <table>
    <tr>
    <td>Indata till</td>
    <td>Beskrivning</td>
    <td>Finns för </td>
    </tr>
    <tr>
    <td>Storlek</td>
    <td><p>Ändra storleken på textfälten i formuläret.<p>
   </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycke</li>
    <li>Text med formatering</li>
    <li>Beskrivning</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etikett</td>
    <td><p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför fältet. Du kan när som helst ändra etiketten.<p>
    <p>VIKTIGT: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p></td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycke</li>
    <li>Text med formatering</li>
    </ul></td>
    </tr>
    <tr>
     <td>Namn</td>
    <td><p>(Obligatoriskt) Det här namnet är det som identifierar fältet. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p>
    <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p>
    </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycke</li>
    <li>Text med formatering</li>
    <li>Beskrivning</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instruktioner</td>
    <td>Ange eventuell ytterligare information om fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycke</li>
    <li>Text med formatering</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Välj den typ av data som ska hämtas i det anpassade fältet.</p> <p><b>OBS</b>:   
    <ul> 
    <li>Det går inte att redigera det här fältet efter att formuläret har sparats. Om du tänker använda fältet i matematiska beräkningar måste du välja ett tal- eller valutaformat.</li> 
    <li>När du väljer Nummer eller Valuta kortas nummer som börjar med 0 automatiskt av systemet.</li>
    <li>Teckengränsen för nummerfält är 16. Du kan också använda ett textfält för att ange tal och undvika gränsen.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycke</li>
    </ul></td>
    </tr>
    <tr>
    <td>Visningstyp</td>
    <td>Växla mellan textrutorna för en rad och ett stycke.</td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycke</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlänk</td>
    <td> Om du vill använda en hyperlänk i den beskrivande texten lägger du till den här. Den beskrivande texten visas som en länk på objekt som formuläret är kopplat till.</td>
    <td><ul><li>Beskrivning</li></ul></td>
    </tr>
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopiera ikon](assets/copy-field.png)

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

### Lägg till beräknade fält

I ett anpassat formulär kan du lägga till ett beräknat anpassat fält som använder befintliga data för att generera nya data när det anpassade formuläret kopplas till ett objekt.

Mer information om hur du lägger till ett beräknat fält finns i [Lägga till beräknade fält med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Lägga till alternativknappar, kryssrutegrupper och listrutor

Du kan lägga till alternativknappar, kryssrutegrupper, listrutor och flervalslistrutor i ett anpassat formulär.

+++ **Utöka för att visa beskrivningar av tillgängliga fält**

* **Alternativknappar**: Kräver att användare bara väljer ett alternativ.
* **Kryssrutegrupp**: Tillåter användare att välja flera alternativ.
* **Listruta för enstaka val**: Visar en lista med alternativ i listrutor.
* **Flervalsmeny**: Tillåter användare att välja flera alternativ i en listruta.

+++

>[!NOTE]
>
>Fält som tillåter flera val, som kryssrutegrupp och flervalslistruta, är svåra att schemalägga och gruppera i rapporter. Om du vill att det ska vara enklare att rita och gruppera i rapporter kan du skapa separata fält för varje val (till exempel ett textfält med en rad).

Så här lägger du till alternativknappar, kryssrutegrupper och listrutor:

1. Leta upp ett av följande fält till vänster på skärmen och dra det till ett avsnitt på arbetsytan.

   * Alternativknappar
   * Kryssrutegrupp
   * Listruta med ett val
   * Listruta för flera val

   ![Dra ett fält till arbetsytan](assets/drag-field-to-section.png)

1. Till höger på skärmen konfigurerar du de alternativ som är tillgängliga för den typ av anpassat fält som du lägger till:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Indata till</td>
    <td>Beskrivning</td>
    <td>Finns för </td>
    </tr>
    <tr> 
     <td role="rowheader">Etikett</td> 
     <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Namn</td> 
     <td> <p>(Obligatoriskt) Det här namnet är det som identifierar fältet. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> 
    <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td>
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instruktioner</td> 
    <td> <p>Ange eventuell ytterligare information om det anpassade fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Välj den typ av data som ska hämtas i det anpassade fältet.</p> <p><b>OBS</b>:   
     <ul> 
    <li>Det går inte att redigera det här fältet efter att formuläret har sparats. Om du tänker använda fältet i matematiska beräkningar måste du välja ett tal- eller valutaformat.<br></li> 
    <li>När du väljer Nummer eller Valuta kortas nummer som börjar med 0 automatiskt av systemet.</li>
    <li>Teckengränsen för nummerfält är 16. Du kan också använda ett textfält för att ange tal och undvika gränsen.</li>
     </ul></p></td> 
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Visningstyp</td> 
    <td>Växla mellan alternativknappar, kryssrutegrupper, listrutor för enstaka val eller listrutor för flera val för fältet.</td> 
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Gör ett obligatoriskt fält</td> 
    <td>Välj det här alternativet om du vill att fältet ska vara obligatoriskt för att användaren ska kunna fylla i det anpassade formuläret. </td> 
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Val </td> 
    <td> 
    <ol> 
    <li> <p>Klicka på <b>Alternativ</b> och aktivera sedan något av följande:</p> 
    <ul> 
    <li><strong>Visa värden</strong>: Visar värdena för varje alternativ i fältet. Etiketten för varje val visas som standard.</li> 
     <li><strong>Sorteringsalternativ A-Z</strong>: Sorterar de alternativ du lägger till i bokstavsordning i fältet.</li> 
    </ul> 
    </li> 
    <li> <p>För varje val som du lägger till för användaren klickar du på kugghjulsikonen <img src="assets/gear-icon-settings.png"> och väljer sedan något av följande alternativ:</p> 
    <ul> 
    <li><strong>Välj som standard</strong>: Välj alternativet som standard i fältet.</li> 
    <li> <p><strong>Dölj alternativ</strong>: Dölj alternativet i fältet. Dolda alternativ är fortfarande tillgängliga i rapporter.</p> </li> 
    <li> <p><strong>Ta bort alternativ</strong>: Ta bort alternativet från fältet.</p> <p><b>VARNING</b>: Om du har aktuella objekt som använder det här alternativet ska du inte ta bort det från fältet. Om du tar bort den går historikdata förlorade. Välj i stället alternativet att dölja det, vilket förhindrar att användarna väljer det i framtiden.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta med ett val</li>
    <li>Listruta för flera val</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopiera ikon](assets/copy-field.png)

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

### Lägg till rubriker och datumfält

Du kan lägga till huvud- och datumfält i ett anpassat formulär.

+++ **Utöka för att visa beskrivningar av tillgängliga fält**

* **Typhead**: Tillåter användare att skriva namnet på ett objekt som finns i Workfront. En lista med förslag visas när användaren börjar skriva. Den här fälttypen har stöd för följande objekt:
   * Användare
   * Grupp
   * Jobbroll
   * Portfolio
   * Program
   * Projekt
   * Team
   * Mall
   * Företag
* **Datum**: Visar en kalender där användare kan välja datum och tid.

+++

Så här lägger du till texthuvud- och datumfält:

1. Leta upp ett av följande fält till vänster på skärmen och dra det till ett avsnitt på arbetsytan.

   * Typeahead
   * Datum

   ![](assets/drag-field-to-section.png)

1. Till höger på skärmen konfigurerar du de alternativ som är tillgängliga för den typ av anpassat fält som du lägger till:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Fältinställning</td>
    <td>Beskrivning</td>
    <td>Finns för </td>
    </tr>
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar fältet. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> 
      <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td>
    <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Ange eventuell ytterligare information om det anpassade fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Visa tid på dagen</td> 
      <td>Välj det här alternativet om du vill visa tiden på dagen tillsammans med datumet i fältet.</td> 
         <td><ul>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Refererad objekttyp</td> 
      <td> <p>Markera den objekttyp som du vill associera med fältet.</p> <p>När du har klickat på Använd eller Spara+Stäng kan du inte ändra fälttypen.</p> <p><b>OBS</b>:   
        <ul> 
         <li>Om Workfront-administratören har anpassat namnet på Portfolio, Program eller Projekt i Workfront användargränssnitt, visas Workfront-standardnamnet för objektet i den här listrutan, inte det anpassade namnet. Kontakta Workfront-administratören om du behöver hjälp med detta.<br></li> 
         <li>Följande objekttyper stöds i iOS och Android Workfront Mobile Apps: User, Company, Group, Job Role, Portfolio, Program, Project och Template.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Lägg till filter</td>
      <td><p>Lägg till ett filter för en objekttyp för att begränsa vilka objekt som användare kan välja när de använder fältet. </p> <p>Du kan till exempel begränsa ett fält så att användarnamn bara kan väljas om de uppfyller följande villkor:</p> 
       <ul> 
        <li>De tillhör en grupp eller grupper som du anger</li> 
        <li>De är kopplade till en roll eller jobbtitel som du anger</li> 
        <li>De tillhör samma grupp som den person som använder fältet</li> 
       </ul> <p>Du måste definiera filtret för den objekttyp som du har valt med syntaxen för textläge. Mer information om hur du skapar ett filter i textläge finns i <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Redigera ett filter i textläge</a>.</p>
       <p><b>OBS</b>:
       <ul> 
        <li>Om du redigerar ett befintligt anpassat formulär och lägger till ett filter i ett texthuvudfält, tas inga objekt bort (utanför filteromfånget) som användare redan har lagt till med fältet.</li> 
        <li>Filtret är inte tillgängligt på mobila enheter. Om du använder filtret för ett Typeahead-fält visas fältet på användarens mobila enheter som inte påverkas av filtret.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Typeahead</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Gör ett obligatoriskt fält</td> 
      <td>Välj det här alternativet om du vill att fältet ska vara obligatoriskt för att användaren ska kunna fylla i det anpassade formuläret. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopiera ikon](assets/copy-field.png)

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

### Lägg till externa sökfält

Ett externt uppslagsfält anropar ett externt API och returnerar värden som alternativ i ett nedrullningsbart fält. Användare som arbetar med objektet som det anpassade formuläret är kopplat till kan välja ett eller flera av dessa alternativ i listrutan. Det externa sökfältet är också tillgängligt i listor och rapporter.

Exempel på hur du använder det externa sökfältet för att anropa samma instans av Workfront eller ett offentligt API finns i [Exempel på det externa sökfältet i ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* Externa sökfält stöds inte i Outlook-plugin-programmet.
>* Externa sökfält är inte tillgängliga i listor när fältet är beroende av ett annat fält.

Så här lägger du till en extern sökning:

1. Leta upp **extern sökning** till vänster på skärmen och dra den till ett avsnitt på arbetsytan.
1. Konfigurera alternativen för det anpassade fältet till höger på skärmen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar fältet. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p>
      <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td>
     </tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Ange eventuell ytterligare information om det anpassade fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td>
      <td><p>Välj den typ av data som ska hämtas i det anpassade fältet.</p>
      <p><strong>OBS!</strong></p>
      <ul><li>Du kan ändra formattyp när formuläret har sparats, med en begränsning: Alla befintliga värden på objekt måste kunna konverteras till den nya typen. (Om formattypen till exempel är Text och ett objekt lagrar värdet "abc", kan du inte konvertera fältet och får ett felmeddelande om att systemet inte kan konvertera "abc" till tal/valuta.) Om du tänker använda fältet i matematiska beräkningar måste du välja ett tal- eller valutaformat.</li>
      <li>När du väljer Nummer eller Valuta kortas nummer som börjar med 0 automatiskt av systemet.</li>
      <li>Teckengränsen för nummerfält är 16. Du kan också använda ett textfält för att ange tal och undvika gränsen.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Bas-API-URL</td> 
      <td><p>Skriv eller klistra in URL:en för API:t.</p><p>API-URL:en måste returnera ett JSON-innehåll av de alternativ som du vill visa i listrutan. Du kan använda fältet JSON-sökväg för att välja specifika värden från den returnerade JSON-filen som ska vara listrutealternativ.</p><p>När du anger API-URL:en kan du välja att skicka följande värden i URL:en:</p>
      <ul>
      <li>$$HOST - Detta representerar den aktuella Workfront-värden och kan användas för att göra /search API-anrop till Workfront API. När jokertecknet används hanteras autentiseringen och användarna behöver inte skicka autentiseringshuvuden. (Användare kan t.ex. söka efter uppgifter med bas-URL:en <code>$$HOST/attask/api/task/search</code> och kan söka efter uppgifter och välja värden från en returnerad lista med uppgifter.)</li>
      <li><p>$$QUERY - Detta representerar den söktext som slutanvändaren skriver i fältet och gör att du kan implementera frågefiltrering för slutanvändarna. (Användaren söker efter värdet i listrutan.)</p>
      <p>Om API:t som du refererar till tillåter det kan du även inkludera modifierare i sökfrågan för att identifiera hur sökningen ska fungera. Du kan t.ex. använda följande som bas-API-URL för att tillåta användare att söka efter Workfront-projekt som innehåller viss text: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Läs mer om Workfront sökmodifierare i <a href="/help/quicksilver/wf-api/general/api-basics.md">API Basics</a>.</p>
      <p><strong>OBS!</strong> Om du inte använder $$QUERY och användartyptexten i sökrutan begränsas de val du redan har. Om du däremot använder $$QUERY och användaren skriver något, utförs ett nytt nätverksanrop till ditt API. Om du har fler än 2 000 värden i API:t, och API:t stöder frågor, kan du använda $$QUERY för att inte bara söka efter befintliga 2 000-värden, utan även från det ursprungliga API:t med de begränsade alternativen.</p></li>
      <li><p>{fieldName} - Där fieldName är ett anpassat eller inbyggt fält i Workfront. På så sätt kan du implementera filtren för överlappande listrutor när du skickar värdet för ett redan markerat fält till fältet för extern sökning för att filtrera ned alternativen. (Fältet Region finns till exempel redan i formuläret och du begränsar en lista med länder från API:t till de som finns i en viss region.)</p>
      <p>För ett externt uppslagsfält som är beroende av andra fält (med syntaxen {fieldName}) är alternativen som returneras från API begränsade till dem som matchar alla strängar eller värden som anges i de andra fälten. (Den här funktionen stöds inte i listor och rapporter.)</p></li>
      <li>{referenceObject}.{fieldName} - Där fältet ingår i ett objekt. Syntaxen liknar anpassade uttryck. (Till exempel portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>OBS!</strong> Granska dokumentationen för API:t som du arbetar med för de specifika frågor som du kan definiera.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP-metod</td> 
      <td>Välj <strong>Get</strong>, <strong>Post</strong> eller <strong>Put</strong> som metod.</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON-sökväg</td>
      <td><p>Skriv eller klistra in JSON-sökvägen för API:t.</p> <p>Med det här alternativet kan data extraheras från den JSON som returneras av API-URL:en. Det är ett sätt att välja vilka värden från JSON som ska visas i listrutealternativen.</p><p>Om din API-URL till exempel returnerar JSON i det här formatet:</br>
      <pre>
      {
       data: {
         { name: "USA"},
         { name: "Canada"}
       }
      }
      </pre>
      </p>
      <p>kan du använda "$.data[*].name" för att välja USA och Kanada som listrutealternativ.</p> <p>Mer information om JSON-sökvägen och hur du ser till att du skriver rätt JSON-sökväg finns på <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Sidhuvuden</td>
      <td><p>Klicka på <strong>Lägg till huvud</strong> och skriv eller klistra in det nyckel/värde-par som krävs för autentisering med API:t.</p><p><strong>Obs!</strong> Rubrikfälten är inte en säker plats där du kan lagra autentiseringsuppgifter, och du bör vara försiktig med vad du anger och sparar.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Flervalsmeny</td>
      <td><p>Välj det här alternativet om du vill tillåta användaren att välja mer än ett värde i listrutan.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">Gör ett obligatoriskt fält</td>
      <td><p>Välj det här alternativet om du vill att fältet ska vara obligatoriskt för att användaren ska kunna fylla i det anpassade formuläret.</p></td>
     </tr>       
    </tbody>
   </table>

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

>[!NOTE]
>
>Följande objekt är tekniska begränsningar för anropet till det externa API:t:
>
>* Maximalt antal alternativ: 2 000 (endast de första 2 000 unika alternativen från det returnerade JSON visas)
>* Timeout: 3 sekunder
>* Antal återförsök: 3
>* Väntetid mellan återförsök: 500 ms
>* Förväntad svarsstatus: 2xx

### Lägga till bilder, PDF och videoklipp

Du kan lägga till bilder, PDF och videoklipp i ett anpassat formulär. Användare som arbetar med det objekt som det anpassade formuläret är kopplat till kan endast se bild, PDF eller video i följande områden:

* Objektets detaljområde (t.ex. området Projektinformation för ett projekt)
* Rutan Redigera för objektet, om det har det nya Adobe Workfront-gränssnittet (t.ex. rutorna Redigera projekt och Redigera uppgift)

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Utöka för att visa beskrivningar av tillgängliga fält**

* **Bild**: Tillåter användare att lägga till bildfiler.
* **PDF**: Tillåter användare att lägga till PDF
* **Videor**: Tillåter användare att lägga till videofiler.

+++

Så här lägger du till bilder, PDF eller videofilmer:

1. Leta upp ett av följande fält till vänster på skärmen och dra det till ett avsnitt på arbetsytan.

   * Bild
   * PDF
   * Video

   ![](assets/drag-field-to-section.png)

1. Ange eller redigera någon av följande egenskaper för widgeten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar widgeten. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoriskt) Skriv eller klistra in URL:en för widgeten där den lagras på Internet.</p> 
      <p>Om du lägger till en videowidget kan du göra det genom att lägga till följande i URL-rutan:</p> 
      <ul> 
      <li> <p>Länk till YouTube eller Vimeo</p> </li> 
      <li> <p>Google Drive - videolänk</p> </li> 
      <li> <p>Länka till video med MP4- och MOV-tillägg</p> </li> 
      <li> <p>Länk till video som redan har överförts till dokumentområdet i din Workfront-instans. Instruktioner finns i <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Lägga till en videowidget i ett anpassat formulär i området Dokument</a> i den här artikeln.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Skriv in ytterligare information om widgeten. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Storlek</td> 
      <td>Ändra visningsstorleken för widgeten efter behov.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopiera ikon](assets/copy-field.png)

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

#### Lägga till en videowidget i ett anpassat formulär från området Dokument{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>När du lägger till en video i ett anpassat formulär på det här sättet gäller endast de behörigheter som angetts för det anpassade formuläret för videon när användarna öppnar formuläret för ett objekt, inte de behörigheter som angetts för videon i området Dokument.

1. Gå till videon i området Dokument och generera ett korrektur för den, enligt beskrivningen i [Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öppna beviset.
1. Högerklicka var som helst i videon och välj sedan **Kopiera videoadress**.
1. Klistra in den kopierade adressen i rutan **URL** i det anpassade formuläret där du lägger till videowidgeten.
1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

### Lägg till inbyggda Workfront-fält

Du kan lägga till inbyggda Workfront-fält i dina anpassade formulär. När det anpassade formuläret bifogas till ett objekt fylls fältet i från objektdata. Fältet Beskrivning i ett anpassat formulär som är kopplat till ett projekt hämtas till exempel i projektbeskrivningen. (Fältet kan visa &quot;Ej tillämpligt&quot; om inga data är tillgängliga.)

+++ **Expandera om du vill visa en lista över inbyggda fält som stöds**

I den här tabellen visas de tillgängliga inbyggda fälten för specifika Workfront-objekt i ett anpassat formulär.

| Fältnamn | Projekt | Uppgift | Problem | Mall | Malluppgift | Portfolio | Program | Grupp |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Faktiskt slutförandedatum | ✓ | ✓ | ✓ |   |   |   |   |   |
| Faktisk varaktighet | ✓ |   |   |   |   |   |   |   |
| Faktiska timmar | ✓ |   | ✓ |   |   |   |   |   |
| Faktiskt startdatum | ✓ | ✓ | ✓ |   |   |   |   |   |
| Företag | ✓ |   |   | ✓ |   |   |   |   |
| Villkor | ✓ | ✓ | ✓ |   |   |   |   |   |
| Villkorstyp | ✓ |   |   | ✓ |   |   |   |   |
| Beskrivning | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Varaktighet |   | ✓ |   |   | ✓ |   |   |   |
| Varaktighetstyp |   | ✓ |   |   | ✓ |   |   |   |
| Varaktighetsenhet |   | ✓ |   |   | ✓ |   |   |   |
| Anges av | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Anmälningsdatum | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Grupp | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Senast uppdaterad av | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Senaste uppdateringsdatum | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Namn | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Ägare | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Planerat slutförandedatum | ✓ | ✓ | ✓ |   |   |   |   |   |
| Planerad varaktighet | ✓ |   |   | ✓ |   |   |   |   |
| Planerade timmar | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Planerat startdatum | ✓ |   |   |   |   |   |   |   |
| Portfolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Prioritet | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Program | ✓ |   |   | ✓ |   |   |   |   |
| Planerat slutförandedatum | ✓ | ✓ |   |   |   |   |   |   |
| Planerad varaktighet, minuter |   | ✓ |   |   |   |   |   |   |
| Planerat startdatum | ✓ | ✓ |   |   |   |   |   |   |
| Referensnummer | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Schemaläge | ✓ |   |   | ✓ |   |   |   |   |
| Allvarlighetsgrad |   |   | ✓ |   |   |   |   |   |
| Sponsorn | ✓ |   |   | ✓ |   |   |   |   |
| Status | ✓ | ✓ |   |   |   |   |   |   |
| Artikelpunkter |   | ✓ |   |   |   |   |   |   |
| Mall | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. På skärmens vänstra sida letar du reda på **Ursprunglig fältreferens** och drar den till ett avsnitt på arbetsytan.
1. Konfigurera alternativen för det anpassade fältet till höger på skärmen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td>
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar fältet. När du konfigurerar fältet för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p>
      <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Ange eventuell ytterligare information om fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Referensfält</td> 
      <td><p>(Obligatoriskt) Välj ett internt Workfront-fält.<p><p>Endast inbyggda fält för formulärets objekt är tillgängliga. Om t.ex. listan Objekttyper längst upp i formulärdesignern visar Projekt, kan du välja inbyggda fält för projekt, men inte fält som är specifika för uppgifter.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Storlek</td> 
      <td>(Valfritt) Ändra fältets visningsstorlek efter behov.</td> 
     </tr> 
    </tbody> 
   </table>

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

### Lägg till Adobe XD-filer

Du kan lägga till en Adobe XD-prototyp direkt i ett anpassat formulär. Användare som arbetar med det objekt som det anpassade formuläret är kopplat till kan bara se Adobe XD-filen i följande områden:

* Objektets detaljområde (t.ex. området Projektinformation för ett projekt)
* Rutan Redigera för objektet, om det har det nya Adobe Workfront-gränssnittet (t.ex. rutorna Redigera projekt och Redigera uppgift)

Lägga till en Adobe XD-fil:

1. Leta upp **Adobe XD** till vänster på skärmen och dra den till ett avsnitt på arbetsytan.
1. Ange eller redigera någon av följande egenskaper för widgeten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter. Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar widgeten. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p>
    <p>Mer information finns i <a href="design-a-form.md#notes-on-field-names-and-labels">Anteckningar om fältnamn och etiketter</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoriskt) Skriv eller klistra in en giltig XD prototyplänk.</p> 
      <p>Obs! Inställningen Länkåtkomst på fliken Dela i Adobe XD måste vara inställd på Vem som helst med länken. Annars kan användarna inte visa prototypen. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Skriv in ytterligare information om widgeten. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Storlek</td> 
      <td>(Valfritt) Ändra visningsstorleken för widgeten efter behov.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopiera ikon](assets/copy-field.png)

1. Om du vill spara ändringarna klickar du på **Använd** och går vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

<!--
### Add Planning connection fields

>[!IMPORTANT]
>
>The information in this section refers to Adobe Workfront Planning, an additional capability from Adobe Workfront. 
>
>You must have the following to access Workfront Planning:
>
>* A new Workfront plan and license. Workfront Planning is not available for legacy Workfront plans or licenses. 
>* An additional license for Workfront Planning. 
>* Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.
>
> For a complete list of requirements to access Workfront Planning, see [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md). 
> 
>For more information about Workfront Planning, see [Adobe Workfront Planning overview](/help/quicksilver/planning/general/planning-overview.md).

You can view records connected from Workfront Planning in a custom field on a Workfront object by adding a  Planning connection custom field to an object's custom form. 

You can add the Planning connection field to all objects' custom forms. However, you can display connected records only on the custom forms associated with Workfront objects that can be connected from Workfront Planning. 

>[!NOTE]
>
>Users viewing information in the custom field must have access to Workfront Planning and to the workspaces that contain the record types connected to Workfront objects.


To add a Planning connection field:

1. On the left side of the screen, find **Planning connection** and drag it to a section on the canvas. 
1. On the right side of the screen, configure the options for the custom field:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Required) Type a descriptive label to display above the field. You can change the label at any time.</p> <p><b>IMPORTANT</b>:</p> <p>Avoid using special characters in this label.</p> 
      <p>We recommend that you choose a label by which you can easily identify where the Planning record is coming from. Add information like the name of the workspace or the name of the record type. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td>
      <td> <p>(Required) The name is how the system identifies the field. When you are configuring the field for the first time and you type the label, the Name field populates automatically to match it. But the Label and Name fields are not synchronized—this gives you the freedom to change the label that your users see without having to change the name that the system sees.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructions</td> 
      <td> <p>(Recommended) Type any additional information about the field. When users fill out the custom form, they can hover over the question mark icon to view a tool tip containing the information you type here.</p>
      <p>Here, you can add explicit information about the record and the objects you are connecting. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Object type</td> 
      <td><p>(Required) Select a Workfront object type that is connected to a record type in Workfront Planning.</p>
      You may select from the following object types:
      <ul><li> Project</li>
      <li> Portfolio</li><li> Program</li><li> Company</li><li> Group</li></ul>
       <p>Only Workfront object types for the form's object types are available.</p> <p> For example, if the Object Types list at the top of the form designer shows Project, you can only select Project in this field, and you cannot select Portfolios, although portfolios can also be connected to record types.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Workspace</td> 
      <td> <p>(Required) Select the workspace where the records you want to display in Workfront come from in Workfront Planning.</p> <p> Only workspaces that are connected to the object types you selected in the I=Object type field display. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Record Type</td> 
      <td><p>(Required) Select the Workfornt Planning record type whose records are connected to the Workfront object associated with this form.</p><p>Only record types that have connections to the object type you selected in the Object type field display. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Connection field</td> 
      <td><p>(Required) Select the Workfront Planning connection field that displays the Workfront objects that are associated with this form.</p> <p> <b>NOTE</b></p><p>You can have multiple connection fields between the same object and record types.</p>  </td> 
     </tr>
    </tbody> 
   </table>

1. (Optional) Repeat the previous steps to add any other fields. 

    or

    To copy a field, hover over a field, and click the copy icon.

    ![copy icon](assets/copy-field.png)

1. To save your changes, click **Apply** and move on to another section to continue building your form.

    or

    Click **Save and Close**.

    You can now attach the form to an object connected from Workfront Planning and do one of the following:

    * View Workfront Planning record types connected to the Workfront object
    * Connect or disconnect records from the Workfront object associated with the form. 

    For more information, see [Manage record connections from Workfront objects](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

-->

## Organisera och förhandsgranska ett formulär med formulärdesignern

Mer information om hur du organiserar ett anpassat formulär med avsnittsbrytningar och ser en förhandsgranskning av formuläret finns i [Ordna och förhandsgranska ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
