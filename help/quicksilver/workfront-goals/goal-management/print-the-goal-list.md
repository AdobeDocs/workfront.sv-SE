---
product-previous: workfront-goals
navigation-topic: goal-management
title: Skriv ut mållistan i Adobe Workfront-mål
description: Du kan skriva ut en lista med mål i mållistedelen av Adobe Workfront-mål. Vid utskrift skickas en fil till skrivaren eller skapas en PDF-fil om webbläsarens utskriftsmål är inställt på Spara som PDF.
author: Alina
feature: Workfront Goals
exl-id: 66488d2f-ed35-4571-93e3-e0e025da7b33
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Skriv ut mållistan i Adobe Workfront-mål

>[!IMPORTANT]
>
>Funktionerna som beskrivs i den här artikeln har tagits bort från Workfront, med början i version 23.1.
>
>Den här artikeln kommer också att tas bort kort efter version 23.1, i början av 2023. Nu rekommenderar vi att du uppdaterar bokmärkena i enlighet med detta.

Du kan skriva ut en lista med mål i mållistedelen av Adobe Workfront-mål. Vid utskrift skickas en fil till skrivaren eller skapas en PDF-fil om webbläsarens utskriftsmål är inställt på Spara som PDF.

## Åtkomstkrav

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

Du måste ha följande åtkomst för att kunna utföra de åtgärder som beskrivs i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> <p>Mer information finns i <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för Adobe Workfront Goals för att få tillgång till de funktioner som beskrivs i den här artikeln. </p> <p>Mer information finns i <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Krav för att använda Workfront-mål</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till mål</p> <p><b>ANMÄRKNING</b><p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Bevilja åtkomst till Adobe Workfront-mål</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> 
    <div> 
     <p>Visa eller öka behörigheter för mål</p> 
     <p>Mer information om delningsmål finns i <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Dela ett mål i Workfront-mål</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Skriv ut mållistan

>[!TIP]
>
>* När du skriver ut en lista med mål innehåller filen bara den information som visas på skärmen. Objekt som tas bort genom filtrering av en lista med mål visas inte i PDF-filen.
>* När du inte expanderar målen i listan innan du skriver ut listan visar PDF-filen bara mål utan resultat och aktiviteter.
>


1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Mål** i det övre högra hörnet.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Detta öppnar området Workfront-mål.

   Mållistan visas som standard.

1. (Valfritt) Använd filter i mållistan för att visa de mål som är relevanta för dig.

   Information om filtrering av information i mållistan finns i [Filtrera information i Adobe Workfront mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Klicka **Skriv ut**. Skriv ut-rutan visas.
1. (Villkorligt) Beroende på vilken webbläsare du använder och vilka andra program du har installerat på datorn kan du välja bland följande mål:

   * Skriva ut till en skrivare
   * Skriv ut till PDF
   * Spara listan med mål på en lokal enhet eller en online-enhet (till exempel Google Drive)
   * Skicka listan med mål till ett annat program (t.ex. One Note)

1. (Valfritt) Justera utskriftsalternativen.
1. Klicka **Skriv ut**.

   Listan med mål levereras till det valda målet.
