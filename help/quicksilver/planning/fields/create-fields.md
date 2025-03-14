---
title: Skapa fält
description: I Adobe Workfront Planning kan du skapa anpassade fält för varje typ av posttyp. Du kan sedan associera fältet med Workfront Planning-poster.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '4333'
ht-degree: 0%

---


<!--Should the structure of this article be like this other one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# Skapa fält

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->


{{planning-important-intro}}

I Adobe Workfront Planning kan du skapa anpassade fält för posttyper. Du kan sedan associera fälten med Workfront Planning-poster för att förbättra postinformationen.

Du måste skapa posttyper innan du kan skapa fält som ska kopplas till dem. Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

Du kan skapa fält på följande sätt i Workfront Planning:

* Från början
* Genom att ansluta posttyper
* Genom att skapa en posttyp
* Skapa en arbetsyta från en mall
* Importera posttyper med en Excel- eller CSV-fil
* Genom att importera kopior av befintliga Workfront-fält

Mer information om Workfront Planning-fält finns i [Fältöversikt](/help/quicksilver/planning/fields/fields-overview.md).

## Åtkomstkrav

+++ Expandera för att visa åtkomstkrav..

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
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning-paket*</p></td> 
   <td> 
<p>Alla </p> 
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta <!--<span class="preview">and record type</span>--> </a> </p>  
   <p>Systemadministratörer har behörighet för alla arbetsytor, inklusive de som de inte skapade.</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level control for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Skapa fält från grunden {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

<!--the first 3 steps are the same as in Import fields from Workfron-->

{{step1-to-planning}}

1. Klicka på arbetsytan vars poster du vill skapa fält för.

   Arbetsytan öppnas och posttyperna visas.

1. Klicka på kortet för en posttyp.

   Alla befintliga poster som är associerade med posttypen visas i tabellvyns rader.

   >[!TIP]
   >
   >    Om inga poster visas kanske du inte har några poster än, eller så kanske du har ett filter som begränsar det som visas på skärmen.

   Alla befintliga fält som är associerade med posttypen visas i kolumnerna i tabellvyn.

   >[!TIP]
   >
   >    Vissa fält kan vara dolda. Klicka på Fält och aktivera växlingen mellan de fält som du vill visa som kolumner i tabellvyn.

1. Klicka på ikonen **+** i tabellvyns övre högra hörn

   eller

   Håll markören över en kolumnrubrik, klicka på den nedåtriktade pilen efter fältnamnet och klicka sedan på **Infoga vänster** eller **Infoga höger** för att lägga till det nya fältet.
1. På fliken **Nytt fält** söker du efter en fälttyp i rutan **Fälttyp** eller väljer någon av följande fälttyper:

   På fliken **Nytt fält** kan du söka efter en fälttyp i rutan **Fälttyp** med hjälp av ett relaterat nyckelord, eller välja bland de fälttyper som listas nedan.

   >[!TIP]
   >
   >    Du kan skriva &quot;Budget&quot; och fälttyperna &quot;Number&quot; och &quot;Currency&quot; i en kort lista.



   * [Enkelradig text](#single-line-text)
   * [Stycke](#paragraph)
   * [Flera val](#multi-select)
   * [Enkelval](#single-select)
   * [Datum](#date)
   * [Number](#number)
   * [Procent](#percentage)
   * [Valuta](#currency)
   * [Kryssruta](#checkbox)
   * [Formel](#formula)
   * [Folk](#people)
   * [Skapad av](#created-by)
   * [Skapad den](#created-date)
   * [Senast ändrad av](#last-modified-by)
   * [Senast ändrat den](#last-modified-date)

   >[!IMPORTANT]
   >
   >    Du kan inte ändra fälttypen när du har sparat den.

   <!--Add this to the IMPORTANT above and make it a NOTE - should do directly to Prod:
    * You can use any keyword that might be related to any of the field type names. For example, a search for "Budget" will display the Number or Currency field type.-->

1. Fortsätt med att lägga till varje fält enligt beskrivningen i avsnitten nedan.

### Enkelradig text {#single-line-text}

Enkelradiga textfält fångar begränsad alfanumerisk information. Du kan till exempel samla information om ägare, intressenter, team eller organisationsenheter i ett textfält med en rad. Innehållet i ett textfält med en rad kan innehålla upp till 1 000 tecken. <!-- used to be 250 but just tested with 1000 and it allowed this as a maximum. -->

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Enkelradig text**.

   ![](assets/single-line-text-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumnrubrik i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
1. Klicka på **Skapa**.

   Det nya enradiga fältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.


### Stycke {#paragraph}

Styckefält hämtar ytterligare alfanumerisk information om en post, som liknar fältet Beskrivning.

>[!TIP]
>
>* Du kan ha högst 20 styckefält för en posttyp.
>
>* Innehållet i ett styckefält kan innehålla upp till 10 000 tecken.
>* Du kan använda RTF-formatering för att förbättra innehållet i styckefält när de visas i tabellvyn eller på detaljsidan för en post. Mer information finns i [Redigera poster](/help/quicksilver/planning/records/edit-records.md).
>


1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Stycke**.

   ![](assets/paragraph-field-type.png)


1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
1. Klicka på **Skapa**.

   Det nya styckefältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.


### Flera val {#multi-select}

Du kan använda ett flervalsfält för att hämta ytterligare information i valfritt format genom att välja mer än ett alternativ i en listruta.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Flera val**.

   ![](assets/multi-select-field-type.png)


1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Alternativ**: De alternativ som användare kan välja när fältet uppdateras. Du kan använda både siffror och bokstäver som namn på varje val.
1. Klicka på **Lägg till alternativ** om du vill lägga till fler alternativ. Det finns ingen gräns för hur många alternativ du kan lägga till i ett flervalsfält.
1. (Valfritt) Dra och släpp varje alternativ manuellt i önskad ordning, eller välj
   **Sorteringsalternativ A-Z** om du vill att valen automatiskt ska visas i alfabetisk ordning. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Valfritt) Om du vill ta bort ett alternativ klickar du på ikonen **x** till höger om den.
1. Klicka på färgrutan till vänster om ett alternativ för att utöka färgväljaren och anpassa färgen för varje alternativ.

1. Klicka på **Färgrutor** för att välja en fördefinierad färg

   eller

   Klicka på **Egen** om du vill välja en egen färg med hjälp av en färgväljare eller en hexadecimal kod.
1. Klicka utanför färgrutan för att stänga den.
1. Klicka på **Skapa**.

   Det nya flervalsfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Enkelval {#single-select}

Med envalsfält hämtas ytterligare information i valfritt format genom att du väljer ett alternativ i en nedrullningsbar meny.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Enkelval**.

   ![](assets/single-select-field-type.png)


1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Alternativ**: De alternativ som är tillgängliga att välja på den nedrullningsbara menyn när fältet har sparats. Du kan ha både siffror och bokstäver för namnet på varje val.

1. Klicka på **Lägg till alternativ** om du vill lägga till fler alternativ. Det finns ingen gräns för hur många alternativ du kan lägga till i ett envalsfält.
1. (Valfritt) Dra och släpp varje alternativ manuellt i önskad ordning eller markera alternativet **Sorteringsalternativ A-Z** om du vill att valen automatiskt ska visas i alfabetisk ordning. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Valfritt) Om du vill ta bort ett alternativ klickar du på ikonen **x** till höger om den.
1. Klicka på färgrutan till vänster om ett alternativ för att utöka färgväljaren och anpassa färgen för varje alternativ.
1. Klicka på **Färgrutor** för att välja en fördefinierad färg

   eller

   Klicka på **Egen** om du vill välja en egen färg med hjälp av en färgväljare eller en hexadecimal kod.

1. Klicka utanför färgrutan för att stänga den.
1. Klicka på **Skapa**.

   Det nya envalsfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Datum {#date}

Du kan använda ett datumfält för att samla in ytterligare information i datum- och tidsformat.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Datum**.

   ![](assets/date-field-type.png)


1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Datumformat**: Den typ av datumformat som du vill visa i det här fältet. <!--update this casing - submitted bug for it-->

     Välj bland följande format:
      * **Språk**: Matchar språkområdet i webbläsaren.
      * **Standard**: 05/16/2023
      * **Lång**: 16 maj 2023
      * **Europeisk**: 16/05/2023
      * **ISO**: 2023-05-16
      * **Inkludera tid**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är som standard omarkerat. Du kan inte inkludera en tid efter att du har skyddat fältet.

     Välj bland följande alternativ:

      * **24hr**: Till exempel: 18:00
      * **12hr**: Exempel: 6:00 PM

1. Klicka på **Skapa**.

   Det nya datumfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Nummer {#number}

Nummerfälttyper samlar in information i talformat.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Number**.

   ![](assets/number-field-type.png)
1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa tal i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt negativa tal och negativa värden lagras på posterna som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

1. Klicka på **Skapa**.

   Det nya nummerfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Procent {#percentage}

Procentfälttyper samlar in information i talformat följt av ett procenttecken.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Procent**.

   ![](assets/percentage-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa procentvärden i det här fältet. Det här alternativet är som standard avmarkerat.

     >[!NOTE]
     >
     >Om du väljer Tillåt negativa tal och negativa värden lagras på posterna som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

   * **Visa som**: Välj hur du vill att procentvärdena ska visas i tabellvyn i den nedrullningsbara menyn. Välj bland följande alternativ:
      * **Number**: Procentvärdet visas som ett tal följt av procenttecknet.
      * **Bar**: Procentvärdet visas som en stapel bredvid procenttalet. Fältets fyllningsfärg anger procentvärdet. Det här är standardvalet.
      * **Cirkel**: Procentvärdet visas som konturen för en cirkel bredvid procenttalet. Fyllningsfärgen för cirkelns kontur anger procentvärdet.

   >[!NOTE]
   >
   >* Den markering du gör i fältet Visa som gäller endast det procentvärde som är synligt i tabellvyn. Procentvärdet för fältet visas som ett tal följt av procenttecknet överallt i Workfront Planning. Detta gäller även för fältet av procenttyp när det visas som ett uppslagsfält i andra posters tabellvyer.
   >* Du kan ändra Visa som markering när du redigerar fältet senare.

1. Klicka på **Skapa**.

   Det nya procentfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Valuta {#currency}

Valutafälttyper samlar in information i ett talformat som föregås av en valutasymbol.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Valuta**.

   ![](assets/currency-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Valuta**: Den typ av valuta som du vill visa i det här fältet. Detta är en lista över valutor enligt ISO (International Organization of Standardization).
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

   ![](assets/checkbox-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
1. Klicka på **Skapa**.

   Det nya kryssrutefältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Formel

Formelfält genererar ett nytt värde med hjälp av befintliga värden från andra fält i en posttyp och en funktion som anger hur befintliga värden ska beräknas.

Mer information finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Formel**.

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Ange ett namn för det nya fältet.
   * **Beskrivning**: Lägg till information om det nya fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Formel**: Börja skriva minst ett tecken för att komma åt ett uttryck och markera det sedan när det visas i listan.

1. Klicka på det markerade uttrycket för att visa definitionen och dess formatering.

   ![](assets/description-of-formula-expression.png)

   Mer information om vilka uttryck som stöds finns i [Översikt över formelfält](/help/quicksilver/planning/fields/formula-fields.md).


   >[!TIP]
   >
   >Du får ett varningsmeddelande när du redigerar eller skapar ett formelfält som kan orsaka en cirkelreferens till sig själv eller delade fält. Du kan inte spara ett formelfält som antingen refererar till sig själv eller till artiklar som refereras i beräkningen.


1. Lägg till fältnamn som de visas i Workfront Planning för att referera till dem i en formel.

   >[!NOTE]
   >
   >* Du kan inte lägga till flervalsfält i en formel.
   >
   >* Du kan referera till ett fält som är upp till fyra fält (och objekt) utanför den aktuella posttypen. Om du till exempel skapar ett formelfält för en aktivitetsposttyp (1) och aktiviteten är kopplad till kampanjposttypen (2) som är kopplad till ett Workfront-projekt (3), kan du referera till projektets budgetfält (4) i formeln som du skapar för aktivitetsposttypen.
   >
   >![](assets/formula-example-project-budget-four-fields-removed.png)
   >

1. I fältet **Format** väljer du bland följande alternativ för att identifiera formatet på resultatet som visas i formeltypsfältet:

   * **Text**: Resultatet av formelfältet visas som oformaterad text.
   * **Number**: Resultatet av formelfältet visas som ett tal.
   * **Procent**: Resultatet av formelfältet visas som ett tal följt av en procentsymbol.
   * **Valuta**: Resultatet av formelfältet visas som ett tal som föregås eller följs av en valutasymbol.
   * **Taggar**: Resultatet av formelfältet visas som en tagg med objektets namn.

     >[!TIP]
     >
     >Vi rekommenderar taggar för fält som visar arrayer. I det här fallet visas varje arraymedlem som en separat tagg.

     ![](assets/formula-field-formats-list-with-tag-selected-highlighted.png)

   * **Datum**: Resultatet av formelfältet visas som ett datum.

     En förhandsgranskning av hur resultatet kommer att se ut visas under fältet **Format**.

     >[!WARNING]
     >
     >Om formelresultatet inte matchar det valda formatet visas ett felmeddelande där det visas.

1. Klicka på **Skapa**.

   Det nya formelfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Folk

Du kan använda fälttypen Personer för att lägga till en användare <!--, job role, or team--> i en post. Det här är ett type-ahead-fält och du kan bara lägga till användare <!--, roles, or teams--> som redan finns i din Workfront-instans.

>[!TIP]
>
>När du lägger till namnet på en användare i ett personfält visas namnet på användaren och den primära jobbrollen i fältet.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Personer**.

   ![](assets/people-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.
   * **Tillåt flera värden**: Välj det här alternativet om du vill tillåta användare att lägga till fler än en användare i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt flera värden och flera användare lagras på de poster som fältet är kopplat till, kan du inte längre avmarkera inställningen när du redigerar det här fältet.

1. Klicka på **Skapa**.

   Det nya fältet av typen Personer läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Skapad av

Du kan använda fälttypen Skapad av för att lägga till användaren som skapade posten i en post. Det här är ett skrivskyddat fält och fyller automatiskt i med namnet på den användare som var inloggad när posten skapades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Skapad av**.

   ![](assets/created-by-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.

1. Klicka på **Skapa**.

   Det nya fältet Skapat efter typ läggs till som en kolumn till posttypen och dess värden är förifyllda med namnet på den användare som skapade varje post.


### Skapad den

Du kan använda fälttypen Skapat för att lägga till datumet då posten skapades i en post. Det här är ett skrivskyddat fält som automatiskt fylls i med datumet (och eventuellt med tiden) när posten skapades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Skapad**.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created date"-->
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

   ![](assets/last-modified-by-field-type.png)

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du håller markören över fältets kolumn i en tabell eller när du klickar på informationsikonen bredvid fältnamnet på postens informationssida.

1. Klicka på **Skapa**.

   Det nya fältet Senast ändrad efter typ läggs till som en kolumn till posttypen och dess värden är förifyllda med namnet på den användare som senast ändrade varje post.


### Senast ändrat den

Du kan använda fälttypen Senaste ändringsdatum för att lägga till datumet när en post senast ändrades till en post. Det här är ett skrivskyddat fält som automatiskt fylls i med datumet (och eventuellt med tiden) när posten senast ändrades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln och välj sedan fälttypen **Skapad**.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Lägg till följande information på fliken **Nytt fält**:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postsidan. <!--this might change and they might prepopulate it with "Created date"-->
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

   Det nya fältet Senast ändrad datumtyp läggs till som en kolumn till posttypen och dess värden är förifyllda med datumet (eller datum och tid) när posten senast ändrades.

## Skapa fält genom att ansluta posttyper

Du kan skapa länkade postfält när du lägger till en ny anslutning mellan två posttyper, eller en posttyp och en objekttyp från andra program.

Mer information om hur du ansluter posttyper för Workfront Planning finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

<!--## Create fields by importing record types using an Excel or CSV file

For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).-->

## Skapa fält genom att skapa en posttyp

När du skapar en posttyp skapas även flera fält som är kopplade till den nya posttypen som standard. Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Skapa fält genom att skapa en arbetsyta från en mall

I Adobe Workfront Planning skapas fält för posttyper när du skapar en arbetsyta från en mall.

Mer information finns i [Skapa arbetsytor](/help/quicksilver/planning/architecture/create-workspaces.md).



## Skapa fält när du importerar posttyper från en CSV- eller Excel-fil

Du kan importera fält när du importerar posttyper med hjälp av en CSV- eller Excel-fil.

Mer information finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

## Skapa fält genom att importera dem från Workfront

Du kan importera kopior av befintliga Workfront-fält.

När du importerar fält från Workfront skapas en kopia av varje fält för en posttyp av Workfront Planning.

När du har kopierat fälten är fälten oberoende av varandra och de utbyter inte information.

Mer information finns i [Importera fält från Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


