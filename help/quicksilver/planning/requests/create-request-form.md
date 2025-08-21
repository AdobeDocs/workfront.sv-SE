---
title: Skapa och hantera ett begärandeformulär i Adobe Workfront Planning
description: När du har valt en posttyp i Adobe Workfront Planning kan du skapa ett begärandeformulär och associera det med den posttypen. Du kan sedan dela en länk till den med andra interna eller externa användare. Användare som har en länk till formuläret kan fylla i fältvärdena på det och genom att skicka det kan de lägga till en ny post för den posttyp som är associerad med det.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 359131cef04fdb46def64428a7a693c3f00b2cd4
workflow-type: tm+mt
source-wordcount: '2564'
ht-degree: 0%

---

# Skapa och hantera ett begärandeformulär i Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Du kan skapa ett begärandeformulär och associera det med en posttyp i Adobe Workfront Planning. Du kan sedan dela formuläret med andra och de kan skicka in begäranden för att skapa poster av den typen.

I den här artikeln beskrivs hur en arbetsytehanterare kan skapa ett begärandeformulär som är associerat med en posttyp.

Mer information om hur du skickar en begäran till en posttyp för att skapa en post finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven. 

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
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att få tillgång till Workfront Planning.</p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <ul>
   <li><p>Hantera behörigheter till en arbetsyta och en posttyp</p></li>
    <li><p>Systemadministratörer kan hantera arbetsytor som de inte skapade. </p></li>
    </ul>
   <p>Information om delningsbehörigheter för Workfront Planning-objekt finns i  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Workfront Planning</a> 
  </td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Begränsningar för fält- och värdesvisning i begärandeformulär

Det finns begränsningar i hur vissa fält visas i begärandeformuläret och hur deras värden senare visas på posterna eller på sidan med information om begäran när du har skickat en begäran.

Mer information om hur du skickar begäranden om Workfront Planning finns i [Skicka begäranden om Adobe Workfront Planning för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

* Följande är begränsningar för hur vissa fält visas i begärandeformulär, poster som skapats av ett begärandeformulär eller på sidan med information om begäran:

   * Du kan inte lägga till fält av följande typer i ett begärandeformulär:

      * Skapad av, senast ändrad av, <span class="preview">Godkänd av</span>
      * Skapad den, senast ändrat den, <span class="preview">Godkänt den</span>
      * Workfront-objektens sökfält
      * Sökfält för Workfront Planning-anslutna poster

* Följande är skillnader mellan hur fältformat visas i formulärbyggaren och hur fältvärdena formateras på posten eller på sidan med information om begäran:

   * Fälten Valuta, Nummer och Procent visas som ett textfält med en rad i formulärbyggaren.

     Fältformatet bevaras dock och fältvärdena visas som valuta, siffror och procenttal efter att begäran har skickats, på posttypen och på sidan med information om begäran.

* Här nedan beskrivs hur vissa fältvärden visas i begärandeformulär och sidorna med förfrågningsinformation:

   * Specialformatering för valutafält, tal och procent bevaras inte. Decimalprecisionen bevaras t.ex. inte för dessa fälts värden i dessa områden.
   * Värden för personfält visas som ID.
   * Formelfält som inte refererar till andra fält eller beräkningar visar inga värden. Ett fält med formeln `STRING` visar till exempel ett N/A-värde.
   * Formelfält som refererar till valutafält visar värden utan redovisning för valutakurser.
   * Värdena i styckefälten visar ett N/A-värde i begärandeformuläret och de visar html-taggar i stället för formaterad text på sidan med information om begäran.

## Börja skapa ett begärandeformulär

Du kan skapa ett begärandeformulär från den posttyp som är associerad med formuläret, <span class="preview">eller från området Begäranden i Workfront.</span>

### Skapa ett begärandeformulär av en posttyp

{{step1-to-planning}}

1. Klicka på arbetsytan där du vill lägga till poster.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.

1. Klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn i sidhuvudet och klicka sedan på **Skapa begärandeformulär** eller **Hantera begärandeformulär** om du redan har ett formulär och vill skapa ytterligare.
1. (Villkorligt) Om du vill lägga till ett annat formulär klickar du på **Nytt begärandeformulär**.

   Rutan Skapa begärandeformulär öppnas.

1. Uppdatera namnet på begärandeformuläret i rutan Skapa begärandeformulär. Som standard är formulärets namn **Namnlöst formulär**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Valfritt) Lägg till en **beskrivning** för begärandeformuläret.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klicka på **Skapa**.

   Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.
1. Fortsätt till [Konfigurera formuläret](#configure-the-form).

<div class="preview">

### Skapa ett begärandeformulär från området Begäranden i Workfront

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Begäranden**.
1. Klicka på **Begär formulär** i skärmens övre högra hörn.
1. (Villkorligt) Om du redigerar ett befintligt begärandeformulär markerar du det i listan och fortsätter sedan med [Konfigurera formuläret](#confgure-the-form).
1. Om du skapar ett nytt begärandeformulär klickar du på **Nytt begärandeformulär** i skärmens övre högra hörn.

   Rutan Skapa begärandeformulär öppnas

1. Uppdatera namnet på begärandeformuläret i rutan Skapa begärandeformulär. Som standard är formulärets namn **Namnlöst formulär**.
1. I fältet Objekttyper väljer du den posttyp som begärandeformuläret ska kopplas till. Posttyper grupperas i den arbetsyta som de finns på.
1. (Valfritt) Lägg till en **beskrivning** för begärandeformuläret.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klicka på **Skapa**.

   Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.
1. Fortsätt till [Konfigurera formuläret](#configure-the-form).

</div>

## Konfigurera formuläret

1. Börja skapa eller redigera ett begärandeformulär, vilket beskrivs i något av följande avsnitt:

   * [Skapa ett begärandeformulär av en posttyp](#create-a-request-form-from-a-record-type)
   * <span class="preview">[Skapa ett begärandeformulär från området Förfrågningar i Workfront](#create-a-request-form-from-the-requests-area-of-workfront)</span>

   Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.

   ![Formulärredigeringsläge för kampanjförfrågningar](assets/campaigns-request-form-edit-mode.png)

   Formuläret innehåller som standard följande information:

   * Postfält som är tillgängliga i tabellvyn för den valda posttypen. <!--they are working on removing the limitation below-->

   * **Standardavsnitt**: Det här är standardavsnittsbrytningen som Workfront tillämpar på begärandeformuläret. Alla postfält visas i området **Standardavsnitt**.
   * Fältet **Ämne**: Fältet som identifierar begäran i Workfront. Det går inte att redigera konfigurationen och värdet för ämnesfältet.

     >[!NOTE]
     >
     >* Fältet **Ämne** kräver ett värde när det är synligt i begärandeformuläret. Du kan dock ta bort fältet **Ämne** om det behövs, och den som beställer kan inte se det i formuläret när de skickar begäran.
     >* När ämnesfältet saknas i ett begärandeformulär men det finns ett namnfält för den framtida postens namn, tilldelas namnet på begäran automatiskt samma namn som den skapade posten.
     >* När både ämnes- och namnfälten saknas i formuläret för begäran namnges begäran med följande mönster: `< Record name > request form < Entry date of the request >`. Posten heter **Namnlös**.

   * Alla fält som är associerade med posttypen.

     Fälten i begärandeformuläret är synliga för alla som skickar en begäran till den här posttypen.

1. (Valfritt) Håll markören över fält i formuläret som du vill ta bort och klicka sedan på ikonen **x** för att ta bort dem. De läggs till på fliken **Fält** till vänster om formuläret.

   Ta till exempel bort fältet **Ämne** eftersom det inte visas i Workfront Planning. <!--remove this example if this becomes visible in Planning?-->

1. (Valfritt) Så här tar du bort **standardavsnittet** från formuläret:

   1. Ta bort alla fält från standardavsnittet.
   1. Klicka på **Innehållselement** och lägg till ett nytt avsnitt och lägg sedan till ett namn för avsnittet.
   1. Lägg till fält i det nya avsnittet.
   1. Klicka på ikonen **x** för att ta bort **standardavsnittet**.
1. Klicka på ett fält och använd sedan kontrollerna på den högra panelen i formuläret för att definiera deras storlek eller någon av följande information:

   * **Etikett**: Det här är namnet på fältet som det kommer att visas i begärandeformuläret. Detta ändrar inte postfältets namn.
   * **Instruktioner**: Lägg till mer information om fältet.
   * **Gör ett obligatoriskt fält**: När du väljer det här alternativet måste fältet ha ett värde. Annars kan formuläret inte skickas.
   * **Lägg till logik**: Definiera vilka villkor som måste uppfyllas för att fältet ska kunna visas eller döljas.

   >[!TIP]
   >
   >   Fälttypen för varje fält visas längst upp på den högra panelen när du har valt fältet i formuläret.
   >     

1. (Valfritt) Klicka på fliken **Innehållselement** till vänster i formuläret och lägg till något av följande element:

   * **Beskrivande text**
   * **Avsnittsbrytning**

   Mer information om hur du skapar ett anpassat formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Valfritt) Klicka på **Förhandsgranska** om du vill visa hur formuläret kommer att visas för andra användare när de kommer att använda det för att skicka en ny post.

1. (Valfritt) Klicka på fliken **Konfiguration** och lägg sedan till minst en användare <span class="preview">eller team</span> i fältet **Godkännare** för att godkänna nya begäranden för det här postformuläret.

   ![Fliken Konfiguration](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * När du associerar ett begärandeformulär med godkännare måste alla nya begäranden först godkännas av alla godkännare innan de genererar en ny post.
   * Du kan lägga till en eller flera godkännare i ett begärandeformulär.
   * Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte.
   * Alla godkännare måste fatta ett beslut innan en begäran godkänns eller avslås.
   * <span class="preview">Om ett team har angetts som godkännare krävs endast ett beslut från teamet.</span>

     Mer information om hur du lägger till godkännanden i begärandeformulär finns i [Lägga till godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Valfritt) Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om formulärets namn i rubriken och klicka sedan på **Redigera** för att uppdatera formulärets namn.

1. Klicka på **Publicera** för att publicera formuläret och få en unik länk för det.

   Följande saker händer:

   * Knappen **Publicera** har tagits bort.
   * Knappen **Avpublicera** läggs till i formuläret. Om du klickar på den går det inte att komma åt formuläret.
   * En **Dela**-knapp läggs till i formuläret.
   * Formuläret blir tillgängligt under Begäranden på huvudmenyn i Workfront.

1. Klicka på **Dela** om du vill dela formuläret med andra.

   Mer information om hur du delar ett begärandeformulär finns i avsnittet [Dela ett begärandeformulär](#share-a-request-form) i den här artikeln
1. Klicka på vänsterpilen till vänster om formulärets namn i rubriken för att stänga formuläret.

   Tabellvyn **Begär formulär** öppnas och formuläret läggs till i den.

1. (Valfritt) Hovra över namnet på ett begärandeformulär i tabellvyn, klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png) till höger om formulärnamnet och klicka på något av följande:

   * **Redigera formulär**: Klicka här om du vill redigera information i formuläret ytterligare.
   * **Avpublicera**: Klicka här för att avpublicera formuläret som tar bort det från området med förfrågningar i Workfront.
   * **Dela**: Klicka här för att ändra vem som har åtkomst till formuläret.
   * **Kopiera länk**: Klicka här om du snabbt vill kopiera länken för begärandeformuläret utan att öppna formuläret.
   * **Ta bort**: Klicka här för att ta bort formuläret. Alla förfrågningar och poster som lagts till med formuläret tas inte bort. Formuläret kan inte återskapas.

   ![Mer meny i begärandeformulär från listan över begärandeformulär](assets/more-menu-on-request-form-from-request-forms-list.png)

1. Klicka på vänsterpilen till vänster om **Begär formulär** i sidhuvudet för att stänga tabellen med förfrågningsformulär.

   Posttypssidan öppnas.
1. (Valfritt och villkorligt) Klicka på menyn **Mer** ![Mer ](assets/more-menu.png) till höger om posttypens namn i rubriken och gör sedan något av följande:

   1. Klicka på **Uppdatera begärandeformuläret** för att göra ändringar i begärandeformuläret och klicka sedan på ett begärandeformulär för att öppna och redigera det.
   1. Klicka på **Kopiera länk för att begära formulär** om du vill dela länken till formuläret med andra.

1. (Valfritt) Gå till området **Begäranden** i Workfront och leta reda på det delade formuläret för att skicka en begäran. Mer information finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Dela ett begärandeformulär

1. Skapa ett begärandeformulär enligt beskrivningen i avsnittet [Skapa ett begärandeformulär för en posttyp](#create-a-request-form-for-a-record-type) i den här artikeln.
1. Klicka på **Mer**-menyn ![Mer-menyn](assets/more-menu.png) till höger om begärandeformulärets namn på posttypens sida.
1. Klicka på **Dela** om du vill dela formuläret med andra.

1. Om du vill dela formuläret internt väljer du fliken **Intern delning**, söker efter namnet på en användare, ett team, en jobbroll, en grupp eller ett företag i fältet **Bevilja åtkomst för att skicka det här formuläret** och markerar det när det visas i listan. Behörigheten **Skicka** är markerad som standard för varje entitet.

   ![Delningsruta för begärandeformulär](assets/share-box-for-request-form.png)

1. (Valfritt) Klicka på listrutan efter namnet på en entitet och klicka sedan på **Ta bort** för att ta bort dem från listan och sluta dela formuläret med dem.

   >[!NOTE]
   >
   >Förutom team, grupper, företag och jobbroller kan du bara dela med användare som har lagts till i Adobe Admin Console. Du kan inte lägga till användare med endast Workfront. Mer information finns i [Hantera användare i Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. I avsnittet **Vem kan skicka begäranden via det här formuläret** väljer du bland följande alternativ för att ange vilka typer av användare som kan få åtkomst till det här formuläret:

   * Endast inbjudna personer har åtkomst
   * Alla som visar eller har högre åtkomst till arbetsytan
   * Alla som har Contribute eller senare åtkomst till arbetsytan
1. (Valfritt) Klicka på **Kopiera länk** om du vill dela länken till formuläret med personer som har behörighet att göra det. Länken kopieras till Urklipp.
1. Om du vill dela formuläret offentligt väljer du fliken **Offentlig delning** och aktiverar sedan inställningen **Skapa offentlig länk** .

   ![Offentlig delning för begärandeformulär](assets/share-request-form-publicly-tab.png)

   >[!WARNING]
   >
   >* När du aktiverar inställningen **Skapa offentlig länk** kan vem som helst få åtkomst till formuläret och skicka en ny post, även personer utanför organisationen som inte har något Workfront-konto.
   >
   >* Ett formulär som innehåller följande fälttyper kan inte delas offentligt:
   >
   >     * Workfront- eller AEM Assets-anslutningar
   >     * Folk
   >

1. Välj ett **länkförfallodatum**.

   Du kan välja framtida datum inom 180 dagar från dagens datum.

   >[!TIP]
   >
   >Efter att delningsdatumet har gått ut är förfrågningsformuläret inte längre tillgängligt i området Begäranden i Workfront och länkarna som delas med andra användare är inte längre tillgängliga.

   Användarna får ett felmeddelande när länken har upphört att gälla och du måste uppdatera länkdatumet och generera en ny länk som de kan dela innan de kan komma åt formuläret igen.


1. (Valfritt och villkorligt) Klicka på **Spara** för att spara delningsinformationen för formuläret.
1. (Villkorligt) Om formuläret har sparats tidigare klickar du på **Kopiera länk**.

   Alternativen för formulärdelning sparas och länken kopieras till Urklipp. Nu kan du dela den med andra.

   Mer information om hur du skapar poster med hjälp av en länk till ett begärandeformulär finns i [Skicka Adobe Workfront Planning-begäranden](/help/quicksilver/planning/requests/submit-requests.md).

1. Klicka på **Spara** i det nedre högra hörnet på fliken **Formulär** för att spara formuläret.
