---
title: Skicka Adobe Workfront Planning-begäranden
description: När någon delar en länk till ett begärandeformulär med dig från en posttypsida i Adobe Workfront Planning, kan du lägga till en begäran om att skapa poster för den posttyp som är associerad med förfrågningsformuläret.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 88b8443525043a0710dfc6f93739e54f2e78a569
workflow-type: tm+mt
source-wordcount: '1816'
ht-degree: 0%

---

# Skicka Adobe Workfront Planning-begäranden för att skapa poster

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

När en arbetsytehanterare har skapat ett begärandeformulär för en posttyp i Adobe Workfront Planning kan du använda formuläret för att skicka begäranden som skapar poster för den posttyp som är associerad med formuläret.

Du kan skicka in en begäran om Workfront Planning från följande områden:

* Under Begäranden i Workfront.
* Från en direktlänk till det begärandeformulär som delats.

  I den här artikeln beskrivs hur du kan skicka en begäran om att lägga till nya poster till en posttyp från området Begäranden i Workfront, eller från en delad länk.
* Från posttypssidan när du lägger till eller begär en ny post. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

Workfront-användare och externa användare kan skicka förfrågningar till posttyperna Planning och skapa poster. <!--double check on the external users-->

Mer information om hur en arbetsytehanterare kan skapa ett begärandeformulär och associera det med en posttyp finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </td>
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
   <td>
   <p>Extern licens, Contributor, Light eller Standard</p>
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
   <p>Visa eller högre behörigheter för en arbetsyta <!--<span class="preview">and record type</span>-->, om du är en Workfront-användare</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Om du vill komma åt Planning-området i Workfront måste du ha tilldelats en layoutmall som innehåller Planning-området på huvudmenyn. </p>
   <p> Du behöver dock inte komma åt Planning-området för att kunna skicka in begäranden till Workfront Planning. </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Följande måste finnas innan du kan skicka en begäran till ett Workfront Planning-formulär:

* Följande måste finnas i Workfront Planning:

   * En arbetsyta
   * En posttyp.
   * Ett begärandeformulär som är associerat med en posttyp.

     Mer information finns i [Skapa ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Ansökningsformuläret måste delas på ett sätt som du kan komma åt. Följande scenarier finns:

   * Internt måste formuläret delas med användare som har behörigheten Visa eller högre till arbetsytan.

     Workfront-användare kan antingen öppna formuläret via en länk eller hitta förfrågningsformuläret i området Begäranden i Workfront.

   * Om du inte har något Workfront-konto har en länk till formuläret delats med externa personer.

     Workfront-användare kan även komma åt en länk som delas med externa personer.

* Länken till formuläret får inte upphöra att gälla.

## Att tänka på när du skickar begäranden till Workfront Planning

* Du kan inte redigera en begäran i Workfront efter att du har skickat den.
* Varje skickad begäran skapar en post för den posttyp som är kopplad till det formulär du använder, om formuläret inte är kopplat till ett godkännande, eller om godkännandet har beviljats av alla godkännare.
* Poster som skapas genom att skicka frågeformulär kan inte skiljas från poster som läggs till med någon annan metod i Workfront Planning.

  Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Skickade begäranden visas på fliken Planering i avsnittet Skickat i området Begäranden i Workfront.
* Det finns begränsningar i hur vissa fälttyper visas i ett begärandeformulär eller på sidan med information om förfrågan när ett formulär har skickats.

  Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Skicka en begäran till Workfront Planning under Begäranden i Workfront

>[!NOTE]
>
>Efter de månatliga releaserna i Production är funktionerna som beskrivs i det här avsnittet även tillgängliga i produktionsmiljön för kunder som aktiverat snabba releaser.

{{step1-to-requests}}

1. Aktivera inställningen **Växla till en ny upplevelse** i skärmens övre högra hörn.
Om du aktiverar den här inställningen blir Workfront Planning-förfrågningsformulären tillgängliga i området **Förfrågningar** i Workfront.

   >[!TIP]
   >
   >Den här inställningen är bara tillgänglig när följande är på plats:
   >
   >* Ditt företag har köpt ett Workfront Planning-paket.
   >* Din Workfront-instans är registrerad på Adobe Unified Experience.
   >* Du kan visa minst en arbetsyta.
   >

1. Klicka på **Ny begäran**.

   ![Ny begäranderuta med enhetliga Workfront- och planeringskort](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   Rutan **Ny begäran** öppnas med följande information:

   * De sex senast öppnade begärandeköerna för Workfront och planeringsförfrågningsformulären visas i avsnittet Senaste.
   * 50 ytterligare begärandeköer för Workfront och planeringsförfrågningsformulär visas i alfabetisk ordning i avsnittet **Alla förfrågningsformulär**. Du kan söka efter en begärandekö som inte visas som standard.

1. Gör något av följande:

   * Klicka på kortet för ett av planeringsförfrågningsformulären i avsnitten Senaste eller Alla förfrågningsformulär
   * Börja skriva namnet på ett planeringsbegärandeformulär i sökrutan och klicka sedan på kortet när det visas i listan.

   Formuläret för begäran öppnas.

1. Uppdatera fälten som är tillgängliga i begärandeformuläret. Fält med en röd asterisk är obligatoriska.
1. Klicka på **Skicka**.

   Begärandeformuläret stängs och du återgår till området **Begäranden**.

   Ditt formulär skickas och följande saker händer:

   * Om begärandeformuläret inte var kopplat till ett godkännande läggs begäran till på fliken Planering i avsnittet Skickat i området Workfront-förfrågningar och en ny post läggs till i posttypen som är kopplad till formuläret.

   * Om begärandeformuläret associerades med ett godkännande läggs begäran till på fliken Planering i avsnittet Skickat i området Workfront-förfrågningar. En ny post läggs bara till på posttypssidan när alla godkännare har godkänt den.

     Mer information finns i [Lägga till ett godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Området med förfrågningar och växlar för den enhetliga fliken för arbetsflödesplanering](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >Alla användare som har tillgång till minst en arbetsyta kan visa fliken Planering i området Begäranden. Du kan bara visa de förfrågningar som du eller någon annan har skickat till arbetsytorna som du har minst behörighet att visa. Workfront-administratörer kan visa alla begäranden som skickas till valfri arbetsyta i systemet.

   * Du får ett meddelande i appen och ett e-postmeddelande om att begäran antingen har skickats eller skickats för granskning.
   * Om begärandeformuläret associerades med ett godkännande får godkännarna ett meddelande i appen och ett e-postmeddelande för att granska och godkänna begäran.

     >[!NOTE]
     >
     >Meddelanden via e-post och appar visas bara när din organisations instans av Workfront är kopplad till Adobe Unified Experience.
     >
     >Det finns en länk till begäran i e-postbekräftelsen eller godkännandemeddelandet.

   1. (Valfritt) Klicka på **Visa din begäran** i bekräftelsemeddelandet om du vill öppna begäran eller klicka på ikonen **X** om du vill stänga bekräftelsen.

1. (Valfritt) Klicka på fliken **Planering** i området Begäranden för att visa din begäran och klicka sedan på namnet på begäran.

   Sidan med information om förfrågan öppnas.

   ![Sidan Begär information](assets/request-details-page.png)

1. (Villkorligt) Om begärandeformuläret inte är kopplat till ett godkännande, eller om begäran har godkänts, klickar du på namnet på begäran och sedan på postens namn i fältet **Post**.

   Postens sida öppnas i Workfront Planning.

   >[!TIP]
   >
   >* Om postens primära fält inte har uppdaterats i begärandeformuläret visas postens namn i postfältet i begäran som **Namnlöst**.
   >
   >* Om begärandeformuläret är kopplat till ett godkännande måste det godkännas innan du kan få åtkomst till posten från begärandesidan.

1. (Valfritt) Klicka på namnet på **posttypen**.

   Posttypssidan öppnas i Workfront Planning.

## Skicka en begäran till Workfront Planning från en delad länk till ett begärandeformulär

1. Gå till länken som delas med dig från en Workfront Planning-posttyp.

1. Uppdatera fälten som är tillgängliga i formuläret. Fält med asterisk är obligatoriska.

   >[!TIP]
   >
   >   Om fältet **Ämne** är tillgängligt visas det inte i Workfront Planning när begäran har skickats.
   >
   >Vi rekommenderar att du uppdaterar så många fält i din begäran som möjligt för att göra den nya posten identifierbar när den läggs till i posttypen i Workfront Planning.

1. Klicka på **Skicka**.

   Ditt formulär skickas och följande saker händer:

   * Om begärandeformuläret inte var kopplat till ett godkännande läggs begäran till på fliken Planering i avsnittet Skickat i området Workfront-förfrågningar och en ny post läggs till i posttypen som är kopplad till formuläret.

   * Om begärandeformuläret associerades med ett godkännande läggs begäran till på fliken Planering i avsnittet Skickat i området Workfront-förfrågningar. En ny post läggs bara till på posttypssidan när alla godkännare har godkänt den.

     Mer information finns i [Lägga till ett godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Fliken Planering i begäranden](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Alla användare som har tillgång till minst en arbetsyta kan visa fliken Planering i området Begäranden. Du kan bara visa de förfrågningar som du eller någon annan har skickat till arbetsytorna som du har minst behörighet att visa. Workfront-administratörer kan visa alla begäranden som skickas till valfri arbetsyta i systemet. <!--ensure this is correct; asking team in slack-->

   * Du får ett meddelande i appen och ett e-postmeddelande om att begäran antingen har skickats eller skickats för granskning.
   * Om begärandeformuläret associerades med ett godkännande får godkännarna ett meddelande i appen och ett e-postmeddelande för att granska och godkänna begäran.

     >[!NOTE]
     >
     >Meddelanden via e-post och appar visas bara när din organisations instans av Workfront är kopplad till Adobe Unified Experience.

1. (Valfritt) Klicka på **Visa din begäran** för att öppna begäran i Workfront.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Valfritt) Klicka på **Huvudmeny** > **Förfrågningar** > fliken **Planering** för att visa din förfrågan och klicka sedan på namnet på förfrågan.

   Sidan med information om förfrågan öppnas.

   ![Sidan Begär information](assets/request-details-page.png)

1. (Villkorligt) Om begärandeformuläret inte är kopplat till ett godkännande, eller om begäran har godkänts, klickar du på namnet på begäran och sedan på postens namn i fältet **Post**.

   Postens sida öppnas i Workfront Planning.

   >[!TIP]
   >
   >* Om postnamnet inte har lagts till i begärandeformuläret visas postens namn i fältet Post i begäran som **Namnlöst**.
   >
   >* Om begärandeformuläret är kopplat till ett godkännande måste det godkännas innan du kan få åtkomst till posten från begärandesidan.

1. (Valfritt) Klicka på namnet på **posttypen**.

   Posttypssidan öppnas i Workfront Planning.




