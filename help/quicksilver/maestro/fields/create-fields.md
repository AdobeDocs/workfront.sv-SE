---
title: Skapa fält
description: I Adobe Maestro kan du skapa anpassade fält för varje typ av operativ posttyp eller taxonomi. Du kan sedan associera fältet med Maestro-poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 4946a65188391df62ad3e135a5b1dbba9a16dc89
workflow-type: tm+mt
source-wordcount: '3160'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Formula fields
description: In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with Maestro records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Skapa fält

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

I Adobe Maestro kan du skapa anpassade fält för driftsposttyper eller taxonomier. Du kan sedan associera fälten med Maestro-poster för att förbättra postinformationen.

Du måste skapa posttyper innan du kan skapa fält som ska kopplas till dem. Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

Du kan skapa fält på följande sätt i Maestro:

* Från början
* Genom att ansluta posttyper
* Importera posttyper med hjälp av en Excel- och CSV-fil
* Genom att skapa en posttyp
* Skapa en arbetsyta från en mall

Mer information om Maestro-fält finns i [Fältöversikt](../fields/fields-overview.md)

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Skapa fält från grunden {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i det övre högra hörnet av Workfront eller **Huvudmeny** icon ![](assets/main-menu-shell.png)  i det övre vänstra hörnet, om det är tillgängligt, klickar du på **Maestro** ![](assets/maestro-icon.png).

   Den senast använda arbetsytan bör öppnas som standard.

1. (Valfritt) Expandera den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta, markera arbetsytan vars posttyper du vill skapa fält för och klicka sedan på posttypen.

   Alla befintliga poster som är associerade med posttypen visas i tabellvyns rader.

   >[!TIP]
   >
   >    Om inga poster visas kanske du inte har några poster än, eller så kanske du har ett filter som begränsar det som visas på skärmen.

   Alla befintliga fält som är associerade med posttypen visas i kolumnerna i tabellvyn. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Klicka på **+** i tabellvyns övre högra hörn för att lägga till nya fält.
1. I **Nytt fält** väljer du bland följande fälttyper:

   * [Enkelradig text](#single-line-text)
   * [Stycke](#paragraph)
   * [Flera val](#multi-select)
   * [Enkelval](#single-select)
   * [Datum](#date)
   * [Nummer](#number)
   * [Procent](#percentage)
   * [Valuta](#currency)
   * [Kryssruta](#checkbox)
   * [Folk](#people)
   * [Skapad av](#created-by)
   * [Skapad den](#created-date)
   * [Senast ändrad av](#last-modified-by)
   * [Senast ändrat den](#last-modified-date)

   >[!IMPORTANT]
   >
   >    Du kan inte ändra fälttypen när du har sparat den.

1. Fortsätt med att lägga till varje fält enligt beskrivningen i avsnitten nedan.

### Enkelradig text {#single-line-text}

Enkelradiga textfält fångar begränsad alfanumerisk information. Du kan till exempel samla information om ägare, intressenter, team eller organisationsenheter i ett textfält med en rad. Innehållet i ett textfält med en rad kan innehålla upp till 250 tecken. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Enkelradig text** fälttyp.

   ![](assets/single-line-text-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumnrubrik i en tabell.
1. Klicka **Skapa**.

   Det nya enradiga fältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.


### Stycke {#paragraph}

Styckefält hämtar ytterligare alfanumerisk information om en post, som liknar fältet Beskrivning.

>[!TIP]
>
>* Innehållet i ett styckefält kan innehålla upp till 1 000 tecken.
>
>* Du kan använda RTF-formatering för att förbättra innehållet i styckefält när de visas i tabellvyn eller på detaljsidan för en post.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Stycke** fälttyp.

   ![](assets/paragraph-field-type.png)


1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
1. Klicka **Skapa**.

   Det nya styckefältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.


### Flera val {#multi-select}

Du kan använda ett flervalsfält för att hämta ytterligare information i valfritt format genom att välja mer än ett alternativ i en listruta.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Flera val** fälttyp.

   ![](assets/multi-select-field-type.png)


1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Val**: De alternativ som är tillgängliga att välja på den nedrullningsbara menyn när fältet har sparats. Du kan ha både siffror och bokstäver för namnet på varje val.
1. Klicka **Lägg till alternativ** för att lägga till så många alternativ som behövs. Det finns ingen gräns för hur många alternativ du kan lägga till i ett flervalsfält.
1. (Valfritt) Dra och släpp varje alternativ manuellt i önskad ordning, eller välj
   **Sorteringsalternativ A-Z** om du vill att valen ska visas automatiskt i alfabetisk ordning. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Klicka på **x** till höger om ett val för att ta bort det.
1. Klicka på färgrutan till vänster om ett alternativ för att utöka färgväljaren och anpassa färgen för varje alternativ.
1. Klicka **Skapa**.

   Det nya flervalsfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Enkelval {#single-select}

Med envalsfält hämtas ytterligare information i valfritt format genom att du väljer ett alternativ i en nedrullningsbar meny.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Enkelval** fälttyp.

   ![](assets/single-select-field-type.png)


1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Val**: De alternativ som är tillgängliga att välja på den nedrullningsbara menyn när fältet har sparats. Du kan ha både siffror och bokstäver för namnet på varje val.

1. Klicka **Lägg till alternativ** för att lägga till så många alternativ som behövs. Det finns ingen gräns för hur många alternativ du kan lägga till i ett envalsfält.
1. (Valfritt) Dra och släpp varje alternativ manuellt i önskad ordning, eller välj **Sorteringsalternativ A-Z** om du vill att valen ska visas automatiskt i alfabetisk ordning. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Klicka på **x** till höger om ett val för att ta bort det.
1. Klicka på färgrutan till vänster om ett alternativ för att utöka färgväljaren och anpassa färgen för varje alternativ.
1. Klicka **Skapa**.

   Det nya envalsfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Datum {#date}

Du kan använda ett datumfält för att samla in ytterligare information i datum- och tidsformat.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Datum** fälttyp.

   ![](assets/date-field-type.png)


1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Datumformat**: Den typ av datumformat som du vill visa i det här fältet. <!--update this casing - submitted bug for it-->

     Välj bland följande format:
      * **Språk**: Matchar språkområdet i webbläsaren.
      * **Standard**: 05/16/2023
      * **Lång**: 16 maj 2023
      * **europeisk**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Inkludera ett tidsfält**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är som standard omarkerat. <!--update this setting name - submitted bug for it to be changed-->

     Välj bland följande alternativ:

      * **24 timmar**: Till exempel: 18:00
      * **12 timmar**: Exempel: 6:00 PM

1. Klicka **Skapa**.

   Det nya datumfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Nummer {#number}

Nummerfälttyper samlar in information i talformat.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Nummer** fälttyp.

   ![](assets/number-field-type.png)
1. Lägg till följande information i **Nytt fält** tab:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa tal i fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt negativa tal och negativa värden lagras på posterna som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

1. Klicka **Skapa**.

   Det nya nummerfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Procent {#percentage}

Procentfälttyper samlar in information i talformat följt av ett procenttecken.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Procent** fälttyp.

   ![](assets/percentage-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa procentvärden i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt negativa tal och negativa värden lagras på posterna som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

1. Klicka **Skapa**.

   Det nya procentfältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Valuta {#currency}

Valutafälttyper samlar in information i ett talformat som föregås av en valutasymbol.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Valuta** fälttyp.

   ![](assets/currency-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Valuta**: Den typ av valuta som du vill visa i det här fältet. Detta är en lista över valutor enligt ISO (International Organization of Standardization).
   * **Precision**: Antalet decimaler som du vill registrera för fältet. Du kan visa upp till 6 decimaler.
   * **Tillåt negativa tal**: Välj det här alternativet om du vill tillåta negativa valutavärden i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt negativa tal och negativa värden lagras på posterna som fältet är kopplat till, kan du inte längre avmarkera inställningen i framtiden.

1. Klicka **Skapa**.

   Det nya valutafältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Kryssruta

Du kan använda fälttypen Kryssruta för att lägga till en kryssruta till en post. Du kan använda det här fältet för att ange ett specifikt attribut eller en specifik status för den aktuella posten. Du kan till exempel använda den som en flagga för att spåra slutförande, godkännande eller andra binära attribut för varje post.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Kryssruta** fälttyp.

   ![](assets/checkbox-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
1. Klicka **Skapa**.

   Det nya kryssrutefältet läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Folk

Du kan använda fälttypen Personer för att lägga till en användare <!--, job role, or team--> till en post. Det här är ett typsnittsfält och du kan bara lägga till användare<!--, roles, or teams--> som redan finns i Workfront.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Folk** fälttyp.

   ![](assets/people-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:
   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida.
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Tillåt flera värden**: Välj det här alternativet om du vill tillåta användare att lägga till fler än en användare i det här fältet. Det här alternativet är som standard avmarkerat.

   >[!NOTE]
   >
   >    Om du väljer Tillåt flera värden och flera användare lagras på de poster som fältet är kopplat till, kan du inte längre avmarkera inställningen när du redigerar det här fältet.

1. Klicka **Skapa**.

   Det nya fältet av typen Personer läggs till som en kolumn till posttypen och dess värden kan kopplas till poster.

### Skapad av

Du kan använda fälttypen Skapad av för att lägga till användaren som skapade posten i en post. Det här är ett skrivskyddat fält och fyller automatiskt i med namnet på den användare som var inloggad när posten skapades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Skapad av** fälttyp.

   ![](assets/created-by-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.

1. Klicka **Skapa**.

   Det nya fältet Skapat efter typ läggs till som en kolumn till posttypen och dess värden är förifyllda med namnet på den användare som skapade varje post.


### Skapad den

Du kan använda fälttypen Skapat för att lägga till datumet när en post skapades i en post. Det här är ett skrivskyddat fält som automatiskt fylls i med datumet (och eventuellt med tiden) när posten skapades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Skapad den** fälttyp.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Lägg till följande information i **Nytt fält** tab:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Datumformat**: Välj bland följande format:

      * **Språk**: Matchar språkområdet i webbläsaren.
      * **Standard**: 05/16/2023
      * **Lång**: 16 maj 2023
      * **europeisk**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Inkludera ett tidsfält**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är som standard omarkerat. <!--submitted a UI text change for this - check the UI-->

     Välj bland följande alternativ:

      * **24 timmar**: Till exempel: 18:00
      * **12 timmar**: Exempel: 6:00 PM

1. Klicka **Skapa**.

   Det nya fältet Skapad av-datum läggs till som en kolumn till posttypen och dess värden är förifyllda med datumet (eller datum och tid) när posten skapades.


### Senast ändrad av

Du kan använda fälttypen Senast ändrad av för att lägga till användaren som senast ändrade posten till en post. Det här är ett skrivskyddat fält och fyller automatiskt i med namnet på den användare som var inloggad när posten senast uppdaterades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Senast ändrad av** fälttyp.

   ![](assets/last-modified-by-field-type.png)

1. Lägg till följande information i **Nytt fält** tab:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.

1. Klicka **Skapa**.

   Det nya fältet Senast ändrad efter typ läggs till som en kolumn till posttypen och dess värden är förifyllda med namnet på den användare som senast ändrade varje post.


### Senast ändrat den

Du kan använda fälttypen Senaste ändringsdatum för att lägga till datumet när en post senast ändrades till en post. Det här är ett skrivskyddat fält som automatiskt fylls i med datumet (och eventuellt med tiden) när posten senast ändrades.

1. Börja skapa ett fält enligt beskrivningen i avsnittet [Skapa fält från grunden](#create-fields-from-scratch) i den här artikeln väljer du **Skapad den** fälttyp.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Lägg till följande information i **Nytt fält** tab:

   * **Namn**: Namnet på fälttypen så som den kommer att visas i en tabell eller på postens detaljsida. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beskrivning**: Ytterligare information om fältet. Beskrivningen av ett fält visas när du hovrar över fältets kolumn i en tabell.
   * **Datumformat**: Välj bland följande format:

      * **Språk**: Matchar språkområdet i webbläsaren.
      * **Standard**: 05/16/2023
      * **Lång**: 16 maj 2023
      * **europeisk**: 16/05/2023
      * **ISO**: 2023-05-16
   * **Inkludera ett tidsfält**: Välj det här alternativet om du vill inkludera en tidsstämpel. Detta är som standard omarkerat. <!--submitted a UI text change for this - check the UI-->

     Välj bland följande alternativ:

      * **24 timmar**: Till exempel: 18:00
      * **12 timmar**: Exempel: 6:00 PM

1. Klicka **Skapa**.

   Det nya fältet Senast ändrad datumtyp läggs till som en kolumn till posttypen och dess värden är förifyllda med datumet (eller datum och tid) när posten senast ändrades.

## Skapa fält genom att ansluta posttyper

Du kan skapa länkade postfält när du lägger till en ny anslutning mellan två Maestro-posttyper, eller en posttyp och en objekttyp från andra program.

Mer information om hur du ansluter Maestro-posttyper finns i [Koppla posttyper](../architecture/connect-record-types.md)

## Skapa fält genom att importera posttyper med en Excel- och CSV-fil

Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

## Skapa fält genom att skapa en posttyp

När du skapar en posttyp skapas även flera fält som är kopplade till den nya posttypen som standard. Mer information finns i [Skapa driftsposttyper](../architecture/create-record-types.md).

## Skapa fält genom att skapa en arbetsyta från en mall

I Maestro skapas fält för driftsposttyper och taxonomier när du skapar en arbetsyta från en mall.

Mer information finns i [Skapa arbetsytor](../architecture/create-workspaces.md).