---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Förstå och uppdatera projektprioriteringar
description: Det finns flera sätt att använda prioriteringar för projekt och de kommunicerar inte med varandra. Vi rekommenderar att du väljer en av prioriteringarna för projekt som passar dina behov och hänvisar till den när du kategoriserar vikten av dina projekt.
author: Alina
feature: Work Management
exl-id: b1e0b6c5-f2a7-455b-836b-6c0ead85e3ad
source-git-commit: b08edd8dd7c339dffdba4c9ff5aa0a365229e794
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Förstå och uppdatera projektprioriteringar

Det finns flera sätt att använda prioriteringar för projekt och de kommunicerar inte med varandra. Vi rekommenderar att du väljer en av prioriteringarna för projekt som passar dina behov och hänvisar till den när du kategoriserar vikten av dina projekt.

## Åtkomstkrav

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
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
</table>
-->
Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Typer av projektprioritet i Adobe Workfront

Följande prioriteter kan användas för att rangordna projekt i Adobe Workfront:

* **Fältet Projektprioritet**: Du kan tilldela en prioritet till ett projekt manuellt. I den här artikeln beskrivs hur du manuellt tilldelar en prioritet till ett projekt.

  Mer information finns i avsnittet [Överväganden om projektprioritet](#considerations-about-project-priority) i den här artikeln.

* **Ett projekts prioritet i Portfolio-optimering**, om projektet är kopplat till en portfölj:

  Mer information om prioriteten för ett projekt i Portfolio-optimering finns i artikeln [Prioritera projekt i Portfolio-optimering](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

* **Projektets prioritet i resursplaneraren**: Du kan prioritera projekt manuellt i resursplaneraren för att ange vilka projekt som ska få resurser först.

  Mer information om hur du prioriterar projekt i resursplaneraren finns i avsnittet Projektplaneringsprioritet i artikeln [Översikt över navigering i resursplanering](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Överväganden om projektprioritet {#considerations-about-project-priority}

Du kan koppla en prioritet till projekt i Workfront. Om du anger en prioritet för projektet kommunicerar det med alla i systemet hur viktigt det är.

Tänk på följande när du väljer en prioritet för dina projekt:

* Din Workfront-administratör definierar de prioriteringar som är tillgängliga i Workfront. När du har skapat dem kan du koppla dem till projekt i fältet Prioritet.

  Mer information om hur du skapar prioriteringar i Workfront finns i artikeln [Skapa och anpassa prioriteringar](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

* När du uppdaterar fältet Prioritet för ett projekt överförs den här prioriteten inte till Portfolio-optimering eller Resursplanering. Projektets prioritetsfält är bara en manuell flagga som du placerar i projektet för att ange dess betydelse för andra användare.
* Ett projekts prioritetsvärde används främst för rapportering.

  Du kan till exempel söka efter alla projekt som har prioritetsvärdet Urgent när du använder det här fältet i ett projektfilter.
* Uppgifter och frågor har också prioritet, men uppgifter, utgåvor och projektprioriteringar fungerar oberoende av varandra och påverkar inte automatiskt varandra. Du kan ha ett problem med hög prioritet eller en åtgärd med medelhög prioritet i ett projekt med låg prioritet.
* Du kan uppdatera prioriteten för projekt i följande områden i Workfront:

   * I **Redigera projekt** -dialogrutan.
   * I **Projektinformation** -fliken i ett projekt.
   * I en projektlista eller rapport.

## Uppdatera fältet för projektprioritet

1. Gå till det projekt vars prioritet du vill uppdatera.
1. Klicka **Projektinformation** till vänster.
1. Klicka på **Redigera** icon ![](assets/qs-edit-icon.png) i det övre högra hörnet av området Projektinformation och klicka sedan på **Ökning**.

1. I **Prioritet** väljer du bland följande alternativ:

   * Ingen
   * Låg
   * Normal

     Detta är standardprioritet.

   * Hög
   * Urgent

   ![](assets/project-priority-picker-list-on-project-details-nwe-350x192.png)

1. Klicka **Spara ändringar**.

   Du måste kommunicera med andra användare och förstå vad varje prioritetsnivå betyder för projektet.
