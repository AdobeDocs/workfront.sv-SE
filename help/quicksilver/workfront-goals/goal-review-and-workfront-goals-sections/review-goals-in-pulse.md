---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Granska målen i avsnittet Adobe Workfront Goals Pulse
description: Du kan visa alla mål i organisationen, oavsett vem ägaren är. Mer information om hur du skapar mål finns i Skapa mål i Adobe Workfront-mål.
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# Granska målen i avsnittet Adobe Workfront Goals Pulse

>[!IMPORTANT]
> 
>Funktionerna som beskrivs i den här artikeln har tagits bort från Workfront, med början i version 23.1.\
>Den här artikeln kommer också att tas bort kort efter version 23.1, i början av 2023. Nu rekommenderar vi att du uppdaterar bokmärkena i enlighet med detta.


Du kan visa alla mål i organisationen, oavsett vem ägaren är. Mer information om hur du skapar mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

Du kan använda avsnittet Pulse i Adobe Workfront Goals som ett samarbetsverktyg där du kan granska och delta i en ström med uppdateringar om aktuella mål som tillhör dig, dina team, grupper eller din organisation och se till att målen hålls aktuella. Workfront Target grupperar förloppsuppdateringar, kommentarer och redigeringshistorik efter mål i avsnittet Pulse.

## Åtkomstkrav

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
   <td> <p>Visa eller öka åtkomsten till mål</p> <p>Obs!  <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra din åtkomstnivå finns i:</p> 
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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande innan du kan börja:

* En layoutmall som innehåller området Mål på huvudmenyn.

## Hantera måluppdateringar och kommentarer i avsnittet Pulse 

>[!TIP]
>
>Endast mål som har checkats in minst en gång visas i avsnittet Pulse.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Mål** i skärmens övre högra hörn.

   Detta öppnar området Workfront-mål.

   Alla mål visas som standard.

1. Klicka **Puls** i den vänstra panelen.

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   En lista med mål visas. Listan innehåller följande kolumner med information om varje mål:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Mål</td> 
         <td>Målnamnet.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Ägare</td> 
         <td>Målägarens namn.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Period</td> 
         <td>Den tidsperiod för vilken målet har schemalagts.</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Förlopp</td> 
         <td>Förloppsindikatorn för målet, som vanligtvis är ett procentvärde.</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>Status (inkluderar justeringsikon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>Status för målet som kan vara något av följande:</p> 
         <ul> 
         <li>Aktiv</li> 
         <li>Utkast</li> 
         <li>Inaktiv</li> 
         <li>Stängd</li> 
         </ul> <p>Justeringsikonen visas för mål som är justerade mot andra mål. Mer information om hur du justerar mål finns i <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Justera mål genom att koppla dem till Adobe Workfront mål</a>.</p>

   <p>Statuskolumnen innehåller även inkrementella uppdateringar som gjorts för varje resultat eller aktivitet med varje incheckning av målet.</p>

   Om målet t.ex. har en manuell förloppsindikator och du checkar in målet och uppdaterar aktiviteten till 50 %, visas statuskolumnen 50 % för det målets aktivitet. Senare kan du uppdatera samma aktivitet till 60 %. I det här fallet visas en ny rad under samma mål för samma aktivitet för 10 % - eftersom du precis har lagt till 10 % till aktivitetens förlopp.
   </td>
   </tr> 
      </tbody> 
      </table>

1. (Valfritt) Välj den typ av information som du vill visa genom att uppdatera filtren i det övre högra hörnet av avsnittet Pulse.

   Pulslistan visar mål och deras uppdaterade historik som matchar villkoren för det valda filtret.

   Mer information om filtreringsmål finns i [Filtrera information i Adobe Workfront mål](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Klicka på högerpilen till vänster om målnamnet för att expandera ett mål och visa ytterligare information om uppdateringarna för varje mål.

   Följande information visas i avsnittet Pulse under varje mål:

   * Resultatnamn och ägare. Information om resultaten finns i [Lägg till resultat i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * Aktivitetsnamn och ägare. Mer information om aktiviteter finns i [Lägga till aktiviteter i mål i Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * Resultat och aktiviteter förloppsindikatorer och förloppsstatus. Mer information om hur Workfront-mål beräknar målförloppet finns i [Översikt över målets förlopp och villkor i Adobe Workfront-mål](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. Klicka **Lägga till en kommentar** för att lägga till en kommentar för målet, och sedan klicka **Bokför**. Kommentaren visas i incheckningsområdet samt på fliken Uppdateringar på panelen Målinformation. Vi rekommenderar att du använder Pulse-avsnittet för att kommentera mål som inte har uppdaterats på ett tag och frågar målägaren om en uppdatering.

1. (Valfritt) Klicka på **Visa alla uppdateringar** för att visa alla måluppdateringar. Då öppnas fliken Uppdateringar på panelen Målinformation till höger.
1. Klicka på namnet på ett mål för att öppna **Målinformation** till höger och granska mer information om målet samt hantera det och dess resultat och aktiviteter. Mer information om hur du granskar enskilda mål finns i [Uppdatera mål i avsnittet Målinformation i Adobe Workfront-mål](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Valfritt och villkorligt) Klicka på **justeringsikonen** ![](assets/align-icon.png) för att öppna målet i avsnittet Måljustering, om målet är justerat efter andra mål.

1. (Valfritt) Expandera **Mål per sida** och välj bland följande alternativ för att visa ytterligare mål:

   * 20. Det här är standardvalet.
   * 50
   * 100


