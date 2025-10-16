---
product-area: resource-management
navigation-topic: resource-planning
title: Leta reda på resursplaneraren
description: Du kan använda Resursplanering för att hantera tilldelningen av resurser till projekt. Du kan komma åt resursplaneraren för flera projekt samtidigt eller för ett projekt från projektets ärendeområde.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Leta reda på resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Du kan använda Resursplanering för att hantera tilldelningen av resurser till projekt. Du kan komma åt resursplaneraren för flera projekt samtidigt eller för ett projekt från projektets ärendeområde.

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
   <td><p>Ljus eller högre för ett projekt; Standard för flera projekt</p>
       <p>Granska eller högre för ett projekt, Planera för flera projekt</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till resurshantering</p> </td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för projekt och användare </p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Kontrollera att alla krav för åtkomst och arbete med resursplaneraren är uppfyllda innan du börjar använda den. På så sätt ser du till att rätt information visas i resursplaneraren innan du börjar budgetera dina resurser.

Mer information om krav för resursplanering finns i [Kom igång med resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Leta reda på resursplaneraren

Du kan hitta resursplaneraren i två områden i Workfront, beroende på om du vill budgetera dina resurser för flera projekt eller bara för ett projekt.

* [Använd resursplaneraren för flera projekt](#use-the-resource-planner-for-multiple-projects)
* [Använd resursplaneraren för ett projekt](#use-the-resource-planner-for-one-project)

### Använd resursplanering för flera projekt {#use-the-resource-planner-for-multiple-projects}

När du använder Resursplanering för flera projekt representerar resursallokeringsnumren nummer i flera projekt.

Så här öppnar du planeringsavsnittet i resursområdet:

{{step1-to-resourcing}}

Planeraren visas som standard.  Mer information om budgeteringsresurser i resursplaneraren finns i artikeln [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![Resursplanering som standard](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Klicka på **Resurspooler** i den vänstra panelen.
Mer information om hur du skapar resurspooler finns i [Skapa resurspooler](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Använd resursplaneraren för ett projekt {#use-the-resource-planner-for-one-project}

När du använder Resursplanering för ett projekt representerar resursernas allokeringsnummer nummer nummer för det valda projektet.

1. Gå till ett projekt som du vill budgetera resurser för.
1. Klicka på **Affärsfall** i den vänstra panelen.
1. Bläddra till avsnittet **Resursbudgetering** i affärsärendet.
1. Klicka på **Redigera resursbudgetering** om du vill lägga till resurspooler i projektet och börja budgetera dina resurser.

   >[!TIP]
   >
   >Du kan bara lägga till en resurspool i området Resursbudgetering i affärsärendet när projektet inte har några associerade resurspooler. När projektet redan har en resurspool visas användarna i poolen och deras jobbroller som standard i området Resursbudgetering.

   ![Resursbudgetering](assets/resource-budgeting-area-on-project-350x70.png)

   Mer information om budgeteringsresurser för ett projekt finns i artikeln [Budgetresurser i affärsärendet](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
