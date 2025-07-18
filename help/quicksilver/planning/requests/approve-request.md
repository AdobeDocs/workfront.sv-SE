---
title: Godkänn en begäran i Adobe Workfront Planning
description: När en användare skickar en begäran till ett begärandeformulär som är kopplat till ett godkännande i Adobe Workfront Planning får godkännarna ett meddelande och ett e-postmeddelande om det väntande godkännandet. De måste godkänna begäran innan Workfront Planning skapar ett objekt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Godkänn en begäran i Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

När en användare skickar en begäran till ett begärandeformulär som är kopplat till ett godkännande i Adobe Workfront Planning får godkännarna ett meddelande och ett e-postmeddelande om det väntande godkännandet. De måste godkänna begäran innan Workfront Planning skapar ett objekt.

I den här artikeln beskrivs hur en arbetsytehanterare kan godkänna en begäran om att skapa en post i Workfront Planning.

Vi rekommenderar att du också ser följande artiklar:

* [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md)
* [Lägga till ett godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Att tänka på när det gäller att godkänna begäranden

* Skickade begäranden visas på fliken Planering i avsnittet Skickat i området Begäranden i Workfront med en av följande begärandestatusar:

   * **Väntande granskning**: Den här statusen visas när ingen av godkännarna har öppnat begäranobjektet.
   * **Under granskning**: Statusen **Väntande granskning** ändras till **Under granskning** när minst en godkännare öppnar begäranobjektet. Status för begäran förblir **Under granskning** tills alla godkännare har godkänt begäran.
   * **Godkänd**: När en godkännare godkänner begäranobjektet blir deras individuella status **Godkänd**, men den övergripande statusen för begäranobjektet förblir **Under granskning** tills alla godkännare har fattat sina beslut. När alla godkännare godkänner en begäran blir förfrågansstatusen **Godkänd**.
   * **Slutförd**: Om alla godkännare godkänner begäranobjektet ändras dess status till **Slutförd** eller om begäran inte behövde något godkännande.
   * **Avvisad**: Om någon godkännare avvisar begärandeobjektet blir statusen **Avvisad**. Ingen post skapas och en ny begäran måste skickas för att posten ska kunna skapas.

* <span class="preview">Du kan visa godkännandeinformation för en post som skapats genom att skicka ett begärandeformulär i fälten Godkänd av och Godkänd. Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).</span>

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
   <li><p>Hantera behörigheter till en arbetsyta och en posttyp </p></li>
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


## Godkänn en begäran om att skapa en post

När användare har lagt till begäranden i ett formulär för posttypbegäran som är kopplat till ett godkännande, skickas begäran till godkännarna.

Godkännare får följande meddelanden om en begäran som väntar på deras godkännande:

* Ett meddelande i appen
* Ett e-postmeddelande

>[!NOTE]
>
>Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att användare ska kunna ta emot e-post och meddelanden i appen.

Så här godkänner du en begäran:

1. Gör något av följande:

   * Om du har tillgång till Workfront Planning och kan visa minst en arbetsyta klickar du på **Huvudmeny** ![Huvudmeny för punkter](assets/dots-menu.png) i skärmens övre högra hörn, eller på **Huvudmeny** ![Huvudmenyn för rader](assets/lines-menu.png) i det övre vänstra hörnet, om det är tillgängligt, och klickar sedan på **Förfrågningar** > **Skickade** > **Planera** och klicka på begäran med statusen **Väntande granskning** eller **Under granskning** .

     >[!TIP]
     >
     >Om du inte har tillgång till Workfront Planning, eller om du inte har åtkomst till att visa några arbetsytor, kan du bara få åtkomst till en begäran om att godkänna den via e-post eller meddelanden i appen.

   * Klicka på ikonen för området **Meddelanden** ![Meddelanden i det enhetliga gränssnittet](assets/notifications-area-icon-unified-shell.png) i skärmens övre högra hörn och klicka på meddelandet om en begäran som väntar på ditt godkännande för att öppna begäran.
   * Gå till e-postmeddelandet i ditt e-postmeddelande som meddelar dig om en begäran som väntar på ditt godkännande och klicka sedan på **Öppna begäran** för att öppna begäran. <!--add the name of the button here, from the email-->

   Förfrågningssidan öppnas i skrivskyddat läge.

   ![Skrivskyddad begärandesida med granskningsstatus](assets/read-only-reqeust-page-in-review-status.png)

1. (Valfritt) Klicka på ikonen **Godkännanden** ![Godkännanden](assets/approvals-icon.png) i det övre högra hörnet av begäran för att visa godkännarna.
1. Klicka på **Granska och godkänn** och välj sedan något av följande:

   * **Godkänn**: Detta godkänner begäran. En post skapas omedelbart för den posttyp som är associerad med begärandeformuläret efter att alla godkännare har godkänt begäran.
   * **Avvisa**: Detta avvisar begäran, även om du är den enda godkännaren som avvisar den. Ingen post skapas för den posttyp som är associerad med begärandeformuläret.

   Användaren som skickade begäran får ett e-postmeddelande och i ett program-meddelanden när deras begäran har godkänts eller avvisats.

   Status för begäran ändras till följande, beroende på beslutet om godkännande:

   * **Slutförd**: Begäran har godkänts.
   * **Avvisad**: Begäran nekades.

   Begäran finns kvar på fliken Planering i avsnittet Skickat i området Begäranden i Workfront.
