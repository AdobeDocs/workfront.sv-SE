---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Prioritera projekt i resursplaneraren
description: Projekt listas i prioritetsordning i resursplaneraren med det viktigaste projektet överst.
author: Lisa
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 0%

---

# Prioritera projekt i resursplaneraren

Projekt listas i prioritetsordning i resursplaneraren med det viktigaste projektet överst.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till resurshantering som inkluderar åtkomst till Redigera prioriteringar och budgettimmar i Resursplanering</p> <p>Redigera åtkomst till finansiella data, projekt och användare</p></td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för de projekt som du vill budgetera information för med möjlighet att hantera finanser</p></td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standardordning för projekt i resursplaneraren

Som standard listas projekten i projektvyn i resursplaneraren med hänsyn till villkoren nedan.

>[!IMPORTANT]
>
>Projekt listas endast enligt de tre villkoren nedan första gången du öppnar resursplaneraren. Den här standardprioriteten blir automatiskt din anpassade prioritet och kan inte återställas till den ursprungliga prioriteten någon gång du gör något av följande:
>
>* När du klickar på Spara när du vill.
>* När du ändrar projektplaneringsprioriteten manuellt. Mer information om hur du ändrar projektplaneringsprioriteten manuellt finns i avsnittet [Ändra projektplaneringsprioriteten manuellt](#manually-change-the-project-planning-priority) i den här artikeln.
>
>När projektprioriteten har blivit din egen prioritet påverkar inte längre ändringar i projektinformationen ordningen för de projekt som använder dessa kriterier. Därefter kan du bara prioritera projekt manuellt.

De ursprungliga standardvillkoren för att lista projekten i projektvyn är följande, i den här ordningen:

1. Efter justeringspoäng i projektet.\
   Mer information om projektets justeringsresultat finns i [Använda ett styrkort i ett projekt och generera ett justeringsresultat](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. Med projektets planerade startdatum (om justeringsfältet är null eller samma för flera projekt).
1. I bokstavsordning (om fältet Justering är null eller lika med och det planerade startdatumet är samma för flera projekt).

Tänk på följande när du arbetar med projektprioriteringar i resursplaneraren:

* Du kan bara anpassa projektprioriteten manuellt när du använder projektvyn. Detta ändrar även ordningen på projekten i resursplaneraren.
* När du använder roller eller användarvyer i resursplaneraren visas projekten i samma prioritetsordning som i projektvyn.
* Ordningen på projekten i resursplaneraren är unik för dig. Andra användare kan visa samma projekt i Resursplanering, men i en annan ordning. Du kan inte rapportera i fältet Projektplaneringsprioritet. Detta visas bara i resursplaneraren och fungerar som en flagga för att prioritera dina projekt.

Projekt som är kopplade till en portfölj kan ha en prioritet på portföljnivå. Du kan aktivera visning av ett projekts portföljprioritet i resursplaneraren, förutom resursplaneringsprioriteten. Du kan också beställa projekten efter deras portföljprioritet.

## Ändra projektplaneringsprioriteten manuellt {#manually-change-the-project-planning-priority}

Du måste ha behörigheten Redigera för resurshantering och Hantera för att kunna ordna om projekt i resursplaneraren.

Genom att ge projekten en ny prioritet kan du rangordna dem efter prioritet.

Så här redigerar du projektplaneringsprioriteten:

1. Gå till **Resursplaneraren**.

1. Klicka i fältet till vänster om det projektnamn som innehåller ett nummer, ange ett nummer för att ändra planeringsprioritet och tryck sedan på Retur.\
   ![Ändra planeringsprioritet](assets/mceclip4.png)\
   eller\
   Håll markören över namnet på projektet och klicka på indikatorn till vänster om projektnamnet. Dra den och släpp den på rätt plats för att ändra prioriteten.

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   När du väljer nummer att prioritera projekt väljer du lägre nummer för högre (viktigare) prioriteringar och högre nummer för lägre (mindre viktiga) prioriteringar. När du ändrar prioritetsnumret för ett projekt till ett lägre antal (högre prioritet), flyttas alla andra projekt i resursplaneraren nedåt i listan (blir mindre viktiga).\
   När du ändrar prioritetsnumret för ett projekt till ett högre antal (lägre prioritet), flyttas alla andra projekt i resursplaneraren upp i listan (blir viktigare).

1. Klicka på **Spara**.\
   Ordningen på projekten ändras enligt dina val och detta blir din anpassade projektprioritet i resursplaneraren. Andra användare kan inte se din prioritetsordning för projekten i resursplaneraren, även om de kanske kan visa samma projekt i sina resursplanerare.

## Ordna projekt enligt deras Portfolio-prioritet i resursplaneraren

>[!IMPORTANT]
>
>Företaget måste ha en Business-plan eller en senare Workfront-plan för att kunna prioritera projekt i Portfolio Optimizer.
>
>Mer information om Workfront-planer finns i [Våra planer](https://business.adobe.com/products/workfront/pricing.html).
>
>Mer information om hur du prioriterar projekt i Portfolio Optimizer finns i [Prioritera projekt i Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Öppna **Resursplaneraren** i **projektvyn**.
1. Klicka på ikonen **Inställningar** .
1. Aktivera inställningen **Visa Portfolio-prioriteringar** för att visa projektprioriteter enligt den Portfolio som de är tilldelade till. Projektens prioritet enligt portföljerna visas bredvid resursplaneringsprioriteten. Den här inställningen är inaktiverad som standard.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![Portfolio prioritet](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Projektens portföljprioriteringar visas endast i projektvyn i resursplaneraren.

1. Klicka på **Beställ** om du vill beställa projekten enligt portföljens prioriteringar.

   Om du har projekt som tillhör mer än en portfölj kan du se flera projekt med samma portföljprioritet i resursplaneraren. I det här fallet listas projekt med samma portföljprioritet enligt följande kriterier, i den här ordningen:

   1. Justeringspoäng
   1. Planerat startdatum
   1. Projektnamn

   ![Portfolio-prioritet beställd](assets/rp-portfolio-priority-ordered-350x198.png)

1. Klicka på **Spara**.

## Effekten av ändring av projektplaneringsprioriteten på tillgängliga användartimmar

Projektplaneringsprioriteten påverkar användarnas tillgängliga timmar. De användare som är associerade med projektet med den högsta prioriteten visar sin fulla tillgänglighet för kolumnen Tillgängliga timmar (AVL) för det här projektet, enligt sina scheman.

Samma användare som är associerade med det andra projektet i prioritetsordning kommer att visa värdet Tillgängliga timmar, vilket är skillnaden mellan deras totala antal tillgängliga timmar och det som redan har budgeterats för det första projektet i kolumnen Budgeterade timmar osv. Mer information om budgeteringsresurser i resursplaneraren finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Om inga timmar har budgeterats för det första projektet (i prioritetsordning) för en användare, men timmar har budgeterats för det andra projektet för samma användare, visar användaren hela antalet tillgängliga timmar för båda projekten.

Vi rekommenderar att du uppdaterar kolumnen Budgeterade timmar för dina användare i den ordning som de har i projekten i resursplaneraren, så att du alltid kan se tillgängliga timmar för användaren.

>[!NOTE]
>
>Eftersom prioriteten för projektplanering är unik för alla resurshanterare, kan ditt andra prioritetsprojekt vara ett förstahandsprojekt för en annan användare som visar samma projekt i sin resursplanerare. Om en annan resurshanterare budgeterar en resurs för sitt första projekt, kommer antalet tillgängliga timmar att minska för den resursen för ditt första projekt baserat på den ändringen.
>
>Användaren som budgeterar timmarna allokerar den resursen först och minskar antalet tillgängliga timmar för resursen i hela systemet. Antalet tillgängliga timmar ska uppdateras för alla användare så snart de budgeterade timmarna har sparats för en resurs i resursplaneraren.
>
>Mer information om tillgängliga timmar finns i [Tillgänglighet och tilldelning av resurser](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
