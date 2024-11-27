---
title: Skicka Adobe Workfront Planning-begäranden
description: När någon delar en länk till ett begärandeformulär med dig från en posttypsida i Adobe Workfront Planning, kan du lägga till en begäran om att skapa poster för den posttyp som är associerad med förfrågningsformuläret.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: d7c7b09b033705142b2c658c9d275e63299d3fd0
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---


# Skicka Adobe Workfront Planning-begäranden för att skapa poster

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

När någon delar en länk till ett begärandeformulär med dig från en posttypsida i Adobe Workfront Planning, kan du lägga till en begäran om att skapa poster för den posttyp som är associerad med förfrågningsformuläret.

Workfront-användare och externa användare kan skicka förfrågningar till posttyperna Planning och skapa poster. <!--double check on the external users-->

I den här artikeln beskrivs hur du kan skicka en begäran om att lägga till nya poster i en posttyp.

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
   <p>Visa eller högre behörigheter för en arbetsyta om du är Workfront-användare</p> 
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
   * En posttyp som är associerad med ett begärandeformulär. Mer information finns i [Skapa ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Formuläret för begäran måste delas med en länk på ett sätt som gör att du kan komma åt det. Följande scenarier finns:

   * Om du har ett Workfront-konto har länken bara delats med interna medarbetare och du har tillgång till arbetsytan med högre eller högre behörighet. Personer utanför Workfront kan inte komma åt en länk som delas internt.
   * Om du inte har något Workfront-konto har länken delats med externa personer. Workfront-användare kan även komma åt en länk som delas med externa personer.

* Länken till formuläret får inte upphöra att gälla.

## Att tänka på när du skickar begäranden till Workfront Planning

* Du kan bara få åtkomst till ett begärandeformulär för Workfront Planning-begäranden från en specifik länk till formuläret.
* Du kan inte redigera en begäran efter att du har skickat den till Workfront Planning.
* Varje skickad begäran skapar en post för den posttyp som är associerad med formuläret som du använder <!--<span class="preview">if the form is not associated with an approval, or if the approval has been granted.</span> -->
* Poster som skapas genom att frågeformulär skickas kan inte skiljas från poster som läggs till med någon annan metod. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).
* <span class="preview">Skickade begäranden visas på fliken Planering i avsnittet Skickat i området Begäranden i Workfront </span>.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some incosistency between unified-approvals-service and intake-approvals-flow.-->


## Skicka en begäran till Workfront Planning

1. Gå till länken som delas med dig från en Workfront Planning-posttyp.

1. Uppdatera fälten som är tillgängliga i formuläret. Fält med asterisk är obligatoriska.

   >[!TIP]
   >
   >   Om fältet **Ämne** är tillgängligt visas det inte i Workfront Planning när begäran har skickats.
   >
   >Vi rekommenderar att du uppdaterar så många fält i din begäran som möjligt för att göra den nya posten identifierbar när den läggs till i posttypen i Workfront Planning.

1. Klicka på **Skicka**.

   Ditt formulär skickas och följande saker händer:

   * <!--If the request form was not associated with an approval, or <span class="preview">if the approval was granted</span>, a-->En ny post läggs till i posttypen som är kopplad till formuläret.


   * <!--If the request form was not associated with an approval, the--> <span class="preview"> Begäran läggs till i avsnittet Skickat i området Workfront-förfrågningar och en ny post läggs till på posttypssidan.</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">Alla användare som har tillgång till minst en arbetsyta kan visa fliken Planering i området Begäranden. Du kan bara visa de begäranden som du har skickat. Workfront-administratörer kan visa alla begäranden i systemet. </span> <!--ensure this is correct; asking team in slack-->

   <!--
   * <span class="preview">If the request form was associated with an approval, the request is temporarily saved to the Planning tab in the Submitted section of the Workfront Requests area. No record is created for the record type associated with the request form.</span>

      <span class="preview">For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>  
   -->
   <!--

   * <span class="preview">You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.</span> 
   * <span class="preview">If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.</span> 
   -->



