---
title: Adobe Workfront Planning Access - översikt
description: Alla användare i organisationen har inte samma åtkomst och behörigheter för att använda Adobe Workfront Planning. I den här artikeln beskrivs den åtkomst och de behörigheter som användare kan behöva för att kunna använda funktionerna i Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---


# Åtkomstöversikt för Adobe Workfront Planning

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Workfront Planning, en extrafunktion från Adobe Workfront.
>
>Ditt företag måste köpa ytterligare en licens för Workfront Planning för att få tillgång till dess funktioner.
>
>Mer information får du av din kontoansvarige
>
>Mer information om Workfront Planning finns i [Översikt över Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Det finns begränsningar för licens- och delningsbehörighet för att använda Adobe Workfront Planning.

I den här artikeln beskrivs den åtkomst och de inställningar du behöver för att kunna använda funktionerna i Workfront Planning.

## Åtkomstkrav

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Du måste ha följande åtkomst för att få åtkomst till Workfront Planning:

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
<p>Något av följande Workfront Planning-planer:</p>
<ul><li>Planering</li>
<li>Planering Plus</li>
</ul>
<p>Kontakta din kontoansvarige på Workfront om du vill ha mer information om vad som ingår i respektive Workfront Planning-plan. </p>
   </td>

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
   <ul><li><p>Standard, Light eller Contributor för att visa Workfront Planning-information</p></li>
   <li><p>Standard, för att skapa arbetsytor och vyer</p></li></ul>
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
   <li><p>Visa eller högre behörigheter för arbetsytor, posttyper och vyer som du inte har skapat för att komma åt dem och deras objekt.</p></li>
   <li><p>Contribute eller högre behörigheter för arbetsytor och posttyper som du inte skapat för att redigera dem samt skapa, redigera eller ta bort posttyper och poster.</p></li>
   <li><p>Contribute eller högre behörigheter för vyer som du inte har skapat, för att redigera, ta bort och dela dem</p>
   </li>
    <li><p>Systemadministratörer kan hantera arbetsytor som de inte skapade. </p></li>
    <li><p>Systemadministratörer kan inte komma åt vyer som de inte skapade. </p></li></ul>
   <p>Information om delningsbehörigheter för Workfront Planning-objekt finns i  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> 
<p>Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard.</p>
<p> Användare med en Light- eller Contributor-licens måste tilldelas en layoutmall som innehåller Planning-alternativet i följande områden:</p>
   <ul><li>Huvudmeny</li>
   <li>Vänster panel med projekt, portfolior och program</li>
   </ul>
   <p>Mer information finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Skapa och hantera layoutmallar</a>.</p>

</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Dela planeringsområdet med en layoutmall

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

När din organisation har köpt ytterligare en Workfront Planning-licens kan din systemadministratör lägga till Planning-alternativet i följande områden genom att ändra och tilldela dig till en layoutmall:

* Huvudmeny
* Landningssida
* Panelen Vänster för projekt, portfolior och program
* Stift

Standardanvändare och systemadministratörer har planeringsområdena aktiverade som standard i följande områden:

* Huvudmeny
* Vänster panel med projekt, portfolior eller program

Så här lägger du till eller tar bort Workfront Planning-områden från användare av din Workfront-instans:

1. Logga in på **Workfront** som Workfront-administratör.

1. Gå till **Huvudmenyn** > **Inställningar** > **Gränssnitt** > **Layoutmallar** och öppna eller skapa en layoutmall.

   Mer information om hur du anpassar en layoutmall finns i [Skapa och hantera layoutmallar](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Tilldela layoutmallen till de användare som du vill ska ha tillgång till Workfront Planning.

   Mer information finns i [Tilldela användare till en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alla användare som är tilldelade mallen kan nu komma åt Workfront Planning på huvudmenyn.

   Användare kan börja skapa arbetsytor, posttyper, poster och fält.

## Ge åtkomst

Det finns inga åtkomstkontroller för Workfront för Workfront Planning.

Användare med alla typer av Workfront-licenser har tillgång till Workfront Planning.

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Bevilja behörigheter

Du måste ge användarna behörigheter till arbetsytorna och vyerna i Workfront Planning som du skapar så att de kan komma åt dem.

Mer information finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Din Adobe Workfront-licenstyp fungerar med dina Workfront Planning-behörigheter så att du kan visa, bidra och hantera Workfront Planning-objekt.

Information om hur licenstyperna påverkar behörighetsnivåer för Workfront Planning-objekt finns i [Översikt över licenstypen när Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md) används.


