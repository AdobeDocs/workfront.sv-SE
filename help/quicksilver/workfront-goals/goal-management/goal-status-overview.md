---
content-type: overview;reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Översikt över målstatus i Adobe Workfront-mål
description: Målstatus anger om ett mål är aktivt och om det håller på att spelas in, eller om det är inaktivt, utformat eller redan har uppnåtts.
author: Alina
feature: Workfront Goals
exl-id: dc70dfac-2bdd-41ab-b316-0cd20f749423
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Översikt över målstatus i Adobe Workfront-mål

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

>[!NOTE]
>
>Din organisation måste ha följande för att kunna använda de funktioner som beskrivs i den här artikeln:
>
>* En Pro eller högre [Adobe Workfront](https://www.workfront.com/plans).
>* En Adobe Workfront Goals-licens förutom en Workfront-licens.
>
>Kontakta er kontoansvarige på Workfront för att få veta mer om en Workfront Goals-licens.

Mer information om åtkomst till Workfront-mål finns på [Krav för att använda Workfront-mål](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


Målstatus anger om ett mål är aktivt och om det håller på att spelas in, eller om det är inaktivt, utformat eller redan har uppnåtts.

## Tänk på detta när du uppdaterar målstatusvärden i Workfront-mål

* Du kan inte uppdatera statusen för mål som du har skapat eller som delats med dig manuellt. Status för mål uppdateras beroende på vilka åtgärder du vidtar för målet. Om du till exempel aktiverar ett mål ändras statusen Utkast till Aktiv.
* Det finns vissa begränsningar och ibland kan du inte ändra status för ett mål till en annan status enligt följande regler:

   | Från/till | Utkast | Aktiv | Inaktiv | Stängd |
   |---|---|---|---|---|
   | Utkast | - | Ja | Nej | Nej |
   | Aktiv | Nej | - | Ja | Ja |
   | Inaktiv | Nej | Ja | - | Nej |
   | Stängd | Nej | Ja | Nej | - |

* Om du öppnar ett stängt mål uppdateras även målets förlopp.
* Vissa åtgärder som du utför på ett mål uppdaterar också dess status. Mer information om hur du kan uppdatera målstatus finns i följande artiklar:

   * [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md)
   * [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md)
   * [Ta bort och inaktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/delete-and-deactivate-goals.md)
   * [Stäng och öppna mål igen i Adobe Workfront-mål](../../workfront-goals/goal-management/close-and-reopen-goals.md)

## Översikt över målstatus i Workfront-mål

Mer information om hur du skapar mål för Workfront finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).

Mer information om hur du aktiverar mål finns i [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md).

Mål kan ha någon av följande statusar i Workfront-mål:

* [Utkast](#draft)
* [Aktiv](#active)
* [Inaktiv](#inactive)
* [Stängd](#closed)

### Utkast {#draft}

* Detta är standardstatus för ett nyligen skapat mål. Mer information om hur du skapar mål finns i [Skapa mål i Adobe Workfront-mål](../../workfront-goals/goal-management/create-goals.md).
* Workfront-mål registrerar inte framsteg i ett utkast.
* Du kan inte uppdatera förloppet för ett utkast.
* Du kan inte stänga eller inaktivera utkast eftersom de saknar förloppsinformation.
* Ritade mål bidrar inte till förloppsberäkningen av andra mål och beaktas inte i diagram.
* Ritade mål visas inom följande områden av Workfront-mål:

   * Mållista
   * Måljusteringssektion (endast som justerat mål)


>[!IMPORTANT]
>
>När du har ändrat status för ett mål till någon annan status kan målet aldrig placeras i utkaststatus igen.

### Aktiv {#active}

* Du kan bara aktivera ett utkast när du associerar det med ett resultat, en aktivitet eller justerar ett annat mål mot det. När du aktiverar målet ändras dess status till Aktiv. Mer information om hur du aktiverar mål finns i [Aktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/activate-goals.md).
* Workfront Goals registrerar framsteg i de aktiva målen.
* Aktiva mål bidrar till förloppsberäkningen av andra mål, och de beaktas i diagram.
* Aktiva mål visas inom följande områden av Workfront mål:

   * Mållista
   * Måljusteringsavsnitt
   * Förloppet för aktiva mål visas i diagram

* Du kan återaktivera ett stängt eller inaktivt mål.

### Inaktiv {#inactive}

* Du kan inaktivera ett aktivt mål när ägaren har slutat arbeta med det tillfälligt eller permanent. Du kan behålla den för historik. Detta uppdaterar målets status till Inaktiv.

   Mer information om hur du inaktiverar mål finns i avsnittet Inaktivera mål i artikeln [Ta bort och inaktivera mål i Adobe Workfront-mål](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

* Du kan inte inaktivera ett utkast eller ett stängt mål.
* Du kan återaktivera ett inaktivt mål och fortsätta arbeta med det.
* Workfront-mål räknar inte ut förloppet för inaktiva mål.
* Du kan inte uppdatera förloppet för ett inaktivt mål.
* Inaktiva mål bidrar inte till förloppsberäkningen av andra mål och beaktas inte i diagram.
* Inaktiva mål har en förloppshistorik eftersom de tidigare var aktiva, till skillnad från utkast.
* Inaktiva mål visas inom följande områden av Workfront-mål:

   * Mållista
   * Måljusteringssektion (endast som justerade mål)

### Stängd {#closed}

* Du kan stänga ett mål när du vill ange att du har uppnått det eller att du inte längre arbetar med det, och inte heller kommer du att göra det i framtiden. Mer information om att stänga mål finns i [Stäng och öppna mål igen i Adobe Workfront-mål](../../workfront-goals/goal-management/close-and-reopen-goals.md).

   >[!TIP]
   >
   >Om du planerar att arbeta med ett mål som ännu inte har uppnåtts, rekommenderar vi att du ändrar statusen till Inaktiv i stället för Stängd.

* Man kan inte stänga mål som aldrig har aktiverats, som skräddarsydda mål.
* Du kan öppna ett stängt mål igen och fortsätta arbeta med det.
* Workfront Goals stoppar inspelningen av förloppet vid stängda mål.
* Du kan inte uppdatera förloppet för ett stängt mål.
* Stängda mål visas inom följande områden av Workfront mål:

   * Mållista
   * Måljusteringssektion (endast som justerade mål)
   * Information från stängda mål tas också med i diagramavsnittet.
