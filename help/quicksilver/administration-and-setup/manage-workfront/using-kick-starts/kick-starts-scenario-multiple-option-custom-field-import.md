---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,sparkstart,kickstarter,sparkstarter
navigation-topic: use-kick-starts
title: 'Kickstartscenario: Importera anpassade fält med flera alternativ till Workfront'
description: Du kan importera anpassade fält med flera alternativ i Adobe Workfront med funktionen Snabbstart.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 70f3dac7-f449-4dc8-9d7d-a5284b37f9ec
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '2160'
ht-degree: 0%

---

# Scenario för att komma igång: Importera anpassade fält med flera alternativ till Workfront

Du kan importera anpassade fält med flera alternativ i Adobe Workfront med funktionen Snabbstart.

Exempel på anpassade fält med flera alternativ är:

* Flervalsmeny
* Listruta
* Kryssrutor
* Alternativknappar

Dessa fält kan ibland ha många (ibland hundratals) alternativ. Om du importerar dem med snabbstartsfunktionen kan du som Workfront-administratör spara mycket tid och se till att du undviker fel.

>[!IMPORTANT]
>
>Du måste följa stegen som beskrivs i avsnitten nedan, i den här ordningen, för att importera anpassade fält med flera alternativ med en snabbstart:
>
>1. Exportera befintliga anpassade data från Workfront (valfritt steg)
>1. Exportera snabbstartsmallen för anpassade data
>1. Fyll i Excel-kalkylbladet Kickstart
>1. Överför Excel-kalkylbladet till Workfront

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p> Nytt: Standard</p>
   eller
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportera befintliga anpassade data från Workfront (valfritt steg)

Om du inte känner till databasstrukturen för Workfront, eller om du inte känner till den snabbstartfil som Workfront behöver för att importera information, rekommenderar vi att du först exporterar en snabbstartfil från Workfront med befintlig information, liknande den som finns i fälten som du vill importera.

Om du till exempel vill importera anpassade formulär eller anpassade fält måste du först exportera en snabbstartfil med befintliga anpassade data.

Om du exporterar dina befintliga data först kan du skanna dem och se hur nya data behöver formateras.

Om du har god förståelse för databasobjekten och strukturen i Workfront kan du fortsätta med avsnittet nedan.

Så här exporterar du befintliga data från Workfront:

{{step-1-to-setup}}

1. Expandera **System** på den vänstra menyn och klicka sedan på **Exportera data (snabbstart)**.

1. Välj **Anpassade data** i avsnittet **Vad som ska inkluderas**.

   ![Välj anpassade data](assets/kickstarts-select-existing-data.png)

1. Välj filen **.xlsx** i avsnittet **Hämtningsformat**.

   >[!TIP]
   >
   >Beroende på hur mycket anpassade data du har i systemet kan det ta lång tid.

1. Klicka på **Hämta**. En .xlsx-fil laddas ned till datorn. Navigera till den och öppna den.

   ![Exporterade data i Excel](assets/existing-data-excel-parameter-sheet.png)

1. Granska den hämtade filen och notera följande:

   * Filen innehåller flera blad. Du behöver kanske inte känna till informationen i varje blad, men du kommer att använda vissa av bladen för att importera informationen. Ägna lite tid åt att bekanta dig med deras innehåll och särskilt med formatet på innehållet i varje blad.
   * Var särskilt uppmärksam på kolumnnamnen och i vilket format data i varje kolumn visas.
   * Du får inte ändra kolumnernas namn eller ordningsföljd i någon av tabellerna. Kolumnrubrikerna anger fält som du måste fylla i med dina uppgifter, på varje rad. Om kolumnrubriken visas i fet stil är det ett obligatoriskt fält, så du måste ha information i den kolumnen.

   >[!IMPORTANT]
   >
   >Vissa kolumnrubriker kanske inte visas i fet stil, men de kan ändå behövas.

   * Behåll den hämtade filen för framtida referens och fortsätt till följande avsnitt.

## Exportera snabbstartsmallen för anpassade data

När du har läst in information om befintliga anpassade fält i systemet kan du hämta en ny startmall för importen.

{{step-1-to-setup}}

1. Expandera **System** i den vänstra menyn.

1. Klicka på **Importera data (snabbstart)**.

1. Markera kryssrutan **Anpassade data** i området **Hämta ett tomt snabbstartkalkylblad** och klicka på **Hämta**.

   ![Välj anpassade data](assets/kickstarts-blank-spreadsheet-options.png)

   En tom fil som startar snabbt laddas ned till datorn.

   >[!NOTE]
   >
   >Antalet blad i filen, deras namn samt antalet kolumner och namnen på kolumnerna i varje blad bör vara identiska med dem från den snabbstart som laddades ned i det ovan nämnda avsnittet som innehöll dina befintliga anpassade data.

## Fyll i Excel-kalkylbladet Kickstart

Innan du fyller i Excel-kalkylbladet ska du hämta snabbstartmallen enligt beskrivningen i avsnittet ovan.

>[!IMPORTANT]
>
>Försök inte importera information med hjälp av ett Excel-kalkylblad. Alla kalkylblad för import av information till Workfront med hjälp av snabbstartsfunktionen måste matcha innehållet i de filer du laddar ned från Workfront och som beskrivs i den här artikeln.

Så här fyller du i Excel-kalkylbladet med information om de nya anpassade fälten:

1. Öppna Excel-kalkylbladet som du laddade ned i föregående avsnitt och granska bladen. Varje ark representerar ett objekt i programmet.

   Exempel: **Parameter** (som refererar till anpassat fält), **Parameteralternativ** (som refererar till alternativet Anpassat fält), **Kategori** (som refererar till anpassat formulär).

   Du måste skriva objektens namn och attribut i det format som stöds av Workfront-databasen.

   Mer information om innebörden av dessa objekt finns i [Ordlistan för  [!DNL Adobe Workfront] terminologi](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   Mer information om namnen på objekten i Workfront-databasen finns i [API-utforskaren](../../../wf-api/general/api-explorer.md).

   ![Blad som ingår i dataexport](assets/sheets-included-in-custom-data-export-kick-start-file.png)

1. Kontrollera att följande information är korrekt formaterad:

   * Den första raden i varje blad måste vara tom, annars genereras ett fel.
   * Kolumnrubrikerna i varje blad representerar attribut för de objekt som kan anges under en import. Alla kolumnrubriker måste finnas kvar i samma ordning som du hittar dem när du exporterar kalkylbladet och de kan inte byta namn.
   * Kolumnrubrikerna i fetstil är obligatoriska fält och de måste ha ett värde.

     >[!TIP]
     >
     >Vissa kolumner är obligatoriska men de är inte i fet stil. Kolumnerna `isNew` och `ID` har till exempel inte fetstil, men de är obligatoriska fält.

1. Markera bladet `**PARAM Parameter`** och lägg till information om de nya anpassade fälten i följande obligatoriska kolumner:

   * **`isNew`** = ange **`TRUE`** i den här kolumnen för varje rad som representerar ett nytt anpassat fält. Detta anger att fältet är nytt och inte finns i Workfront.

     >[!TIP]
     >
     >Om en rad representerar ett befintligt fält som redan finns i Workfront anger du **`isNew`** = **`FALSE`**.

   * **`ID`** = måste vara ett unikt nummer för varje rad som representerar ett nytt fält. Du kan använda valfritt nummer som börjar med 1, förutsatt att varje nytt fält har ett unikt nummer.
   * **`setDataType`** = För varje rad som representerar ett nytt fält anger du den datatyp som fältet stöder. Datatypen måste anges så som den skulle visas i databasen. Välj bland följande datatyper:

      * **`NMBR`** för Number
      * **`CURC`** för valuta
      * **`TEXT`** för text

   * `**setDisplaySize**`= Visningsstorleken (**setDisplaySize**) för anpassade fält med flera alternativ är alltid 0.
   * **`setDisplayType`** = För varje rad som representerar ett nytt fält anger du fältets visningstyp. Visningstypen måste anges som den skulle visas i databasen.

     Välj bland följande alternativ för anpassade fält med flera alternativ:

      * **`MULT`** för flervalslistruta
      * **`SLCT`** för listruta
      * **`RDIO`** för alternativknappar
      * **`CHCK`** för kryssrutor

     >[!TIP]
     >
     >Information om datatyp och visningstyp finns i [API-utforskaren](../../../wf-api/general/api-explorer.md), expandera objektet **Parameter** och sök efter dessa attribut på fliken **Fält**.

   * **`setName`** = ange namnet på anpassade fält som du vill att de ska visas i Workfront.

     >[!INFO]
     >
     >Vi kan till exempel importera två anpassade fält, _Varumärke_, ett kryssrutefält och _Media_, ett alternativknappsfält.

   * Kolumnerna **`setName`** och **`setValue`** innehåller vanligtvis samma information och de bör återspegla de namn som du vill ha i Workfront-gränssnittet för det nya fältet.

   Värdet för ett fält är det namn som visas i rapporter, till exempel, medan namnet visas i de anpassade formulär som är kopplade till objekt.

   Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   ![Parameterblad fyllt i](assets/parameter-sheet-filled-out-kick-starts.png)

1. Markera bladet **`POPT Parameter Options`** och lägg till information om alternativen för varje anpassat fält i följande obligatoriska kolumner:

   * **`isNew`** = ange **`TRUE`** i den här kolumnen för varje rad som representerar ett nytt fältalternativ.

     >[!TIP]
     >
     >    Om en rad representerar ett befintligt alternativ anger du **`isNew`** = **`FALSE`**.

   * **`ID`** = måste vara ett unikt nummer för varje rad som representerar ett nytt alternativ. Du kan använda valfritt nummer som börjar med 1, förutsatt att varje nytt alternativ har ett unikt nummer.
   * **`setIsDefault`** = ange `TRUE` för de alternativ som du vill visa som standard, och `FALSE` för alla andra alternativ, för varje fält.  Vi vill till exempel att _Nike_ ska vara standardalternativet för _Varumärke_ och _Skriv ut_ ska vara standardalternativet för _Media_.

     >[!TIP]
     >
     >Du kan bara ha ett standardalternativ för varje fält.

   * **`setParameterID`** = de alternativ som motsvarar det anpassade fältet _Varumärke_ har **`setParameterID`** 1, och de alternativ som motsvarar _Media_ har **`setParameterID`**&#x200B;2. `PARAM` och `POPT` blad korsrefererar varandra för att ange vilka alternativ som tillhör vilka anpassade fält.
   * **`setDisplayOrder`**= Visningsordningskolumnen anger i vilken ordning alternativen visas i det anpassade fältet. Du kan börja med 1 och fortsätta i stigande ordning för alla alternativ, oavsett vilka fält de tillhör. Det viktiga här är att ha unika nummer för varje alternativ.
   * Kolumnerna **`setLabel`** och `**setValue`** innehåller vanligtvis samma information och de bör återspegla de namn som du vill ha i Workfront-gränssnittet. Värdet för ett alternativ är det namn som visas i rapporter, till exempel, medan etiketten visas i de anpassade formerna när den kopplas till ett objekt. Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   * **`setIsHidden`** = ange `TRUE` om du vill att något av alternativen ska vara dolt.

   ![Parameterblad fyllt i](assets/parameter-option-sheet-filled-out-kick-starts.png)

1. (Valfritt) Om du även vill skapa ett anpassat formulär där du senare kan lägga till de nya fälten, markerar du bladet **`CTGY Category`** och uppdaterar följande obligatoriska kolumner för den anpassade formulärinformationen:

   * **`isNew`** = ange **`TRUE`** i den här kolumnen för varje rad som representerar ett nytt anpassat formulär.
   * **`ID`** = ange ett unikt nummer för varje rad som representerar ett nytt formulär. Du kan använda valfritt nummer som börjar med 1, förutsatt att varje nytt alternativ eller rad har ett unikt nummer.
   * **`setGroupID`** = lägg till grupp-ID för din hemgrupp eller någon annan grupp i systemet vars medlemmar du vill ska ha åtkomst till det här formuläret. Detta är ett obligatoriskt fält.

   Om du vill ta reda på `ID` för en grupp kan du antingen skapa en grupprapport och lägga till fältet `ID` i vyn, eller navigera till en grupp och hitta gruppens URL. Grupp-ID:t finns i URL:en för gruppens sida. Om URL:en för gruppen till exempel är `https://companyName.my.workfront.com/group/575b000800467a6f66e747932c807464/members` är grupp-ID:t `575b000800467a6f66e747932c807464`.

   * **`setCatObjCode`**= Det här är objektkoden för den objekttyp som du vill att formuläret ska skapas för. Ange en kod bland följande alternativ:
      * **`CMPY`** för företag
      * **`TASK`** för aktivitet
      * **`PROJ`** för projekt
      * **`PORT`** för Portfolio
      * **`PRGM`** för program
      * **`USER`** för användare
      * **`DOCU`** för dokument
      * **`OPTASK`** för ärende
      * **`EXPNS`** för utgift
      * **`ITRN`** för iterering
      * **`BILL`** för faktureringsposter
      * **`GROUP`** för grupp

     >[!NOTE]
     >
     >För formulär med flera objekt anger du det första objektet som du skulle markera när du skapar ett formulär i användargränssnittet. Ange till exempel `setCatObjCode` till `TASK` om du vill välja Uppgift i Workfront-gränssnittet och sedan Problem, Portfolio osv., men du inte vill att formuläret ska vara tillgängligt för Projekt.

   * **`setName`** = det här är namnet på det anpassade formuläret som du vill att det ska visas i Workfront-gränssnittet.

     ![Kategoriblad fyllt i](assets/category-sheet-filled-out-kick-starts.png)

1. Spara kalkylbladet som en .xls- eller .xlsx-fil på datorn. Excel-kalkylbladet är ifyllt och kan nu importeras till Workfront.

## Överför Excel-kalkylbladet till Workfront

När du har utfört stegen som beskrivs i föregående avsnitt fortsätter du med följande för att överföra de nya fälten och formulären till Workfront:

{{step-1-to-setup}}

1. Klicka på **System > Importera data (snabbstart)**.

1. Klicka på **Välj fil** under avsnittet **Överför data med snabbstartskalkylblad**.

1. Bläddra efter det Excel-kalkylblad du har förberett på datorn och markera det när du hittar det.

   Filen överförs automatiskt och ett meddelande om att importen lyckades visas. Beroende på hur mycket information du importerar kan det här steget ta några sekunder till en minut.

   De nya anpassade fälten och formulären finns nu i Workfront. Du hittar dem under Anpassad Forms i Konfigurera.

   >[!NOTE]
   >
   >De nya formulären och fälten som du importerade är ännu inte sammankopplade. Formuläret importeras utan anpassade fält. Du måste lägga till fälten manuellt i det nya anpassade formuläret eller i ett annat befintligt anpassat formulär.

   Mer information om hur du lägger till fält i anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Villkorligt) Om importen inte lyckades får du ett felmeddelande som anger vad problemet är. Försök att identifiera fältet, bladet och radnumret som problemet påträffades i och korrigera informationen i Excel-filen. Försök sedan att importera filen en gång till.

1. (Villkorligt) Beroende på vad problemet är kan viss information redan ha importerats, vilket anges i felmeddelandet. Du måste göra något av följande innan du kan importera bladet igen:

   * Ta bort den information som har importerats från Workfront från området Anpassad Forms och korrigera sedan felmeddelandet.
   * Ange att ett fält eller ett formulär redan finns i systemet för de fält eller formulär som redan har importerats och korrigera sedan.
Om du vill ange att ett fält eller ett anpassat formulär redan finns i Workfront måste du se till att fältet `inNew` är markerat som `FALSE` i blad som innehåller information om formuläret (`CTGY`) eller fältet (`PARAM`) på importbladet för att komma igång.
