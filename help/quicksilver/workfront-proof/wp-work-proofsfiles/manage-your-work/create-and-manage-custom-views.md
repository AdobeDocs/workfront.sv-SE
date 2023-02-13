---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Skapa och hantera anpassade vyer i [!DNL Workfront Proof]
description: Du kan skapa anpassade vyer av dina filer och korrektur för att lista de objekt du vill ha på det sätt du vill att de ska visas. Du kan också exportera informationen i den anpassade vyn som en rapport (i CSV, kommaavgränsat värde, filformat).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2359'
ht-degree: 0%

---

# Skapa och hantera anpassade vyer i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Du kan skapa anpassade vyer av dina filer och korrektur för att lista de objekt du vill ha på det sätt du vill att de ska visas. Du kan också exportera informationen i den anpassade vyn som en rapport (i CSV, kommaavgränsat värde, filformat).

>[!NOTE]
>
>Anpassade vyer är bara tillgängliga för Select- och Premium-planer. Kontakta vårt säljteam för en offert.

## Skapa en anpassad vy

När du skapar en anpassad vy kan du välja:

* Om korrektur, filer eller båda ska inkluderas
* Vilka kolumner som visas
* Vilken kolumn som ska sorteras efter
* Sorteringsordningen för kolumnen (stigande eller fallande)
* Vilka typer av filter som ska användas för att bestämma vilken information som ska tas med i vyn

När den anpassade vyn har skapats kan den användas omedelbart. Namnet på den nya vyn finns också i listrutan under rubriken Mina anpassade vyer (under standardvyer).

Så här skapar du en anpassad vy:

1. Gå till **[!UICONTROL Views]** sida.
1. Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Gör något av följande, beroende på om du vill skapa en ny anpassad vy från början eller skapa en ny anpassad vy baserad på en befintlig standardvy:

   * Så här skapar du en ny anpassad vy baserad på en befintlig standardvy: I listrutan väljer du den befintliga standardvyn som du vill använda som bas för den nya anpassade vyn. Klicka på **[!UICONTROL View Settings]** ikonen och klicka sedan på **[!UICONTROL Copy]** till ny anpassad vy.

   * ![](assets/proof-custom-view-icon.png)

   * Så här skapar du en ny anpassad vy från grunden: Klicka på **[!UICONTROL New View]** ikon.
   * ![](assets/proof-newview.png)

1. I **[!UICONTROL Details]** anger du följande information:

   * **[!UICONTROL Name]** (obligatoriskt): Namnet på den nya vyn. Använd ett unikt namn så att användarna enkelt kan hitta den anpassade vyn i listrutan i Vyer.
   * **[!UICONTROL Items]**: Välj om du vill att både korrektur och fil, endast korrektur eller bara filer ska inkluderas i vyn. Som standard inkluderas både korrektur och filer.

1. I **[!UICONTROL Columns]** anger du vilka kolumner du vill ta med i den anpassade vyn.

   1. Klicka på högerpilsikonen.
   1. ![](assets/proof-view-rightarrow.png)

   1. Dubbelklicka på namnet på den markerade kolumnen.
   1. Du måste markera minst en kolumn och en kolumn kan bara läggas till en gång.
   1. Välj en kolumn i **[!UICONTROL Available columns]** området som du vill ta med i den nya vyn.
   1. Kolumnerna flyttas från **[!UICONTROL Available columns]** till **[!UICONTROL Selected columns]** lista.

   1. Du kan välja bland standardkolumnerna eller så kan du välja Anpassade fält och Beslutsorsaker som kolumner i den anpassade vyn. (Om du har konfigurerat de här kolumnerna i ditt konto visas de i standardlistan med tillgängliga kolumner.)
   1. Standardkolumner som du kan inkludera

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Namn på aktivt stadium</strong></td>   
      <td>Namnet på den aktiva fasen i det automatiserade arbetsflödet.</td>  
      </tr>  
      <tr>   
      <td><strong>Kommentarer</strong></td>   
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
      <td><p>Förloppsindikator. Visar korrektur som ännu inte har startats, öppnats, kommenterats eller beslutats.</p><p>Den här informationen är inte sorterad efter.</p></td>
      </tr>
      <tr>
      <td><strong>Korrekturnamn</strong></td>
      <td>Bevisets namn.</td>
      </tr>
      <tr>
      <td><strong>Korrekturtyp</strong></td>
      <td><p>Typ av bevis: Statisk fil, Statisk webbsida, Interaktiv webb (.zip-överföring), Interaktiv webbsida (https), Video, Ljud och Övrigt. </p><p>Kombinerade korrektur identifieras som"Kombinerad korrekturtyp". Korrekturens filtyp.</p></td>
      </tr>
      <tr>
      <td><strong>Filstorlek (MB)</strong></td>
      <td><p>Bevisets filstorlek i relation till diskanvändningskvoten.</p><p>Denna information tillhandahålls för den aktuella versionen av beviset. Om det inte finns någon aktuell version är det för den senaste versionen.</p></td>
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
      <td><strong>Versionsnummer för korrektur</strong></td>
      <td><i>Versionsnumret för korrekturet.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Valfritt) Gör något av följande om du vill flytta kolumnen till **[!UICONTROL Selected columns]** så att den tas med i den nya vyn:

      * Ändra ordning på kolumner i **[!UICONTROL Selected columns]** lista.
      * Den ordning i vilken kolumnerna visas i **[!UICONTROL Selected columns]** -listan avgör i vilken ordning kolumnerna visas i den anpassade vyn.
      * Kolumnerna visas i **[!UICONTROL Selected columns]** i den ordning som du har lagt till dem i **[!UICONTROL Available columns]** lista.

      * Ändra ordning på en kolumn i **[!UICONTROL Selected columns]** markerar du namnet på kolumnen och drar den antingen uppåt eller nedåt i listan.

      * Ta bort en kolumn från **[!UICONTROL Selected columns]** genom att klicka på namnet på den markerade kolumnen och sedan på **[!UICONTROL Left]** pil. Du kan också dubbelklicka på namnet på den markerade kolumnen (kolumnen flyttas tillbaka till **[!UICONTROL Available columns]** lista).

      * En kolumn kan bara läggas till en gång. Om du till exempel flyttar kommentarkolumnen från [!UICONTROL Available] till [!UICONTROL Selected columns] listan kommer namnet på den här kolumnen att försvinna från [!UICONTROL Available columns] lista.

1. I **[!UICONTROL Sorting]** anger du följande information:

   * **Sortera efter:** Använd [!UICONTROL Sorting] om du vill ange i vilken ordning objekten ska visas i den anpassade vyn. Om du inte markerar en kolumn för sortering är standardvärdet Ingen kolumn, d.v.s. ingen särskild sorteringskolumn eller sorteringsordning.
   * Endast de kolumner som du markerade på [!UICONTROL Columns] -fliken finns i [!UICONTROL Sort by column] nedrullningsbar lista.
   * **Stigande eller fallande:** Välj om du vill sortera kolumnen antingen stigande eller fallande som standard.

1. Använd **[!UICONTROL Filters]** för att definiera ett eller flera villkor för att markera objekt som ska tas med i den anpassade vyn. Filter är särskilt användbara om du vill använda den anpassade vyn som en rapport.
1. Om du vill ta med alla objekt i den anpassade vyn hoppar du över **[!UICONTROL Filters]** -avsnitt.
1. Tillgängliga filter:

   * **Fält:** Välj fält för det här filtret (Kommentarer är standardfältet.) Fältlistan innehåller alla standardfält (som i [!UICONTROL Columns] -fliken). Listan är inte begränsad till de kolumner som du har markerat för visning.
   * **Operatör:** Vilka operatorer som är tillgängliga för filtret beror på vilken typ av fält du har valt. Välj en operator som visar relationen mellan fältet och värdefältet. Du kommer att fylla i dessa uppgifter senare.
   * **Värde:** Välj eller ange ditt valda värde i det här fältet, enligt fältet och den operator du valde. Beroende på vilken operator du väljer kan det finnas ett värdefält eller två eller inga. Se exemplen nedan.
   * **Filter tillämpas med följande logik:** För filtervillkor mellan olika fält används operatorn AND. Flera filtervillkor som använder samma fält använder operatorn OR för samma fält.

      Om du bara vill visa korrektur med noll kommentarer, väljer du följande värden:

      * Fält: Kommentarer
      * Operatör: Lika med
      * Värdefält: 0

      Om du bara vill visa korrektur med två eller flera kommentarer, väljer du följande värden:

      * Fält: Kommentarer
      * Operatör: Större eller lika med
      * Värdefält: 2

      Om du bara vill visa korrektur med mellan 1 och 4 kommentarer väljer du följande värden:

      * Fält: Kommentarer
      * Operatör: Mellan
      * Värdefält (första fältet): 1
      * Värdefält (andra fältet): 4

         Du kan ändra ett filter som du har lagt till i den anpassade vyn utan problem eller ta bort det genom att klicka på kryssikonen bredvid [!UICONTROL setup] vid behov.

         Eftersom fältlistan inte är begränsad till de kolumner som du har markerat i [!UICONTROL Columns] ska du vara försiktig när du skapar ett filter som innehåller en kolumn som du inte har valt för visning i din anpassade vy. I följande filter för vyn väljs alla korrektur med ett versionsräknarvärde på 2 eller mer:

         * Fält = Versionsräknare
         * Operator = större eller lika med
         * Värdefält = 2

            >[!NOTE]
            >
            >Du kan ändra ett filter som du har lagt till i den anpassade vyn utan problem eller ta bort det genom att klicka på kryssikonen bredvid [!UICONTROL setup] vid behov.





1. I **[!UICONTROL Sharing]** väljer du vilka användare på ditt konto som ska kunna se din anpassade vy.
1. Anpassade vyer är specifika för den användare som skapar dem. Som standard visas den nya anpassade vyn bara för den som skapat den. Du kan dock välja att dela den anpassade vyn genom att välja något av följande alternativ:

   * **Endast du kan se den här anpassade vyn** (standard): Välj det här alternativet om du vill att den anpassade vyn ska vara tillgänglig endast för dig.
   * **Alla användare kan se den här anpassade vyn**: Välj det här alternativet om du vill att den anpassade vyn ska vara tillgänglig för alla användare på ditt konto.
   * **Välj användare som kan se den här anpassade vyn**: Välj det här alternativet om du vill att den anpassade vyn endast ska vara tillgänglig för vissa användare.
   * Börja skriva namnet eller e-postadressen till den användare som du vill ska ha åtkomst till den anpassade vyn och klicka sedan på namnet när det visas i listrutan.
   * Om du väljer att inte dela vyn med andra användare kan du göra det senare genom att redigera den anpassade vyn.

1. Klicka på **[!UICONTROL Create]**.
1. Vyn Anpassad visas och är tillgänglig på [!DNL Views] sida. Mer information om vyer finns i [Hantera objekt på [!DNL Views] Sida in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

## Redigera anpassade vyer

Du kan enkelt redigera en anpassad vy. Så här redigerar du en anpassad vy:

1. Gå till **[!UICONTROL Views]** sida.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på [!UICONTROL Views] knapp (1)
1. Välj den vy som du vill redigera i listrutan.\
   ![](assets/proof-view-edit.png)

1. Klicka på **[!UICONTROL View Options]** och sedan klicka **[!UICONTROL Edit view]**.\
   ![](assets/proof-view-options.png)\
   Sidan Redigera anpassad vy visas.

1. Klicka på [!UICONTROL Actions] -menyn. (3)\
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

1. Gå till **[!UICONTROL Views]** sida.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på **[!UICONTROL Views]** -knappen. (1)
1. Välj din anpassade vy i listan. (2)
1. Klicka på **[!UICONTROL Actions]** -menyn. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Copy] på menyn. (4)\
   ![copying_custom_view.png](assets/copying-custom-view-350x258.png)

1. På sidan Kopiera anpassad vy fylls alla ursprungliga inställningar i. Ändra den anpassade vyn enligt ditt val och klicka på **[!UICONTROL Copy view]** -knappen. Du kommer nu till den nya vyn omedelbart.\
   ![](assets/copy-custom-view-page-350x542.png)

## Dela anpassade vyer

Med funktionen Dela kan du dela en vy med andra användare i ditt konto om du inte redan har valt dem i delningsavsnittet för vyn. När du delar en anpassad vy med andra användare visas vyn i deras [!UICONTROL My custom views] i listrutan Vyer.

Så här delar du en anpassad vy med andra användare:

1. Gå till **[!UICONTROL Views]** sida.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på **[!UICONTROL Views]** knapp (1)
1. Välj din anpassade vy i listan (2)
1. Klicka på **[!UICONTROL Actions]** -menyn. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Share view] från menyn (4)
1. Sidan Redigera anpassad vy visas.
1. I [!UICONTROL Sharing] markerar du de användare som du vill dela vyn med och klickar på **[!UICONTROL Update view]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportera anpassade vyer till CSV-filer

Så här exporterar du data från en anpassad vy till en CSV-fil:

1. Gå till **[!UICONTROL Views]** sida.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på **[!UICONTROL Views]** -knappen. (1)
1. Välj din anpassade vy i listan. (2)
1. Klicka på **[!UICONTROL Actions]** -menyn. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Export to CSV] på menyn. (4)\
   ![exporting_custom_view.png](assets/exporting-custom-view-350x258.png)\
   I ett separat webbläsarfönster, &#39;Genererar rapport: 100 % visas plus antalet poster (antalet objekt som ingår i rapporten från din anpassade vy)

1. (Villkorligt) Om ett säkerhetsmeddelande visas som anger att rapporthämtningen är blockerad klickar du på så att hämtningen kan fortsätta.
1. Klicka **[!UICONTROL Save]** när fönstret Filhämtning visas och du tillfrågas om du vill öppna eller spara filen.
1. Välj en plats på datorn och spara filen.

## Ta bort anpassade vyer

Du kan enkelt ta bort en anpassad vy. Så här gör du:

1. Gå till **[!UICONTROL Views]** sida.\
   Mer information om vyer finns i [Hantera objekt på sidan Vyer i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicka på **[!UICONTROL Views]** -knappen.
1. Välj den anpassade vyn i listan
1. Klicka på **[!UICONTROL Actions]** -menyn. (3)\
   Den här knappen är bara tillgänglig om du tar med kolumnen Korrekturnamn i vyn.

1. Välj [!UICONTROL Delete] på menyn. (4)\
   ![deleting_custom_view.png](assets/deleting-custom-view-350x258.png)

1. Klicka **[!UICONTROL Delete]** (5) för att bekräfta att du vill ta bort den aktuella anpassade vyn\
   ![delete_1_.png](assets/delete--1--350x187.png)

1. Standardvyn Alla objekt visas och den borttagna anpassade vyn visas inte längre i dialogrutan **[!UICONTROL Views]** nedrullningsbar meny.
