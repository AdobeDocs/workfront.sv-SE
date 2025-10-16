---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Förstå och uppdatera projektprioriteringar
description: Det finns flera sätt att använda prioriteringar för projekt och de kommunicerar inte med varandra. Vi rekommenderar att du väljer en av prioriteringarna för projekt som passar dina behov och hänvisar till den när du kategoriserar vikten av dina projekt.
author: Alina
feature: Work Management
exl-id: b1e0b6c5-f2a7-455b-836b-6c0ead85e3ad
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Förstå och uppdatera projektprioriteringar

Det finns flera sätt att använda prioriteringar för projekt och de kommunicerar inte med varandra. Vi rekommenderar att du väljer en av prioriteringarna för projekt som passar dina behov och hänvisar till den när du kategoriserar vikten av dina projekt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Typer av projektprioritet i Adobe Workfront

Följande prioriteter kan användas för att rangordna projekt i Adobe Workfront:

* **Fältet Projektprioritet**: Du kan tilldela en prioritet till ett projekt manuellt. I den här artikeln beskrivs hur du manuellt tilldelar en prioritet till ett projekt.

  Mer information finns i avsnittet [Att tänka på när det gäller projektprioritet](#considerations-about-project-priority) i den här artikeln.

* **Prioriteten för ett projekt i Portfolio Optimizer**, om projektet är associerat med en portfölj:

  Mer information om prioriteten för ett projekt i Portfolio Optimizer finns i artikeln [Prioritera projekt i Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

* **Prioriteten för ett projekt i resursplaneraren**: Du kan prioritera projekt manuellt i resursplaneraren för att ange vilka projekt som ska få resurser först.

  Mer information om hur du prioriterar projekt i resursplaneraren finns i avsnittet om projektplaneringsprioritet i artikeln [Navigeringsöversikt för resursplanering](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Överväganden om projektprioritet {#considerations-about-project-priority}

Du kan koppla en prioritet till projekt i Workfront. Om du anger en prioritet för projektet kommunicerar det med alla i systemet hur viktigt det är.

Tänk på följande när du väljer en prioritet för dina projekt:

* Din Workfront-administratör definierar de prioriteringar som är tillgängliga i Workfront. När du har skapat dem kan du koppla dem till projekt i fältet Prioritet.

  Mer information om hur du skapar prioriteringar i Workfront finns i artikeln [Skapa och anpassa prioriteringar](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

* När du uppdaterar fältet Prioritet för ett projekt överförs den här prioriteten inte till Portfolio Optimizer eller Resursplanering. Projektets prioritetsfält är bara en manuell flagga som du placerar i projektet för att ange dess betydelse för andra användare.
* Ett projekts prioritetsvärde används främst för rapportering.

  Du kan till exempel söka efter alla projekt som har prioritetsvärdet Urgent när du använder det här fältet i ett projektfilter.
* Uppgifter och frågor har också prioritet, men uppgifter, utgåvor och projektprioriteringar fungerar oberoende av varandra och påverkar inte automatiskt varandra. Du kan ha ett problem med hög prioritet eller en åtgärd med medelhög prioritet i ett projekt med låg prioritet.
* Du kan uppdatera prioriteten för projekt i följande områden i Workfront:

   * I dialogrutan **Redigera projekt** .
   * På fliken **Projektinformation** i ett projekt.
   * I en projektlista eller rapport.

## Uppdatera fältet för projektprioritet

1. Gå till det projekt vars prioritet du vill uppdatera.
1. Klicka på **Projektinformation** i den vänstra panelen.
1. Klicka på ikonen **Redigera** ![Redigera](assets/qs-edit-icon.png) i det övre högra hörnet av området Projektinformation och klicka sedan på **Översikt**.

1. Välj bland följande alternativ i fältet **Prioritet**:

   * Ingen
   * Låg
   * Normal

     Detta är standardprioritet.

   * Hög
   * Urgent

   ![Prioritetslista i ett projekt](assets/project-priority-picker-list.png)

1. Klicka på **Spara ändringar**.

   Du måste kommunicera med andra användare och förstå vad varje prioritetsnivå betyder för projektet.
