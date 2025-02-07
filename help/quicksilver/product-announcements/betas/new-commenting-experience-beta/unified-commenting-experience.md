---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Ny kommentarsfunktion
description: En uppdatering av kommentarsfunktionerna i Adobe Workfront håller på att utvecklas. Den här uppdateringen innehåller ett nytt gränssnitt, nya funktioner och förbättrade prestanda i uppdateringsavsnittet för markerade objekt.
author: Alina
feature: Product Announcements
role: User
hide: true
hidefromtoc: true
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---

# Ny kommentarsfunktion

<!--take out legacy, preview, prod references from below-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

-->

>[!IMPORTANT]
>
>Informationen i den här artikeln hänvisar till funktioner som släppts till den nya kommentarsfunktionen.
>
>Betaprogrammet för den nya kommentarsupplevelsen inleddes i april 2023 och avslutades i oktober 2023, med versionen från oktober 2023.
>
>Sedan 11 april 2024 har alla funktioner för den nya kommentarsfunktionen varit tillgängliga i produktionsmiljön för alla kunder.
>
> Tidigare kommentarer har tagits bort från Workfront.

## Funktioner

Den nya kommentarsfunktionen innehåller förbättringar och ändringar i uppdateringsavsnittet för Adobe Workfront-objekt.

Bland förbättringarna i den nya kommentarsfunktionen finns följande:

* Förbättrade prestanda och användarupplevelser
* Separation av användarkommentarer från aktivitetsuppdateringar i systemet
* Realtidsindikator när nya kommentarer läggs till i ett objekt
* Redigera kommentarer när de har skickats

Följande funktioner har tagits bort från den nya versionen:

* Kommentera en systemuppdatering. Tidigare har kommentarer som lagts till i systemuppdateringar importerats som skrivskyddade kommentarer på den nya fliken Systemaktivitet.
* Möjlighet att redigera status, villkor, datum för genomförande och Procent färdigt när du kommenterar uppgifter och ärenden.

  Vi rekommenderar att du lägger till dessa fält på panelen Sammanfattning av uppgifter och problem så att du enkelt kan komma åt dem från listor, Hem, Workfront Balancer eller en tidrapport.
* Möjlighet att redigera det anpassade formuläret
* Informationen&quot;för &lt; användarnamn >&quot; när en Workfront- eller gruppadministratör loggar in som en annan användare och lägger till en kommentar för dennes räkning togs ursprungligen bort. Den återinfördes den 19 oktober 2023.
* Alternativet Fråga efter godkännande när du taggar personer när du lägger till en kommentar i ett dokument.
* Inställningen &quot;Visa procent färdigt vid uppdateringsstatus&quot; när du redigerar en användares profilruta tas bort. Funktionen för att uppdatera procentandelen färdigt för en uppgift eller ett problem har tagits bort.


<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

Följande tabell visar vilka funktioner som kommer att vara tillgängliga i den nya kommenteringsfunktionen samt deras tillgänglighet i områden där de stöds:

<table>
  <tr>
   <td><strong>Funktion </strong>
   </td>
   <td><strong>Befintlig i gammal kommentarsfunktion </strong>
   </td>
   <td><strong>Finns i den nya kommentarsfunktionen </strong>
   </td>

<td><strong>Introducerades i den nya kommentarsfunktionen </strong>
   </td>
   </tr>
  <tr>
   <td>Skapa/läsa/svara/ta bort kommentarer 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>

<td> 
   </td>

</tr>
  <tr>
   <td>RTF (exklusive citat och känslolägesikoner)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>

<td> 
   </td>
  </tr>

<tr>
   <td>RTF (emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>

</tr>

<tr>
   <td>RTF (blockcitattecken)
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
    <td> 2 kv 2023
   </td>

</tr>
  <tr>
<tr>
   <td> Citatkommentarer
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 2 kv 2023
   </td>

</tr>
  <tr>
   <td>Reagera på kommentarer (Gilla) 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>

</tr>
  <tr>
   <td>Bifoga bilder till kommentarer 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
      <td> 
   </td>

</tr>
  <tr>
   <td>Tagga personer i kommentarer 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>

</tr>
  <tr>
   <td>Ta bort kopplade deltagare
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Tagga automatiskt alla tråddeltagare
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Kommentarer som är privata för ett företag 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Ångra publicering av en kommentar 
   </td>
   <td>✓ 
   </td>
   <td>Ersatt med redigeringskommentar 
   </td>
     <td> 
   </td>
  </tr>
  <tr>
   <td>Inaktivera systemuppdateringar 
   </td>
   <td>✓ 
   </td>
   <td>Ersätts med fliken Aktivitet 
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Redigera kommentarer 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Spara kommentarutkast när du navigerar bort från sidan 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Se nya kommentarer i realtid (inklusive när en kommentar tas bort)
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Loggtid 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Kopiera trådlänk 
   </td>
   <td>✓ 
   </td>
   <td> Ersatt med länken Kopiera
   </td>
   <td>2 kv 2023 
   </td>
  </tr>
  <tr>
   <td>Länken Kopiera kommentar 
   </td>
   <td>✓ 
   </td>
   <td> Ersatt med länken Kopiera
   </td>
   <td> 
   </td>
    </tr>
  <tr>
   <td>Citattext 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
  <td>2 kv 2023 
   </td>
   </tr>
  <tr>
   <td>Kopiera brödtext 
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td>
   </td>
   </tr>
    <tr>
   <td>Sök i kommentarer 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td>1 kv 2024 
   </td>

</tr>

<tr>
   <td>Kopiera och klistra in bilder i en kommentar
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td>1 kv 2024 
   </td>
     </tr>

<tr>
   <td>Dra och släpp bilder i en kommentar
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td>1 kv 2024 
   </td>
    </tr>

<tr>
   <td>Redigera eget formulär 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Möjlighet att redigera status, villkor, datum för genomförande när kommentarer görs 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>Svara på systemuppdateringar 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>Visa"för" när du lägger till kommentarer som är inloggade som en annan användare
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td>
   </td>
  </tr>

<tr>
   <td>Möjlighet för projektägaren att ändra schemalagt slutförandedatum för en aktivitet när implementeringsdatumet ändras från uppdateringsavsnittet
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
</table>

## Frigör tidslinje

>[!IMPORTANT]
>
>Mer information om de funktioner som släppts till den nya kommentarsfunktionen under betatestningsperioden finns i [Ny aktivitet för att frisläppa betaversionen av kommentarer](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Mer information om hur du hanterar uppdateringar för Workfront-objekt finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


I följande information beskrivs tidslinjen med viktiga milstolpar för den nya kommentarsfunktionen i produktionsmiljön. Förutom milstolparna nedan kommer vi att fortsätta att förbättra kommentarsupplevelsen med mindre förbättringar.

Mer information om funktionerna som släppts för den nya kommentarsfunktionen efter att betaperioden stängts finns i den aktuella versionsöversikten. Mer information finns i [Produktreleaser](/help/quicksilver/product-announcements/product-releases/product-releases.md).

Här följer en planerad tidslinje för den nya kommentarsfunktionen:

* Med version 23.2 (6 april 2023):
   * Kommentarsupplevelsen som Beta ger upphov till i frågor
   * Frisläppt den nya kommentarsfunktionen för mål (som den enda upplevelsen)
* Med version 23.3 (20 juli 2023):
   * Kommentarsupplevelsen i Beta för projekt, uppgifter och dokument har startats.
   * Frisläppt den nya kommentarsupplevelsen för kort i kortområdet (som den enda upplevelsen)
* Under den fjärde utgåvan av kvartal 2023 (begränsad utgåva, endast tillgänglig för kunder som väljer den snabba utgåvan):
   * Frisläppt den nya kommentarsfunktionen för mallar, malluppgifter, program, portfolior, team, användare och tidrapporter (som den enda upplevelsen)
   * Kommentarsupplevelsen i Beta för projekt, uppgifter, problem och dokument har uppdaterats så att den blir standardalternativet. &quot;Beta&quot;-etiketten har tagits bort.
* Med den fjärde utgåvan för kvartal 2023 (23.10) (26 oktober 2023)
   * Frisläppte den nya kommentarsfunktionen för mallar, malluppgifter, program, portfolior, team, användare och tidrapporter (som den enda upplevelsen) till alla kunder.
   * Gör den nya kommentarsfunktionen för projekt, uppgifter, utgåvor och dokument till standardalternativet.

  >[!IMPORTANT]
  >
  >    Detta avslutar Beta-steget i den nya kommenteringsupplevelsen.

   * Alla funktioner som lanserats för den nya kommentarsupplevelsen börjar med den här datumdelen i den aktuella vanliga månadsvisa och kvartalsvisa versionen.
* I slutet av 2023:
   * Behåll den gamla kommentarsfunktionen som ett sekundärt alternativ för följande objekt: projekt, uppgifter, utgåvor och dokument. Den nya kommentarsfunktionen är standardalternativet för alla användare för dessa objekt.
   * De nya kommentarerna är den enda upplevelsen för alla andra objekt.

* Med den andra utgåvan för kvartal 2024 (11 april 2024):

  Tog bort alternativet att växla tillbaka till den tidigare kommentarströmmen och göra den nya kommentarströmmen till den enda upplevelsen för alla objekt.

* 3 oktober 2024:

  Knappen Lämna feedback i uppdateringsområdet har tagits bort.

## Hitta den nya kommentarsfunktionen

Den nya kommentarsupplevelsen finns i följande delar av Workfront:

* I uppdateringsavsnittet för alla objekt.

  Mer information om hur du kommer åt uppdateringsavsnittet för Workfront-objekt finns i [Översikt över uppdateringsavsnittet](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

* I panelen Sammanfattning av uppgifter, problem och dokument i alla områden där detta är tillgängligt (listor, tidrapporter, belastningsutjämnare och hemsida).
* I hemområdet för uppgifter och problem.



<!--

The new commenting experience is currently available for all customers and for all environments.

Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

    * Project
    * Task (this includes Stories)
    * Issue
    * Document

      >[!NOTE]
      >
      ><span class="preview">The legacy commenting experience has been removed from the Preview environment since April 1, 2024. </span>

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

    * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations
    
    There is no option to enable the new commenting experience for iterations. Only the legacy commenting experience is available for iterations. 

-->


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

<!--

To enable the commenting experience option for projects, tasks, issues, and documents: 

1. (Conditional) In the Production environment, go to an object that you want to activate the new commenting experience for, then click **Updates** in the left panel.
1. (Conditional) If it is disabled, enable the **New commenting** option in the upper-right corner of the Updates area to enable it. This should be enabled by default. 
<span class="preview">The New commenting option has been removed from the Preview environment.</span> 

    ![New commenting toggle off](assets/new-commenting-toggle-off-highlighted.png)

1. Start typing an update in the **Comments** tab. The Comments tab is the default tab when the new experience opens

    Or

    Click the  **System Activity** tab to view the activity updates generated by Workfront. 

1. (Optional) To disable the new commenting experience and return to legacy commenting, deselect the **New commenting** option. 

-->
