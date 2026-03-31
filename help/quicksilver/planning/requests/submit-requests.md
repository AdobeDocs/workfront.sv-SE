---
title: Skicka Adobe Workfront Planning-begäranden
description: När någon delar en länk till ett begärandeformulär med dig från en posttypsida i Adobe Workfront Planning, kan du lägga till en begäran om att skapa poster för den posttyp som är associerad med förfrågningsformuläret.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 0%

---

# Skicka Adobe Workfront Planning-begäranden för att skapa poster

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

När en arbetsytehanterare har skapat ett begärandeformulär för en posttyp i Adobe Workfront Planning kan du använda formuläret för att skicka begäranden som skapar poster för den posttyp som är associerad med formuläret.

Du kan skicka in en begäran om Workfront Planning från följande områden:

* Från området Förfrågningar i Workfront eller från widgeten Mina förfrågningar i Hem.
* Från en direktlänk till det begärandeformulär som delats.
* Från posttypssidan, när du lägger till en ny post genom att skicka en begäran. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

I den här artikeln beskrivs hur du kan skicka en begäran om att lägga till nya poster till en posttyp från området Begäranden i Workfront, eller från en delad länk.

Workspace-chefer kan skapa förfrågningsformulär som du kan använda som användare eller extern person för att skicka förfrågningar till posttyperna Planning. Förfrågningarna skapar poster för den posttyp som är associerad med förfrågningsformuläret.

Mer information om hur en arbetsytehanterare kan skapa ett begärandeformulär och associera det med en posttyp finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

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
   <td><p>Alla</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Visa eller högre behörigheter för en arbetsyta och posttyp om du är en Workfront-användare</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Följande måste finnas innan du kan skicka en begäran till ett Workfront Planning-formulär:

* Följande måste finnas i Workfront Planning:

   * En arbetsyta
   * En posttyp
   * Ett begärandeformulär som är associerat med en posttyp.

     Mer information finns i [Skapa ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Ansökningsformuläret måste delas på ett sätt som du kan komma åt. Följande scenarier finns:

   * Internt måste formuläret delas med användare som har behörigheten Visa eller högre till arbetsytan.

     Workfront-användare kan antingen öppna formuläret via en länk eller hitta förfrågningsformuläret i området Begäranden i Workfront.

   * Externt genom att dela en länk till postformuläret med externa personer som inte har något Workfront-konto.

     Workfront-användare kan även komma åt länken som delas med externa personer.

* Om den delas med en länk får länken till formuläret inte upphöra att gälla.

## Att tänka på när du skickar begäranden till Workfront Planning

* Du kan inte redigera en begäran i Workfront efter att du har skickat den.
* Varje skickad begäran skapar en post för den posttyp som är kopplad till det formulär du använder, om formuläret inte är kopplat till ett godkännande, eller om godkännandet har beviljats av alla godkännare.
* Poster som skapas genom att skicka förfrågningsformulär är identiska med poster som läggs till med någon annan metod i Workfront Planning.

  Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* Poster som skapas när förfrågningsformulär skickas är kopplade till den ursprungliga begäran. Det går inte att ta bort den här anslutningen.
* Du kan visa både poster som skapats och förfrågningar som använts för att skapa dem i följande områden:
   * Området med förfrågningar i Workfront.

  <div class="preview">

   * I ett anslutet fält på en posttypssida i Workfront Planning när du lägger till begäran som en ansluten post.
   * I ett anslutet fält i området Detaljer för en post i Workfront Planning när du lägger till begäran som en ansluten post.

  </div>

  >[!TIP]
  >
  ><span class="preview">Du kan visa namnet på begäran i fältet Ämne i området Begäranden i Workfront eller i fältet Original request connection i Workfront Planning. </span>

* Skickade planeringsbegäranden visas bara i den nya begärande upplevelsen. Du kan inte se Planering-begäranden i den äldre upplevelsen av begäranden.

  Mer information finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Det finns begränsningar i hur vissa fälttyper visas i ett begärandeformulär eller på sidan med information om förfrågan när ett formulär har skickats.

  Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Skicka en begäran till Workfront Planning under Begäranden i Workfront

{{step1-to-requests}}

1. Aktivera inställningen **Använd ny upplevelse** i skärmens övre högra hörn.
Om du aktiverar den här inställningen blir Workfront Planning-förfrågningsformulären tillgängliga i området **Begäranden** i Workfront.

   >[!TIP]
   >
   >Den här inställningen är bara tillgänglig när din Workfront-instans har anslutits till Adobe Unified Experience.
   >
   >För att kunna skicka in Workfront Planning-begäranden i det här området måste du uppfylla följande villkor:
   >
   >* Ditt företag har köpt en licens för Workfront Planning.
   >
   >* Du kan visa minst en arbetsyta.

1. Klicka på **Vilken begäran vill du skicka?**-fält om du vill öppna en lista med förfrågningsformulär.
1. Välj ett begärandeformulär i listan eller skriv in namnet på det begärande formuläret och markera det när det visas i listan.

   Ett fönster öppnas med det efterfrågade formulärnamnet överst.

   >[!TIP]
   >
   >Workfront begärandeköer innehåller namnet på kön och namnet på formuläret i listan över förfrågningar. Vid planering av begäranden visas endast formulärnamnet i listan med begäranden.

1. Uppdatera fältet **Ämne**. Det här är namnet på begäran. Detta är ett obligatoriskt fält.
1. Uppdatera fältet **Namn**. Det här är namnet på den framtida posten.

   >[!TIP]
   >
   >Fältet **Namn** är unikt för din organisation och kan visa en annan etikett i din Workfront-instans. Fältet är det primära fältet i posten.

1. Uppdatera de återstående fälten i begärandeformuläret. Fält med en röd asterisk är obligatoriska.
1. (Villkorligt) Om din organisation tillåter **formulärfyllning** som drivs av AI, kan du överföra dokument som du uppmanas till. AI använder dessa dokument för att fylla i formuläret, och du kan godkänna eller avvisa AI-förslagen innan du skickar begäran.


   Instruktioner finns i [Använd formulärfyllning från AI för att fylla i en begäran med hjälp av uppmaningar eller dokument](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Klicka på **Skicka**.

   Begärandeformuläret stängs och du återgår till området **Begäranden**.

   Ditt formulär skickas och följande saker händer:

   * Om begärandeformuläret inte var kopplat till ett godkännande läggs begäran till i listan över förfrågningar i området Workfront-förfrågningar och widgeten Mina förfrågningar i Hem, och en ny post läggs till i posttypen som är kopplad till formuläret.

     Följande fält visar information om begäran och registrering i området Förfrågningar och widgeten Mina förfrågningar i Hem:

      * **Ämne**: Namnet på den ursprungliga begäran som lagts till i området Begäranden. Du kan inte dölja eller ta bort fältet **Ämne** från listan över förfrågningar.
      * **Skapat objekt**: Namnet på posten som skapades från begäran så som den visas i Planning.
      * **Objekttyp**: Namnet på arbetsytan och posttypen där poster skapades från begäran i Planning.
      * **Status**: Status för begärandeobjektet.
      * **Formulär för begäran**: Namnet på det begärandeformulär som är associerat med posttypen i Planning.
     <!--* <span class="preview"**Created object status**: The status of the created record.</span> -->

   * Om begärandeformuläret associerades med ett godkännande läggs begäran till i listan över förfrågningar i området Workfront-förfrågningar och i widgeten Mina förfrågningar med statusen **Väntande granskning**. En ny post läggs bara till på posttypssidan efter att godkännarna har godkänt den.

     Mer information finns i [Lägga till ett godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * <span class="preview">Du kan lägga till anslutningsfältet **Originalbegäran** till en posttyp i Planning för att visa namnet på den ursprungliga begäran som skapade en post. Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * Begäran är bara synlig för ägaren, godkännaren och de personer som har minst behörigheten Visa på arbetsytan. Workfront-administratörer kan visa alla begäranden som skickas till valfri arbetsyta i systemet.
   * Du får ett meddelande i appen och ett e-postmeddelande om att begäran antingen har skickats eller skickats för granskning.
   * Om begärandeformuläret associerades med ett godkännande får godkännarna ett meddelande i appen och ett e-postmeddelande för att granska och godkänna begäran.

     >[!NOTE]
     >
     >E-postmeddelandet och meddelandet i appen visas bara när din organisations instans av Workfront är kopplad till Adobe Unified Experience.
     >
     >Det finns en länk till begäran i e-postbekräftelsen eller godkännandemeddelandet.

1. (Valfritt) Klicka på **Visa din begäran** i bekräftelsemeddelandet om du vill öppna begäran eller klicka på ikonen **X** om du vill stänga bekräftelsen.
1. (Valfritt) Om du vill hantera hur informationen visas i listan med begäranden uppdaterar du följande vyelement för listan:

   * Visa
   * Filter
   * Kolumner

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   Mer information finns i [Skapa och hantera vyer i området Förfrågningar](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).

   <!--   
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. Klicka på namnet på en begäran i listan.

   Sidan med information om förfrågan öppnas.

   ![Begär sida med kommentar](assets/new-request-page-with-comment.png)

1. (Valfritt) Ange en kommentar i området **Kommentarer**.
1. (Villkorligt) Om begärandeformuläret inte är kopplat till ett godkännande, eller om begäran har godkänts, klickar du på namnet på begäran och sedan på namnet på posten i fältet **Skapat objekt**.

   Postens sida öppnas i Workfront Planning.

   >[!TIP]
   >
   >* Om postens primära fält inte har uppdaterats i begärandeformuläret visas postens namn i postfältet i begäran som **Namnlöst**.
   >
   >* Om begärandeformuläret är kopplat till ett godkännande måste det godkännas innan du kan få åtkomst till posten från begärandesidan. Posten skapas inte förrän godkännandet har beviljats.

1. (Valfritt) Klicka på namnet på **posttypen**.

   Posttypssidan öppnas i Workfront Planning.

## Skicka en begäran till Workfront Planning från en delad länk till ett begärandeformulär

Informationen i det här avsnittet gäller endast för personer som skickar en begäran via en delad länk och som kanske inte har ett Workfront-konto.

Externa personer har inte åtkomst till interna Workfront-områden, till exempel **Förfrågningar** eller **Hem**.

1. Gå till länken som delas med dig från en Workfront Planning-posttyp.

1. Uppdatera fälten som är tillgängliga i formuläret. Fält med asterisk är obligatoriska.

   >[!TIP]
   >
   >   Om fältet **Ämne** är tillgängligt visas det inte i Workfront Planning när begäran har skickats.
   >
   >Vi rekommenderar att du uppdaterar så många fält i din begäran som möjligt för att göra den nya posten identifierbar när den läggs till i posttypen i Workfront Planning.

1. Klicka på **Skicka**.

   Formuläret har skickats och du får en bekräftelse.

   Om formuläret är kopplat till ett godkännande måste det godkännas innan det kan skapa en post.

1. (Valfritt) Klicka på **Skicka en ny begäran** om du vill lägga till en ny begäran till samma delade länk.

<!--
   * If the request form was not associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget in Home, and a new record is added to the record type associated with the form. This is available only when you log in to Workfront.
   
   * If the request form was associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget. A new record is added to the record type page only after all the approvers have approved it. This is available only when you log in to Workfront.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      >[!IMPORTANT]
      >
      >You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. <!--ensure this is correct; asking team in slack
   
   
   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.
      >[!NOTE]
      >
      >The email and in-app notification are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.
   
   <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>


1. (Optional) Click **View your request** to open the request in Workfront.


Or

Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.

   The request details page opens. 

   ![Request page with comment](assets/new-request-page-with-comment.png)

1. (Optional) Enter a comment in the **Comments** area.
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Created object** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Object type**. 

   The record type page opens in Workfront Planning. 

-->

## Skapa en begäran genom att kopiera en befintlig begäran

Du kan kopiera en begäran i listan över förfrågningar i Workfront, redigera informationen och skicka den som en ny förfrågan.

Detta är endast tillgängligt i den nya upplevelsen av begärande.

Att kopiera en befintlig planeringsbegäran och skicka den som en ny liknar att kopiera en befintlig Workfront-begäran.

Mer information finns i [Kopiera och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Skapa utkast och förfrågningar från befintliga utkast

Du kan skapa ett utkast av en begäran, sedan gå tillbaka till utkastet och skicka det som en begäran senare.

Detta är endast tillgängligt i den nya upplevelsen av begärande. Att skapa utkast och begäranden från befintliga utkast i Workfront Planning är detsamma som att skapa dem från Adobe Workfront.

Mer information finns i [Skapa begäranden från utkast](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

## Ta bort utkast eller skickade begäranden

Du kan ta bort skickade begäranden eller utkast av dem när du använder det nya gränssnittet.

När du tar bort en planeringsförfrågan händer följande:

* Begäran kan inte återställas.
* Posten som skapas från begäran tas inte bort.
* Borttagna utkast kan inte återställas. Det finns inga poster associerade med utkast.

Att ta bort planeringsbegäranden liknar att ta bort Workfront-begäranden.

Mer information finns i [Ta bort en skickad begäran eller ett utkast av en begäran](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md).







