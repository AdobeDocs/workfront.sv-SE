---
title: Skapa och hantera ett begärandeformulär i Adobe Workfront Planning
description: När du har valt en posttyp i Adobe Workfront Planning kan du skapa ett begärandeformulär och associera det med den posttypen. Du kan sedan dela en länk till den med andra interna eller externa användare. Användare som har en länk till formuläret kan fylla i fältvärdena på det och genom att skicka det kan de lägga till en ny post för den posttyp som är associerad med det.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '3518'
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

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Alla Workfront-paket och alla Planning-paket</p>
eller
<p>Alla arbetsflödespaket och alla planeringsdokument</p>
<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta eller posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begränsningar för fält- och värdesvisning i begärandeformulär

Det finns begränsningar i hur vissa fält visas i begärandeformuläret och hur deras värden senare visas på posterna eller på sidan med information om begäran när du har skickat en begäran.

Mer information om hur du skickar begäranden om Workfront Planning finns i [Skicka begäranden om Adobe Workfront Planning för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

* Följande är begränsningar för hur vissa fält visas i begärandeformulär, poster som skapats av ett begärandeformulär eller på sidan med information om begäran:

   * Du kan inte lägga till fält av följande typer i ett begärandeformulär:

      * Skapad av, senast ändrad av, Godkänd av
      * Skapat den, senast ändrat den, Godkänt den
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

## Skapa ett begärandeformulär

Om du vill skapa ett begärandeformulär måste du börja skapa formuläret, ställa in formulärinformationen och avsluta genom att publicera och dela formuläret.

### Börja skapa ett begärandeformulär

Du kan skapa ett begärandeformulär från den posttyp som är associerad med formuläret <!--span class="preview">, or from the Requests area of Workfront.</span>-->.

#### Skapa ett begärandeformulär av en posttyp

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
1. Fortsätt till [Konfigurera information för begärandeformuläret](#set-up-details-for-the-request-form).

<!--

<div class="preview">

#### Create a request form from the Requests area of Workfront

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner, then click **Requests**.
1. In the upper-right corner of the screen, click **Request forms**.
1. (Conditional) If you are editing an existing request form, select it from the list, then continue to [Configure the form](#confgure-the-form).
1. If you are creating a new request form, in the upper-right corner of the screen, click **New request form**.

   The Create request form box opens

1. In the Create request form box, update the name of the request form. By default, the name of the form is **Untitled form**. 
1. In the Object types field, select the record type that the request form will be associated with. Record types are grouped into the workspace that they exist within.
1. (Optional) Add a **Description** for the request form. 

1. Click **Create**. 

   The request form for the selected record type opens in the Form tab.
1. Continue to [Set up details for the request form](#set-up-details-for-the-request-form).



</div>

-->

### Ställ in information för begärandeformuläret

Formulärinformationen är uppdelad i flikar.

* På fliken **Formulär** kan du lägga till fält och innehållselement i formuläret
* På fliken **Konfiguration** kan du ange en godkännandeprocess för formuläret och ange alternativ för slutförande av begäran.

  >[!NOTE]
  >
  ><span class="preview">I förhandsvisningsmiljön ersätter fliken Inställningar fliken Konfiguration.</span>
  <!--* <span class="preview">The **Automations** tab allows you to automate what will occur based on features of the request made with the form.</span>-->

#### Ställ in formulärinformation

1. Börja skapa eller redigera ett begärandeformulär, enligt beskrivningen i avsnittet [Börja skapa ett begärandeformulär](#begin-creating-a-request-form).

   eller

   Leta reda på formuläret för begäran i listan Formulär för begäran, klicka i rutan bredvid formulärnamnet och klicka på **Redigera formulär** i det blå fältet längst ned på skärmen.

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
1. Fortsätt till något av följande:

   * [Konfigurera konfigurationsinformation](#set-up-configuration-details) om du vill konfigurera mer information för formuläret i produktionsmiljön
   * <span class="preview">[Konfigurera inställningar](#configure-settings) om du vill konfigurera mer information för formuläret i produktionsmiljön</span>
   * [Slutför skapandet av begärandeformuläret](#complete-request-form-creation) om du inte vill konfigurera fler inställningar.

#### Ställ in konfigurationsinformation

>[!NOTE]
>
>Fliken är bara tillgänglig i produktionsmiljön.

På fliken Konfiguration kan du ange godkännandeprocessen och konfigurera när en begäran som skapats från det här formuläret ska markeras som Slutförd.

1. Börja skapa eller redigera ett begärandeformulär, enligt beskrivningen i avsnittet [Börja skapa ett begärandeformulär](#begin-creating-a-request-form).

   Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.
1. (Valfritt) Konfigurera formulärinformation enligt beskrivningen i [Konfigurera formulärinformation](#set-up-form-details).

1. (Valfritt) Om du vill lägga till godkännare klickar du på fliken **Konfiguration** och lägger sedan till minst en användare eller grupp i fältet **Godkännare** för att godkänna nya begäranden för det här postformuläret.

   ![Fliken Konfiguration](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Du kan lägga till en eller flera godkännare i ett begärandeformulär.
   * Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte. Begäran finns kvar under Begäranden i Workfront.
   * Om du lägger till mer än en godkännare och alternativet Endast ett beslut krävs inte är aktiverat, måste alla godkännare fatta ett beslut innan en begäran godkänns eller avslås.
   * Om ett team utses till godkännare krävs endast ett beslut från teamet.

   Mer information om hur du lägger till godkännanden i begärandeformulär finns i [Lägga till godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Villkorligt) Om du vill att posten ska skapas efter att någon av godkännarna har godkänt den, markerar du kryssrutan **Endast ett beslut krävs**.

1. Välj om du vill att en begäran som skapats från det här formuläret ska markeras som fullständig när det begärda objektet skapas, eller när det begärda objektet slutförs.
1. (Villkorligt) Om du har valt att begäran ska markeras som slutförd när det begärda objektet slutförs, markerar du det fält och det värde som anger när objektet är klart. Du kan till exempel välja fältstatus och värdet Fullständig för att slutföra begäran när det skapade objektets status är Fullständig.
1. Fortsätt till <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Slutför formulärskapandet för begäran](#complete-request-form-creation).

<div class="preview">

### Konfigurera inställningar

>[!NOTE]
>
>Den här fliken är bara tillgänglig i förhandsvisningsmiljön.

På fliken Inställningar kan du ange godkännanderegler och konfigurera när en begäran som skapats från det här formuläret ska markeras som Slutförd.

#### Konfigurera godkännanderegler

Godkännanderegler definierar godkännandeprocessen baserat på fältvärden som används i de skickade förfrågningarna.

Om ett begärandeformulär till exempel har fältet&quot;Kampanjtyp&quot; kan en regel skapas som skickar begäran till en person när fältet har värdet&quot;Digital&quot;, och en annan person när det har värdet&quot;Skriv ut&quot;.

Tänk på följande när du lägger till godkännanderegler:

* Reglerna prioriteras efter order. Om villkoren för den första regeln är uppfyllda tillämpas den regeln, även om villkoren för reglerna längre ned i listan också är uppfyllda.
* Om inga villkor uppfylls används standardregeln.
* Du kan lägga till en eller flera godkännare till en godkännanderegel.
* Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte. Begäran finns kvar under Begäranden i Workfront.
* Om du lägger till mer än en godkännare och alternativet Endast ett beslut krävs inte är aktiverat, måste alla godkännare fatta ett beslut innan en begäran godkänns eller avslås.
* Om ett team utses till godkännare krävs endast ett beslut från teamet.

Mer information om hur du lägger till godkännanden finns i [Lägga till godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

Så här anger du godkännanderegler för ett begärandeformulär:

1. Börja skapa eller redigera ett begärandeformulär, enligt beskrivningen i avsnittet [Börja skapa ett begärandeformulär](#begin-creating-a-request-form).

   Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.
1. (Valfritt) Konfigurera formulärinformation enligt beskrivningen i [Konfigurera formulärinformation](#set-up-form-details).

1. Om du vill börja konfigurera godkännanderegler klickar du på ikonen för godkännande ![](assets/approvals-icon-on-form.png) i den vänstra navigeringen.

1. (Valfritt) Om du vill ange en standardprocess för godkännande lägger du till minst en användare eller grupp i fältet **Godkännare** i området Standardregel för godkännande. Klicka sedan på kryssrutan **Endast ett beslut krävs** om du vill att posten ska skapas när någon av standardgodkännarna har godkänt den.

   ![Standardområde för godkännanderegel](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Valfritt) Gör följande för varje ytterligare regel för godkännande:

   1. Klicka på **Lägg till godkännanderegel**
   1. Klicka på platshållartiteln &quot;Namnlös godkännanderegel&quot; och ange ett namn för godkännanderegeln.
   1. Klicka på **Markera ett fält** och markera fältet som aktiverar regeln.
   1. Välj operatorn för regeln. Operatorer varierar beroende på fälttyp.
   1. Om den markerade operatorn kräver ett värde klickar du på plusikonen och lägger till ett eller flera värden.
   1. (Valfritt) Lägg till fler villkor med AND eller OR genom att klicka på Lägg till villkor och konfigurera det ytterligare villkoret.
   1. I området Åtgärder i godkännanderegeln i fältet **Godkännare** lägger du till minst en användare eller grupp som ska anges som godkännare när villkoret är uppfyllt.
   1. (Villkorligt) Om du vill att posten ska skapas efter att någon av godkännarna har godkänt den, markerar du kryssrutan **Endast ett beslut krävs**.

1. (Valfritt) Om du vill ändra ordningen på regler för routning klickar du på draghandtaget på regelns vänstra sida och drar linjen till önskad plats.

   Det går inte att ändra ordningen på standardregeln.

1. (Valfritt) Om du vill ta bort en routningsregel klickar du på **X** till höger om regeln.
1. Klicka på **Spara** för att spara godkännandereglerna.
1. Fortsätt till [Ange alternativ för slutförande av begäran](#set-request-completion-options)

#### Ange alternativ för slutförande av begäran

Med alternativen för slutförande kan du ange om en begäran ska markeras som slutförd när det begärda objektet skapas eller när det skapade objektet slutförs. Du definierar när objektet är färdigt baserat på ett angivet villkor.

1. Börja skapa eller redigera ett begärandeformulär, enligt beskrivningen i avsnittet [Börja skapa ett begärandeformulär](#begin-creating-a-request-form).

   Formuläret för begäran om den valda posttypen öppnas på fliken Formulär.
1. (Valfritt) Konfigurera formulärinformation enligt beskrivningen i [Konfigurera formulärinformation](#set-up-form-details).

1. Välj om du vill att en begäran som skapats från det här formuläret ska markeras som fullständig när det begärda objektet skapas, eller när det begärda objektet slutförs.
1. (Villkorligt) Om du har valt att begäran ska markeras som slutförd när det begärda objektet slutförs, markerar du det fält och det värde som anger när objektet är klart. Du kan till exempel välja fältstatus och värdet Fullständig för att slutföra begäran när det skapade objektets status är Fullständig.
1. Fortsätt till <!--[Set up Automations details](#set-up-configuration-details) if you want to configure more details for the form, or go to -->[Slutför formulärskapandet för begäran](#complete-request-form-creation).

</div>

<!--
 
<div class="preview">

#### Set up Automations

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. 

For information on creating automations in other areas of Workfront Planning, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. Currently, the only available trigger for request form automation is `When request object status equals pending creation`.

1. Update the following fields in the **Actions** section: 

   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Currently, the only available Action for request form automation is `Create record`.

     >[!TIP]
     >
     >After you saved the automation, you can no longer change the action selected in this field.
1. Continue to  [Complete request form creation](#complete-request-form-creation).


</div>

-->

### Skapa formulär för fullständig begäran

1. Skapa och konfigurera formuläret enligt beskrivningen i [Börja skapa ett begärandeformulär](#begin-creating-a-request-form) och [Konfigurera information för begärandeformuläret](#set-up-details-for-the-request-form).
1. (Valfritt) Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om formulärets namn i rubriken och klicka sedan på **Redigera** för att uppdatera formulärets namn.

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

## Hantera befintliga förfrågningsformulär


1. Klicka på arbetsytan där du vill hantera förfrågningsformulär.

   Arbetsytan öppnas och posttyperna visas som kort.

1. Klicka på ett posttypskort. Mer information om hur du skapar en posttyp finns i [Skapa posttyper](/help/quicksilver/planning/architecture/create-record-types.md).

   Posttypssidan öppnas i den vy som du senast använde. Som standard öppnas en posttypssida i tabellvyn.

1. Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om posttypens namn i sidhuvudet och klicka sedan på **Hantera begärandeformulär**.

   Alla förfrågningsformulär som är associerade med posttypen visas i en tabellvy.

1. (Valfritt) Hovra över namnet på ett begärandeformulär i tabellvyn, klicka sedan på menyn **Mer** ![Mer](assets/more-menu.png) till höger om formulärnamnet och klicka på något av följande:

   * **Redigera formulär**: Klicka här om du vill redigera information i formuläret ytterligare.
   * **Avpublicera**: Klicka här för att avpublicera formuläret som tar bort det från området med förfrågningar i Workfront.
   * **Dela**: Klicka här för att ändra vem som har åtkomst till formuläret.
   * **Kopiera länk**: Klicka här om du snabbt vill kopiera länken för begärandeformuläret utan att öppna formuläret.
   * **Ta bort**: Klicka här för att ta bort formuläret. Alla förfrågningar och poster som lagts till med formuläret tas inte bort. Formuläret kan inte återskapas.

   ![Mer meny i begärandeformulär från listan över begärandeformulär](assets/more-menu-on-request-form-from-request-forms-list.png)

1. Klicka på vänsterpilen till vänster om **Begär formulär** i sidhuvudet för att stänga tabellen med förfrågningsformulär.

   Posttypssidan öppnas.
1. (Valfritt och villkorligt) Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) till höger om posttypens namn i rubriken och gör sedan något av följande:

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
