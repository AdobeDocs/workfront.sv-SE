---
title: Designa ett formulär med formulärdesignern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan utforma ett anpassat formulär med formulärdesignern.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '4918'
ht-degree: 0%

---

# Designa ett formulär med formulärdesignern

Du kan utforma ett anpassat formulär med formulärdesignern. Du kan koppla anpassade formulär till olika Workfront-objekt för att samla in data om dessa objekt.

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
   <td>
   <p>Ny plan: Standard</p>
   <p>eller</p>
   <p>Aktuell plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer beviljar den här åtkomsten finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Börja utforma ett anpassat formulär

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** till vänster.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klicka **Nytt anpassat formulär.**
1. Välj vilka objekttyper du vill bifoga det anpassade formuläret till och klicka sedan på **Fortsätt**.

   ![](assets/choose-object-type.jpg)

1. I **Namn krävs** anger du den anpassade formulärtiteln.
1. (Valfritt) Om du vill lägga till fler objekttyper i formuläret så att det kan kopplas till fler objekt klickar du på **Lägg till** icon ![](assets/add-objects-icon.png) efter **Objekttyper** väljer du sedan önskad typ på menyn som visas. Du kan upprepa detta om du vill lägga till så många objekttyper som du vill.

   Du kan också klicka på X för en objekttyp för att ta bort den från formuläret.

   >[!CAUTION]
   >
   >Om du tar bort ett anpassat formulär tas även alla anpassade data bort från objekten som är kopplade till formuläret. Det går inte att återställa borttagna data. Överväg att inaktivera ett anpassat formulär i stället. När du inaktiverar ett anpassat formulär som du inte längre använder behåller du alla tillhörande historiska data.
   >
   >Mer information finns i [Ta bort objekttyper i ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. Sedan kan du börja lägga till fält i det anpassade formuläret. Se följande avsnitt:
   * [Återanvända ett befintligt fält eller en befintlig widget som redan används i ett annat anpassat formulär](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Lägg till textfält](#add-text-fields)
   * [Lägg till beräknade fält](#add-calculated-fields)
   * [Lägg till alternativknappar, kryssrutegrupp och listrutor](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Lägg till rubriker och datumfält](#add-typeahead-and-date-fields)
   * [Lägga till bilder, PDF och videoklipp](#add-images-pdfs-and-videos)
   * [Lägg till Adobe XD-filer](#add-adobe-xd-files)

## Lägg till nya eller befintliga fält i det anpassade formuläret

Du kan använda nya eller befintliga fält när du utformar ditt anpassade formulär.

## Återanvända ett befintligt fält eller en befintlig widget som redan används i ett annat anpassat formulär

1. Klicka på längst upp till vänster på skärmen **Fältbibliotek**.

1. Dra fältet eller widgeten hit du vill ha den i det anpassade formuläret.
1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   >[!NOTE]
   >
   >Du kan lägga till upp till 500 fält och widgetar i ett anpassat formulär. Prestandaförsämringen kan dock inträffa när det finns mer än 100 blanketter, beroende på hur komplex den är.
   >
   >
   >Exempel på komplexa formulär är formulär med överlappande parametrar, beräknade anpassade datafält och flera värdealternativ i ett enda fält.

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till textfält

Du kan lägga till flera olika textfält i ett anpassat formulär.

+++ **Expandera om du vill visa beskrivningar av tillgängliga textfält**

* **Textfält med en rad**: Användare kan skriva en enda textrad i fältet.
* **Textfält för stycke**: Användare kan skriva flera textrader i fältet.
* **Textfält med formatering**: Används för att skriva flera textrader i fältet och formatera texten med fet, kursiv stil, understrykning, punkter, numrering, hyperlänkar och blockcitattecken. En teckengräns på 15 000 tillåter mycket text och formatering.

  Mer information om hur du får åtkomst till det här fältet via API finns i Lagring av RTF-fält i API:t.

  >[!NOTE]
  >
  >Textfält med formatering är inte tillgängliga för Workfront mobilappar (i kommande versioner).

* **Beskrivning**: Du kan inkludera instruktioner och länka till sidor utanför Workfront.

+++

Lägga till ett textfält:

1. Leta upp ett av följande textfält till vänster på skärmen och dra det till ett avsnitt på arbetsytan:

   * Enkelradstext
   * Stycketext
   * Textfält med formatering
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
    <li>Stycketext</li>
    <li>Text med formatering</li>
    <li>Beskrivande text - kommer snart</li>
    </ul></td>
    </tr>
    <tr>
    <td>Etikett</td>
    <td><p>Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.<p>
    <p>VIKTIGT: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p></td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycketext</li>
    <li>Text med formatering</li>
    </ul></td>
    </tr>
    <tr>
     <td>Namn</td>
    <td><p>(Obligatoriskt) Det här namnet är det som identifierar fältet. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p>
    <p><b>VIKTIGT</b>:   
      <ul> 
      <li>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront. <p>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.</p> </li>
      <li> <p>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.</p> </li>
      <li><p>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.</p></li>
    </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycketext</li>
    <li>Text med formatering</li>
    <li>Beskrivning</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instruktioner</td>
    <td>Skriv in ytterligare information om widgeten. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycketext</li>
    <li>Text med formatering</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Välj den typ av data som ska hämtas i det anpassade fältet.</p> <p><b>ANMÄRKNING</b>:   
    <ul> 
    <li>Det går inte att redigera det här fältet efter att formuläret har sparats. Om du tänker använda fältet i matematiska beräkningar måste du välja ett tal- eller valutaformat.<br></li> 
    <li>När du väljer Nummer eller Valuta kortas nummer som börjar med 0 automatiskt av systemet.</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycketext</li>
    </ul></td>
    </tr>
    <tr>
    <td>Visningstyp</td>
    <td>Växla mellan textrutorna för en rad och ett stycke.</td>
    <td><ul>
    <li>Enkelradig text</li>
    <li>Stycketext</li>
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

   ![kopieringsikon](assets/copy-field.png)

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till beräknade fält

I ett anpassat formulär kan du lägga till ett beräknat anpassat fält som använder befintliga data för att generera nya data när det anpassade formuläret kopplas till ett objekt.

Information om hur du lägger till ett beräkningsfält finns i [Lägg till beräknade fält med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Lägg till alternativknappar, kryssrutor och listrutor

Du kan lägga till alternativknappar, kryssrutor och listrutor i ett anpassat formulär.

+++ **Expandera om du vill visa beskrivningar av tillgängliga fält**

* **Alternativknappar**: Kräver att användarna bara väljer ett alternativ.
* **Kryssrutegrupp**: Tillåter användare att välja flera alternativ.
* **Listruta**: Innehåller en lista med alternativ i listrutan.

+++

>[!NOTE]
>
>Fält som tillåter flera markeringar, som kryssrutegruppen och listrutan, är svåra att schemalägga och gruppera i rapporter. Om du vill att det ska vara enklare att rita och gruppera i rapporter kan du skapa separata fält för varje val (till exempel ett textfält med en rad).

Så här lägger du till alternativknappar och kryssrutor:

1. Leta upp ett av följande fält till vänster på skärmen och dra det till ett avsnitt på arbetsytan.

   * Alternativknappar
   * Kryssrutegrupp
   * Listruta

   ![](assets/drag-field-to-section.png)

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
     <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Namn</td> 
     <td> <p>(Obligatoriskt) Det här namnet är det som identifierar det anpassade fältet när du lägger till det i olika områden i Workfront, till exempel rapporter, Hem- och API-interaktioner.</p> <p>När du konfigurerar det anpassade fältet för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> 
    <p><b>VIKTIGT</b>:   
     <ul> 
    <li>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront. <p>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.</p> </li>
    <li> <p>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.</p> </li>
     <li><p>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.</p></li>
     </ul> <p>Varje anpassat fältnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. Mer information finns i <a href="#Add" class="MCXref xref">Lägga till ett anpassat fält i ett anpassat formulär</a> i den här artikeln.</p> </td>
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
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
    <li>Listruta</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Välj den typ av data som ska hämtas i det anpassade fältet.</p> <p><b>ANMÄRKNING</b>:   
     <ul> 
    <li>Det går inte att redigera det här fältet efter att formuläret har sparats. Om du tänker använda fältet i matematiska beräkningar måste du välja ett tal- eller valutaformat.<br></li> 
    <li>När du väljer Nummer eller Valuta kortas nummer som börjar med 0 automatiskt av systemet.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Visningstyp</td> 
    <td>Växla mellan alternativknappar, kryssrutegrupper, listrutor och flervalslistrutor för fältet.</td> 
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Gör ett obligatoriskt fält</td> 
    <td>Välj det här alternativet om du vill att fältet ska vara obligatoriskt för att användaren ska kunna fylla i det anpassade formuläret. </td> 
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Val </td> 
    <td> 
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
    <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopieringsikon](assets/copy-field.png)

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till rubriker och datumfält

Du kan lägga till huvud- och datumfält i ett anpassat formulär.

+++ **Expandera om du vill visa beskrivningar av tillgängliga fält**

* **Typeahead**: Tillåter användare att skriva namnet på ett objekt som finns i Workfront. En lista med förslag visas när användaren börjar skriva. Den här fälttypen har stöd för följande objekt:
   * Användare
   * Grupp
   * Jobbroll
   * Portfolio
   * Program
   * Projekt
   * Team
   * Mall
   * Företag
* **Datumfält**: Visar en kalender där användare kan välja datum och tid.

+++

Så här lägger du till typsnittsdatumfält:

1. Leta upp ett av följande fält till vänster på skärmen och dra det till ett avsnitt på arbetsytan.

   * Typeahead
   * Datumfält

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
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datumfält</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar det anpassade fältet när du lägger till det i olika områden i Workfront, till exempel rapporter, Hem- och API-interaktioner.</p> <p>När du konfigurerar det anpassade fältet för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> 
      <p><b>VIKTIGT</b>:   
      <ul> 
      <li>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront. <p>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.</p> </li>
      <li> <p>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.</p> </li>
      <li><p>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.</p></li>
      </ul> <p>Varje anpassat fältnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. Mer information finns i <a href="#Add" class="MCXref xref">Lägga till ett anpassat fält i ett anpassat formulär</a> i den här artikeln.</p> </td>
         <td><ul>
    <li>Typeahead</li>
    <li>Datumfält</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Ange eventuell ytterligare information om det anpassade fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Datumfält</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Visa tid på dagen</td> 
      <td>Välj det här alternativet om du vill visa tiden på dagen tillsammans med datumet i fältet.</td> 
         <td><ul>
    <li>Datumfält</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Refererad objekttyp</td> 
      <td> <p>Markera den objekttyp som du vill associera med fältet.</p> <p>När du har klickat på Använd eller Spara+Stäng kan du inte ändra fälttypen.</p> <p><b>ANMÄRKNING</b>:   
        <ul> 
         <li>Om Workfront-administratören har anpassat namnet på Portfolio, Program eller Projekt i Workfront användargränssnitt, visas Workfront-standardnamnet för objektet i den här listrutan, inte det anpassade namnet. Kontakta Workfront-administratören om du behöver hjälp med detta.<br></li> 
         <li>Följande objekttyper stöds i iOS och Android Workfront mobilappar: User, Company, Group, Job Role, Portfolio, Program, Project och Template.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Gör ett obligatoriskt fält</td> 
      <td>Välj det här alternativet om du vill att fältet ska vara obligatoriskt för att användaren ska kunna fylla i det anpassade formuläret. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datumfält</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till andra fält eller widgetar.

   eller

   Om du vill kopiera ett fält håller du pekaren över ett fält och klickar på kopieikonen.

   ![kopieringsikon](assets/copy-field.png)

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till externa sökfält

Ett externt uppslagsfält anropar ett externt API och returnerar värden som alternativ i ett nedrullningsbart fält. Användare som arbetar med objektet som det anpassade formuläret är kopplat till kan välja ett eller flera av dessa alternativ i listrutan.

Så här lägger du till en extern sökning:

1. På skärmens vänstra sida finns **Extern sökning** och dra den till ett avsnitt på arbetsytan.
1. Konfigurera alternativen för det anpassade fältet till höger på skärmen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar det anpassade fältet.</p> <p>När du konfigurerar det anpassade fältet för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> 
      <p><b>VIKTIGT</b>:   
      <ul> 
      <li>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront. <p>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.</p> </li>
      <li> <p>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.</p> </li>
      <li><p>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.</p></li>
      </ul> <p>Varje anpassat fältnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. Mer information finns i <a href="#Add" class="MCXref xref">Lägga till ett anpassat fält i ett anpassat formulär</a> i den här artikeln.</p> </td>
     </tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Ange eventuell ytterligare information om det anpassade fältet. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td>
      <td><p>Välj den typ av data som ska hämtas i det anpassade fältet.</p>
      <p><strong>OBS!</strong></p>
      <ul><li>Du kan ändra formattyp när formuläret har sparats, med en begränsning: Alla befintliga värden på objekt måste kunna konverteras till den nya typen. (Om formattypen till exempel är Text och ett objekt lagrar värdet "abc", kan du inte konvertera fältet och får ett felmeddelande om att systemet inte kan konvertera "abc" till tal/valuta.) Om du tänker använda fältet i matematiska beräkningar måste du välja ett tal- eller valutaformat.</li>
      <li>När du väljer Nummer eller Valuta kortas nummer som börjar med 0 automatiskt av systemet.</li></ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Bas-API-URL</td> 
      <td><p>Skriv eller klistra in URL:en för API:t.</p><p>API-URL:en måste returnera ett JSON-innehåll av de alternativ som du vill visa i listrutan. Du kan använda fältet JSON-sökväg för att välja specifika värden från den returnerade JSON-filen som ska vara listrutealternativ.</p><p>När du anger API-URL:en kan du välja att skicka följande värden i URL:en:</p>
      <ul><li>$$QUERY - Detta representerar den söktext som slutanvändaren skriver i fältet och gör att du kan implementera frågefiltrering för slutanvändarna. (Användaren söker efter värdet i listrutan.)</li>
      <li>$$HOST - Detta representerar den aktuella Workfront-värden och kan användas för att göra /search API-anrop till Workfront API. När jokertecknet används hanteras autentiseringen och användarna behöver inte skicka autentiseringshuvuden. (Användare kan t.ex. söka efter uppgifter med bas-URL:en "$$HOST/attask/api/task/search" och kan söka efter uppgifter och välja värden från en returnerad lista med uppgifter.)</li>
      <li>{fieldName} - Där fieldName är ett anpassat eller inbyggt fält i Workfront. På så sätt kan du implementera filtren för överlappande listrutor när du skickar värdet för ett redan markerat fält till fältet för extern sökning för att filtrera ned alternativen. (Fältet Region finns till exempel redan i formuläret och du begränsar en lista med länder från API:t till de som finns i en viss region.)</li>
      <li>{referenceObject}.{fieldName} - Där fältet ingår i ett objekt. Syntaxen liknar anpassade uttryck. (Till exempel portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>OBS!</strong> Granska dokumentationen för API:t som du arbetar med för de specifika frågor som du kan definiera.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP-metod</td> 
      <td>Välj <strong>Hämta</strong>, <strong>Bokför</strong>, eller <strong>Put</strong> för metoden.</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON-sökväg</td>
      <td><p>Skriv eller klistra in JSON-sökvägen för API:t.</p> <p>Med det här alternativet kan data extraheras från den JSON som returneras av API-URL:en. Det är ett sätt att välja vilka värden från JSON som ska visas i listrutealternativen.</p><p>Om din API-URL till exempel returnerar JSON i det här formatet:</br>
      <pre>
      { data: { name: "USA"}, { name: "Canada"} }
      </pre>
      </p>
      <p>kan du använda "$.data[*].name" för att välja USA och Kanada som listrutealternativ.</p> <p>Mer information om JSON-sökvägen och hur du skriver rätt JSON-sökväg finns i <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Sidhuvuden</td>
      <td><p>Klicka <strong>Lägg till sidhuvud</strong>och skriv eller klistra in nyckelvärdepar som krävs för autentisering med API:t.</p><p><strong>OBS!</strong> Rubrikfälten är inte ett säkert ställe att lagra inloggningsuppgifter på och du bör vara försiktig med vad du anger och sparar.</p></td>
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

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

>[!NOTE]
>
>Följande objekt är tekniska begränsningar för anropet till det externa API:t:
>
>* Maximalt antal alternativ: 200 (endast de första 200 alternativen från det returnerade JSON visas)
>* Timeout: 3 sekunder
>* Antal återförsök: 3
>* Väntetid mellan återförsök: 500 ms
>* Förväntad svarsstatus: 2xx
>* Användarna kan se det valda värdet (och redigera värdet) i listor och rapporter i Workfront, men kommer inte att se listrutan med alternativ från det externa API:t.

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

+++ **Expandera om du vill visa beskrivningar av tillgängliga fält**

* **Bild**: Tillåter användare att lägga till ____ bildfiler.
* **PDF**: Tillåter användare att lägga till PDF
* **Videor**: Tillåter användare att lägga till ____ videofiler.

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
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar widgeten.</p> <p>När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> <p><b>VIKTIGT</b>: Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i widgeten. Om du gör det kommer systemet inte längre att känna igen widgeten där den nu kan refereras i andra områden av Workfront. </p> <p>Varje widgetnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoriskt) Skriv eller klistra in URL:en för widgeten där den lagras på Internet.</p> 
      <p>Om du lägger till en videowidget kan du göra det genom att lägga till följande i URL-rutan:</p> 
      <ul> 
      <li> <p>Länk till YouTube eller Vimeo</p> </li> 
      <li> <p>Google Drive - videolänk</p> </li> 
      <li> <p>Länka till video med MP4- och MOV-tillägg</p> </li> 
      <li> <p>Länk till video som redan har överförts till dokumentområdet i din Workfront-instans. Instruktioner finns i <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Lägga till en videowidget i ett anpassat formulär från området Dokument</a> i den här artikeln.</p> </li> 
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

   ![kopieringsikon](assets/copy-field.png)

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

#### **Lägga till en videowidget i ett anpassat formulär från området Dokument**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>När du lägger till en video i ett anpassat formulär på det här sättet gäller endast de behörigheter som angetts för det anpassade formuläret för videon när användarna öppnar formuläret för ett objekt, inte de behörigheter som angetts för videon i området Dokument.

1. Gå till videon i området Dokument och generera ett korrektur för den enligt beskrivningen i [Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öppna beviset.
1. Högerklicka var som helst i videon och välj sedan **Kopiera videoadress**.
1. Klistra in den kopierade adressen i det anpassade formuläret där du lägger till videowidgeten **URL** box.
1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till Adobe XD-filer

Du kan lägga till en Adobe XD-prototyp direkt i ett anpassat formulär. Användare som arbetar med det objekt som det anpassade formuläret är kopplat till kan bara se Adobe XD-filen i följande områden:

* Objektets detaljområde (t.ex. området Projektinformation för ett projekt)
* Rutan Redigera för objektet, om det har det nya Adobe Workfront-gränssnittet (t.ex. rutorna Redigera projekt och Redigera uppgift)

Lägga till en Adobe XD-fil:

1. På skärmens vänstra sida finns **Adobe XD** och dra den till ett avsnitt på arbetsytan.
1. Ange eller redigera någon av följande egenskaper för widgeten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar widgeten. När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p>
    <p><b>VIKTIGT</b>:   
      <ul> 
      <li>Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i Workfront. Om du gör det kommer systemet inte längre att känna igen det anpassade fältet där det nu kan refereras till i andra områden av Workfront. <p>Om du t.ex. lägger till det anpassade fältet i en rapport och senare ändrar namnet, känner Workfront inte igen det i rapporten och det slutar fungera som det ska om du inte lägger till det i rapporten igen med det nya namnet.</p> </li>
      <li> <p>Vi rekommenderar att du inte skriver in ett namn som redan används för inbyggda Workfront-fält.</p> </li>
      <li><p>Vi rekommenderar att du inte använder punkt-/punkttecken i det anpassade fältnamnet för att förhindra fel när du använder fältet i olika områden av Workfront.</p></td> 
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

   ![kopieringsikon](assets/copy-field.png)

1. Klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

## Organisera och förhandsgranska ett formulär med formulärdesignern

Mer information om hur du organiserar och ser en förhandsgranskning av formuläret finns i [Organisera och förhandsgranska ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
