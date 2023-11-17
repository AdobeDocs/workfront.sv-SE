---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Ny kommentarsfunktion
description: En uppdatering av kommentarsfunktionerna i Adobe Workfront håller på att utvecklas. Den här uppdateringen innehåller ett nytt gränssnitt, nya funktioner och förbättrade prestanda i uppdateringsavsnittet för markerade objekt.
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 937498a68a994d19b0005d518d7e313c48961672
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Ny kommentarsfunktion


<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder.  </span>

<span class="preview">Information om det aktuella releaseschemat finns i [Första utgåvan, kvartal 2024, översikt](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>Informationen i den här artikeln avser funktioner som har släppts till den nya kommentarsfunktionen.
>
>Betaprogrammet för de nya kommentarerna inleddes i april 2023 och avslutades i oktober 2023. Betaprogrammet för den nya kommentarsupplevelsen avslutades i oktober 2023-versionen.
>
>Funktionerna som beskrivs i den här artikeln lanserades för alla kunder i oktober 2023, om inget annat anges.

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## Funktioner

Den nya kommentarsfunktionen innehåller förbättringar och ändringar i uppdateringsavsnittet för Adobe Workfront-objekt.

Bland förbättringarna i den nya kommentarsfunktionen finns följande:

* Förbättrade prestanda och användarupplevelser
* Separation av användarkommentarer från aktivitetsuppdateringar i systemet
* Realtidsindikator när nya kommentarer läggs till i ett objekt
* Redigera kommentarer när de har skickats

Följande funktioner har tagits bort från den nya versionen:

* Kommentera en systemuppdatering
* Möjlighet att redigera status, villkor, bekräfta datum samtidigt som kommentarer görs
* Redigera eget formulär
* Informationen&quot;för &lt; användarnamn >&quot; när en Workfront- eller gruppadministratör loggar in som en annan användare och lägger till en kommentar för dennes räkning togs ursprungligen bort. Den återinfördes den 19 oktober 2023.
* Alternativet Fråga efter godkännande när du taggar personer när du lägger till en kommentar i ett dokument.

>[!NOTE]
>
>Objekten som anges nedan har endast de kommentarer och systemuppdateringar som börjar den 1 januari 2019 tillgängliga i den nya kommentarsupplevelsen.
>
>Du kan visa kommentarer och systemuppdateringar för dessa objekt före 1 januari 2019 när du visar uppdateringsavsnittet i den aktuella upplevelsen:
>
>* Problem
>* Projekt
>* Uppgifter
>* Dokument

Mer information finns i [Nya vanliga frågor och svar om kommenteringsupplevelser](../../betas/new-commenting-experience-beta/new-commenting-faq.md).

Följande tabell visar vilka funktioner som kommer att vara tillgängliga i den nya kommenteringsfunktionen samt deras tillgänglighet i områden där de stöds:

<table>
  <tr>
   <td><strong>Funktion </strong>
   </td>
   <td><strong>Gammal kommentarsfunktion </strong>
   </td>
   <td><strong>Finns i den nya kommentarsupplevelsen </strong>
   </td>
   <td><strong>Kommer att introduceras i den nya kommentarsfunktionen </strong>
   </td>
   <td><strong>När kommer att introduceras i den nya kommentarsfunktionen </strong>
   </td>
   <td><strong>Forskning </strong>
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
   </td>
   <td> 2 kv 2023
   </td>
   <td> 
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
   <td> 
   </td>
   <td> 2 kv 2023
   </td>
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
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
   <td> 
   </td>
   <td>2 kv 2023 
   </td>
   <td> 
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
   <td> 
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
   <td> 
   </td>
   <td>2 kv 2023 
   </td>
   <td> 
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
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Sök i kommentarer 
   </td>
   <td> 
   </td>
   <td> <span class="preview">✓</span>
   </td>
   <td> 
   </td>
   <td>1 kv 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Kopiera och klistra in bilder i en kommentar
   </td>
   <td> 
   </td>
   <td> <span class="preview">✓</span>
   </td>
   <td> 
   </td>
   <td>1 kv 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Dra och släpp bilder i en kommentar
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>1 kv 2024 
   </td>
   <td>✓ 
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
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Möjlighet att redigera status, villkor, bekräfta datum samtidigt som kommentarer görs 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
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
   <td>
   </td>
   <td> 
   </td>
  </tr>
</table>

## Frigör tidslinje

Information om de funktioner som nyligen släppts till den nya kommentarsfunktionen, samt en tidslinje för en release, finns på [Ny aktivitet för att kommentera betaversionen](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).

Mer information om hur du hanterar uppdateringar för Workfront-objekt finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Hitta den nya kommentarsfunktionen

&lt;!—VIKTIGT! När vi gör oss av med den gamla upplevelsen flyttar du en version av den till artikeln Update work eller översikten Update section - för att säga att upplevelsen är annorlunda för alla förutom för iterationer—>

Den nya kommentarsupplevelsen är för närvarande tillgänglig för alla kunder och för alla miljöer.

Beroende på vilka objekt du har tillgång till kommentarfunktionerna för kan du se följande funktionalitet för uppdateringsavsnittet:

* Både den nya och gamla kommentarsfunktionen för följande objekt:

   * Projekt
   * Uppgift (här ingår artiklar)
   * Problem
   * Dokument

  >[!TIP]
  >
  >Använd alternativet Ny kommentering för att visa den nya kommentarsfunktionen (när du aktiverar den) eller den äldre kommentarsfunktionen (när du inaktiverar den), som beskrivs i det här avsnittet. Den nya kommentarsfunktionen är standard.

   * Bara den nya kommentarsfunktionen för objekten som listas nedan. Det finns inget alternativ för att aktivera den gamla kommentarfunktionen för dessa objekt:

      * Mål

     >[!NOTE]
     >
     >Du måste ha ytterligare en licens för Adobe Workfront Goals för att få tillgång till det här området av Workfront. Mer information finns i [Krav för att använda Workfront-mål](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
      * Kort ombord
      * Team
      * Mall
      * Malluppgift
      * Tidrapport
      * Program
      * Portfolio
      * Användare

* Endast den äldre kommentarsfunktionen för följande objekt:

   * Iterationer

     Det finns inget alternativ för att aktivera den nya kommentarfunktionen för iterationer. Det är bara den gamla kommentarsfunktionen som är tillgänglig för iterationer.


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

Så här aktiverar du alternativet för kommenteringsfunktion för projekt, uppgifter, utgåvor och dokument:

1. Gå till ett objekt som du vill aktivera den nya kommentarsfunktionen för och klicka sedan på **Uppdateringar** till vänster.
1. (Villkorligt) Om det är inaktiverat aktiverar du **Nya kommentarer** i det övre högra hörnet av uppdateringsområdet för att aktivera det. Detta bör vara aktiverat som standard.

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. Börja skriva en uppdatering i **Kommentar** -fliken. Fliken Kommentarer är standardfliken när den nya funktionen öppnas

   eller

   Klicka på  **Systemaktivitet** för att visa aktivitetsuppdateringar som genererats av Workfront.

1. (Valfritt) Om du vill inaktivera den nya kommentarsfunktionen och återgå till tidigare kommentarer avmarkerar du **Nya kommentarer** alternativ.

