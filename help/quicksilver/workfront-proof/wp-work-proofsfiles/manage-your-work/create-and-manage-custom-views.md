---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Skapa och hantera anpassade vyer i  [!DNL Workfront Proof]
description: Du kan skapa anpassade vyer av dina filer och korrektur för att lista de objekt du vill ha på det sätt du vill att de ska visas. Du kan också exportera informationen i den anpassade vyn som en rapport (i CSV, kommaavgränsat värde, filformat).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2374'
ht-degree: 0%

---

# Skapa och hantera anpassade vyer i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan skapa anpassade vyer av dina filer och korrektur för att lista de objekt du vill ha på det sätt du vill att de ska visas. Du kan också exportera informationen i den anpassade vyn som en rapport (i CSV, kommaavgränsat värde, filformat).

>[!NOTE]
>
>Anpassade vyer är bara tillgängliga för Select- och Premium-planer. Kontakta vårt säljteam om du vill ha en offert.

## Skapa en anpassad vy

När du skapar en anpassad vy kan du välja:

* Om korrektur, filer eller båda ska inkluderas
* Vilka kolumner som visas
* Vilken kolumn som ska sorteras efter
* Sorteringsordningen för kolumnen (stigande eller fallande)
* Vilka typer av filter som ska användas för att bestämma vilken information som ska tas med i vyn

När den anpassade vyn har skapats kan den användas omedelbart. Namnet på den nya vyn finns också i listrutan under rubriken Mina anpassade vyer (under standardvyer).

Så här skapar du en anpassad vy:

1. Gå till sidan **[!UICONTROL Views]**.
1. Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Gör något av följande, beroende på om du vill skapa en ny anpassad vy från början eller skapa en ny anpassad vy baserad på en befintlig standardvy:

   * Så här skapar du en ny anpassad vy baserad på en befintlig standardvy: Välj den befintliga standardvyn som du vill använda som bas för den nya anpassade vyn i listrutan. Klicka på ikonen **[!UICONTROL View Settings]** och sedan på **[!UICONTROL Copy]** för att visa en ny anpassad vy.

   * ![Ikon för anpassad vy](assets/proof-custom-view-icon.png)

   * Så här skapar du en ny anpassad vy från grunden: Klicka på ikonen **[!UICONTROL New View]**.
   * ![Ny vy](assets/proof-newview.png)

1. Ange följande information i avsnittet **[!UICONTROL Details]**:

   * **[!UICONTROL Name]** (obligatoriskt): Den nya vyns namn. Använd ett unikt namn så att användarna enkelt kan hitta den anpassade vyn i listrutan i Vyer.
   * **[!UICONTROL Items]**: Välj om du vill att både korrektur och fil, endast korrektur eller bara filer ska inkluderas i vyn. Som standard inkluderas både korrektur och filer.

1. I avsnittet **[!UICONTROL Columns]** anger du vilka kolumner du vill ta med i den anpassade vyn.

   1. Klicka på högerpilen.
   1. ![Högerpil](assets/proof-view-rightarrow.png)

   1. Dubbelklicka på namnet på den markerade kolumnen.
   1. Du måste markera minst en kolumn och en kolumn kan bara läggas till en gång.
   1. Markera en kolumn i området **[!UICONTROL Available columns]** som du vill ta med i den nya vyn.
   1. Kolumnerna flyttas från listan **[!UICONTROL Available columns]** till listan **[!UICONTROL Selected columns]**.

   1. Du kan välja bland standardkolumnerna eller så kan du välja Anpassade fält och Beslutsorsaker som ska vara kolumner i den anpassade vyn. (Om du har konfigurerat de här kolumnerna i ditt konto visas de i standardlistan med tillgängliga kolumner.)
   1. Standardkolumner som du kan ta med

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Namn på aktivt stadium</strong></td>   
      <td>Namnet på den aktiva fasen i det automatiserade arbetsflödet.</td>  
      </tr>  
      <tr>   
      <td><strong>Kommentar</strong></td>   
      <td>Antal kommentarer som tagits emot.</td>
      </tr>  
      <tr>   
      <td><strong>Räknare</strong></td>
      <td>Visar ett antal bevis som har överförts till ditt konto (du måste ha ett alternativ för bevisräknare aktiverat i Kontoinställningar).</td>
      </tr>
      <tr>
      <td><strong>Skapad</strong></td>
      <td>Datum och tid då objektet skapades.</td>
      </tr>
      <tr>
      <td><strong>Skapare</strong></td>
      <td>Användaren som skapade objektet.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Date added to proof]</strong></td>
      <td>Datumet då du lades till i beviset. </td>
      </tr>
      <tr>
      <td><strong>Deadline</strong></td>
      <td>Tidsgränsen för hela beviset.</td>
      </tr>
      <tr>
      <td><strong>Beslut</strong></td>
      <td>Antal beslut som anges av det förväntade antalet (t.ex. 0 av 1, 1 av 1 osv.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Downloads]</strong></td>
      <td>Antalet gånger som originalfilen har hämtats.</td>
      </tr>
      <tr>
      <td><strong>Filnamn</strong></td>
      <td>Namnet på filen eller korrekturet.</td>
      </tr>
      <tr>
      <td><strong>Mapp</strong></td>
      <td>Mappen som innehåller objektet.</td>
      </tr>
      <tr>
      <td><strong>Senaste aktivitet</strong></td>
      <td>Datum och tid för den senaste aktiviteten för artikeln.</td>
      </tr>
      <tr>
      <td><strong>Senaste beslut om</strong></td>
      <td>Datum och tid för det senaste beslutet.</td>
      </tr>
      <tr>
      <td><strong>Min deadline</strong></td>
      <td>Din egen deadline på korrektur där du uttryckligen läggs till som granskare/godkännare (om det används).</td>
      </tr>
      <tr>
      <td><strong>Ägare</strong></td>
      <td>Objektets ägare.</td>
      </tr>
      <tr>
      <td><strong>Ägarland</strong></td>
      <td>Det land som är registrerat i systemet för bevisets ägare. </td>
      </tr>
      <tr>
      <td><strong>Överordnat bevis</strong></td>
      <td>Namnet på det överordnade korrekturet.</td>
      </tr>
      <tr>
      <td><strong>Förlopp</strong></td>
      <td><p>Förloppsindikator. Visar korrektur som ännu inte har startats, öppnats, kommenterats eller beslutats.</p><p>Informationen sorteras inte på.</p></td>
      </tr>
      <tr>
      <td><strong>Korrekturnamn</strong></td>
      <td>Bevisets namn.</td>
      </tr>
      <tr>
      <td><strong>Korrekturtyp</strong></td>
      <td><p>Korrekturtyp: Statisk fil, Statisk webbsida, Interaktiv webb (.zip-överföring), Interaktiv webbsida (https), Video, Ljud och Övrigt. </p><p>Kombinerade korrektur identifieras som"Kombinerad korrekturtyp". Korrekturens filtyp.</p></td>
      </tr>
      <tr>
      <td><strong>Filstorlek (MB)</strong></td>
      <td><p>Bevisets filstorlek i relation till diskanvändningskvoten.</p><p>Denna information tillhandahålls för den aktuella versionen av korrekturet. Om det inte finns någon aktuell version är det för den senaste versionen.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Tidsgräns för aktivt stadium</strong></p></td>
      <td>Tidsgräns för faser i det automatiserade arbetsflödet.</td>
      </tr>
      <tr>
      <td><strong>Scennamn</strong></td>
      <td>Namn på varje fas i det automatiserade arbetsflödet. Detta inkluderar tidigare faser, aktiva faser och framtida faser.</td>
      </tr>
      <tr>
      <td><strong>Läge</strong></td>
      <td>Aktiv, Låst, Utkast eller Skickat.</td>
      </tr>
      <tr>
      <td><strong>Status</strong></td>
      <td>Väntande, ändringar som krävs, Godkänd med ändringar, Godkänd eller Inte relevant.</td>
      </tr>
      <tr>
      <td><strong>Taggar</strong></td>
      <td>Eventuella taggar som är kopplade till objektet.</td>
      </tr>
      <tr>
      <td><strong>Kommande scennamn</strong></td>
      <td> Namnet på varje fas som ännu inte har startats i det automatiserade arbetsflödet. </td>
      </tr>
      <tr>
      <td><strong>Versionsräknare</strong></td>
      <td> Antalet versioner av objektet. </td>
      </tr>
      <tr>
      <td><strong>Versionsnummer</strong></td>
      <td><i>Versionsnumret för korrekturet.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Valfritt) Gör något av följande om du vill flytta kolumnen till området **[!UICONTROL Selected columns]** så att den tas med i den nya vyn:

      * Ändra ordning på alla kolumner i listan **[!UICONTROL Selected columns]**.
      * Den ordning i vilken kolumnerna visas i listan **[!UICONTROL Selected columns]** avgör i vilken ordning kolumnerna visas i den anpassade vyn.
      * Kolumnerna visas i listan **[!UICONTROL Selected columns]** i den ordning som du har lagt till dem från listan **[!UICONTROL Available columns]**.

      * Om du vill ändra ordning på en kolumn i listan **[!UICONTROL Selected columns]** markerar du namnet på kolumnen och drar den antingen uppåt eller nedåt i listan.

      * Ta bort en kolumn från listan **[!UICONTROL Selected columns]** genom att klicka på namnet på den markerade kolumnen och sedan klicka på pilen **[!UICONTROL Left]** . Du kan också dubbelklicka på namnet på den markerade kolumnen (kolumnen flyttas tillbaka till listan **[!UICONTROL Available columns]**).

      * En kolumn kan bara läggas till en gång. Om du till exempel flyttar kommentarskolumnen från [!UICONTROL Available] till [!UICONTROL Selected columns] försvinner namnet på den här kolumnen från listan [!UICONTROL Available columns].

1. Ange följande information i avsnittet **[!UICONTROL Sorting]**:

   * **Sortera efter:** Använd fliken [!UICONTROL Sorting] om du vill ange i vilken ordning objekten ska visas i den anpassade vyn. Om du inte markerar en kolumn för sortering är standardvärdet Ingen kolumn, d.v.s. ingen särskild sorteringsordning.
   * Endast de kolumner som du har markerat på fliken [!UICONTROL Columns] tas med i listrutan [!UICONTROL Sort by column].
   * **Stigande eller Fallande:** Välj om du vill sortera kolumnen antingen stigande eller fallande som standard.

1. Använd avsnittet **[!UICONTROL Filters]** för att definiera ett eller flera villkor för att välja objekt som ska inkluderas i den anpassade vyn. Filter är särskilt användbara om du vill använda den anpassade vyn som en rapport.
1. Om du vill ta med alla objekt i den anpassade vyn hoppar du över avsnittet **[!UICONTROL Filters]**.
1. Tillgängliga filter:

   * **Fält:** Markera fältet för det här filtret (Kommentarer är standardfältet.) Fältlistan innehåller alla standardfält (som på fliken [!UICONTROL Columns] ). Listan är inte begränsad till de kolumner som du har markerat för visning.
   * **Operator:** Vilka operatorer som är tillgängliga för filtret beror på vilken typ av fält du har valt. Välj en operator som visar relationen mellan fältet och värdefältet. Du kommer att fylla i dessa uppgifter senare.
   * **Värde:** Markera eller ange ditt valda värde i det här fältet, enligt fältet och den operator som du valde. Beroende på vilken operator du väljer kan det finnas ett värdefält eller två eller inga. Se exemplen nedan.
   * **Filter tillämpas med följande logik:** Filtervillkor mellan olika fält använder operatorn AND. Flera filtervillkor som använder samma fält använder operatorn OR för samma fält.

     Om du bara vill visa korrektur med noll kommentarer, väljer du följande värden:

      * Fält: Comments
      * Operatör: Lika med
      * Värdefält: 0

     Om du bara vill visa korrektur med två eller flera kommentarer, väljer du följande värden:

      * Fält: Comments
      * Operatör: Större eller lika med
      * Värdefält: 2

     Om du bara vill visa korrektur med mellan 1 och 4 kommentarer väljer du följande värden:

      * Fält: Comments
      * Operatör: Mellan
      * Värdefält (första fältet): 1
      * Värdefält (andra fältet): 4

        Du kan ändra ett filter som du har lagt till i den anpassade vyn utan problem eller ta bort det genom att klicka på kryssikonen bredvid filtret [!UICONTROL setup] om det behövs.

        Eftersom fältlistan inte är begränsad till de kolumner du har markerat på fliken [!UICONTROL Columns] bör du vara försiktig när du skapar ett filter som innehåller en kolumn som du inte har valt för visning i den anpassade vyn. I följande filter för vyn väljs alla korrektur med ett versionsräknarvärde på 2 eller mer:

         * Fält = Versionsräknare
         * Operator = större eller lika med
         * Värdefält = 2

           >[!NOTE]
           >
           >Du kan ändra ett filter som du har lagt till i den anpassade vyn utan problem eller ta bort det genom att klicka på kryssikonen bredvid filtret [!UICONTROL setup] om det behövs.



1. I avsnittet **[!UICONTROL Sharing]** väljer du vilka användare i ditt konto som ska kunna se din anpassade vy.
1. Anpassade vyer är specifika för den användare som skapar dem. Som standard visas den nya anpassade vyn bara för den som skapat den, men du kan välja att dela den anpassade vyn genom att välja något av följande alternativ:

   * **Endast du kan se den här anpassade vyn** (standard): Välj det här alternativet om du vill att den anpassade vyn ska vara tillgänglig endast för dig.
   * **Alla användare kan se den här anpassade vyn**: Välj det här alternativet om du vill att den anpassade vyn ska vara tillgänglig för alla användare på ditt konto.
   * **Välj användare som kan se den här anpassade vyn**: Välj det här alternativet om du vill att den anpassade vyn endast ska vara tillgänglig för vissa användare.
   * Börja skriva namnet eller e-postadressen till den användare som du vill ska ha åtkomst till den anpassade vyn och klicka sedan på namnet när det visas i listrutan.
   * Om du väljer att inte dela vyn med andra användare kan du göra det senare genom att redigera den anpassade vyn.

1. Klicka på **[!UICONTROL Create]**.
1. Den anpassade vyn visas och är tillgänglig på sidan [!DNL Views]. Mer information om vyer finns i [Hantera objekt på  [!DNL Views] sidan i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Redigera anpassade vyer

Du kan enkelt redigera en anpassad vy. Så här redigerar du en anpassad vy:

1. Gå till sidan **[!UICONTROL Views]**.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på knappen [!UICONTROL Views] (1)
1. Välj den vy som du vill redigera i listrutan.\
   ![Redigera vy](assets/proof-view-edit.png)

1. Klicka på knappen **[!UICONTROL View Options]** och sedan på **[!UICONTROL Edit view]**.\
   ![Visningsalternativ](assets/proof-view-options.png)\
   Sidan Redigera anpassad vy visas.

1. Klicka på menyn [!UICONTROL Actions]. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.
1. Välj [!UICONTROL Edit view] på menyn. (4) \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. Sidan Redigera anpassad vy visas.

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Om du redigerar din anpassade vy ordnas kolumnerna i listan Valda kolumner automatiskt i alfabetisk ordning. Du måste ordna om dem om det behövs innan du uppdaterar vyn.


## Kopiera anpassade vyer

Med funktionen Kopiera vy kan du enkelt skapa en kopia av en befintlig anpassad vy. Det här är till exempel mycket användbart om du vill skapa separata vyer för alla designers, där varje vy är densamma förutom korrekturägaren (designern).

Så här kopierar du en anpassad vy:

1. Gå till sidan **[!UICONTROL Views]**.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på knappen **[!UICONTROL Views]**. (1)
1. Välj din anpassade vy i listan. (2)
1. Klicka på menyn **[!UICONTROL Actions]**. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Copy] på menyn. (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. På sidan Kopiera anpassad vy fylls alla ursprungliga inställningar i. Ändra den anpassade vyn efter ditt val och klicka på knappen **[!UICONTROL Copy view]**. Du kommer nu till den nya vyn omedelbart.\
   ![Kopiera anpassad vy](assets/copy-custom-view-page-350x542.png)

## Dela anpassade vyer

Med funktionen Dela kan du dela en vy med andra användare i ditt konto om du inte redan har valt dem i delningsavsnittet för vyn. När du delar en anpassad vy med andra användare visas vyn i deras [!UICONTROL My custom views]-avsnitt i listrutan Vyer.

Så här delar du en anpassad vy med andra användare:

1. Gå till sidan **[!UICONTROL Views]**.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på knappen **[!UICONTROL Views]** (1)
1. Välj din anpassade vy i listan (2)
1. Klicka på menyn **[!UICONTROL Actions]**. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Share view] på menyn (4)
1. Sidan Redigera anpassad vy visas.
1. I avsnittet [!UICONTROL Sharing] markerar du de användare som du vill dela vyn med och klickar på **[!UICONTROL Update view]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportera anpassade vyer till CSV-filer

Så här exporterar du data från en anpassad vy till en CSV-fil:

1. Gå till sidan **[!UICONTROL Views]**.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på knappen **[!UICONTROL Views]**. (1)
1. Välj din anpassade vy i listan. (2)
1. Klicka på menyn **[!UICONTROL Actions]**. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Export to CSV] på menyn. (4)\
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)\
   I ett separat webbläsarfönster visas&quot;Generera rapport: 100 %&quot; plus antalet poster (antalet objekt i rapporten från din anpassade vy)

1. (Villkorligt) Om ett säkerhetsmeddelande visas som anger att rapporthämtningen är blockerad klickar du på så att hämtningen kan fortsätta.
1. Klicka på **[!UICONTROL Save]** när fönstret Filhämtning visas och du tillfrågas om du vill öppna eller spara filen.
1. Välj en plats på datorn och spara filen.

## Ta bort anpassade vyer

Du kan enkelt ta bort en anpassad vy. Så här gör du:

1. Gå till sidan **[!UICONTROL Views]**.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på knappen **[!UICONTROL Views]**.
1. Välj den anpassade vyn i listan
1. Klicka på menyn **[!UICONTROL Actions]**. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Delete] på menyn. (4)\
   ![deleting_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Klicka på **[!UICONTROL Delete]** (5) för att bekräfta att du vill ta bort den aktuella anpassade vyn\
   ![delete_1_.png](assets/delete--1--350x187.png)

1. Standardvyn Alla objekt visas och den borttagna anpassade vyn visas inte längre i listrutan **[!UICONTROL Views]**.
