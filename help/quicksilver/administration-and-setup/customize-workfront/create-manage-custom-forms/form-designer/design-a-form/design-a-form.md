---
title: Designa ett formulär med formulärdesignern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan utforma ett anpassat formulär med formulärdesignern.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: f416fc6a021a63e3a0cbd905de8e5892455f21a9
workflow-type: tm+mt
source-wordcount: '3618'
ht-degree: 0%

---


# Designa ett formulär med formulärdesignern

{{highlighted-preview-article-level}}

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
   <p>Aktuell plan: Standard</p>
   <p>eller</p>
   <p>Äldre plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer ger åtkomst finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Börja designa ett anpassat formulär

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Anpassad Forms** i den vänstra panelen.

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

1. Spara ändringarna genom att klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till textfält

Du kan lägga till flera olika textfält i ett anpassat formulär.

+++ **Expandera om du vill visa beskrivningar av tillgängliga textfält**

* **Textfält med en rad**: Tillåter användare att skriva en enda textrad i fältet.
* **Textfält för stycke**: Tillåter användare att skriva flera textrader i fältet.
* **Textfält med formatering**: Används för att skriva flera textrader i fältet och för att formatera texten med fet stil, kursiv stil, understrykning, punkter, numrering, hyperlänkar och blockcitattecken. En teckengräns på 15 000 tillåter mycket text och formatering.

   Mer information om hur du får åtkomst till det här fältet via API finns i Lagring av RTF-fält i API:t.

   >[!NOTE]
   >
   >Textfält med formatering är inte tillgängliga för Workfront mobilappar (i kommande versioner).
* **Beskrivande text**: Gör att du kan inkludera instruktioner och länka till sidor utanför Workfront.
+++

Så här lägger du till ett textfält:

1. Leta upp ett av följande textfält till vänster på skärmen och dra det till ett avsnitt på arbetsytan:

   * Enkelradig text:
   * Stycketext
   * Textfält med formatering
   * Beskrivande texter

   ![](assets/drag-field-to-section.png)

1. Till höger på skärmen konfigurerar du de alternativ som är tillgängliga för den typ av anpassat fält som du lägger till:

   <table>
    <tr>
    <td>Indata till</td>
    <td>Beskrivning</td>
    <td>Finns för </td>
    </tr>
    <tr>
    <td>Etikett</td>
    <td><p>Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.<p>
    <p>VIKTIGT! Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p></td>
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
    <li>Beskrivande text</li>
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
    <li>När du väljer Nummer eller Valuta trunkeras nummer som börjar med 0 automatiskt.</li> 
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
    <td><ul><li>Beskrivande text</li></ul></td>
    </tr>
   </table>

1. Spara ändringarna genom att klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till beräknade fält

I ett anpassat formulär kan du lägga till ett beräknat anpassat fält som använder befintliga data för att generera nya data när det anpassade formuläret kopplas till ett objekt.

Information om hur du lägger till ett beräkningsfält finns i [Lägg till beräknade fält med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Lägg till alternativknappar, kryssrutor och listrutor

Du kan lägga till alternativknappar, kryssrutor och listrutor i ett anpassat formulär.

+++ **Expandera om du vill visa beskrivningar av tillgängliga fält**

* **Alternativknappar**: Kräver att användare bara väljer ett alternativ.
* **Kryssrutegrupp**: Tillåter användare att välja flera alternativ.
* **Listruta**: Innehåller en lista med alternativ i listrutan.

+++

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
     <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
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
    <li>När du väljer Nummer eller Valuta trunkeras nummer som börjar med 0 automatiskt.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Alternativknappar</li>
    <li>Kryssrutegrupp</li>
    <li>Listruta</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Visningstyp</td> 
    <td>Växla mellan alternativknappar, kryssrutegrupper och listrutor för fältet.</td> 
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
    <li> <p><strong>Ta bort alternativ</strong>: Ta bort alternativet från fältet.</p> <p><b>VARNING</b>: Om du har aktuella objekt med det här alternativet tar du inte bort det från fältet. Om du tar bort den går historikdata förlorade. Välj i stället alternativet att dölja det, vilket förhindrar att användarna väljer det i framtiden.</p> </li> 
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
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför det anpassade fältet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
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
         <li>Följande objekttyper stöds i mobilapparna iOS och Android Workfront: Användare, företag, grupp, jobbroll, Portfolio, program, projekt och mall.</li> 
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

1. Spara ändringarna genom att klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

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

Så här lägger du till bilder, PDF eller videoklipp:

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
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
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

1. Spara ändringarna genom att klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

#### **Lägga till en videowidget i ett anpassat formulär från området Dokument**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>När du lägger till en video i ett anpassat formulär på det här sättet gäller endast de behörigheter som angetts för det anpassade formuläret för videon när användarna öppnar formuläret för ett objekt, inte de behörigheter som angetts för videon i området Dokument.

1. Gå till videon i området Dokument och generera ett korrektur för den enligt beskrivningen i [Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öppna korrekturet.
1. Högerklicka var som helst i videon och välj sedan **Kopiera videoadress**.
1. Klistra in den kopierade adressen i det anpassade formuläret där du lägger till videowidgeten **URL** box.
1. Spara ändringarna genom att klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

### Lägg till Adobe XD-filer

Du kan lägga till en Adobe XD-prototyp direkt i ett anpassat formulär. Användare som arbetar med det objekt som det anpassade formuläret är kopplat till kan bara se Adobe XD-filen i följande områden:

* Objektets detaljområde (t.ex. området Projektinformation för ett projekt)
* Rutan Redigera för objektet, om det har det nya Adobe Workfront-gränssnittet (t.ex. rutorna Redigera projekt och Redigera uppgift)

Så här lägger du till en Adobe XD-fil:

1. Till vänster på skärmen finns **Adobe XD** och dra den till ett avsnitt på arbetsytan.
1. Ange eller redigera någon av följande egenskaper för widgeten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
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
      <p>Obs! Länkåtkomstinställningen på fliken Dela i Adobe XD måste vara inställd på Alla med länken. Annars kan användarna inte visa prototypen. 
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

1. Spara ändringarna genom att klicka på **Använd** och gå vidare till ett annat avsnitt för att fortsätta skapa formuläret.

   eller

   Klicka **Spara och stäng**.

## Organisera och förhandsgranska ett formulär med formulärdesignern

Mer information om hur du organiserar och ser en förhandsgranskning av formuläret finns i [Organisera och förhandsgranska ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).