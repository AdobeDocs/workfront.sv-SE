---
content-type: overview
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Översikt över måljustering i Adobe Workfront-mål
description: Målanpassningen säkerställer att alla i organisationen är på samma sida om vad som måste uppnås genom att anpassa sina mål till varandra och till de organisatoriska målen för team, grupper och företaget.
author: Alina
feature: Workfront Goals
exl-id: e073cf10-2333-4095-b932-73d105f0c5a4
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Översikt över måljustering i Adobe Workfront-mål

>[!NOTE]
>
>Din organisation måste ha följande för att kunna använda de funktioner som beskrivs i den här artikeln:
>* En Pro eller högre [Adobe Workfront](https://www.workfront.com/plans).
>* En Adobe Workfront Goals-licens förutom en Workfront-licens. Kontakta er kontoansvarige på Workfront för att få veta mer om en Workfront Goals-licens.
>
>Mer information om åtkomst till Workfront-mål finns på [Krav för att använda Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

Målanpassning är en viktig del av målhanteringen. Ni kan se till att alla i organisationen är på samma sida om vad som måste göras för att driva strategin framåt genom att anpassa deras mål till varandra och till de organisatoriska målen för team, grupper och företaget.

Efter att de högsta målen för företag, team eller grupper har fastställts och granskats måste direktrapporter och teammedlemmar sedan skapa mer fokuserade mål som överlappar den högsta nivån. Omfattningen av dessa mål bör vara mer smal och ta hänsyn till den person som har utsetts till ansvarig för målet och deras omfattning. Målet bör svara på frågan om vad de och deras team måste uppnå för att uppnå det överordnade mål som det är anpassat till.

Mer information om god praxis när du justerar mål finns i [Kom igång med Adobe Workfront-mål](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Överväganden för att justera mål

* Ett mål kan inte bidra till mer än ett annat mål samtidigt. Även om du kan ha flera underordnade mål justerade mot samma överordnade mål, kan ett underordnat mål bara ha en överordnad. Mer information om mål för överordnade och underordnade finns i [Förstå mål för överordnade och underordnade](#understand-parent-and-children-goals) i den här artikeln.
* Ett mål kan ha flera justerade (eller underordnade) mål samt flera aktiviteter och resultat. Dessutom kan varje underordnat mål ha andra aktiviteter och resultat som påverkar dess förlopp samt förloppet för det överordnade målet.

   >[!TIP]
   >
   >Vi rekommenderar att du håller den här strukturen så enkel som möjligt.

* Du bör uppdatera olika typer av mål beroende på din roll. Exempel:

   * Som enskild deltagare rekommenderar vi att ni bidrar till era egna mål som bör anpassas efter mål på team-, grupp- och företagsnivå. När du uppdaterar dina egna mål bör du uppdatera utvecklingen för alla andra överordnade mål.
   * Som koncernchef eller affärschef rekommenderar vi att du bidrar till dina mål samt uppdaterar de som tilldelats team, grupper och företaget.

## Måljusteringstyper

Det finns två sätt att anpassa mål:

* **En justering längst ned upp**: Du kan koppla ett underordnat mål direkt till ett överordnat mål. Mer information om justering nedifrån och upp-mål finns i [Justera mål genom att koppla dem till Adobe Workfront mål](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* **En justering uppifrån och ned**: Du kan konvertera ett resultat eller en aktivitet för ett mål till ett annat mål. Det nya målet blir det underordnade målet för det ursprungliga målet som blir överordnat. Mer information om justering uppifrån och ned finns i [Justera mål genom att konvertera resultat och aktiviteter till mål](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

Mer information om mål för överordnade och underordnade finns i [Förstå mål för överordnade och underordnade](#understand-parent-and-children-goals) i den här artikeln.

## Förstå mål för överordnade och underordnade {#understand-parent-and-children-goals}

När du justerar mål mot varandra blir ett mål det överordnade målet och det andra det underordnade målet. Förloppet för underordnade mål påverkar förloppet för de överordnade målen. Detta skapar en målhierarki.

Tänk på följande när du arbetar med underordnade och överordnade mål:

* Du kan justera flera mål för underordnade till samma överordnade mål.
* Ett underordnat mål kan bara ha ett överordnat mål.
* Förloppet för de mål som anges av deras resultat och aktiviteter påverkar förloppet för det överordnade målet. Andra aktiviteter eller resultat som är kopplade till det överordnade målet påverkar också förloppet för det överordnade målet.
* Du kan inte uppdatera förloppet för ett underordnat mål på det överordnade målets nivå. Du måste uppdatera det underordnade målets aktiviteter och resultat, och detta uppdaterar automatiskt förloppet för det underordnade målet samt för det överordnade målet.

   Information om hur du uppdaterar förloppet för mål finns i [Uppdatera målstatus i Adobe Workfront-mål](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Hitta justerade mål

Efter att ha justerat målen ingår de i samma hierarki och är synliga inom olika områden av Workfront mål.

<!--
* In the Production enviroment, you can view children and parent goals in the following areas:

    * The Goal Details panel
    * Goal List
    * Goal Alignment section
    * Check-in section
    * Pulse section
    * You can view all the parent goals of a goal in the Goal Hierarchy field of a Project or Goal report.
-->
Du kan visa underordnade och överordnade mål inom följande områden:

* Avsnittet Förloppsindikatorer på en målsida, under gruppen Typ:Mål.
* Måljusteringsdelen på sidan Mål.




