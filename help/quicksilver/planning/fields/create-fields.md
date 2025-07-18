---
title: Skapa fält
description: I Adobe Workfront Planning kan du skapa anpassade fält för varje typ av posttyp. Du kan sedan koppla fältet till Workfront Planning-poster.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '5201'
ht-degree: 0%

---


<!--Should the structure of this article be like this other one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=sv-SE ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# Skapa fält

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är endast tillgänglig i förhandsversionsmiljön för alla kunder. Efter de månatliga versionerna till produktion är samma funktioner också tillgängliga i produktionsmiljön för kunder som har aktiverat snabba versioner. </span>

<span class="preview">Information om snabba versioner finns i [Aktivera eller inaktivera snabba versioner för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

I Adobe Workfront Planning kan du skapa anpassade fält för posttyper. Du kan sedan koppla fälten till Workfront Planning-poster för att förbättra postinformationen.

Du måste skapa posttyper innan du kan skapa fält som ska associeras med dem. Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

Du kan skapa fält på följande sätt i Workfront Planning:

* Från grunden
* Genom att ansluta posttyper
* Genom att skapa en posttyp
* Genom att skapa en arbetsyta från en mall
* Genom att importera posttyper med hjälp av en Excel- eller CSV-fil
* Genom att importera kopior av befintliga Workfront-fält

Mer information om Workfront Planning-fält finns i [Fältöversikt](/help/quicksilver/planning/fields/fields-overview.md).

## Krav för åtkomst

+++ Expandera för att visa åtkomstkrav.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planering av Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Någon av följande Workfront-planer:</p> 
<ul><li>Utvald</li> 
<li>Primtal</li> 
<li>Sist</li></ul> 
<p>Workfront Planning är inte tillgängligt för äldre Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planeringspaket*</p></td> 
   <td> 
<p>Någon </p> 
<p>Om du vill ha mer information om vad som ingår i varje Workfront Planning-plan kontaktar du din Workfront-kontoansvarige. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-plattform</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste vara registrerad i Adobe Unified Experience för att kunna komma åt Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience för Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licens för Adobe Workfront*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning är inte tillgängligt för äldre Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration av åtkomstnivå</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Behörigheter för objekt</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta och posttyp</a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, även de som de inte har skapat.</p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om åtkomstkrav för Workfront finns [i Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa fält från grunden {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

<!--the first 3 steps are the same as in Import fields from Workfront-->

{{step1-to-planning}}

1. Klicka på den arbetsyta vars poster du vill skapa fält för.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på kortet för en posttyp.

   Alla befintliga poster som är associerade med posttypen visas i raderna i tabellvyn.

   >[!TIP]
   >
   >    Om inga poster visas kanske du inte har några poster ännu, eller så kanske du har ett filter som begränsar vad du ser på skärmen.

   Alla befintliga fält som är associerade med posttypen visas i kolumnerna i tabellvyn.

   >[!TIP]
   >
   >    Vissa fält kan vara dolda. Klicka på Fält och aktivera växlingsknappen för de fält som du vill visa som kolumner i tabellvyn.

1. Klicka på **+** -ikonen i det övre högra hörnet av tabellvyn

   eller

   Håll muspekaren över rubriken för en kolumn, klicka på den nedåtriktade pilen efter fältnamnet och klicka sedan på **Infoga vänster** eller **Infoga höger** för att lägga till det nya fältet.
1. På fliken Nytt **fält** söker du efter en fälttyp i **rutan Fälttyp** eller väljer bland följande fälttyper:

   På fliken Nytt **fält** söker du efter en fälttyp i **rutan Fälttyp** med hjälp av ett relaterat nyckelord eller väljer bland fälttyperna som listas nedan.

   >[!TIP]
   >
   >    Du kan skriva &quot;Budget&quot; och fälttyperna Nummer och Valuta visas i en kort lista.



   * [Text med en rad](#single-line-text)
   * [Paragraf](#paragraph)
   * [Välj flera](#multi-select)
   * [Välj en gång](#single-select)
   * [Datum](#date)
   * [Nummer](#number)
   * [Procent](#percentage)
   * [Valuta](#currency)
   * [Kryssrutan](#checkbox)
   * [Formel](#formula)
   * [Folk](#people)
   * [Skapad av](#created-by)
   * [Skapat den](#created-date)
   * [Senast ändrad av](#last-modified-by)
   * [Datum för senaste ändring](#last-modified-date)
   * <span class="preview">[Godkänt datum](#approved-date)</span>
   * <span class="preview">[Godkänd av](#approved-by)</span>
     <!--* [Object](#object-field-type)-->

   >[!IMPORTANT]
   >
   >Du kan inte ändra fälttypen för fältet när du har sparat det.

   <!--Add this to the IMPORTANT above and make it a NOTE - should do directly to Prod:
    * You can use any keyword that might be related to any of the field type names. For example, a search for "Budget" will display the Number or Currency field type.-->

1. Fortsätt med att lägga till varje fält enligt beskrivningen i avsnitten nedan.

### Text med en rad {#single-line-text}

Enradiga textfält samlar in begränsad alfanumerisk information. Du kan till exempel samla in information om ägare, intressent, team eller organisationsenhet i ett textfält med en rad. Innehållet i ett enradigt textfält kan innehålla upp till 1 000 tecken. <!-- used to be 250 but just tested with 1000 and it allowed this as a maximum. -->

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan typen Enradig textfält** .

   ![Typ av textfält med en rad](assets/single-line-text-field-type.png)

1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det visas i en tabell eller på sidan Detaljer för posten. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumnrubrik i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
1. Klicka på **Skapa**.

   Det nya enradsfältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.


### Paragraf {#paragraph}

Styckefält samlar in ytterligare alfanumerisk information om en post, ungefär som fältet Beskrivning.

>[!TIP]
>
>* Du kan ha högst 20 styckefält för en posttyp.
>
>* Innehållet i ett styckefält kan innehålla upp till 10 000 tecken.
>* Du kan använda RTF-formatering för att förbättra innehållet i styckefält när de visas i tabellvyn eller på detaljsidan för en post. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).
>


1. Börja skapa ett fält på det sätt som beskrivs i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Stycke** .

   ![Typ av styckefält](assets/paragraph-field-type.png)


1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det visas i en tabell eller på sidan Detaljer för posten. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
1. Klicka på **Skapa**.

   Det nya styckefältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.


### Flera val {#multi-select}

Du kan använda ett flervalsfält för att hämta ytterligare information i valfritt format genom att välja mer än ett alternativ i en listruta.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Flera val**.

   ![Flervalsfälttyp](assets/multi-select-field-type.png)


1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Fältets namn, så som det kommer att visas i en tabell eller på postens informationssida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Alternativ**: De alternativ som användarna kan välja när de uppdaterar det här fältet. Du kan använda både siffror och bokstäver för namnet på varje val.
1. Klicka på **Lägg till alternativ** för att lägga till fler alternativ. Det finns ingen gräns för hur många val du kan lägga till i ett flervalsfält.
1. (Valfritt) Dra och släpp varje val manuellt i önskad ordning, eller välj
   **Sortera val A-Ö** om du vill att valen automatiskt ska listas i alfabetisk ordning. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Valfritt) Om du vill ta bort ett val klickar du på **x-ikonen** till höger om det.
1. Klicka på färgrutan till vänster om ett alternativ för att utöka färgväljaren och anpassa färgen för varje alternativ.

1. Klicka på **Färgrutor** för att välja en fördefinierad färg

   Eller

   Klicka på **Anpassad** för att välja en anpassad färg med hjälp av en färgväljare eller en hexadecimal kod.
1. Klicka utanför färgrutan för att stänga den.
1. Klicka på **Skapa**.

   Det nya flervalsfältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.

### Välj en gång {#single-select}

Enkelvalsfält samlar in ytterligare information i valfritt format genom att välja ett alternativ från en rullgardinsmeny.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Enkelval** .

   ![Fälttyp med ett val](assets/single-select-field-type.png)


1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det visas i en tabell eller på sidan Detaljer för posten. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Val**: De alternativ som är tillgängliga att välja från rullgardinsmenyn efter att fältet har sparats. Du kan ha både siffror och bokstäver för namnet på varje val.

1. Klicka på **Lägg till alternativ** för att lägga till fler alternativ. Det finns ingen gräns för hur många val du kan lägga till i ett enkelvalsfält.
1. (Valfritt) Dra och släpp varje val manuellt i önskad ordning, eller välj **alternativet Sortera val A-Ö** om du vill att valen automatiskt ska listas i alfabetisk ordning. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Valfritt) Om du vill ta bort ett val klickar du på **x-ikonen** till höger om det.
1. Klicka på färgrutan till vänster om ett alternativ för att expandera färgväljaren och anpassa färgen för varje alternativ.
1. Klicka på **Färgrutor** för att välja en fördefinierad färg

   Eller

   Klicka på **Anpassad** för att välja en anpassad färg med hjälp av en färgväljare eller en hexadecimal kod.

1. Klicka utanför färgrutan för att stänga den.
1. Klicka på **Skapa**.

   Det nya enkelvalsfältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.

### Datum {#date}

Du kan använda ett datumfält för att samla in ytterligare information i datum- och tidsformat.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Datum** .

   ![Typ av datumfält](assets/date-field-type.png)


1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Datumformat**: Den typ av datumformat som du vill visa i det här fältet. <!--update this casing - submitted bug for it-->

     Välj bland följande format:
      * **Språk**: Matchar webbläsarens nationella inställningar.
      * **Standard**: 2023-05-16
      * **Lång**: 16 maj 2023
      * **Europeiska**: 16/05/2023
      * **ISO:** 2023-05-16
      * **Inkludera tid**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är avmarkerat som standard. Du kan inte inkludera en tid efter att du har säkrat fältet.

     Välj bland följande alternativ:

      * **24hr**: Till exempel: 18:00
      * **12hr**: Exempel: 6:00 PM

1. Klicka på **Skapa**.

   Det nya datumfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Nummer {#number}

Nummerfälttyper samlar in information i talformat.

>[!TIP]
>
>Nummerfält visas som en typ av enradigt textfält i en formulärbyggare för begäran.
>
>Fältformatet bevaras dock och värdena i dessa fält visas som siffror efter att begäran har skickats, på posttypen och på sidan med information om begäran.
>&#x200B;>Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Number**.

   ![Nummerfältstyp](assets/number-field-type.png)
1. Lägg till följande information på fliken Nytt **fält** :

   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa tal i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt negativa tal, och negativa värden lagras i de poster som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

1. Klicka på **Skapa**.

   Det nya numeriska fältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.

### Procent {#percentage}

Fälttyper för procent samlar in information i ett numeriskt format följt av ett procenttecken.

>[!TIP]
>
>Procentfält visas som en textfältstyp med en rad i ett formulärverktyg för begäran.
>
>Fältformatet bevaras dock och värdena i dessa fält visas i procenttal efter att begäran har skickats, på posttypen och på sidan med information om begäran.
>&#x200B;>Mer information finns [i Skapa och hantera ett förfrågningsformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Procent** .

   ![Typ av fält för procentsats](assets/percentage-field-type.png)

1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa procentvärden i det här fältet. Det här alternativet är avmarkerat som standard.

     >[!NOTE]
     >
     >Om du väljer Tillåt negativa tal, och negativa värden lagras i de poster som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

   * **Visa som**: I rullgardinsmenyn väljer du hur du vill att procentvärdena ska visas i tabellvyn. Välj bland följande alternativ:
      * **Tal**: Procentvärdet visas som ett tal följt av procenttecknet.
      * **Stapel**: Procentvärdet visas som en stapel bredvid procenttalet. Stapelns fyllningsfärg anger procentvärdet. Det här är standardvalet.
      * **Cirkel**: Procentvärdet visas som konturen av en cirkel bredvid procenttalet. Fyllningsfärgen på cirkelns kontur anger procentvärdet.

   >[!NOTE]
   >
   >* Det val du gör i fältet Visa som gäller endast för det procentvärde som visas i tabellvyn. Procentvärdet i fältet visas som ett tal följt av procenttecknet överallt annars i Workfront Planning. Detta gäller även för fältet av procenttyp när det visas som ett uppslagsfält i andra posters tabellvyer.
   >* Du kan ändra Visa som markering när du redigerar fältet senare.

1. Klicka på **Skapa**.

   Det nya procentfältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.

### Valuta {#currency}

Typer av valutafält samlar in information i ett numeriskt format som föregås av en valutasymbol.

>[!TIP]
>
>Valutafält visas som en textfältstyp med en rad i ett formulärverktyg för begäran.
>
>Fältformatet bevaras dock och värdena i dessa fält visas som valuta när begäran har skickats, på posttypen och på sidan med information om begäran.
>&#x200B;>Mer information finns [i Skapa och hantera ett förfrågningsformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Valuta** .

   ![Typ av fält Valuta](assets/currency-field-type.png)

1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Valuta**: Den typ av valuta som du vill visa i det här fältet. Detta är en lista över valutor enligt International Organizaton of Standardization (ISO).
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa valutavärden i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt negativa tal och negativa värden lagras på posterna som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

1. Klicka på **Skapa**.

   Det nya valutafältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Kryssruta

Du kan använda fälttypen Kryssruta för att lägga till en kryssruta till en post. Du kan använda det här fältet för att ange ett specifikt attribut eller en specifik status för den aktuella posten. Du kan till exempel använda den som en flagga för att spåra slutförande, godkännande eller andra binära attribut för varje post.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Kryssruta**.

   ![Fälttyp för kryssruta](assets/checkbox-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Fältets namn, så som det kommer att visas i en tabell eller på postsidan. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
1. Klicka på **Skapa**.

   Det nya kryssrutefältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.

### Formel

Formelfält genererar ett nytt värde med hjälp av befintliga värden från andra fält i en posttyp och en funktion som anger hur de befintliga värdena ska beräknas.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Formel** .

   ![Nytt formelfält med lista över uttryck](assets/new-formula-field-with-list-of-expressions.png)

1. Lägg till följande information på fliken Nytt **fält** :

   * **Namn**: Ange ett namn för det nya fältet.
   * **Beskrivning**: Lägg till information om det nya fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Formel**: Börja skriva minst ett tecken för att komma åt ett uttryck och välj det sedan när det visas i listan.

1. Klicka på det markerade uttrycket för att visa definitionen och visa dess formatering.

   ![Beskrivning av formeluttryck](assets/description-of-formula-expression.png)

   Mer information om vilka uttryck som stöds finns i [Översikt](/help/quicksilver/planning/fields/formula-fields.md) över formelfält.


   >[!TIP]
   >
   >Du får ett varningsmeddelande när du redigerar eller skapar ett formelfält som kan orsaka en cirkelreferens till sig själv eller delade fält. Du kan inte spara ett formelfält som antingen refererar till sig självt eller till element som refereras till i beräkningen.


1. Lägg till fältnamn så som de visas i Workfront Planning för att referera till dem i en formel.

   >[!NOTE]
   >
   >* Du kan inte lägga till flervalsfält i en formel.
   >
   >
   >* Du måste stava namnet på fälten som du inkluderar i formlerna så som du ser dem i Workfront Planning. Workfront textlägessyntax och jokertecken stöds inte i Workfront Planning-formler.
   >
   >* Du kan referera till ett fält som är upp till fyra fält (och objekt) utanför den aktuella posttypen. Om du till exempel skapar ett formelfält för en aktivitetsposttyp (1) och aktiviteten är kopplad till kampanjposttypen (2) som är kopplad till ett Workfront-projekt (3), kan du referera till projektets budgetfält (4) i formeln som du skapar för aktivitetsposttypen.
   >
   >![Formelexempel för projektbudget fyra fält har tagits bort ](assets/formula-example-project-budget-four-fields-removed.png)
   >

1. I fältet **Format** väljer du bland följande alternativ för att identifiera formatet på resultatet som visas i formeltypsfältet:

   * **Text**: Resultatet av formelfältet visas som oformaterad text.
   * **Number**: Resultatet av formelfältet visas som ett tal.
   * **Procent**: Resultatet av formelfältet visas som ett tal följt av en procentsymbol.
   * **Valuta**: Resultatet av formelfältet visas som ett tal som föregås eller följs av en valutasymbol.
   * **Taggar**: Resultatet av formelfältet visas som en tagg med objektets namn.

     >[!TIP]
     >
     >Vi rekommenderar taggar för fält som visar matriser. I det här fallet visas varje matrismedlem som en separat tagg.

     ![Lista över formelfältsformat med markerad tagg markerad](assets/formula-field-formats-list-with-tag-selected-highlighted.png)

   * **Datum**: Resultatet av formelfältet visas som ett datum.

     En förhandsgranskning av hur resultatet kommer att se ut visas under **fältet Format** .

     >[!WARNING]
     >
     >Om resultatet av formeln inte matchar det valda formatet kommer fältet att visa ett felmeddelande där det visas.

1. Klicka på **Skapa**.

   Det nya formelfältet läggs till som en kolumn i posttypen och dess värden kan associeras med poster.

### Folk

Du kan använda fälttypen Personer för att lägga till en användare <!--, job role, or team--> i en post. Det här är ett fält i förväg och du kan bara lägga till användare<!--, roles, or teams--> som redan finns i din Workfront-instans.

>[!TIP]
>
>* När du lägger till namnet på en användare i ett personfält visas namnet på användaren och deras primära jobbroll i fältet.
>
>* Personfält visas som en referensfälttyp (eller anslutningsfälttyp) i en formulärkonstruktör för begäran.
>
>Mer information finns [i Skapa och hantera ett förfrågningsformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Personer** .

   ![Typ av fält Personer](assets/people-field-type.png)

1. Lägg till följande information på fliken Nytt **fält** :
   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Tillåt flera värden**: Välj det här alternativet om du vill tillåta användare att lägga till mer än en användare i det här fältet. Det här alternativet är avmarkerat som standard.

   >[!NOTE]
   >
   >    Om du väljer Tillåt flera värden och flera användare lagras på de poster som fältet är kopplat till, kan du inte längre avmarkera inställningen när du redigerar det här fältet.

1. Klicka på **Skapa**.

   Det nya fältet av typen Personer läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Skapad av

Du kan använda fälttypen Skapad av för att lägga till användaren som skapade posten i en post. Det här är ett skrivskyddat fält och fyller automatiskt i med namnet på den användare som var inloggad när posten skapades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Skapad av**.

   ![Skapad av fälttyp](assets/created-by-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Fältets namn, så som det kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.

1. Klicka på **Skapa**.

   Det nya fältet Skapad av typ läggs till som en kolumn i posttypen och dess värden fylls i automatiskt med namnet på den användare som skapade varje post.


### Skapat den

Du kan använda fälttypen Skapat datum för att lägga till det datum då posten skapades i en post. Det här är ett skrivskyddat fält som automatiskt fylls i med datumet (och eventuellt med tiden) då posten skapades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Skapat datum** .

   ![Fälttypen Skapat datum](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Lägg till följande information på fliken Nytt **fält** :

   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Datumformat**: Välj bland följande format:

      * **Språk**: Matchar språkområdet i webbläsaren.
      * **Standard**: 05/16/2023
      * **Lång**: 16 maj 2023
      * **Europeisk**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Inkludera ett tidsfält**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är som standard omarkerat. <!--submitted a UI text change for this - check the UI-->

     Välj bland följande alternativ:

      * **24hr**: Till exempel: 18:00
      * **12hr**: Exempel: 6:00 PM

1. Klicka på **Skapa**.

   Det nya fältet Skapad av-datum läggs till som en kolumn till posttypen och dess värden är förifyllda med datumet (eller datum och tid) när posten skapades.


### Senast ändrad av

Du kan använda fälttypen Senast ändrad av för att lägga till användaren som senast ändrade posten till en post. Det här är ett skrivskyddat fält och fyller automatiskt i med namnet på den användare som var inloggad när posten senast uppdaterades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Senast ändrad av**.

   ![Senast ändrad av fälttyp](assets/last-modified-by-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Fältets namn, så som det kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.

1. Klicka på **Skapa**.

   Det nya fältet Senast ändrad av typ läggs till som en kolumn i posttypen och dess värden fylls i automatiskt med namnet på den användare som senast ändrade varje post.


### Datum för senaste ändring

Du kan använda fälttypen Datum för senaste ändring om du vill lägga till det datum då en post senast ändrades i en post. Det här är ett skrivskyddat fält som automatiskt fylls i med datumet (och eventuellt med tiden) när posten senast ändrades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj **sedan fälttypen Skapat datum** .

   ![Fälttyp för senast ändrad datum](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Lägg till följande information på fliken Nytt **fält** :

   * **Namn**: Namnet på fältet, så som det kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller muspekaren över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Datumformat**: Välj bland följande format:

      * **Språk**: Matchar webbläsarens nationella inställningar.
      * **Standard**: 2023-05-16
      * **Lång**: 16 maj 2023
      * **Europeiska**: 16/05/2023
      * **ISO:** 2023-05-16

   * **Inkludera ett tidsfält**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är avmarkerat som standard. <!--submitted a UI text change for this - check the UI-->

     Välj bland följande alternativ:

      * **24 timmar**: Till exempel: 18:00
      * **12hr**: Exempel: 6:00 PM

1. Klicka på **Skapa**.

   Det nya fältet Senast ändrad datumtyp läggs till som en kolumn till posttypen och dess värden är förifyllda med datumet (eller datum och tid) när posten senast ändrades.

<div class="preview">

### Godkänt den

Du kan använda fälttypen Godkänt datum för att lägga till datumet när en begäran godkändes och det resulterade i att posten skapades. Det här är ett skrivskyddat fält och fyller automatiskt i med datumet (och eventuellt med tiden) när begäran godkändes av den senaste godkännaren. I det här fallet bör godkännandedatumet sammanfalla med datumet då posten skapades.

>[!TIP]
>
>Fältet Godkänt datum fylls endast i med information för poster som har skapats genom att skicka ett begärandeformulär som är associerat med godkännare.
>
>Om formuläret är kopplat till mer än en godkännare registreras endast datumet för det senaste godkännandebeslutet i fältet Godkänt datum.


1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Skapad**.

   ![Godkänd datumfältstyp](assets/approved-date-field-type.png)

   1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Fältets namn, så som det kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Datumformat**: Välj bland följande format:

      * **Språk**: Matchar språkområdet i webbläsaren.
      * **Standard**: 05/16/2023
      * **Lång**: 16 maj 2023
      * **Europeisk**: 16/05/2023
      * **ISO**: 2023-05-16

   * **Inkludera ett tidsfält**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är som standard omarkerat.

     Välj bland följande alternativ:

      * **24hr**: Till exempel: 18:00
      * **12hr**: Exempel: 6:00 PM

1. Klicka på **Skapa**.

   Det nya fältet Godkänd datumtyp läggs till som en kolumn till posttypen och dess värden är förifyllda med datumet (eller datum och tid) när postbegäran godkändes, om posten skapades genom att en begäran som är associerad med godkännare skickades.

### Godkänd av

Du kan använda fälttypen Godkänd av för att lägga till den användare som senast godkände begäran för att skapa en post. Det här är ett skrivskyddat fält och det fylls automatiskt i med namnet på den användare som godkände begäran för att skapa posten.

>[!TIP]
>
>Fältet Godkänd av fylls bara i med information för poster som har skapats genom att skicka ett begärandeformulär som är associerat med godkännare.
>
>Om formuläret är associerat med mer än en godkännare registreras namnet på alla godkännare i fältet Godkänt datum, avgränsat med kommatecken.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Godkänd av**.

   ![Godkänd av fälttyp](assets/approved-by-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Fältets namn, så som det kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.

1. Klicka på **Skapa**.

   Det nya fältet Godkänd efter typ läggs till som en kolumn till posttypen och dess värden är förifyllda med namnet på den användare som senast ändrade varje post.

</div>

<!--

## Object field type

You can use the Object field type when you need to store several fields that might include several pieces of information. For example, you can store the source, code, error message, or details of an object in one field. In this case, instead of having several separate single-line text fields for that, you can use an Object field to store all information in one place. 

For example, when using an Object-type field, you can store the following type of information: 

```
"{
""source"": ""string"",
""code"": ""string"",
""subCode"": ""string"",
""message"": ""string"",
""details"": ""string""
}"

```

You can also store an array of values in one field and you would rather rely on user input for each element of the array, instead of using a multi-select field type for the same purpose. For example, you can store information in the following format: 

`["EMEA", "APAC"] `

Consider the following when using Object-type fields:

* In addition to strings and arrays, you can store other value formats like HTML.
* There is no format validation for this field. 
* Object-type fields have a limit of 10,000 characters.

Create an Object field: 

1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **Created date** field type.

    ![Object field type](assets/object-field-type.png)

1. Add the following information in the **New field** tab:

     * **Name**: The name of the field, as it will appear in a table or the record page. (***********this might change and they might prepopulate it with "Created date"********)
     * **Description**: Additional information about the field. The description of a field displays when you hover over the field's column in a table, or when you click the information icon next to the field name in the record's details page.

1. Click **Create**.

    The new Object-type field is added as a column to the record type.

-->

## Skapa fält genom att ansluta posttyper

Du kan skapa länkade postfält när du lägger till en ny koppling mellan två posttyper, eller en posttyp och en objekttyp från andra program.

Mer information om hur du ansluter posttyper för Workfront Planning finns i [Ansluta posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

<!--## Create fields by importing record types using an Excel or CSV file

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).-->

## Skapa fält genom att skapa en posttyp

När du skapar en posttyp skapas också flera fält som är associerade med den nya posttypen som standard. Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Skapa fält genom att skapa en arbetsyta från en mall

Adobe Workfront Planning skapar fält för posttyper när du skapar en arbetsyta från en mall.

Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).



## Skapa fält när du importerar posttyper från en CSV- eller Excel-fil

Du kan importera fält när du importerar posttyper med hjälp av en CSV- eller Excel-fil.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Skapa fält genom att importera dem från Workfront

Du kan importera kopior av befintliga Workfront-fält.

När du importerar fält från Workfront skapas en kopia av varje fält för en Workfront Planning-posttyp.

När du har kopierat fälten är de oberoende av varandra och de utbyter inte information.

Mer information finns i [Importera fält från Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


