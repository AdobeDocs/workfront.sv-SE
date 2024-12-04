---
title: Godkänn en begäran
description: När en användare skickar en begäran till ett begärandeformulär som är kopplat till ett godkännande i Adobe Workfront Planning får godkännarna ett meddelande och ett e-postmeddelande om det väntande godkännandet. De måste godkänna begäran innan Workfront Planning skapar ett objekt.
hide: true
hidefromTOC: true
source-git-commit: ab78b82db567193f32f6c67880b2b037dc78e849
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---


<!--

---
title: Approve a Request
description: When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->


# Godkänn en begäran

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">Informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

När en användare skickar en begäran till ett begärandeformulär som är kopplat till ett godkännande i Adobe Workfront Planning får godkännarna ett meddelande och ett e-postmeddelande om det väntande godkännandet. De måste godkänna begäran innan Workfront Planning skapar ett objekt.

I den här artikeln beskrivs hur en arbetsytehanterare kan godkänna en begäran om att skapa en post i Workfront Planning.

Vi rekommenderar att du också ser följande artiklar:

* [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md)
* [Lägga till ett godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Överväganden om att godkänna begäranden och status för begäranden

Skickade begäranden visas på fliken Planering i avsnittet Skickat i området Begäranden i Workfront med en av följande begärandestatusar:

* **Väntande granskning**: Den här statusen visas när ingen av godkännarna har öppnat begäranobjektet.
* **Under granskning**: Statusen ändras till **Under granskning** när minst en godkännare öppnar begäranobjektet. Status för begäran förblir **Under granskning** tills alla godkännare har godkänt begäran.
* **Godkänd**: När en godkännare godkänner begäranobjektet blir deras individuella status
* **Godkänd**, men den övergripande statusen för begärandeobjektet är **Under granskning** tills alla godkännare har fattat sina beslut.
* **Slutförd**: Om alla godkännare godkänner begäranobjektet ändras dess status till **Slutförd** eller om begäran inte behövde något godkännande.
* **Avvisad**: Om någon godkännare avvisar begärandeobjektet blir statusen **Avvisad**. Ingen post skapas och en ny begäran måste skickas för att posten ska kunna skapas.

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
   <li><p>Hantera behörigheter till en arbetsyta</p></li>
    <li><p>Systemadministratörer kan hantera arbetsytor som de inte skapade. </p></li>
    </ul>
   <p>Information om delningsbehörigheter för Workfront Planning-objekt finns i  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Godkänn en begäran om att skapa en post

När användare har lagt till begäranden i ett formulär för posttypbegäran som är kopplat till ett godkännande, skickas begäran till godkännarna.

Godkännare får följande meddelanden om en begäran som väntar på deras godkännande:

* Ett meddelande i appen
* Ett e-postmeddelande

Så här godkänner du en begäran:

1. Gör något av följande:

   * Om du har tillgång till Workfront Planning klickar du på **Huvudmeny** ![](assets/dots-menu.png) i skärmens övre högra hörn, eller på **Huvudmeny** ![](assets/lines-menu.png) i det övre vänstra hörnet, om det är tillgängligt, och sedan på **Begäranden** > **Skickat** > **Planering**. Klicka sedan på begäran med statusen **}Under granskning**. <!--did they change this to Pending approval; logged  a bug-->

     >[!TIP]
     >
     >    Om du inte har tillgång till Workfront Planning kan du bara godkänna en begäran med dina aviseringar.


   * Gå till området **Notifications** i skärmens övre högra hörn och klicka på meddelandet om en begäran som väntar på ditt godkännande för att öppna begäran.
   * Gå till e-postmeddelandet i ditt e-postmeddelande som meddelar dig om en begäran som väntar på ditt godkännande och klicka sedan för att öppna begäran. <!--add the name of the button here, from the email-->

   Förfrågningssidan öppnas i skrivskyddat läge.

   ![](assets/read-only-reqeust-page-in-review-status.png)
1. (Valfritt) Klicka på ikonen **Godkännanden** ![](assets/approvals-icon.png) i det övre högra hörnet av begäran för att visa godkännarna.
1. Klicka på **Granska och godkänn** och välj sedan något av följande: <!--did they fix the button and removed the &??-->

   * **Godkänn**: Detta godkänner begäran. En post skapas omedelbart för den posttyp som är associerad med begärandeformuläret.
   * **Avvisa**: Detta avvisar begäran. Ingen post skapas för den posttyp som är associerad med begärandeformuläret. <!--check to see if there is a notification sent to the requestor about it being rejected OR approved??--> <!--checking with PM what happens with the other approvers when one of them is rejecting it: does it ask them to approve it? Deleted the request? -->
