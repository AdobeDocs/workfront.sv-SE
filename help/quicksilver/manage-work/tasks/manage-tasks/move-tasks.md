---
product-area: projects
navigation-topic: manage-tasks
title: Flytta uppgifter
description: Du kan flytta uppgifter till olika projekt eller till olika överordnade uppgifter i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 421fd012c2ce6a4ae0b11fe343c279d1a3fd551c
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 0%

---

# Flytta uppgifter

Du kan flytta uppgifter i Adobe Workfront mellan följande objekt:

* En ad hoc-uppgift för ett projekt.
* En uppgift från ett projekt till ett annat projekt.
* En uppgift från ett projekt under en annan överordnad i ett annat projekt.
* En uppgift inom samma projekt under en annan överordnad aktivitet.

Du kan flytta en uppgift på aktivitetsnivå eller flytta en uppgift från en lista med uppgifter.
Du kan flytta en enstaka uppgift, eller flera uppgifter åt gången, från en lista med uppgifter.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra åtgärderna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Ny plan: Standard </p> 
 <p>eller</p>  
<p>Aktuell plan: Arbete eller högre </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för uppgifter</p> <p>Contribute eller högre behörigheter för projektet med möjlighet att lägga till uppgifter</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du flyttar uppgifter

Tänk på följande när du flyttar en uppgift:

* När du flyttar en uppgift från ett projekt till ett annat kan uppgiftsdatumen beräknas om. Omberäkningen tar hänsyn till den tidsplan som det nya projektet använder och projektets Schedule From-information.

* Du kan välja att flytta vissa objekt som är kopplade till uppgiften till den flyttade aktiviteten under den flyttade processen. Som standard överförs dock följande objekt till den flyttade aktiviteten:

   * Problem
   * Inloggade timmar
   * Användarkommentarer
   * Anpassade formulär och anpassad fältinformation
   * Underaktiviteter

Följande objekt flyttas inte med uppgiften som standard:

* Milstolpar

## Flytta aktiviteter i en lista

1. Gå till det projekt som innehåller uppgiften eller aktiviteterna som du vill flytta.
1. Klicka **Uppgifter** i den vänstra panelen för att visa uppgiftslistan.
1. Klicka på **Planläge** icon ![](assets/plan-mode-icon.png) och se till att **Spara automatiskt** växlingsknappen är aktiverad och välj sedan den eller de uppgifter som du vill flytta.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Du kan inte flytta uppgifter när **Spara automatiskt** växlingen är inaktiverad.

1. (Valfritt och villkorligt) Om du vill flytta de markerade aktiviteterna inom samma projekt klickar du på de markerade uppgifterna, drar dem och släpper dem där du vill att de ska flyttas i projektet.

   När du har släppt uppgifterna på rätt plats i projektet sparas ändringarna i uppgiftshierarkin omedelbart. All information som är associerad med varje uppgift flyttas tillsammans med uppgifterna.

1. (Villkorligt) Markera den eller de uppgifter som du vill flytta och gör något av följande:

   * Klicka på **Mer** meny ![](assets/qs-more-menu.png) överst i uppgiftslistan klickar du på **Flytta till**.
   * Högerklicka på de markerade uppgifterna och klicka sedan på **Flytta till**.
   * När du markerar en uppgift klickar du på **Mer** meny ![](assets/more-icon-task-list.png) bredvid uppgiftsnamnet i listan och klicka sedan på **Flytta till**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Rutan Flytta uppgift visas

1. Fortsätt med att flytta aktiviteten enligt beskrivningen i avsnittet [Flytta en uppgift på aktivitetsnivå](#move-a-task-at-the-task-level) i den här artikeln, med början från steg 4.

   <!--
   is this still accurate?!
   -->

## Flytta en uppgift på aktivitetsnivå {#move-a-task-at-the-task-level}

Förutom att flytta uppgifter från en lista med uppgifter kan du även flytta en uppgift på aktivitetsnivå efter att du har öppnat den.

1. Hitta en uppgift i ditt Workfront-system genom att söka efter den.
1. Klicka på namnet på uppgiften för att öppna den.
1. Klicka på **Mer** nedrullningsbar meny ![](assets/qs-more-menu.png) bredvid namnet på uppgiften och klicka sedan på **Flytta till**. Rutan Flytta uppgift visas.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Valfritt) Uppdatera **Aktivitetsnamn**. Aktiviteten flyttas med det nya namnet på den nya platsen. Det ursprungliga namnet på uppgiften registreras inte i Workfront.

   >[!TIP]
   >
   >Fältet Uppgiftsnamn är nedtonat och går inte att redigera när du väljer att flytta flera uppgifter i en lista. Du kan hålla muspekaren över fältet Uppgiftsnamn så visas en lista med alla markerade uppgifter.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Ange namnet på **Målprojekt** där du vill flytta uppgiften i **Välj målprojekt** fält.

   Om du vill flytta aktiviteten inom samma projekt skriver du namnet på det aktuella projektet.

   >[!TIP]
   >
   >* Projektets namn är skiftlägeskänsligt.
   >* Du kan också börja skriva referensnumret eller ange projektets ID. Detta kan hjälpa dig att skilja mellan projekt med identiska namn.
   >* Endast 100 projekt visas i listan.

1. (Villkorligt) Klicka **Begär åtkomst** om du vill begära åtkomst till projektet, om du inte har åtkomst till det valda projektet.
1. (Villkorligt) Fortsätt att flytta aktiviteten till det valda målprojektet utan att begära åtkomst om du har åtkomst till att lägga till aktiviteter i någon av uppgifterna i målprojektet.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Liknande meddelanden visas om det valda projektet väntar på godkännande, är slutfört eller inte alls, när Workfront-administratören förhindrar att uppgifter läggs till i dessa projekt. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Valfritt) Klicka på **Alternativ** i den vänstra panelen

   eller

   Bläddra nedåt till **Alternativ** i rutan Flytta uppgift avmarkerar du något av objekten i tabellen nedan för att ta bort dem från de flyttade uppgifterna. Alla alternativ är markerade som standard.

   >[!IMPORTANT]
   >
   >Om du avmarkerar objekt i alternativlistan förlorar du data. Information från den befintliga aktiviteten tas bort och kan inte återställas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Markera alla</td> 
      <td>Avmarkera det här alternativet om du vill ta bort all information från aktiviteten när den flyttas till den nya platsen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begränsning</td> 
      <td> <p>Aktivitetsbegränsningen anges till Så snart som möjligt eller Sent som möjligt baserat på inställningen för projektschemaläge.</p> <p> När du väljer det här alternativet överförs den aktuella begränsningen för uppgiften med uppgiften. </p> 
      <p><b>ANMÄRKNING</b>

   När du flyttar eller kopierar en uppgift med datumspecifika begränsningar till ett annat projekt och villkorsdatumen för aktiviteten ligger utanför datumen för det nya projektet, ändras antingen aktivitetsbegränsningen till Så snart som möjligt eller Sent som möjligt eller så justeras datumen för planerad start eller planerad slutförning för projekten.

   Nedan följer exempel på datumspecifika begränsningar:
   <ul>
      <li> Starta den</li>
      <li> Måste avslutas</li>
      <li> Starta tidigast</li>
      <li> Starta senast</li>
      </ul>

   Mer information om uppgiftsbegränsningar och hur uppgiftsbegränsningar eller projektdatum kan påverkas finns i <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Översikt över uppgiftsbegränsning</a> och leta efter en viss begränsning.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td> <p>Alla uppdrag tas bort från uppgiften. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännandeprocess</td> 
      <td>Alla godkännandeprocesser tas bort från uppgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förlopp</td> 
      <td>Aktivitetsstatusen är Ny. I annat fall bevaras den befintliga aktivitetsstatusen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ekonomisk information</td> 
      <td>Den ekonomiska informationen för aktiviteten tas bort och Workfront uppdaterar uppgiftens kostnadstyp till Ingen kostnad och aktivitetens intäktstyp till Inte fakturerbar. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alla föregående</td> 
      <td> <p>När du väljer det här alternativet blir beroendet en föregångare mellan projekt när du flyttar aktiviteten till ett annat projekt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td> <p>Dokumenten som är kopplade till uppgiften överförs inte till den flyttade uppgiften. Detta inkluderar versioner, korrektur och länkade dokument.</p> <p>Detta inkluderar inte dokumentgodkännanden. Dokumentgodkännanden kan aldrig flyttas när en uppgift flyttas.</p> 
      <b>ANMÄRKNING</b>

   Om du inte vill att dokumenten ska flyttas tillsammans med uppgiften, kommer dokumenten att tas bort och placeras i papperskorgen i 30 dagar. En administratör kan återställa dem och de återställs vid den flyttade åtgärden.

   Om uppgiften tas bort efter att den har flyttats placeras de återställda dokumenten i området Dokument på administratörens användarsida, som återställer dem.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Påminnelsemeddelanden</td> 
      <td>Påminnelserna för aktiviteten överförs inte till den flyttade aktiviteten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td>Utgifterna som är inloggade på aktiviteten överförs inte till den flyttade aktiviteten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Behörigheter</td> 
      <td> <p>Workfront tar bort namnen på alla enheter som visas i delningslistan för uppgiften. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Valfritt) Klicka på **Markera överordnad** i den vänstra panelen

   eller

   Bläddra till **Markera överordnad** markerar du sedan den uppgift i målprojektet som du vill ska bli överordnad den flyttade uppgiften.

   >[!TIP]
   >
   >När du väljer att flytta flera uppgifter i en lista blir alla markerade uppgifter underordnade den markerade överordnade.

   Välj en överordnad genom att göra något av följande:

   * Välj en av de överordnade i projektplanen i uppgiftslistan.
   * Klicka på sökikonen ![Ikonen Sök](assets/search-icon.png) och söka efter en överordnad uppgift efter namn.

   Uppgiften visas i listan.

   ![Välj överordnad uppgift när en uppgift flyttas med sökfunktioner ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Markera alternativknappen för den överordnade när du har hittat den.

   Om du inte väljer någon överordnad uppgift flyttas uppgifterna som huvuduppgifter i stället för underuppgifter, och de placeras i slutet av uppgiftslistan i målprojektet.

1. Klicka **Flytta uppgift**

   eller

   Klicka **Flytta uppgifter** när du markerar flera uppgifter i en lista.

   De flyttade aktiviteterna finns nu i det angivna projektet och är antingen underaktiviteter till en överordnad aktivitet eller de sista aktiviteterna i projektet.
