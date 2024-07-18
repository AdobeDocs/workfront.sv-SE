---
product-area: resource-management
navigation-topic: resource-planning
title: Leta reda på resursplaneraren
description: '(Den här artikeln kom ut: utkast till det innehållet i artikeln när den här artikeln publicerades: /Content/Resource Management/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Leta reda på resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Du kan använda Resursplanering för att hantera tilldelningen av resurser till projekt. Du kan komma åt resursplaneraren för flera projekt samtidigt eller för ett projekt från projektets ärendeområde.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro och högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Planera eller högre för att hitta resursplaneraren i det globala området</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst eller senare till resurshantering</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för projekt och användare </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Kontrollera att alla krav för åtkomst och arbete med resursplaneraren är uppfyllda innan du börjar använda den. På så sätt ser du till att rätt information visas i resursplaneraren innan du börjar budgetera dina resurser.

Mer information om krav för resursplanering finns i [Kom igång med resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Leta reda på resursplaneraren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Du kan hitta resursplaneraren i två områden i Workfront, beroende på om du vill budgetera dina resurser för flera projekt eller bara för ett projekt.

* [Använd resursplaneraren för flera projekt](#use-the-resource-planner-for-multiple-projects)
* [Använd resursplaneraren för ett projekt](#use-the-resource-planner-for-one-project)

### Använd resursplanering för flera projekt {#use-the-resource-planner-for-multiple-projects}

När du använder Resursplanering för flera projekt representerar resursallokeringsnumren nummer i flera projekt.

Så här öppnar du planeringsavsnittet i resursområdet:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **Resurs**. Planeraren visas som standard.  Mer information om budgeteringsresurser i resursplaneraren finns i artikeln [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Håll pekaren över den vänstra panelen och klicka på **Resurspooler**.\
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

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Mer information om budgeteringsresurser för ett projekt finns i artikeln [Budgetresurser i affärsärendet](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
