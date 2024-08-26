---
title: Skicka Adobe Workfront Planning-begäranden
description: När någon delar en länk till ett begärandeformulär med dig från en posttypsida i Adobe Workfront Planning, kan du lägga till en begäran om att skapa poster för den posttyp som är associerad med förfrågningsformuläret.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 18183b53c783366f467e7330159923372b51deb6
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Skicka Adobe Workfront Planning-begäranden för att skapa poster

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

När någon delar en länk till ett begärandeformulär med dig från en posttypsida i Adobe Workfront Planning, kan du lägga till en begäran om att skapa poster för den posttyp som är associerad med förfrågningsformuläret.

Workfront-användare och externa användare kan skicka förfrågningar till posttyperna Planning och skapa poster. <!--double check on the external users-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna komma åt Workfront Planning:

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
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td>
   <td>
<p>Alla </p>  
<p>Mer information om vad som ingår i varje Workfront Planning-plan finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront priser och paketering</a>. </td>

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

   * Om du har ett Workfront-konto har länken bara delats med interna personer och du har tillgång till arbetsytan. Personer utanför Workfront kan inte komma åt en länk som delas internt.
   * Om du inte har något Workfront-konto har länken delats med externa personer. Workfront-användare kan också använda en länk som delas med externa personer.

* Länken till formuläret får inte upphöra att gälla.

## Att tänka på när du skickar begäranden till Workfront Planning

* Du kan inte komma åt förfrågningsformulären för Workfront Planning-begäranden utan en specifik länk till formulären.
* Du kan inte redigera en begäran efter att du har skickat den till Workfront Planning.
* Varje skickad begäran skapar en post för den posttyp som är associerad med det formulär som du använder.
* Poster som skapas genom att frågeformulär skickas kan inte skiljas från poster som läggs till med någon annan metod. Mer information finns i [Skapa poster](/help/quicksilver/planning/records/create-records.md).

## Skicka en begäran till Workfront Planning

1. Gå till länken som delas med dig från en Workfront Planning-posttyp.

1. Uppdatera fälten som är tillgängliga i formuläret. Fält med asterisk är obligatoriska.

   >[!TIP]
   >
   >   Om fältet **Ämne** är tillgängligt kanske det inte visas i Workfront Planning. Vi rekommenderar att du uppdaterar så många fält i din begäran som möjligt för att göra den nya posten identifierbar när den läggs till i posttypen.

1. Klicka på **Skicka**.

   Formuläret skickas och en ny post läggs till i posttypen som är kopplad till formuläret.





